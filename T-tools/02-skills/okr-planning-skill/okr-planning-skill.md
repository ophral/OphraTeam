---
name: okr-planning-skill
description: Set OKRs that drive focus, not theater. Use this when planning quarterly or annual objectives, especially across multiple teams. Includes the Doerr methodology, common antipatterns (KPI-as-OKR, etc.), and the cascade structure that aligns without micromanaging.
---

# Skill: OKR Planning

> Creates OKR drafts that align teams around outcomes, not outputs.

## Trigger Words
"OKR", "objectives", "key results", "quarterly planning", "goal setting"

## Format

```markdown
# OKRs: [Team/Department] - [Quarter Year]

**Date:** [Date]
**Type:** OKR Planning Document
**Owner:** [Name]
**Period:** [Q1/Q2/Q3/Q4 Year]
**Status:** [Draft / Calibrating / Committed]

---

## Team Mission (reminder)

[One sentence: what this team exists to do. Provides context for OKR alignment.]

---

## Objective 1: [Ambitious, qualitative goal]

*Why this matters:* [Connection to company strategy]

| # | Key Result | Baseline | Target | Confidence | Owner |
|---|-----------|----------|--------|-----------|-------|
| KR1 | [Measurable outcome] | [Current state] | [Target state] | [%] | [Name] |
| KR2 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |
| KR3 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |

**Key initiatives:** [What we'll do to hit these results]
- [Initiative 1]
- [Initiative 2]

---

## Objective 2: [Ambitious, qualitative goal]

*Why this matters:* [Connection to company strategy]

| # | Key Result | Baseline | Target | Confidence | Owner |
|---|-----------|----------|--------|-----------|-------|
| KR1 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |
| KR2 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |
| KR3 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |

**Key initiatives:**
- [Initiative 1]
- [Initiative 2]

---

## Objective 3: [Ambitious, qualitative goal]

*Why this matters:* [Connection to company strategy]

| # | Key Result | Baseline | Target | Confidence | Owner |
|---|-----------|----------|--------|-----------|-------|
| KR1 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |
| KR2 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |
| KR3 | [Measurable outcome] | [Baseline] | [Target] | [%] | [Name] |

**Key initiatives:**
- [Initiative 1]
- [Initiative 2]

---

## Alignment Check

| Our Objective | Maps to Company Objective |
|---------------|--------------------------|
| [Obj 1] | [Company Obj X] |
| [Obj 2] | [Company Obj Y] |
| [Obj 3] | [Company Obj Z] |

---

## Dependencies and Risks

| Dependency | From Team | Status | Risk if Missing |
|-----------|-----------|--------|-----------------|
| [What we need] | [Who provides it] | [Confirmed/Pending] | [Impact on KRs] |

---

## Scoring Guide

- **1.0:** Fully achieved (sandbag check: was it too easy?)
- **0.7:** Strong progress, stretch target nearly met
- **0.3-0.6:** Meaningful progress but fell short
- **0.0-0.2:** Failed to make progress
```

## Quality Checks

- [ ] Objectives are outcomes, not tasks ("increase retention" not "launch feature X")
- [ ] Key results are measurable (a stranger could verify achievement)
- [ ] Confidence level is realistic (70% target means real stretch)
- [ ] Max 3-5 objectives per team (focus beats breadth)
- [ ] Alignment to company objectives is explicit

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **Doerr's Definition.** Objectives are qualitative and aspirational. Key Results are quantitative and binary (hit or miss).
- **The 70% Rule.** Hitting 100% of OKRs means you set them too easy. Target 70% achievement for stretch OKRs.
- **Three to Five Per Level.** More than five OKRs at any level means you have no priorities.
- **Health Metrics Separate from OKRs.** Things that must stay healthy (customer NPS, system uptime) aren't OKRs. They're health metrics. Conflating them destroys both.
- **Cascade Without Mechanical Translation.** Team OKRs support but don't blindly copy company OKRs. Each layer translates strategy into action for their scope.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- KPIs labeled as OKRs. "Maintain MRR" is a KPI, not an objective.
- Too many. 15 OKRs means no priorities.
- Sandbagged KRs. Setting easy targets so the team hits 100%. Defeats the purpose.
- OKRs without owner. Diffuse responsibility = no responsibility.
- Never-checked OKRs. Set quarterly, forgotten by week 3.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
