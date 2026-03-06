---
layout: post
title: "Locust swarm test"
date: 2026-03-06
tags: [locust, swarm, load-test]
---

## KR (한국어)

### 목표
- (TODO) 목표 RPS / VU / 테스트 범위
- (TODO) 주요 시나리오

### 환경
- Locust: 2.x (TODO 실제 버전)
- Swarm mode: master + worker

### 실행
**Master**
```bash
locust -f locustfile.py --master --web-host 0.0.0.0
```

**Worker**
```bash
locust -f locustfile.py --worker --master-host <MASTER_IP>
```

### 체크리스트
- master/worker 버전 맞추기
- master bind port(기본 5557/5558) 방화벽 열기
- 결과 저장 옵션: `--csv`, `--csv-full-history`

---

## EN (English)

### Goal
- (TODO) target RPS / VUs / scope
- (TODO) key scenarios

### Environment
- Locust: 2.x (TODO exact version)
- Swarm mode: master + worker

### Run
**Master**
```bash
locust -f locustfile.py --master --web-host 0.0.0.0
```

**Worker**
```bash
locust -f locustfile.py --worker --master-host <MASTER_IP>
```

### Checklist
- Match master/worker versions
- Open master bind ports (default 5557/5558)
- Store results: `--csv`, `--csv-full-history`
