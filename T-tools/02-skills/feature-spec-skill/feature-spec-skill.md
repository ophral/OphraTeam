---
name: feature-spec-skill
description: Write feature specs that engineers can build without back-and-forth. Use this when drafting feature requirements for development teams. Includes the user-story format, edge-case checklists, and the level of detail that prevents scope creep.
---

# Skill: Feature Spec

> Creates detailed feature specifications that engineers can build from without guessing.

## Trigger Words
"feature spec", "specification", "technical spec", "feature document", "functional spec"

## Format

```markdown
# Feature Spec: [Feature Name]

**Date:** [Date]
**Type:** Feature Specification
**Author:** [Name]
**Status:** [Draft / Review / Approved / Building]
**PRD reference:** [Link to parent PRD]
**Engineering lead:** [Name]

---

## Overview

**What:** [One sentence describing the feature]
**Why:** [One sentence on the user/business value]
**Who:** [Primary user persona]

---

## User Flow

1. User [action/trigger]
2. System [response]
3. User [next action]
4. System [response]
5. [Continue until flow is complete]

**Entry points:** [How users discover/access this feature]
**Exit points:** [Where users go after completing the flow]

---

## Detailed Requirements

### Functional Requirements

| ID | Requirement | Priority | Acceptance Criteria |
|----|-------------|----------|---------------------|
| F1 | [What the system must do] | [P0/P1/P2] | [How we verify it works] |
| F2 | [What the system must do] | [P0/P1/P2] | [How we verify it works] |
| F3 | [What the system must do] | [P0/P1/P2] | [How we verify it works] |
| F4 | [What the system must do] | [P0/P1/P2] | [How we verify it works] |

### Non-Functional Requirements

| ID | Requirement | Target |
|----|-------------|--------|
| NF1 | Performance | [Response time, throughput] |
| NF2 | Scale | [Expected load, growth] |
| NF3 | Availability | [Uptime target] |
| NF4 | Security | [Relevant requirements] |

---

## Edge Cases

| Scenario | Expected Behavior |
|----------|-------------------|
| [Edge case 1] | [What should happen] |
| [Edge case 2] | [What should happen] |
| [Edge case 3] | [What should happen] |
| [Error state 1] | [How system recovers] |

---

## UI/UX Notes

[Wireframes, mockups, or detailed descriptions of the interface. Reference design files if they exist.]

- **State 1 (empty):** [What user sees with no data]
- **State 2 (loading):** [What user sees while waiting]
- **State 3 (populated):** [Normal state]
- **State 4 (error):** [What user sees when something fails]

---

## Data Model

[Relevant data structures, API contracts, or schema changes needed]

---

## Dependencies

| Dependency | Team/Service | Status | Risk if Late |
|-----------|--------------|--------|--------------|
| [Dependency 1] | [Who owns it] | [Ready/In progress/Blocked] | [Impact] |
| [Dependency 2] | [Who owns it] | [Status] | [Impact] |

---

## Out of Scope

- [Explicitly excluded item 1]
- [Explicitly excluded item 2]
- [Explicitly excluded item 3]
```

## Quality Checks

- [ ] An engineer could build this without asking clarifying questions
- [ ] Edge cases cover failure modes, not just happy paths
- [ ] Acceptance criteria are testable (not subjective)
- [ ] Out of scope prevents scope creep
- [ ] Dependencies are identified with risk assessment

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **User Story Format.** As a [persona], I want [outcome], so that [reason]. Forces the writer to think about who, what, and why.
- **Amazon PR-FAQ.** Press release + FAQ written before building. Customer benefit first, implementation last.
- **Edge Case Discipline.** What happens at zero, at max, at boundary, when offline, when slow, when malicious. Engineers will hit all of these.
- **Definition of Done.** Acceptance criteria as testable statements. "User can do X under Y condition" beats "feature works correctly."
- **The Don't-Build List.** Out-of-scope explicitly stated. Prevents scope creep mid-build.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- Solution language instead of outcome language. Engineers can solve. Tell them what to solve for.
- Missing edge cases. The happy path is documented. Failure modes aren't.
- Vague acceptance criteria. "Works well" is not testable.
- No "not doing this" section. Scope creeps during build.
- Spec written after build started. Negative-leverage activity.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
