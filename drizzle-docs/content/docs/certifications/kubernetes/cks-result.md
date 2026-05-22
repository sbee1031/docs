---
date: '2026-05-20T11:22:36+09:00'
draft: false
title: 'CKS 취득후기'
linkTitle: 'CKS 취득후기'
weight: 3
---

![](/images/cks-result.png)

CKA, CKAD를 취득하고 2년 가까이 쉬다가 블프 때 사두었던 CKS 응시권 만료가 다가와서 부랴부랴 시험을 준비했다.
더 기억이 흐려지기 전에, CKS 취득후기를 남기려고 한다!


# CKS란?
{{< bookmark url="https://training.linuxfoundation.org/certification/certified-kubernetes-security-specialist/" title="Certified Kubernetes Security Specialist (CKS) | Linux Foundation" >}}

CKS(Certificated Kubernetes Security Specialist)는 쿠버네티스 환경에서의 보안 실무 능력을 검증하는 시험으로, CKA 취득이 필수 조건이다.
단순 보안 설정뿐만 아니라, 이미지 빌드부터 배포, 런타임 보안, 로깅 및 감사 등 전체 라이프사이클을 다룬다.

* Cluster Setup (15%)
* Cluster Hardening (15%)
* System Hardening (10%)
* Minimize Microservice Vulnerabilities (20%)
* Supply Chain Security (20%)
* Monitoring, Logging and Runtime Security (20%)

# 시험정보
* 시험 환경 : PSI(원격 시험)
* 소요 시간 : 120분
* 시험 문제 : 15-20문제
* 합격 기준 : 66점
* 재시험 포함 총 2회 시험 응시 가능
* 결과는 24시간 이내 이메일로 안내


# 시험 공부
CKS 공부도 CKA와 마찬가지로 강의 시청 및 실습 위주로 진행하려고 했으나, 응시 기간이 얼마 남지 않은 관계로 실습 먼저 진행하고, 잘 이해가 가지 않는 부분에 대해서는 강의를 보면서 개념을 다시 잡는 방식으로 진행했다. 

CKA, CKAD는 쿠버네티스 공식문서에 나와 있는 것만으로도 충분히 문제를 풀 수 있었는데 CKS는 공식문서만으론 좀 부족하기 때문에 리눅스나 오픈소스 명령어를 많이 익히는게 좋다.

난 KodeKloud 실습 -> 부족한 부분 강의 시청 -> killercoda로 각 유형별 문제 파악 및 복습 -> killer.sh 순서로 시험을 준비했다.

### KodeKloud
{{< bookmark url="https://learn.kodekloud.com/user/courses/certified-kubernetes-security-specialist-cks" title="Certified Kubernetes Security Specialist (CKS) | KodeKloud" >}}

뭄샤드 선생님의 CKS 강의는 KodeKloud만 있어서, 하는 수 없이 구독을 통해 강의를 들을 수 밖에 없었다~~(월 3만 5천원 ...)~~.
비싼데 소장도 불가능한 KodeKloud의 강의를 들은 이유는 딱히 CKA처럼 바이블이라고 불리는 강의도 없을 뿐더러, 실습 환경이 너무 잘 되어 있어서다.
온라인 시험이다 보니 손으로 익히는 감이 제일 중요한데, 여태까지 CKA, CKAD를 준비하면서 KodeKloud 실습 환경보다 편하고 성능 좋은 환경은 못봤다.

강의 구성과 실습 환경 등은 Udemy CKA 강의와 거의 똑같기 때문에 참고하면 된다.

### Killercoda
{{< bookmark url="https://killercoda.com/killer-shell-cks" title="Killer Shell CKS | Killercoda" >}}

CKS는 리눅스 및 오픈소스 명령어들도 익혀야 하는데, Killercoda는 각 문제 유형 및 툴 별로 문제를 골라서 풀어보기 좋다. 
KodeKloud 실습 문제를 많이 풀다보면 답이 외워져서 손가락만 움직이게 될 때가 있는데 이럴 때 유용하게 썼다.

### killer.sh
Killer.sh은 시험 신청 시 무료로 2회 제공해주는 시뮬레이터인데, 시험 환경 적응 및 문제 유형 파악을 위해 시험 전에 풀어보는 것이 좋다.
세션은 36시간만 활성화되기 때문에, 시험 2~3일 전에 풀어보고, 틀린 문제는 정리해놓고 비슷한 유형의 문제들을 더 풀어보면서 준비하면 된다.

공식문서에 Killer.sh이 실제 시험보다 난이도가 어렵다고 나와 있지만, 나는 비슷하거나 실제 시험이 더 어렵다고 느꼈다.


# 시험문제 복기
* kube-bench (kubelet, apiserver anonymous 설정하기)
* ingress
* network policy
* tls secret 생성
* istio sidecar, mTLS
* /dev/mem 접근하는 컨테이너 찾아서 deployment scale 0 (falco)
* audit
* imagepolicywebhook
* noderestriction
* docker root group 변경 및 TCP 제거
* 컨테이너 3개 있는 deploy 중 특정 패키지 버전을 사용하는 이미지의 bom 생성
* 클러스터 버전 업그레이드
* Immutable 설정
* docker/yaml 보안 강화할 수 있도록 수정

# 시험 후기
보안 관련된 지식이 없기도 하고, 쿠버네티스 자체 지식보다 더 많은 것을 요구하는 시험이라 그런지 CKA 때 보다 훨씬 어렵게 느껴졌다.

특히 내가 느꼈던 건,
1. 어떤 툴을 이용해서 해결해야 하는지 문제에서 가르쳐주지 않는다.
2. 다른 오픈소스 공식문서 활용 필요 (Cilium, Falco 등)
3. CKA, CKAD는 대부분의 문제가 컨텍스트 변경만 필요하고 서버를 옮겨다니는 문제는 거의 없는데, CKS는 문제마다 `ssh`로 옮겨 다녀야 한다. -> alias 설정이 무의미해서 일일이 다 손으로 쳐야 한다..
4. 쿠버네티스만 안다고 풀 수 없는 문제도 있다.

CKS는 1차 시험에 불합격해서 2차 시험까지 보게 되었는데, 처음엔 문제 유형별로 감이 좀 부족해서인가 시간이 오래 걸려 다 풀지 못했다.
그래서 재시험을 준비할 때 각 문제별로 기계처럼 답을 외우는 방식이 아니라 오픈소스별로 어떤 식으로 접근하고, 리눅스 명령어 어떤 것들이 필요한지 등의 깊이 있는 부분을 이해하려고 했다.

![](/images/cks-score.png)

2차 시험 때는 1차 때와 비슷한 유형의 문제가 나오기도 하고, 이해가 되니까 문제가 나름 잘 풀려서인지 점수를 높게 받았다.
그런데 시간이 지난 지금 문제도 잘 기억 안 나는 걸 보면 시험용으로 바짝 준비해서 장기 기억으로 가진 못한 것 같다.
여유가 되면 공부했던 내용 복습하면서 한 번 더 개념 정리하는 시간을 가지려고 한다.
