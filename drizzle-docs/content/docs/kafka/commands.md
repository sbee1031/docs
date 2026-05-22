---
date: '2026-05-21T15:18:35+09:00'
draft: false
title: 'Kafka 명령어 모음'
---

>인증이 설정된 경우 명령어에  `--command-config=<auth file>` 추가

## kafka-topics.sh

토픽 조회

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --list
```

토픽 상세 조회

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --describe --topic <topic>
```

토픽 생성

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --create --topic <topic> --partitions <partition> --replication-factor <replicas>
```

토픽 삭제

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --delete --topic <topic>
```

토픽 URP 조회

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --describe --under-replicated-partitions
```

토픽 URP 조회

```
kafka-topics.sh --bootstrap-server <bootstrap-server> --describe --under-min-isr-partitions 
```

## kafka-configs.sh

토픽 retention 설정

```
kafka-configs.sh --bootstrap-server <bootstrap-server> --alter --entity-type topics --entity-name <topic> --add-config retention.ms=<retention>
```

토픽 설정 확인

```
# dynamic config 확인
kafka-configs --bootstrap-server <bootstrap-server> --describe --entity-type <topics/brokers>
kafka-configs --bootstrap-server <bootstrap-server> --describe --entity-type <topics/brokers> --entity-name <topic/broker>

# 기본값 포함 모든 설정 확인
kafka-configs --bootstrap-server <bootstrap-server> --describe --entity-type topics --all
kafka-configs --bootstrap-server <bootstrap-server> --describe --entity-type topics --entity-name <topic/broker> --all
```

## kafka-reassign-partition.sh

파티션 리더 변경

```
# json (__consumer_offsets 토픽 파티션 2번의 리더 변경)
{
  "version": 1,
  "partitions": [
    {
      "topic": "__consumer_offsets",
      "partition": 2,
      "replicas": [1, 0, 2],
      "log_dirs": ["any", "any", "any"]
    }
  ]
}

kafka-reassign-partition.sh --bootstrap-server <bootstrap-server> --execute --reassignment-json-file <file>
```

실행 중인 Partition Reassignment 작업 확인

```
kafka-reassign-partition.sh --bootstrap-server <bootstrap-server> --list
```
