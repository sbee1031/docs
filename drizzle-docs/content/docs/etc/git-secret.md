---
date: '2026-05-21T13:43:11+09:00'
draft: false
title: 'git-secret'
---

Git 저장소에 시크릿(토큰, API 키, 비밀번호 등)을 올려야 하는데, 평문으로 올리면 누구나 볼 수 있기 때문에 위험하다.
git-secret은 **GPG 암호화로 파일을 암호화해서 커밋**하고, **권한이 있는 사람만 복호화**할 수 있게 해준다.

## 특징

저장소에는 항상 암호화된 파일(.secret)만 존재한다. 원본 파일은 `.gitignore`에 자동 등록되어 커밋되지 않는다.

```
tokens/aa          ← 원본 (git에 안 올라감, .gitignore 처리됨)
tokens/aa.secret   ← 암호화된 버전 (git에 올라감)
```

GPG 키가 등록된 계정만 복호화 가능

## 설정 방법

{{% steps %}}

#### 초기 설정

```
cd my-repo/
git secret init          # 저장소에 .gitsecret/ 디렉토리 생성
```

#### 복호화 권한 등록

```
# "이 사람의 GPG 키로 암호화하겠다"는 의미
git secret tell user@email.com
git secret tell dl@email.com
```

`.gitsecret/keys/` 안에 해당 사용자의 GPG 공개키가 저장된다. 이후 `hide`할 때 등록된 모든 사람의 공개키로 암호화된다.

#### 시크릿 파일 등록 및 암호화

```
# 원본 파일을 시크릿으로 등록
git secret add tokens/aa
```
1. `tokens/aa`가 `.gitignore`에 추가된다. (원본 업로드 X)
2. `.gitsecret/paths/mapping.cfg`에 파일 경로가 기록된다.

```
# 암호화
git secret hide
```
`tokens/aa.secret` 파일이 생성됨

#### 암호화 파일 커밋

```
git add -A
git commit -m "add encrypted token"
git push
```
#### 복호화

```
git clone ...
git secret tell {user}   # 이미 등록되어 있으면 스킵
git secret reveal        # .secret 파일들을 복호화 → 원본 생성
```
`reveal`이 성공하면 `tokens/aa.secret` → `tokens/aa` 원본이 생성된다.

{{% /steps %}}



## 핵심 명령어 정리

| 명령어 | 역할 | 용도 |
| --- | --- | --- |
| `git secret init` | 저장소 초기화 | 최초 1회 |
| `git secret tell <email>` | GPG 공개키 등록 (복호화 권한 부여) | 사용자 추가 시 |
| `git secret add <file>` | 파일을 비밀 관리 대상에 등록 | 새 비밀 파일 추가 시 |
| `git secret hide` | 등록된 파일을 암호화 (.secret 생성) | 원본이 변경되었거나 사용자가 추가된 후 |
| `git secret reveal` | .secret 파일을 복호화 (원본 복원) | clone 후, 또는 CI/CD에서 |
| `git secret list` | 관리 중인 비밀 파일 목록 확인 | 디버깅 시 |
| `git secret whoknows` | 복호화 권한이 있는 사용자 목록 | 디버깅 시 |
| `git secret removeperson <email>` | 권한 제거 | 퇴사/이동 시 (이후 hide 다시 해야 함) |



## Jenkins에서의 흐름

```
Jenkins 빌드 시작
  ↓
git clone (repo.git)     ← .secret 파일들만 존재
  ↓
git secret tell {user}   ← Jenkins 서버의 GPG 키 확인
  ↓
git secret reveal        ← .secret → 원본 복호화
  ↓
cat tokens/aa            ← 복호화된 토큰을 읽어서 사용
```
