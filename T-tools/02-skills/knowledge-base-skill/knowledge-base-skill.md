---
name: knowledge-base-skill
description: Build knowledge base articles that solve problems on the first read. Use this when documenting product features, support workflows, or any self-service content. Includes the task-based structure, search-friendly titling, and the SEO patterns that make articles findable.
---

# Skill: Knowledge Base Article

> Creates help center articles that users can find, scan, and solve their problem with in under 60 seconds.

## Trigger Words
"knowledge base", "help article", "help center", "FAQ", "support article"

## Format

```markdown
# [Title: Match What Users Would Search]

**Date:** [Date]
**Type:** Knowledge Base Article
**Product area:** [Feature/section]
**Audience:** [All users / Admins / New users]
**Last verified:** [Date]

---

## Quick Answer

[1-2 sentences: the direct answer. If someone reads only this, they should be unblocked.]

---

## Step-by-Step

1. [Action with specific UI element: "Click **Settings** in the top-right corner"]
2. [Next action: be precise about what to click, where it is]
3. [Next action]
4. [Next action]
5. [Expected result: "You should see [outcome]"]

---

## Common Variations

**If you're on mobile:**
[Different steps or note about availability]

**If you're an admin:**
[Additional options or different path]

**If this doesn't work:**
[First troubleshooting step before escalating]

---

## Screenshots

[Reference where screenshots should appear. Example:]
- Step 2: [Screenshot of Settings page with arrow pointing to relevant button]
- Step 4: [Screenshot of confirmation dialog]

---

## Related Articles

- [Related article 1: title and link]
- [Related article 2: title and link]
- [Related article 3: title and link]

---

## Still Stuck?

[How to contact support. Set expectations on response time.]
```

## Quality Checks

- [ ] Title matches what users would actually search (not internal jargon)
- [ ] Quick answer solves 60% of readers without scrolling
- [ ] Steps are testable (someone could follow them right now)
- [ ] No jargon without explanation
- [ ] Scannable in 10 seconds (bold key elements, short paragraphs)

---

## Top-1% Knowledge

What separates a great practitioner of this format from an average one. Use these as the quality bar.

- **Task-Based Structure.** Articles solve a task, not describe a feature. "How to invite a teammate" beats "Team management overview."
- **Search-Friendly Titles.** Title is what the user types into search. Match the question, don't paraphrase it.
- **The First-Screen Rule.** Most readers don't scroll. The first screen must contain the answer or a clear path to it.
- **Screenshot Discipline.** One screenshot per major step. Annotated. Visual scanners skip walls of text.
- **Linked Next Actions.** Every article ends with "What's next?" linking to the natural follow-on article.

---

## Common Mistakes to Avoid

The predictable failure modes for this format. Check against these before shipping.

- Feature documentation instead of task documentation. Users came to do something, not to learn the system.
- Titles that paraphrase user questions instead of matching them.
- Walls of text without scannable structure.
- No screenshots. The product changed. The article still describes the old UI.
- No update cadence. Articles drift out of accuracy. Trust dies.


---

> **Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
