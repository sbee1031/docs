+++
date = '2026-05-18T11:38:21+09:00'
draft = true
title = 'Result'
+++

## 시험정보



[Certified Kubernetes Application Developer (CKAD) | Linux Foundation Education](https://training.linuxfoundation.org/certification/certified-kubernetes-application-developer-ckad/)

- 시험범위
    - Application Environment, Configuration and Security25%
        
        Discover and use resources that extend Kubernetes (CRD, Operators) : 쿠버네티스 확장을 위한 리소스 탐색 및 사용(CRD, 오퍼레이터)
        
        Understand authentication, authorization and admission control : 인증, 권한 부여 및 어드미션 제어 이해
        
        Understand requests, limits, quotas : request, limit, quota 이해
        
        Understand ConfigMaps : 컨피그맵 이해
        
        Define resource requirements : 리소스 요구사항 정의
        
        Create & consume Secrets : 시크릿 생성 및 사용
        
        Understand ServiceAccounts : 서비스어카운트 이해
        
        Understand Application Security (SecurityContexts, Capabilities, etc.) : 애플리케이션 보안 이해
        
    - Application Design and Build20%
        
        Define, build and modify container images : 컨테이너 이미지 정의, 빌드 및 수정
        
        Choose and use the right workload resource (Deployment, DaemonSet, CronJob, etc.) : 올바른 워크로드 리소스(디플로이, 데몬셋, 크론잡 등) 선택 및 사용
        
        Understand multi-container Pod design patterns (e.g. sidecar, init and others) : 멀티 컨테이너 파드 디자인 패턴 이해(사이드카, init 등)
        
        Utilize persistent and ephemeral volumes : pv 및 ephemeral 볼륨 활용
        
    - Application Deployment20%
        
        Use Kubernetes primitives to implement common deployment strategies (e.g. blue/green or canary) : 배포 전략 구현(블루/그린, 카나리아)
        
        Understand Deployments and how to perform rolling updates : 배포 및 롤링 업데이트 수행방법 이해
        
        Use the Helm package manager to deploy existing packages : 헬름 패키지 관리자를 사용하여 기존 패키지 배포
        
        Kustomize
        
    - Services and Networking20%
        
        Demonstrate basic understanding of NetworkPolicies : 네트워크 정책에 대한 기본 이해 입증
        
        Provide and troubleshoot access to applications via services : 서비스를 통해 애플리케이션에 대한 액세스 제공 및 문제 해결
        
        Use Ingress rules to expose applications : 인그레스를 사용하여 애플리케이션 노출
        
    - Application Observability and Maintenance15%
        
        Understand API deprecations : API 사용 중단 이해
        
        Implement probes and health checks : probes 및 헬스체크 구현
        
        Use built-in CLI tools to monitor Kubernetes applications : CLI 를 사용하여 애플리케이션 모니터링
        
        Utilize container logs : 컨테이너 로그 활용
        
        Debugging in Kubernetes : 쿠버네티스 디버깅
        

## 공부

- 공부자료
    - udemy 강의
        
        [](https://www.udemy.com/home/my-courses/learning/)
        
    - udemy 강의 번역본
        
        [Udemy CKA 강의 정리 0: 목차](https://muni-dev.tistory.com/entry/Udemy-CKA-강의-정리-0-목차)
        
    - kodekloud 실습
        
        [Sign In | KodeKloud](https://beta.kodekloud.com/user/courses/udemy-labs-certified-kubernetes-administrator-with-practice-tests)
        
        [Sign In | KodeKloud](https://beta.kodekloud.com/user/courses/kubernetes-challenges)
        
        - 유료버전
            
            [Udemy Labs - Certified Kubernetes Administrator with Practice Tests - KodeKloud](https://kodekloud.com/courses/labs-certified-kubernetes-administrator-with-practice-tests/)
            
    - 따배쿠 강의
        
        [[따배씨] CKA 시리즈](https://www.youtube.com/playlist?list=PLApuRlvrZKojqx9-wIvWP3MPtgy2B372f)
        
    - K8s Documents
        
        [Kubernetes Documentation](https://kubernetes.io/docs/home/)
        
    - fastcampus 강의
        
        [](https://fastcampus.co.kr/courses/208963/clips/)
        
    - udemy github
        
        https://github.com/kodekloudhub/certified-kubernetes-administrator-course
        
    - cncf curriculum
        - https://github.com/cncf/curriculum
- 북마크
    - Volume
    - ETCD BACKUP & RESTORE : https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/#backing-up-an-etcd-cluster
    - Storage
        - pod 에 pvc volume mount : https://kubernetes.io/docs/concepts/storage/persistent-volumes/#claims-as-volumes
        - hostPath pv 생성 : https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/#create-a-persistentvolume
        - storage class 생성 : https://kubernetes.io/docs/concepts/storage/storage-classes/#storageclass-objects
    - RBAC
        - https://kubernetes.io/docs/reference/access-authn-authz/rbac/
        - command-line utillity : https://kubernetes.io/docs/reference/access-authn-authz/rbac/#command-line-utilities
    - CSR
        - CSR 생성 : https://kubernetes.io/docs/reference/access-authn-authz/certificate-signing-requests/#create-certificatessigningrequest
    - secret
        - create : https://kubernetes.io/docs/concepts/configuration/secret/#working-with-secrets
        - valueFrom secret : [https://kubernetes.io/ko/docs/concepts/configuration/secret/#시크릿을-환경-변수-형태로-사용하기](https://kubernetes.io/ko/docs/concepts/configuration/secret/#%EC%8B%9C%ED%81%AC%EB%A6%BF%EC%9D%84-%ED%99%98%EA%B2%BD-%EB%B3%80%EC%88%98-%ED%98%95%ED%83%9C%EB%A1%9C-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)
        - envFrom secret : [https://kubernetes.io/ko/docs/concepts/configuration/secret/#사용-사례-컨테이너-환경-변수로-사용하기](https://kubernetes.io/ko/docs/concepts/configuration/secret/#%EC%82%AC%EC%9A%A9-%EC%82%AC%EB%A1%80-%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88-%ED%99%98%EA%B2%BD-%EB%B3%80%EC%88%98%EB%A1%9C-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)
    - configmap
        - create : https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#define-a-container-environment-variable-with-data-from-a-single-configmap
        - envFrom cm : https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#configure-all-key-value-pairs-in-a-configmap-as-container-environment-variables
    - API Reference : https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.29/
- 개념정리
    - security context
        
        capabilities 는 컨테이너 레벨에서만 설정 가능
        
        ```bash
        securityContext:
        	runAsUser: 0
        	capabilities: ['NET_ADMIN', 'SYS_TIME']
        ```
        
    - service account
        
        모든 네임스페이스에 default 라는 이름으로 sa 가 생성됨
        
    - Job
        
        Batch 처리에 적합한 컨트롤러로 Pod 는 작업 완료 시 종료됨(비정상 종료 시 재실행)
        
        - restartPolicy : Never/OnFailure
            - job 은 기본적으로 실행이 완료되면 다시 실행되지 않는데, 만약 비정상적으로 실행되어 종료된 경우 재실행 정책을 설정할 때 사용
            - OnFailure : job1 에서 중단됐던 부분부터 재시작
            - Never : 스케줄러에 의해 자동으로 재시작
        - backoffLimit : job 실패 시 재시도 횟수
        - activeDeadlineSeconds : 지정한 시간 안에 실행되지 않으면 Job 을 종료시킴
        - completions : 실행 횟수(하나의 잡 시작/종료 후 또 하나의 잡 실행/종료 반복..)
        - parallelism : 동시실행 횟수
            - completions: 6, parallelism: 2 일 경우 2개씩 잡 실행 * 3번 반복
        
    - 배포전략
        - Blue-Green Update : 구 버전과 신 버전 모두 동작 중인 상태에서 트래픽만 신 버전으로 전환
            - 롤백이 쉽고 업데이트 시간 절감
            - 하드웨어 리소스가 *2 만큼 필요함
            - 다운타임이 발생함
        - Canary Deployment : 업데이트 기존 버전을 유지한 채로 일부 버전만 신규 버전으로 올려서 테스트 후 적용
            - scale 명령으로 가중치를 조절하여 배포 가능
        - Rolling Update
            - maxUnavailable : 사용할 수 없는 최대 파드 수, 반내림(replicas=3, maxUnavailable=25% ⇒ 0.75 == 0, 30% 설정 시 사용 가능한 파드 수는 70% 이상 되도록 운영)
            - maxSurge: 운영 가능한 최대 파드 수, 반올림(replicas=3, maxSurge=25% ⇒ 0.75 == 1)
            - progressDeadlineSeconds : 업데이트 대기시간. 해당 시간 내에 업데이트를 완료하지 못 할 경우 롤백
            - minReadySeconds : 최소 대기시간. 해당 시간 대기 후 running
            - revisionHistoryLimit : revision 기록 개수
    - Helm
        
        쿠버네티스 패키지 매니저
        
        기능
        
        - 클러스터에 차트 설치 및 제거 , 릴리즈 주기 관리
        - 차트로 패키지화 가능
        - 차트저장소와 상호작용
        
        구성
        
        - Chart
        - Repository
    - Github exercises
        - Core Concepts(13%)
            
            ```bash
            Create a namespace called 'mynamespace' and a pod with image nginx called nginx on this namespace
            - k create ns mynamespace
            - k run nginx --image=nginx -n mynamespace
            
            Create the pod that was just described using YAML
            - k run nginx --image=nginx -n mynamespace --dry-run=client -o yaml > nginx.yaml
            - k apply -f nginx.yaml
            apiVersion: v1
            kind: Pod
            metadata:
              name: nginx
            spec:
              containers:
              - name: nginx
                image: nginx
            
            Create a busybox pod (using kubectl command) that runs the command "env". Run it and see the output
            - k run busybox --image=busybox -- env
            - k logs busybox
            
            Create a busybox pod (using YAML) that runs the command "env". Run it and see the output
            - k run busybox --image=busybox --dry-run=client -o yaml -- env > busybox.yaml
            - k apply -f busybox.yaml
            - k logs busybox
            apiVersion: v1
            kind: Pod
            metadata:
              name: busybox
            spec:
              containers:
              - name: busybox
                image: busybox
                command:
                - env
            
            Get the YAML for a new namespace called 'myns' without creating it
            - k create ns myns --dry-run=client -o yaml
            
            Create the YAML for a new ResourceQuota called 'myrq' with hard limits of 1 CPU, 1G memory and 2 pods without creating it
            - k create quota myrq --hard=limits.cpu=1,limits.memory=1G,pods=2 --dry-run=client -o yaml
            apiVersion: v1
            kind: ResourceQuota
            metadata:
              name: myrq
            spec:
              hard:
                limits.cpu: "1"
                limits.memory: 1G
                pods: "2"
            
            Get pods on all namespaces
            - k get po -A
            
            Create a pod with image nginx called nginx and expose traffic on port 80
            - k run nginx --image=nginx --port=80 --expose=true
            
            Change pod's image to nginx:1.7.1. Observe that the container will be restarted as soon as the image gets pulled
            - k set image po nginx nginx=nginx:1.7.1
            
            Get nginx pod's ip created in previous step, use a temp busybox image to wget its '/'
            - k get po -o wide
            - k run busybox --image=busybox --rm -it -- wget -O- <ip>
            - k run busybox --image=busybox --rm -it -- sh -c 'wget -O- <ip>'
            
            Get pod's YAML
            - k get po -o yaml
            
            Get information about the pod, including details about potential issues (e.g. pod hasn't started)
            - k describe po 
            
            Get pod logs
            - k logs po
            
            If pod crashed and restarted, get logs about the previous instance
            - k logs po -p
            
            Execute a simple shell on the nginx pod
            - k exec -it po nginx -- sh
            
            Create a busybox pod that echoes 'hello world' and then exits
            - k run busybox --image=busybox -- echo 'hello world'
            
            Do the same, but have the pod deleted automatically when it's completed
            - k run busybox --image=busybox --rm -it -- echo 'hello world'
            
            Create an nginx pod and set an env value as 'var1=val1'. Check the env value existence within the pod
            - k run nginx --image=nginx --env=var1=var1 -- env
            - k run nginx --image=nginx --env=var1=var1 -- sh -c 'echo $var1'
            ```
            
        - Multi-container Pods(10%)
            
            ```bash
            #Create a Pod with two containers, both with image busybox and command "echo hello; sleep 3600". Connect to the second container and run 'ls'
            - k run m1 --image=busybox --dry-run=client -o yaml -- sh -c 'echo hello; sleep 3600' > m1.yaml
            apiVersion: v1
            kind: Pod
            metadata:
              creationTimestamp: null
              labels:
                run: m1
              name: m1
            spec:
              containers:
              - args:
                - sh
                - -c
                - echo hello; sleep 3600
                image: busybox
                name: m1
              - args:
                - sh
                - -c
                - echo hello; sleep 3600
                image: busybox
                name: m2
              dnsPolicy: ClusterFirst
              restartPolicy: Always
            - k exec -it m1 -c m2 -- ls
            bin    etc    lib    proc   sys    usr
            dev    home   lib64  root   tmp    var
            
            # Create a pod with an nginx container exposed on port 80. Add a busybox init container which downloads a page using "wget -O /work-dir/index.html http://neverssl.com/online". 
            # Make a volume of type emptyDir and mount it in both containers. For the nginx container, mount it on "/usr/share/nginx/html" and for the initcontainer, mount it on "/work-dir". 
            # When done, get the IP of the created pod and create a busybox pod and run "wget -O- IP"
            - k run nginx --image=nginx --port=80 --dry-run=client -o yaml > nginx.yaml
            apiVersion: v1
            kind: Pod
            metadata:
              creationTimestamp: null
              labels:
                run: nginx
              name: nginx
            spec:
              containers:
              - image: nginx
                name: nginx
                ports:
                - containerPort: 80
                resources: {}
                volumeMounts:
                  - name: data
                    mountPath: /usr/share/nginx/html
              initContainers:
              - name: busybox
                image: busybox
                command:
                - sh
                - -c
                - 'wget -O /work-dir/index.html http://neverssl.com/online'
                volumeMounts:
                  - name: data
                    mountPath: /work-dir
              volumes:
                - name: data
                  emptyDir: {}
              dnsPolicy: ClusterFirst
              restartPolicy: Always
            status: {}
            
            - k logs nginx -c busybox
            Connecting to neverssl.com (34.223.124.45:80)
            Connecting to neverssl.com (34.223.124.45:80)
            saving to '/work-dir/index.html'
            index.html           100% |********************************|  2238  0:00:00 ETA
            '/work-dir/index.html' saved
            
            - k get po -o wide
            - wget -O- 192.168.1.23
            ```
            
        - Pod design(20%)
            
            Labels and Annotations
            
            ```bash
            Create 3 pods with names nginx1,nginx2,nginx3. All of them should have the label app=v1
            
            Show all labels of the pods
            
            Change the labels of pod 'nginx2' to be app=v2
            
            Get the label 'app' for the pods (show a column with APP labels)
            
            Get only the 'app=v2' pods
            
            Add a new label tier=web to all pods having 'app=v2' or 'app=v1' labels
            
            Add an annotation 'owner: marketing' to all pods having 'app=v2' label
            
            Remove the 'app' label from the pods we created before
            
            Annotate pods nginx1, nginx2, nginx3 with "description='my description'" value
            
            Check the annotations for pod nginx1
            
            Remove the annotations for these three pods
            
            Remove these pods to have a clean state in your cluster
            ```
            
        - 
        - 
        
    - 명령어
        
        ```bash
        # label 설정
        k label no node01 color=blue
        
        # label 제거
        k label no node01 color-
        
        # pod 생성
        k run nginx --image=nginx --labels=color=blue
        
        # deploy 생성
        k create deploy deploy1 --image=nginx --replicas=3 --expose --port=80
        ```
        
    - service account
        
        system:serviceaccount:default:default
        
    - secret 암호화
        
        기본적으로 시크릿은 암호화되지 않음(디코딩해서 값 확인 가능)
        
        REST 암호화 방법
        
        ```bash
        1. secret 생성
        
        2. 랜덤키 생성
        head -c 32 /dev/urandom | base64
        
        3. EncryptionConfiguration 생성
        apiVersion: apiserver.config.k8s.io/v1
        kind: encryptionConfiguration
        resources:
        	- resources:
        		- secrets
        		providers:
        			- aescbc: # 암호화 알고리즘 선택
        					keys:
        					- name:
        						secret: # 2에서 생성한 랜덤키
        			- identity: {}
        			
        4. kube-apiserver manifest 수정
        .spec.volumes
        .spec.containers.volumeMounts
        .spec.containers.command
        -> --encryption-provider-config={path}
        
        이후 생성한 시크릿 리소스는 암호화되어 저장됨
        기존 리소스도 암호화 하려면 : k get secrets -A -o json | k replace -f -
        ```
        
    - node affinity
        
        ```bash
            spec:
              affinity:
                nodeAffinity:
                  requiredDuringSchedulingIgnoredDuringExecution:
                    nodeSelectorTerms:
                    - matchExpressions:
                      - key: color
                        operator: In
                        values:
                        - blue
        ```
        
    - readiness probe
        
        ```bash
        spec:
          containers:
          - env:
            - name: APP_START_DELAY
              value: "80"
            image: kodekloud/webapp-delayed-start
            imagePullPolicy: Always
            name: simple-webapp
            ports:
            - containerPort: 8080
              protocol: TCP
            readinessProbe:
              httpGet:
                path: /ready
                port: 8080
        ```
        
    - liveness probe
        
        ```bash
        spec:
          containers:
          - livenessProbe:
              httpGet:
                path: /live
                port: 8080
              periodSeconds: 1
              initialDelaySeconds: 80
        ```
        
    - Network Policy
        
        ```bash
        Create a network policy to allow traffic from the Internal application only to the payroll-service and db-service.
        Use the spec given below. You might want to enable ingress traffic to the pod to test your rules in the UI.
        Also, ensure that you allow egress traffic to DNS ports TCP and UDP (port 53) to enable DNS resolution from the internal pod.
        ```
        
        ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/898ae2bb-948b-440a-8885-5f0c6dd8011f/Untitled.png)
        
        ```bash
        # 내 답안
        apiVersion: networking.k8s.io/v1
        kind: NetworkPolicy
        metadata:
          name: internal-policy
          namespace: default
        spec:
          podSelector:
            matchLabels:
              name: internal
          policyTypes:
          - Egress
          egress:
          - to:
            - podSelector: 
                matchLabels:
                  name: payroll
            ports:
            - protocol: TCP
              port: 8080
          - to:
            - podSelector:
                matchLabels:
                  name: mysql
            ports:
            - protocol: TCP
              port: 3306
          - to:
            ports:
            - protocol: TCP
              port: 53 
            - protocol: UDP 
              port: 53 
              
        # 해설
        apiVersion: networking.k8s.io/v1
        kind: NetworkPolicy
        metadata:
          name: internal-policy
          namespace: default
        spec:
          podSelector:
            matchLabels:
              name: internal
          policyTypes:
          - Egress
          - Ingress
          ingress:
            - {}
          egress:
          - to:
            - podSelector:
                matchLabels:
                  name: mysql
            ports:
            - protocol: TCP
              port: 3306
        
          - to:
            - podSelector:
                matchLabels:
                  name: payroll
            ports:
            - protocol: TCP
              port: 8080
        
          - ports:
            - port: 53
              protocol: UDP
            - port: 53
              protocol: TCP
        ```
        
    - context
        
        다른 config 파일을 이용하여 context 지정
        
        ```bash
        kubectl config --kubeconfig=/root/my-kube-config use-context research
        ```
        
    - TLS secret
        
        ```bash
        k create secret tls {secret} --cert={certificate} --key={key}
        ```
        
    - API groups enabling/disabling
        
        https://kubernetes.io/docs/reference/using-api/#enabling-or-disabling
        
        ```bash
        # enable
        --runtime-config=v1alpha1
        
        # disable
        --runtime-config=v1alpha1=false
        
        # 특정 API version enable
        --runtime-config=rbac.authorization.k8s.io/v1alpha1
        ```
        
    - kubectl convert
        
        kubectl convert : 쿠버네티스 커맨드 라인 도구인 `kubectl`의 플러그인으로서, 특정 버전의 쿠버네티스 API로 작성된 매니페스트를 다른 버전으로 변환할 수 있도록 한다.
        
        - Install(https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/#install-kubectl-convert-plugin)
        
        ```bash
        curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl-convert"
        sudo install -o root -g root -m 0755 kubectl-convert /usr/local/bin/kubectl-convert
        kubectl convert --help
        ```
        
        - 특정 버전으로 파드 생성(https://kubernetes.io/docs/reference/using-api/deprecation-guide/#migrate-to-non-deprecated-apis)
        
        ```bash
        
        ```
        
    - helm
        
        helm 설치
        
        ```bash
        # ubuntu
        curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
        sudo apt-get install apt-transport-https --yes
        echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
        sudo apt-get update
        sudo apt-get install helm
        ```
        
        helm 명령어
        
        ```bash
        # helm install
        helm install bravo bitnami/drupal
        
        # search
        helm search repo 
        helm search hub
        
        # helm release
        helm list
        
        # helm repo
        helm repo list
        helm repo add
        
        # 설치만 하고 실행 X
        helm pull --untar bitnami/apache
        
        ```
        
    - Lightning Labs2
        - liveness/readiness probe
            
            ```bash
            We have deployed a few pods in this cluster in various namespaces. Inspect them and identify the pod which is not in a Ready state. Troubleshoot and fix the issue.
            
            Next, add a check to restart the container on the same pod if the command ls /var/www/html/file_check fails. This check should start after a delay of 10 seconds and run every 60 seconds.
            
            You may delete and recreate the object. Ignore the warnings from the probe.
            ```
            
            ```bash
            spec:
              containers:
              - image: kodekloud/nginx
                imagePullPolicy: IfNotPresent
                name: nginx
                ports:
                - containerPort: 9080
                  protocol: TCP
                readinessProbe:
                  failureThreshold: 3
                  httpGet:
                    path: /
                    port: 9080
                    scheme: HTTP
                  periodSeconds: 10
                  successThreshold: 1
                  timeoutSeconds: 1
                livenessProbe:
                  exec:
                    command:
                    - ls
                    - /var/www/html/file_check
                  initialDelaySeconds: 10
                  periodSeconds: 60
            ```
            
        - cronjob
            
            ```bash
            Create a cronjob called dice that runs every one minute. Use the Pod template located at /root/throw-a-dice. The image throw-dice randomly returns a value between 1 and 6. The result of 6 is considered success and all others are failure.
            
            The job should be non-parallel and complete the task once. Use a backoffLimit of 25.
            
            If the task is not completed within 20 seconds the job should fail and pods should be terminated.
            
            You don't have to wait for the job completion. As long as the cronjob has been created as per the requirements.
            ```
            
            ```bash
            apiVersion: batch/v1
            kind: CronJob
            metadata:
              name: dice
            spec:
              schedule: "*/1 * * * *"
              jobTemplate:
                spec:
                  completions: 1
                  backoffLimit: 25 # This is so the job does not quit before it succeeds.
                  activeDeadlineSeconds: 20
                  template:
                    spec:
                      containers:
                      - name: dice
                        image: kodekloud/throw-dice
                      restartPolicy: Never
            ```
            
        - ingress
            
            ```bash
            Create a single ingress resource called ingress-vh-routing. The resource should route HTTP traffic to multiple hostnames as specified below:
            
            The service video-service should be accessible on http://watch.ecom-store.com:30093/video
            
            The service apparels-service should be accessible on http://apparels.ecom-store.com:30093/wear
            
            Here 30093 is the port used by the Ingress Controller
            ```
            
            ```bash
            ---
            kind: Ingress
            apiVersion: networking.k8s.io/v1
            metadata:
              name: ingress-vh-routing
              annotations:
                nginx.ingress.kubernetes.io/rewrite-target: /
            spec:
              rules:
              - host: watch.ecom-store.com
                http:
                  paths:
                  - pathType: Prefix
                    path: "/video"
                    backend:
                      service:
                        name: video-service
                        port:
                          number: 8080
              - host: apparels.ecom-store.com
                http:
                  paths:
                  - pathType: Prefix
                    path: "/wear"
                    backend:
                      service:
                        name: apparels-service
                        port:
                          number: 8080
            ```
            
        - 
    - Mock Exams2
        
        ```bash
        Create a new Ingress Resource for the service my-video-service to be made available at the URL: http://ckad-mock-exam-solution.com:30093/video.
        
        To create an ingress resource, the following details are: -
        
        annotation: nginx.ingress.kubernetes.io/rewrite-target: /
        
        host: ckad-mock-exam-solution.com
        
        path: /video
        
        Once set up, the curl test of the URL from the nodes should be successful: HTTP 200
        ```
        
        ```bash
        kubectl create ingress ingress --rule="ckad-mock-exam-solution.com/video*=my-video-service:8080" --dry-run=client -oyaml > ingress.yaml
        
        apiVersion: networking.k8s.io/v1
        kind: Ingress
        metadata:
          annotations:
            nginx.ingress.kubernetes.io/rewrite-target: /
          name: ingress
        spec:
          rules:
          - host: ckad-mock-exam-solution.com
            http:
              paths:
              - backend:
                  service:
                    name: my-video-service
                    port:
                      number: 8080
                path: /video
                pathType: Prefix
        
        ```
        
        ```bash
        controlplane ~ ➜  k create ing sss --rule="ckad-mock-exam-solution.com/video=my-video-service:8080" --dry-run=client -o yaml
        apiVersion: networking.k8s.io/v1
        kind: Ingress
        metadata:
          creationTimestamp: null
          name: sss
        spec:
          rules:
          - host: ckad-mock-exam-solution.com
            http:
              paths:
              - backend:
                  service:
                    name: my-video-service
                    port:
                      number: 8080
                path: /video
                pathType: Exact
        status:
          loadBalancer: {}
        
        controlplane ~ ➜  k create ing sss --rule="ckad-mock-exam-solution.com/video*=my-video-service:8080" --dry-run=client -o yaml
        apiVersion: networking.k8s.io/v1
        kind: Ingress
        metadata:
          creationTimestamp: null
          name: sss
        spec:
          rules:
          - host: ckad-mock-exam-solution.com
            http:
              paths:
              - backend:
                  service:
                    name: my-video-service
                    port:
                      number: 8080
                path: /video
                pathType: Prefix
        status:
          loadBalancer: {}
        ```
        
    - ingress
        
        ```bash
        There are existing Pods in Namespace space1 and space2 .
        
        We need a new NetworkPolicy named np that restricts all Pods in Namespace space1 to only have outgoing traffic to Pods in Namespace space2 . Incoming traffic not affected.
        
        The NetworkPolicy should still allow outgoing DNS traffic on port 53 TCP and UDP.
        ```
        
        ```bash
        apiVersion: networking.k8s.io/v1
        kind: NetworkPolicy
        metadata:
          name: np
          namespace: space1
        spec:
          podSelector: {}
          policyTypes:
          - Egress
          egress:
          - ports:
            - port: 53
              protocol: TCP
            - port: 53
              protocol: UDP
          - to:
             - namespaceSelector:
                matchLabels:
                 kubernetes.io/metadata.name: space2
        ```
        
        ```bash
        # these should work
        k -n space1 exec app1-0 -- curl -m 1 microservice1.space2.svc.cluster.local
        k -n space1 exec app1-0 -- curl -m 1 microservice2.space2.svc.cluster.local
        k -n space1 exec app1-0 -- nslookup tester.default.svc.cluster.local
        k -n space1 exec app1-0 -- nslookup killercoda.com
        
        # these should not work
        k -n space1 exec app1-0 -- curl -m 1 tester.default.svc.cluster.local
        k -n space1 exec app1-0 -- curl -m 1 killercoda.com
        ```
        
    - 패캠
        
        [Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/73de592f-7a03-4db7-85b5-3f5ff0d5aa0f/Untitled.pdf)
        
- 실습
    - 문제풀이 프로세스
        
        cheatsheet : https://kubernetes.io/ko/docs/reference/kubectl/cheatsheet/
        
        reference docs : https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands
        
        문제 마다  클러스터 확인 후 설정
        
        ```bash
        k config current-context
        k config use-context <cluster>
        
        # 네임스페이스 설정
        k config set-context --current --namespace=<ns>
        
        # root 유저 전환
        sudo -i
        ```
        
        오브젝트 수정 시 백업본 만들어놓기 (`k get po -o yaml > pod-backup.yaml`)
        
        생성 전 dry-run 해보기(`k create ~ --dry-run=client`)
        
        로그 확인
        
        - `crictl ps -a`
        - `journalctl -xe`
        
        - ETCD 스냅샷 백업
            
            ```bash
            # 0. ETCD 서버 접근
            
            # 1. 정보 확인
            cat /etc/kubernetes/manifests/etcd.yaml | grep file
            
            # 2. 백업
            sudo ETCDCTL_API=3 etcdctl \
            --endpoints=https://127.0.0.1:2379 \
            --cacert=<cacert> \
            --cert=<cert> \
            --key=<key> \
            snapshot save <file path>
            ```
            
        - ETCD 스냅샷 복구
            
            stacked ETCD
            
            ```bash
            # 0. ETCD 노드 접근
            
            # 1. ETCD 스냅샷 복구
            sudo ETCDCTL_API=3 etcdctl \
            --data-dir=<new etcd data dir> \
            snapshot restore <file path>
            
            # 2. data volume dir 수정
            sudo vi /etc/kubernetes/manifests/etcd.yaml
            => .volumes.hostPath.path 수정
            
            # 3. ETCD 재시작 확인
            crictl ps -a | grep etcd
            => running 확인
            ```
            
            External ETCD
            
            ```bash
            # 0. ETCD 서버 접근
            마스터 노드에서 ps -ef | grep kube 으로 etcd 서버 확인
            
            # 1. ETCD 스냅샷 복구
            sudo ETCDCTL_API=3 etcdctl \
            --data-dir=<new etcd data dir> \
            snapshot restore <file path>
            
            # 2. 스냅샷 디렉터리 권한 수정
            sudo chown -R etcd:etcd <snapshot dir>
            
            # 3. etcd --data-dir 수정
            sudo vi /etc/systemd/system/etcd.service
            => --data-dir=<> 수정
            
            # 4. 재시작
            sudo systemctl daemon-reload
            sudo systemctl restart etcd
            ```
            
        - 클러스터 업그레이드
            1. controlplane 노드 업그레이드
                
                ```bash
                # 1. kubeadm 업그레이드
                apt update
                apt install <>
                kubeadm version
                
                kubeadm upgrade plan v1.29.0
                kubeadm upgrade apply v1.29.0
                
                # 2. 노드 드레인
                k drain --ignore-daemonsets controlplane
                
                # 3. kubectl, kubelet 업그레이드
                apt install <>
                
                kubectl version
                kubelet --version
                
                # 4. 데몬/kubelet 재시작
                sudo systemctl daemon-reload
                sudo systemctl restart kubelet
                
                # 5. 노드 uncordon
                k uncordon controlplane
                ```
                
            2.  워커노드 업그레이드
                
                ```bash
                # 0. 워커노드 서버 접근
                
                # 1. kubeadm 업그레이드
                apt update
                apt install <>
                kubeadm version
                
                kubeadm upgrade node
                
                # 2. 노드 드레인
                k drain --ignore-daemonsets <node>
                
                # 3. kubectl, kubelet 업그레이드
                apt install <>
                
                kubectl version
                kubelet --version
                
                # 4. 데몬/kubelet 재시작
                sudo systemctl daemon-reload
                sudo systemctl restart kubelet
                
                # 5. 노드 uncordon
                k uncordon <node>
                ```
                
        - deployment 롤링업데이트/롤백
            
            rolling update
            
            ```bash
            k set image deploy <deploy> <container>=<image>:<tag>
            ```
            
            rollback
            
            ```bash
            k rollout history deploy <>
            
            k rollout undo deploy <>
            ```
            
        - 노드 스케줄링/관리
            
            ```bash
            # 스케줄링 중단
            # 기존 할당된 파드는 영향 X
            k cordon <node>
            
            # 스케줄링 재개
            k uncordon <node>
            
            # 노드 드레인
            k drain --ignore-daemonsets <node>
            ```
            
        - 클러스터 리소스 모니터링
            
            ```bash
            # pod 리소스 모니터링
            k top po --sort-by=<cpu | memory>
            K get po --sort-by=.metadata.name
            
            # node 리소스 모니터링
            k top no --sort-by=<cpu | memory>
            
            # pv 
            k get pv --sort-by=.spec.capacity.storage
            
            ```
            
        - 마스터노드 트러블슈팅
            
            static pod config file : `/etc/kubernetes/manifests/` 
            
            `systemctl restart` 할 경우, `enable --now` 를 추가해서 활성화 유지 설정
            
        - 워커노드 트러블슈팅
            
            <aside>
            ☑️ 확인사항
            1. runtime 동작 여부
            
            > Installing Runtime
            > 
            > - Runtime : Path to Unix domain socket
            > - Docker Engine : /var/run/dockershim.sock
            > - containerd : /run/containerd/containerd.sock
            > - CRI-O : /var/run/crio/crio.sock
            
            2. kubelet, kube-proxy 동작 여부
            3. CNI 확인 
            
            </aside>
            
            서비스 영구 활성화 : `systemctl enable --now <>` 
            
        - 인증서/CSR/role 생성 및 rolebinding
            
            인증서를 제공해줄 경우
            
            ```bash
            # 1. CSR 오브젝트 생성
            cat john.csr | base64 | tr -d "\n"
            => 출력내용 csr.yaml 의 request 에 붙여넣기)
            
            vi csr.yaml
            
            apiVersion: certificates.k8s.io/v1
            kind: CertificateSigningRequest
            metadata:
              name: john-developer 
            spec:
              request: LS0tLS1CRUdJTiBDRVJUSUZJQ0FURSBSRVFVRVNULS0tLS0KTUlJQ1ZqQ0NBVDRDQVFBd0VURVBNQTBHQTFVRUF3d0dZVzVuWld4aE1JSUJJakFOQmdrcWhraUc5dzBCQVFFRgpBQU9DQVE4QU1JSUJDZ0tDQVFFQTByczhJTHRHdTYxakx2dHhWTTJSVlRWMDNHWlJTWWw0dWluVWo4RElaWjBOCnR2MUZtRVFSd3VoaUZsOFEzcWl0Qm0wMUFSMkNJVXBGd2ZzSjZ4MXF3ckJzVkhZbGlBNVhwRVpZM3ExcGswSDQKM3Z3aGJlK1o2MVNrVHF5SVBYUUwrTWM5T1Nsbm0xb0R2N0NtSkZNMUlMRVI3QTVGZnZKOEdFRjJ6dHBoaUlFMwpub1dtdHNZb3JuT2wzc2lHQ2ZGZzR4Zmd4eW8ybmlneFNVekl1bXNnVm9PM2ttT0x1RVF6cXpkakJ3TFJXbWlECklmMXBMWnoyalVnald4UkhCM1gyWnVVV1d1T09PZnpXM01LaE8ybHEvZi9DdS8wYk83c0x0MCt3U2ZMSU91TFcKcW90blZtRmxMMytqTy82WDNDKzBERHk5aUtwbXJjVDBnWGZLemE1dHJRSURBUUFCb0FBd0RRWUpLb1pJaHZjTgpBUUVMQlFBRGdnRUJBR05WdmVIOGR4ZzNvK21VeVRkbmFjVmQ1N24zSkExdnZEU1JWREkyQTZ1eXN3ZFp1L1BVCkkwZXpZWFV0RVNnSk1IRmQycVVNMjNuNVJsSXJ3R0xuUXFISUh5VStWWHhsdnZsRnpNOVpEWllSTmU3QlJvYXgKQVlEdUI5STZXT3FYbkFvczFqRmxNUG5NbFpqdU5kSGxpT1BjTU1oNndLaTZzZFhpVStHYTJ2RUVLY01jSVUyRgpvU2djUWdMYTk0aEpacGk3ZnNMdm1OQUxoT045UHdNMGM1dVJVejV4T0dGMUtCbWRSeEgvbUNOS2JKYjFRQm1HCkkwYitEUEdaTktXTU0xMzhIQXdoV0tkNjVoVHdYOWl4V3ZHMkh4TG1WQzg0L1BHT0tWQW9FNkpsYWFHdTlQVmkKdjlOSjVaZlZrcXdCd0hKbzZXdk9xVlA3SVFjZmg3d0drWm89Ci0tLS0tRU5EIENFUlRJRklDQVRFIFJFUVVFU1QtLS0tLQo=
              signerName: kubernetes.io/kube-apiserver-client
              usages:
              - client auth
             
            # 2. approve
            k certificate approve john-developer
            
            # 3. role 생성
            k create role <> --verb=get,list --resource=pod,deployment --namespace=<>
            
            # 4. rolebinding 생성
            k create rolebinding <> --role=<role> --user=<> --namespace=<>
            
            # 5. 확인
            k can-i update po --as=<user> -n=<namespace>
            ```
            
            인증서까지 생성
            
            ```bash
            # 1. key/CSR 생성
            openssl genrsa -out john.key 2048
            
            openssl req -new -key john.key -out john.csr -subj "/CN=john"
            
            cat john.csr | base64 | tr -d "\n"
            => 출력내용 아래 csr.yaml 의 request 에 붙여넣기)
            
            # 2. CSR 생성
            vi csr.yaml
            
            apiVersion: certificates.k8s.io/v1
            kind: CertificateSigningRequest
            metadata:
              name: john-developer 
            spec:
              request: LS0tLS1CRUdJTiBDRVJUSUZJQ0FURSBSRVFVRVNULS0tLS0KTUlJQ1ZqQ0NBVDRDQVFBd0VURVBNQTBHQTFVRUF3d0dZVzVuWld4aE1JSUJJakFOQmdrcWhraUc5dzBCQVFFRgpBQU9DQVE4QU1JSUJDZ0tDQVFFQTByczhJTHRHdTYxakx2dHhWTTJSVlRWMDNHWlJTWWw0dWluVWo4RElaWjBOCnR2MUZtRVFSd3VoaUZsOFEzcWl0Qm0wMUFSMkNJVXBGd2ZzSjZ4MXF3ckJzVkhZbGlBNVhwRVpZM3ExcGswSDQKM3Z3aGJlK1o2MVNrVHF5SVBYUUwrTWM5T1Nsbm0xb0R2N0NtSkZNMUlMRVI3QTVGZnZKOEdFRjJ6dHBoaUlFMwpub1dtdHNZb3JuT2wzc2lHQ2ZGZzR4Zmd4eW8ybmlneFNVekl1bXNnVm9PM2ttT0x1RVF6cXpkakJ3TFJXbWlECklmMXBMWnoyalVnald4UkhCM1gyWnVVV1d1T09PZnpXM01LaE8ybHEvZi9DdS8wYk83c0x0MCt3U2ZMSU91TFcKcW90blZtRmxMMytqTy82WDNDKzBERHk5aUtwbXJjVDBnWGZLemE1dHJRSURBUUFCb0FBd0RRWUpLb1pJaHZjTgpBUUVMQlFBRGdnRUJBR05WdmVIOGR4ZzNvK21VeVRkbmFjVmQ1N24zSkExdnZEU1JWREkyQTZ1eXN3ZFp1L1BVCkkwZXpZWFV0RVNnSk1IRmQycVVNMjNuNVJsSXJ3R0xuUXFISUh5VStWWHhsdnZsRnpNOVpEWllSTmU3QlJvYXgKQVlEdUI5STZXT3FYbkFvczFqRmxNUG5NbFpqdU5kSGxpT1BjTU1oNndLaTZzZFhpVStHYTJ2RUVLY01jSVUyRgpvU2djUWdMYTk0aEpacGk3ZnNMdm1OQUxoT045UHdNMGM1dVJVejV4T0dGMUtCbWRSeEgvbUNOS2JKYjFRQm1HCkkwYitEUEdaTktXTU0xMzhIQXdoV0tkNjVoVHdYOWl4V3ZHMkh4TG1WQzg0L1BHT0tWQW9FNkpsYWFHdTlQVmkKdjlOSjVaZlZrcXdCd0hKbzZXdk9xVlA3SVFjZmg3d0drWm89Ci0tLS0tRU5EIENFUlRJRklDQVRFIFJFUVVFU1QtLS0tLQo=
              signerName: kubernetes.io/kube-apiserver-client
              usages:
              - client auth
              
            # 3. approve
            k certificate approve john-developer
            
            # 4. 인증서(CRT) 생성
            kubectl get csr john -o jsonpath='{.status.certificate}'| base64 -d > john.crt
            
            # 5. role 생성
            k create role developer --verb=get,list,create,update,delete --resource=pod --namespace=development
            
            # 7. rolebinding 생성
            k create rolebinding john-binding --role=developer --user=john --namespace=development
            
            # 8. kubeconfig(user) 등록
            k config set-credentials john --client-key=john.key --client-certificate=john.crt --embed-certs=true
            
            # 9. context 추가
            k config set-context john --cluster=kubernetes --user=john
            
            # 10. check
            k auth can-i update po --as=john -n=development
            또는
            k config use-context john
            k get po
            k get pv => 권한이 없어야 함
            ```
            
        - static pod
            
            `/etc/kubernetes/manifests/` 아래에 파일 생성 시 정적 파드로 생성됨
            
            파드명은 파드명-노드명 으로 생성됨(변경 불가)
            
            워커 노드의 static pod path 는 /var/lib/kubelet/config.yaml 의 static pod path 확인
            
        - secret 생성
            
            using file
            
            ```bash
            apiVersion: v1
            kind: Secret
            metadata:
              name: mysecret
            type: Opaque
            data:
              username: YWRtaW4=
              password: MWYyZDFlMmU2N2Rm
            ```
            
            using kubectl
            
            ```bash
            k create secret generic <secret> \
            --from-literal=username=<> \
            --from-literal=password=<>
            ```
            
        - configmap 생성
            
            using cli
            
            ```bash
            k create cm <cm> --from-literal=PROD=dev
            ```
            
            using file
            
            ```bash
            apiVersion: v1
            kind: ConfigMap
            metadata:
              name: special-config
            data:
              special.how: very
              special.type: charm
            ```
            
        - certificate file
            
            certificate check : `openssl x509 -in file-path.crt -text -noout`
            
            api server
            
            - certificate file : `--tls-cert-file=/etc/kubernetes/pki/apiserver.crt`
            - certificate file apiserver as a client to etcd server : `--etcd-certfile=/etc/kubernetes/pki/apiserver-etcd-client.crt`
            - key apiserver to kubelet server : `--kubelet-client-key=/etc/kubernetes/pki/apiserver-kubelet-client.key`
            
            etcd
            
            - etcd certificate file used to host etcd server : `--cert-file=/etc/kubernetes/pki/etcd/server.crt`
            - etcd ca root certificate : `--trusted-ca-file=/etc/kubernetes/pki/etcd/ca.crt`
        - RBAC
            
            node authorization 확인 : `--authorization-mode=Node,RBAC`
            
        - kube-proxy 트러블슈팅
            
            네트워크가 안될 때 확인
            
            ```bash
            # 1. configmap 확인
            => configmap 의 data 에 파일명 확인
            Data
            ====
            config.conf:
            ----
            
            # 2. kube-proxy ds 의 config dir 이 1 과 일치하는지 확인
                spec:
                  containers:
                  - command:
                    - /usr/local/bin/kube-proxy
                    - --config=/var/lib/kube-proxy/config.conf
            ```
            
        - 파드 및 서비스 생성 후 dns lookup 하기
            
            nginx 파드 및 internal service 생성 후 dns lookup 정보 저장하기
            
            ```bash
            # 1. pod create
            k run nginx --image=nginx
            k get po -o wide
            => pod ip 확인
            
            # 2. expose
            k expose po nginx --name=nginx-service --port=80
            
            # 3. test pod create & nslookup
            k run test-pod --image=busybox:1.28 -- sleep 4000
            
            k exec test-pod -- nslookup nignx-service > file
            k exec test-pod -- nslookup <pod-ip>.<ns>.pod.cluster.local > file
            ```
            
        - jsonpath
            
            ```bash
            k get po -o json | jq -c 'paths'
            
            # container env 의 value 가 ad1 인 컨테이너의 env 이름 출력
            k get po vongole-dev-default-876899fdc-pz8k9 -o jsonpath="{.spec.containers[*].env[?(@.value=='ad1')].name}"
            
            ```
            
        - pod 생성 시 command 넣기
            
            ```bash
            k run busybox --image=busybox -- sleep 4000
            ```
            
        - ingress
            
            
        - network policy
            
            Security → Practice Test Network Policies
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/9ee91a2e-cbbb-4c8e-a009-01976b4211ef/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/706d7cc1-8c60-41c2-b2f7-cef8011d84e1/Untitled.png)
            
            ```bash
            apiVersion: networking.k8s.io/v1
            kind: NetworkPolicy
            metadata:
              name: internal-policy
              namespace: default
            spec:
              podSelector:
                matchLabels:
                  name: internal
              policyTypes:
              - Egress
              - Ingress
              ingress:
                - {}
              egress:
              - to:
                - podSelector:
                    matchLabels:
                      name: mysql
                ports:
                - protocol: TCP
                  port: 3306
            
              - to:
                - podSelector:
                    matchLabels:
                      name: payroll
                ports:
                - protocol: TCP
                  port: 8080
            
              - ports:
                - port: 53
                  protocol: UDP
                - port: 53
                  protocol: TCP
                  
                  
            Spec:
              PodSelector:     name=internal
              Allowing ingress traffic:
                To Port: <any> (traffic allowed to all ports)
                From: <any> (traffic not restricted by source)
              Allowing egress traffic:
                To Port: 3306/TCP
                To:
                  PodSelector: name=mysql
                ----------
                To Port: 8080/TCP
                To:
                  PodSelector: name=payroll
                ----------
                To Port: 53/UDP
                To Port: 53/TCP
                To: <any> (traffic not restricted by destination)
              Policy Types: Egress, Ingress
            ```
            
        - 클러스터에 노드 추가
            
            ```bash
            # 1. controlplane 노드에서 실행
            kubeadm token create --print-join-command
            
            # 2. 추가할 노드에서 실행
            => 1에서 얻은 명령어
            ```
            
        - 
        
    - mock exams
        - 1번
            
            - 1, 5 오답
            
            kubectl expose pod messaging --port=6379 --name messaging-service
            
        - 2
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/9b3f7466-62b6-4ac4-a993-4d70678de183/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/c991acc3-8d45-4aea-b4ec-d26fca7cd747/Untitled.png)
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/673597e1-88a1-4568-9294-0112769b85f3/Untitled.png)
            
    - 오답풀이
        
        ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/0541d7ec-60a6-4613-869f-68da1816b296/Untitled.png)
        
        - 정답
            
            ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/f4131506-ae9e-48aa-a40d-5d282099e108/Untitled.png)
            
        
    - me 3-5
        
        ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/a4a07cd9-01b4-44a2-9ab4-507f6981925c/Untitled.png)
        
    - me-3-2
        
        ![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/53b32102-d276-456e-b23f-e0b1f68d6753/8d92b537-7806-450c-a580-2d127d73fb29/Untitled.png)
        
- killer.sh
    - Killer 문제
        1. The DevOps team would like to get the list of all *Namespaces* in the cluster. Get the list and save it to `/opt/course/1/namespaces`.
        2. Create a single *Pod* of image `httpd:2.4.41-alpine` in *Namespace* `default`. The *Pod* should be named `pod1` and the container should be named `pod1-container`. 
        Your manager would like to run a command manually on occasion to output the status of that exact *Pod*. Please write a command that does this into `/opt/course/2/pod1-status-command.sh`. The command should use `kubectl`.
        3. Team Neptune needs a *Job* template located at `/opt/course/3/job.yaml`. This *Job* should run image `busybox:1.31.0` and execute `sleep 2 && echo done`. It should be in namespace `neptune`, run a total of 3 times and should execute 2 runs in parallel.
        Start the *Job* and check its history. Each pod created by the *Job* should have the label `id: awesome-job`. The job should be named `neb-new-job` and the container `neb-new-job-container`.
        4. Team Mercury asked you to perform some operations using Helm, all in *Namespace* `mercury`:
            1. Delete release `internal-issue-report-apiv1`
            2. Upgrade release `internal-issue-report-apiv2` to any newer version of chart `bitnami/nginx` available
            3. Install a new release `internal-issue-report-apache` of chart `bitnami/apache`. The *Deployment* should have two replicas, set these via Helm-values during install
            4. There seems to be a broken release, stuck in `pending-install` state. Find it and delete it
        5. Team Neptune has its own *ServiceAccount* named `neptune-sa-v2` in *Namespace* `neptune`. A coworker needs the token from the *Secret* that belongs to that *ServiceAccount*. Write the base64 decoded token to file `/opt/course/5/token`.
        6. Create a single *Pod* named `pod6` in *Namespace* `default` of image `busybox:1.31.0`. The *Pod* should have a readiness-probe executing `cat /tmp/ready`. It should initially wait 5 and periodically wait 10 seconds. This will set the container ready only if the file `/tmp/ready` exists.
        The *Pod* should run the command `touch /tmp/ready && sleep 1d`, which will create the necessary file to be ready and then idles. Create the *Pod* and confirm it starts.
        7. The board of Team Neptune decided to take over control of one e-commerce webserver from Team Saturn. The administrator who once setup this webserver is not part of the organisation any longer. All information you could get was that the e-commerce system is called `my-happy-shop`.
        Search for the correct *Pod* in *Namespace* `saturn` and move it to *Namespace* `neptune`. It doesn't matter if you shut it down and spin it up again, it probably hasn't any customers anyways.
        8. There is an existing *Deployment* named `api-new-c32` in *Namespace* `neptune`. A developer did make an update to the *Deployment* but the updated version never came online. Check the *Deployment* history and find a revision that works, then rollback to it. Could you tell Team Neptune what the error was so it doesn't happen again?
        9. In *Namespace* `pluto` there is single *Pod* named `holy-api`. It has been working okay for a while now but Team Pluto needs it to be more reliable.
        Convert the *Pod* into a *Deployment* named `holy-api` with 3 replicas and delete the single *Pod* once done. The raw *Pod* template file is available at `/opt/course/9/holy-api-pod.yaml`.
        In addition, the new *Deployment* should set `allowPrivilegeEscalation: false` and `privileged: false` for the security context on container level.
        Please create the *Deployment* and save its yaml under `/opt/course/9/holy-api-deployment.yaml`.
        10. Team Pluto needs a new cluster internal *Service*. Create a ClusterIP *Service* named `project-plt-6cc-svc` in *Namespace* `pluto`. 
        This *Service* should expose a single *Pod* named `project-plt-6cc-api` of image `nginx:1.17.3-alpine`, create that *Pod* as well. The *Pod* should be identified by label `project: plt-6cc-api`. The *Service* should use tcp port redirection of `3333:80`.
        Finally use for example `curl` from a temporary `nginx:alpine` *Pod* to get the response from the *Service*. Write the response into `/opt/course/10/service_test.html`. 
        Also check if the logs of *Pod* `project-plt-6cc-api` show the request and write those into `/opt/course/10/service_test.log`.
        11. During the last monthly meeting you mentioned your strong expertise in container technology. Now the Build&Release team of department Sun is in need of your insight knowledge. There are files to build a container image located at `/opt/course/11/image`. The container will run a Golang application which outputs information to stdout. You're asked to perform the following tasks:
        | NOTE: Make sure to run all commands as user k8s, for docker use sudo docker
        Change the Dockerfile. The value of the environment variable `SUN_CIPHER_ID` should be set to the hardcoded value `5b9c1065-e39d-4a43-a04a-e59bcea3e03f`
        Build the image using Docker, named `registry.killer.sh:5000/sun-cipher`, tagged as `latest` and `v1-docker`, push these to the registry
        Build the image using Podman, named `registry.killer.sh:5000/sun-cipher`, tagged as `v1-podman`, push it to the registry
        Run a container using Podman, which keeps running in the background, named `sun-cipher` using image `registry.killer.sh:5000/sun-cipher:v1-podman`. 
        Run the container from `k8s@terminal` and not `root@terminal`
        Write the logs your container `sun-cipher` produced into `/opt/course/11/logs`. Then write a list of all running Podman containers into `/opt/course/11/containers`
        12. Create a new *PersistentVolume* named `earth-project-earthflower-pv`. It should have a capacity of *2Gi*, accessMode *ReadWriteOnce*, hostPath `/Volumes/Data` and no storageClassName defined.
        Next create a new *PersistentVolumeClaim* in *Namespace* `earth` named `earth-project-earthflower-pvc` . It should request *2Gi* storage, accessMode *ReadWriteOnce* and should not define a storageClassName. The *PVC* should bound to the *PV* correctly.
        Finally create a new *Deployment* `project-earthflower` in *Namespace* `earth` which mounts that volume at `/tmp/project-data`. The *Pods* of that *Deployment* should be of image `httpd:2.4.41-alpine`.
        13. Team Moonpie, which has the *Namespace* `moon`, needs more storage. Create a new *PersistentVolumeClaim* named `moon-pvc-126` in that namespace. 
        This claim should use a new *StorageClass* `moon-retain` with the *provisioner* set to `moon-retainer` and the *reclaimPolicy* set to *Retain*. The claim should request storage of *3Gi*, an *accessMode* of *ReadWriteOnce* and should use the new *StorageClass*.
        The provisioner `moon-retainer` will be created by another team, so it's expected that the *PVC* will not boot yet. Confirm this by writing the log message from the *PVC* into file `/opt/course/13/pvc-126-reason`.
        14. You need to make changes on an existing *Pod* in *Namespace* `moon` called `secret-handler`. Create a new *Secret* `secret1` which contains `user=test` and `pass=pwd`. 
        The *Secret*'s content should be available in *Pod* `secret-handler` as environment variables `SECRET1_USER` and `SECRET1_PASS`. The yaml for *Pod* `secret-handler` is available at `/opt/course/14/secret-handler.yaml`.
        There is existing yaml for another *Secret* at `/opt/course/14/secret2.yaml`, create this *Secret* and mount it inside the same *Pod* at `/tmp/secret2`. Your changes should be saved under `/opt/course/14/secret-handler-new.yaml`. 
        Both *Secrets* should only be available in *Namespace* `moon`.
        15. 
    - killer 오답노트
        - helm 활용
            
            ```bash
            1. Delete release internal-issue-report-apiv1
            2. Upgrade release internal-issue-report-apiv2 to any newer version of chart bitnami/nginx available
            3. Install a new release internal-issue-report-apache of chart bitnami/apache. The Deployment should have two replicas, set these via Helm-values during install
            4. There seems to be a broken release, stuck in pending-install state. Find it and delete it
            ```
            
            ```bash
            1.
            - helm -n mercury uninstall internal-issue-report-apiv1
            
            2. 
            - helm repo list
            - helm repo update
            - helm search repo nginx
            - helm -n mercury update internal-issue-apiv2 bitnami/nginx
            
            3. 
            - helm show values bitnami/apache | yq e
            - helm -n mercury install internal-issue-report-apache bitnami/apache --set replicaCount=2
            or
            - helm -n mercury install internal-issue-report-apache bitnmai/apache \
            	--set replicaCount=2 \
            	--set image.debug=true
            	
            4.
            - helm list -a -n mercury
            - helm -n mercury uninstall internal-issue-report-daniel
            ```
            
        - secret token 디코딩 후 파일에 저장하기
            
            ```bash
            Team Neptune has its own ServiceAccount named neptune-sa-v2 in Namespace neptune. 
            A coworker needs the token from the Secret that belongs to that ServiceAccount. 
            Write the base64 decoded token to file /opt/course/5/token.
            ```
            
            ```bash
            # sa 에 설정된 secret 확인
            - k describe sa -n neptune neptune-sa-v2 > Tokens 확인
            
            # secret 의 token 확인 및 디코딩 후 파일에 저장
            - k get secret -n neptune neptune secret-1 -o yaml 
            - echo '{token}' | base64 -d > /opt/course/5/token
            ```
            
        - 컨피그맵 활용 *#문제 꼼꼼히 읽기*
            
            ```bash
            Team Moonpie has a nginx server Deployment called web-moon in Namespace moon. Someone started configuring it but it was never completed. 
            To complete please create a ConfigMap called configmap-web-moon-html containing the content of file /opt/course/15/web-moon.html under the data key-name index.html.
            The Deployment web-moon is already configured to work with this ConfigMap and serve its content. Test the nginx configuration for example using curl from a temporary nginx:alpine Pod.
            ```
            
            ```bash
            # 파일명 지정해서 컨피그맵 생성(web-moon.html 파일을 컨피그맵 안에서 index.html 로 저장)
            k create cm -n <> <cm> --from-file=index.html=/opt/course/15/web-moon.html
            
            ```
            
        - liveness probe
            
            ```bash
            Implement a liveness-probe which checks the container to be reachable on port 80. 
            Initially the probe should wait 10, periodically 15 seconds.
            ```
            
            이런식으로 포트만 주어진다면 tcpSocket 사용.
            
            initialDelaySeconds 등 추가 옵션 잊지 말기
            
        - pod 를 deployment 로 변경하기
            
            레이블도 잘 확인할 것
            
    
    [Killer.sh](https://www.notion.so/Killer-sh-328477f985738089ba04f09cf76caebc?pvs=21)
    

## 시험문제 복기

- 1차
    1. Network Policy
        1. echo 네임스페이스에 Network Policy 생성
        2. corp-net 네임스페이스의 파드에서 echo 네임스페이스로 트래픽을 허용하도록
    2. ETCD 백업&복구
    3. 멀티 컨테이너
    4. 스테이트풀셋 replica 조정 + record 포함
    5. 파드 생성
    6. RBAC
        1. clusterrole 생성하여 네임스페이스에만 적용되도록
        2. clusterrole + rolebinding
    7. 마스터노드 업그레이드 (1.29.0 → 1.29.1)
    8. 마스터노드 트러블슈팅
        1. kubelet 재시작
    9. 노드 수 확인하여 파일에 저장하기
        1. taints 에 NoSchedule 이 있는 노드가 있다면 제외
    10. 파드 로그 중 에러가 포함된 라인 파일에 저장하기
    11. static pod 생성
    12. pvc 생성하여 파드에 볼륨마운트
    13. secret 생성하여 파드에 환경변수/볼륨으로 마운트
    14. 노드포트 서비스 생성
    15. 멀티 컨테이너
        1. 파드에 컨테이너를 새로 추가하여 기존 컨테이너의 로그 볼륨 연결
    16. 디플로이먼트 생성
    17. 서비스 생성
