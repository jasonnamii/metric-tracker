# metric-tracker

> 🇰🇷 [한국어 README](./README.ko.md)

**A metrics design, tracking, and review engine built on measurement science — from Goodhart's Law to Shewhart control charts — ensuring you measure what matters without corrupting what you manage.**

## Prerequisites

- **Claude Cowork or Claude Code** environment

## Goal

Bad metrics are worse than no metrics — they create illusions of control while driving perverse behavior. This skill applies rigorous measurement theory (Goodhart, Campbell, Deming, Meadows) to design metrics that actually inform decisions, diagnose variation correctly, and avoid the traps that turn KPIs into organizational dysfunction.

## When & How to Use

Triggers when you mention KPIs, OKRs, metrics, dashboards, or performance reviews. Three modes: **Design** (creating metric systems from goals), **Review** (analyzing metric data with variation theory), and **Redesign** (auditing existing metric systems for pathology). Say "이 프로젝트 KPI 잡아줘" or "이번 달 지표 리뷰해줘".

## Use Cases

| Scenario | Prompt | What Happens |
|---|---|---|
| New project KPIs | `"이 프로젝트 KPI 잡아줘"` | 4-layer design (North Star → Drivers → Health → Counter), pathology screening per metric, review protocol |
| Monthly metrics review | `"이번 달 지표 리뷰해줘"` | Variation type diagnosis (common vs special cause), trend analysis, causal inference with uncertainty tags |
| KPI system audit | `"지금 KPI가 맞는 건지 모르겠어"` | Maps existing metrics to 4 layers, identifies gaps (missing layers, vanity metrics), Goodhart/Surrogation risk assessment |

## Key Features

- **Measurement Pathology Screening** — Every metric checked against Goodhart (weak/strong), Campbell's Law, McNamara Fallacy, Surrogation, and Cobra Effect
- **Variation Type Diagnosis** — Shewhart control chart logic: common cause (don't tamper) vs special cause (investigate). Prevents the most common management error
- **Systems Dynamics Check** — Meadows leverage points, stocks/flows/feedback loops, Theory of Constraints integration
- **Proxy Validation Protocol** — 5 failure patterns for proxy metrics with structured validation cadence
- **Hub+Spoke Architecture** — Lean hub with 5 deep reference files (measurement pathology, variation theory, systems metrics, frameworks, proxy theory)

## Works With

- **[management-skill](https://github.com/jasonnamii/management-skill)** — OKR design (M3) connects to measurement tracking
- **[ceo-pipeline](https://github.com/jasonnamii/ceo-pipeline)** — Milestone success metrics
- **[planning-skill](https://github.com/jasonnamii/planning-skill)** — Success criteria → metric conversion
- **[risk-radar](https://github.com/jasonnamii/risk-radar)** — Health metric anomalies trigger risk scanning

## Installation

```bash
git clone https://github.com/jasonnamii/metric-tracker.git ~/.claude/skills/metric-tracker
```

## Update

```bash
cd ~/.claude/skills/metric-tracker && git pull
```

Skills placed in `~/.claude/skills/` are automatically available in Claude Code and Cowork sessions.

## Part of Cowork Skills

This is one of 25+ custom skills. See the full catalog: [github.com/jasonnamii/cowork-skills](https://github.com/jasonnamii/cowork-skills)

## License

MIT License — feel free to use, modify, and share.
