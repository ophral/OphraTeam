---
name: escalation-playbook-skill
description: Build escalation playbooks that resolve issues fast. Use this when codifying incident response, support escalations, or customer-success crisis protocols. Includes severity matrices, runbook structures, and the post-mortem template that prevents repeats.
---

# Skill: Escalation Playbook

> Creates clear escalation paths so support teams know exactly when and how to escalate.

## Trigger Words
"escalation", "escalation playbook", "when to escalate", "escalation path", "tier 2"

## Format

```markdown
# Escalation Playbook: [Product/Team]

**Date:** [Date]
**Type:** Escalation Playbook
**Applies to:** [Team/role]
**Owner:** [Name]
**Last reviewed:** [Date]

---

## Escalation Philosophy

[2-3 sentences: when escalation is good (not failure). Set the mindset.]

---

## Escalation Tiers

| Tier | Handles | Response Target | Team |
|------|---------|-----------------|------|
| Tier 1 | [What they handle] | [Time target] | [Team/role] |
| Tier 2 | [What they handle] | [Time target] | [Team/role] |
| Tier 3 | [What they handle] | [Time target] | [Team/role] |
| Emergency | [Critical issues] | [Time target] | [Team/role] |

---

## When to Escalate

### Escalate to Tier 2 When:

- [Specific condition, not vague]
- [Specific condition]
- [Specific condition]
- [Time-based: "unresolved after X minutes/hours"]

### Escalate to Tier 3 When:

- [Specific condition]
- [Specific condition]
- [Specific condition]

### Emergency Escalation (immediate):

- [Condition requiring immediate action]
- [Condition requiring immediate action]
- [Condition requiring immediate action]

---

## How to Escalate

### Information Required

Every escalation must include:
1. [Customer details: what to pass along]
2. [Issue summary: format]
3. [Steps already taken: what was tried]
4. [Impact: who's affected, how badly]
5. [Urgency: why now]

### Channels

| Escalation Type | Channel | Who to Contact | Hours |
|-----------------|---------|----------------|-------|
| [Standard] | [Slack/Ticket/Phone] | [Team/person] | [Availability] |
| [Urgent] | [Channel] | [Who] | [Hours] |
| [Emergency] | [Channel] | [Who] | [24/7] |

---

## Escalation Scenarios

### Scenario: [Common escalation situation]

**Trigger:** [What makes this an escalation]
**Tier:** [Where it goes]
**Information needed:** [Specific data for this type]
**Expected resolution:** [What the next tier will do]
**SLA:** [Time target]

### Scenario: [Another common situation]

**Trigger:** [Condition]
**Tier:** [Destination]
**Information needed:** [Specifics]
**Expected resolution:** [Outcome]
**SLA:** [Target]

---

## What NOT to Escalate

- [Situation that seems like escalation but isn't]
- [Situation better handled by: alternative path]
- [Situation that needs: different process entirely]

---

## After Escalation

1. [What the escalating agent should do next]
2. [Follow-up responsibility]
3. [How to track resolution]
4. [When to re-escalate if stalled]
```

## Quality Checks

- [ ] Triggers are specific (not "when it seems complex")
- [ ] Information requirements prevent back-and-forth
- [ ] "What NOT to escalate" prevents noise
- [ ] Channels and contacts are current
- [ ] Time targets are realistic for each tier

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **Severity Tiers.** P0 / P1 / P2 / P3 with clear definitions and response time SLAs. Ambiguity here breaks under pressure.
- **The Single Owner Principle.** Every incident has one incident commander. Confusion about ownership is the #1 reason incidents take longer than they should.
- **The 5-Minute Status Cadence.** During active incidents, status update every 5 minutes. Silence creates panic.
- **Blameless Post-Mortem.** Fix systems, not people. Post-mortems should focus on "what process let this happen," not "who did this."
- **The Runbook.** Pre-written response for common incidents. Don't reinvent under stress.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- No severity definitions. Every issue feels like P0 to the customer reporting it.
- Diffuse ownership. "Someone should look at this." Nobody does.
- Status silence. "We're working on it" 90 minutes later isn't a status update.
- No post-mortem. Same issue happens again three months later.
- Blaming individuals. Talented people leave teams that blame.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
