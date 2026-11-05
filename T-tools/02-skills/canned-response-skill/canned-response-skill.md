---
name: canned-response-skill
description: Write reusable response templates that sound human, not robotic. Use this when building support macros, customer service replies, or any high-frequency message that needs to stay on-brand at scale. Includes empathy patterns and de-escalation language.
---

# Skill: Canned Response

> Creates templated response sets that sound human, solve problems, and maintain brand voice.

## Trigger Words
"canned response", "template response", "saved reply", "macro", "response template"

## Format

```markdown
# Canned Response Set: [Category]

**Date:** [Date]
**Type:** Canned Response Set
**Category:** [Billing / Technical / Onboarding / Account / Feature Request]
**Voice:** [Friendly-professional / Technical-helpful / Empathetic-solution-focused]
**Last reviewed:** [Date]

---

## Response: [Scenario Name]

**Use when:** [Specific trigger or situation]
**Personalize:** [What agent MUST customize before sending]

---

**Subject:** [Subject line if email]

Hi [Name],

[Opening: acknowledge their situation, 1 sentence]

[Solution/answer: clear and direct, 2-4 sentences]

[Next step: what happens now, 1 sentence]

[Closing: warm but not fake]

[Agent name]

---

## Response: [Scenario Name]

**Use when:** [Trigger]
**Personalize:** [Required customization]

---

Hi [Name],

[Opening]

[Body]

[Next step]

[Closing]

---

## Response: [Scenario Name]

**Use when:** [Trigger]
**Personalize:** [Required customization]

---

Hi [Name],

[Opening]

[Body]

[Next step]

[Closing]

---

## Customization Rules

1. **Always personalize:** [Name], [specific issue], [account detail]
2. **Never send without:** Reading the ticket history first
3. **Adjust tone for:** [Situation-specific guidance]
4. **Add context when:** [Situations requiring extra explanation]

---

## Anti-Patterns

- Do NOT: [Common mistake with this response type]
- Do NOT: [Another common mistake]
- Do NOT: [Third common mistake]
```

## Quality Checks

- [ ] Responses sound like a human wrote them (not a robot)
- [ ] Personalization requirements are explicit (agents know what to change)
- [ ] "Use when" is specific enough to avoid wrong-scenario usage
- [ ] Responses solve the problem (not just acknowledge it)
- [ ] Anti-patterns prevent the most common misuse

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **The Empathy / Action / Next-Step structure.** Every reply has those three. "I hear you, here's what I'm doing, here's what happens next."
- **Replaceable variables.** Templates with {{first_name}}, {{issue}}, {{ETA}}. Personal at scale.
- **The tone tiers.** Light/standard/heavy depending on customer sentiment. One template per tier.
- **The de-escalation pattern.** Acknowledge feeling, validate the experience, name the action.
- **The Closing Line.** Every canned response needs a non-canned closing. "Just for you, here's..." matters.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- Robotic openings. "Thank you for reaching out" is fine. "We sincerely apologize for the inconvenience" is canned-response stench.
- No personalization at all. Pure template. Customer feels processed, not served.
- Same template for different sentiment. Angry customer gets the same reply as confused customer. Both feel worse.
- No follow-up trigger. Reply sent, no flag for "check back in 24 hours."
- Templates that lie. "We are working on it" when nobody is. Trust dies once.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
