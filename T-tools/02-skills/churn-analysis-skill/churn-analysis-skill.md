---
name: churn-analysis-skill
description: Analyze why customers leave and turn the answer into action. Use this when investigating churn spikes, building churn dashboards, or preparing retention readouts. Includes cohort framing, root-cause patterns, and actionable narrative structures.
---

# Skill: Churn Analysis

> Creates risk signal assessments and save plays that catch at-risk accounts before it's too late.

## Trigger Words
"churn", "at risk", "churn analysis", "save play", "retention risk", "cancellation"

## Format

```markdown
# Churn Analysis: [Customer Name]

**Date:** [Date]
**Type:** Churn Risk Assessment
**Customer:** [Company]
**ARR at risk:** [Amount]
**Risk level:** [Critical / High / Medium / Early Warning]
**CSM:** [Name]
**Days to renewal:** [Number]

---

## Risk Summary

**Overall risk score:** [1-10, where 10 is "already gone"]
**Primary risk factor:** [One line: the biggest reason they might leave]
**Save probability:** [Estimated % chance we retain them]

---

## Risk Signals

| Signal | Evidence | Severity | First Detected |
|--------|----------|----------|----------------|
| [Usage decline] | [Specific data: e.g., "DAU dropped 40% in 30 days"] | [High/Medium/Low] | [Date] |
| [Champion left] | [Evidence] | [Severity] | [Date] |
| [Support escalation] | [Evidence] | [Severity] | [Date] |
| [Competitive evaluation] | [Evidence] | [Severity] | [Date] |
| [Payment issues] | [Evidence] | [Severity] | [Date] |

---

## Root Cause Analysis

**What we think is driving this:**
[2-4 sentences: honest assessment of why this account is at risk. Is it us? Is it them? Is it market?]

**Contributing factors:**
- [Factor 1: with evidence]
- [Factor 2: with evidence]
- [Factor 3: with evidence]

---

## Customer Perspective

**What they've said:** [Direct quotes or paraphrased feedback from actual conversations]
**What they haven't said but we infer:** [Based on behavior patterns]
**Their alternatives:** [What they'd switch to if they leave]

---

## Save Play

### Immediate Actions (this week)

| Action | Owner | Purpose | Deadline |
|--------|-------|---------|----------|
| [Specific action] | [Name] | [What this achieves] | [Date] |
| [Specific action] | [Name] | [Purpose] | [Date] |
| [Specific action] | [Name] | [Purpose] | [Date] |

### Short-term (30 days)

| Action | Owner | Purpose | Deadline |
|--------|-------|---------|----------|
| [Action] | [Name] | [Purpose] | [Date] |
| [Action] | [Name] | [Purpose] | [Date] |

### Concessions (if needed)

| Concession | Conditions | Approval Needed | Impact |
|-----------|-----------|-----------------|--------|
| [Discount/credit] | [When to offer] | [Who approves] | [Revenue impact] |
| [Extended terms] | [Conditions] | [Approver] | [Impact] |
| [Custom feature] | [Conditions] | [Approver] | [Impact] |

---

## Success Criteria

**We've saved this account when:**
- [Observable indicator 1]
- [Observable indicator 2]
- [Observable indicator 3]

**Review this plan on:** [Date]

---

## If We Lose Them

**Impact:** [ARR loss, logo loss, reference impact, team morale]
**Lessons:** [What we should learn from this]
**Prevention:** [What would have caught this earlier]
```

## Quality Checks

- [ ] Risk signals are based on data, not gut feeling
- [ ] Root cause is honest (even if uncomfortable)
- [ ] Save play has specific actions with owners and deadlines
- [ ] Concessions require approval (not given away in panic)
- [ ] "If we lose them" section forces learning

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **Gross vs Net Churn.** Gross is what left. Net is what left minus expansion. Both matter and tell different stories.
- **Cohort-based analysis.** Aggregate churn rates lie. Cohort views show what's improving and what isn't.
- **Voluntary vs involuntary churn.** Failed payments vs cancellations. Each requires a different fix.
- **The 90-day predictor.** Customers who hit early value rarely churn. Early-warning system: usage drop, exec sponsor change, support volume spike.
- **Sean Ellis's "how disappointed" metric.** 40% "very disappointed" if they couldn't use your product = product-market fit.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- Reporting churn without segment. SMB churn looks different than enterprise.
- Missing the leading indicators. Catching churn at "cancel" is too late.
- No exit interview. Every cancellation should produce one data point.
- Confusing correlation with cause. Customers who churn often had fewer logins. Doesn't mean more logins fixes churn.
- Treating churn as a CS problem. Churn is a product, pricing, and CS problem combined.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
