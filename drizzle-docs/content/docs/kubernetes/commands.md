---
date: '2026-05-21T17:05:35+09:00'
draft: false
title: 'Kubernetes 명령어 모음'
---

공식문서 Quick Reference 참고

{{< bookmark url="https://kubernetes.io/docs/reference/kubectl/quick-reference/" title="kubectl Quick Reference | kubernetes.io" >}}


### 모니터링

```
# 이벤트 확인
kubectl get events

# 로그 확인
kubectl logs <pod>

# 파드 조회
kubectl get pods

# 컨테이너 접속
kubectl exec -it <pods> <container> -- bash
```


### Helm(v2)

```
# 릴리즈 설치
helm install --name <release> -f values.yaml <chart>

# 릴리즈 삭제
helm delete --purge <release>

# 릴리즈 조회
helm list
helm list --all

# values 조회
helm get values <release>

# 백업하기
helm get values <release> --all --output yaml > <release>-values.yaml
helm get manifest <release> > <release>-manifest.yaml
```

### secret

```
# secret 넣을 때 인코딩
echo '<value>' | base64

# 디코딩
echo '<value>' | base64 -d
```

### 기타

리소스 및 축약어 확인

```
kubectl api-resources
```

권한 확인

```
# 현재 컨텍스트에서 가능한 권한 확인
kubectl auth can-i --list
```

리소스 쿼터 확인

```
kubectl get quota
```

events 표준시간 확인

```
kubectl get events -A -o custom-columns=NS:.metadata.namespace,NAME:.involvedObject.name,REASON:.reason,MESSAGE:.message,LASTTIME:.lastTimestamp
```
