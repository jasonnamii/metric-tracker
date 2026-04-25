# metric-tracker

> 🇺🇸 [English README](./README.md)

**측정 과학 기반 지표 설계·추적·리뷰 엔진. Goodhart's Law부터 Shewhart 관리도까지 — 측정하되 관리를 망치지 않는 지표 시스템.**

## 사전 요구

- **Claude Cowork 또는 Claude Code** 환경

## 목표

나쁜 지표는 지표가 없는 것보다 나쁘다 — 통제의 환상을 만들면서 조직을 잘못된 방향으로 몬다. 이 스킬은 엄격한 측정 이론(Goodhart, Campbell, Deming, Meadows)을 적용하여 실제 의사결정에 기여하는 지표를 설계하고, 변동을 올바르게 진단하며, KPI가 조직 기능장애로 변질되는 함정을 방지한다.

## 사용 시점 & 방법

KPI, OKR, 지표, 대시보드, 성과 리뷰 언급 시 자동 발동. 3모드: **설계**(목표에서 지표 체계 생성), **리뷰**(변동 이론 기반 데이터 분석), **재설계**(기존 지표 체계 병리 감사). "이 프로젝트 KPI 잡아줘", "이번 달 지표 리뷰해줘" 등으로 호출.

## 사용 사례

| 상황 | 프롬프트 | 동작 |
|---|---|---|
| 신규 프로젝트 KPI | `"이 프로젝트 KPI 잡아줘"` | 4층 설계(북극성→드라이버→건강→카운터), 지표별 병리 스크리닝, 리뷰 프로토콜 |
| 월간 지표 리뷰 | `"이번 달 지표 리뷰해줘"` | 변동 유형 진단(Common vs Special Cause), 추세 분석, 불확실성 태그 포함 인과 추론 |
| KPI 체계 감사 | `"지금 KPI가 맞는 건지 모르겠어"` | 기존 지표 4층 매핑, 갭 식별(빈 층, 허영지표), Goodhart/Surrogation 위험 평가 |

## 주요 기능

- **측정 병리 스크리닝** — 모든 지표에 Goodhart(약형/강형), Campbell's Law, McNamara Fallacy, Surrogation, Cobra Effect 5축 점검
- **변동 유형 진단** — Shewhart 관리도 로직: Common Cause(건드리지 마라) vs Special Cause(조사하라). 가장 흔한 경영 오류 방지
- **시스템 다이내믹스 점검** — Meadows 지렛대, Stock/Flow/Feedback Loop, 제약이론(TOC) 통합
- **프록시 검증 프로토콜** — 프록시 메트릭 실패 5유형 + 구조적 검증 주기
- **허브+스포크 아키텍처** — 경량 허브 + 5개 전문지식 reference 파일

## 연동 스킬

- **[management-skill](https://github.com/jasonnamii/management-skill)** — OKR 설계(M3) → 측정·추적 연결
- **[ceo-pipeline](https://github.com/jasonnamii/ceo-pipeline)** — 마일스톤 성공 지표
- **[planning-skill](https://github.com/jasonnamii/planning-skill)** — 성공 기준 → 지표 변환
- **[risk-radar](https://github.com/jasonnamii/risk-radar)** — 건강지표 이상 → 리스크 스캐닝 트리거

## 설치

```bash
git clone https://github.com/jasonnamii/metric-tracker.git ~/.claude/skills/metric-tracker
```

## 업데이트

```bash
cd ~/.claude/skills/metric-tracker && git pull
```

`~/.claude/skills/`에 배치된 스킬은 Claude Code 및 Cowork 세션에서 자동으로 사용 가능합니다.

## Cowork Skills

25개 이상의 커스텀 스킬 중 하나입니다. 전체 카탈로그: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## 라이선스

MIT License — 자유롭게 사용, 수정, 공유 가능합니다.
