# Prompt: Close The Loop

You just produced a decision brief or structured document. Almost certainly you pushed back during the session ("you weighted the wrong option", "this frame is off", "the recommendation is too soft", "the Devil's Advocate missed the real risk"). Every one of those corrections reveals how YOU actually think, weigh, and decide. This prompt captures BOTH the brief AND the session feedback so the next decision brief lands closer on the first draft.

This is The Loop. It's what makes week 10 better than week 1.

Copy and paste this into your chat:

---

```
I just used the Thinking track to produce a decision brief or structured summary, and we went through one or more rounds of feedback in this conversation. Now I want to close The Loop so the system learns from BOTH the final brief AND the feedback I gave during the session.

Adam, please manage this:

1. Reconstruct this session.
   Scan our entire conversation in this chat. Identify:
   - The decision I was making (or document I was producing) and which agents were involved (Analyst, Strategist, Devil's Advocate, Chief of Staff, Gatekeeper)
   - The first version the team produced
   - Each piece of feedback I gave (every "you weighted the wrong option", "this frame is off", "the recommendation is too soft", "you missed the real risk", every revision request)
   - Each revised version produced in response
   - The final version we landed on
   - How many revision rounds happened
   Show me a brief session recap (3-5 lines) before continuing.

2. Read what we created in O-output.
   Open the latest folder in O-output/ and review every agent artifact (analyst, strategist, devil's advocate, chief of staff, copywriter, gatekeeper, whichever ran).

3. Read current memory and core files.
   - M-memory/learning-log.md
   - M-memory/feedback-system.md
   - M-memory/feedback-audience.md
   - M-memory/decisions.md
   - C-core/about-me.md
   - C-core/company-context.md
   - C-core/project-brief.md
   - C-core/voice-dna.md
   - C-core/icp-profile.md

4. Categorize every piece of feedback I gave during the session.
   For each feedback item, decide TWO things:

   (a) Which M-memory file does it belong in? Use this routing:
   - "I wouldn't phrase the recommendation that way" / structural or voice corrections → feedback-system.md
   - "The analysis was thin on X" / "the Devil's Advocate missed Y" / "I prefer briefs to lead with the recommendation, not the options" / execution patterns → learning-log.md
   - "After I made the call, here's what actually happened" / real-world outcome of the decision → feedback-audience.md
   - "I'm picking option B" / "this sets our policy on X" / decision actually made → decisions.md (with topic, options, choice, reasoning, confidence)

   (b) Is this a one-time fix or a likely pattern?
   - One-time: specific to this decision's content
   - Pattern: reveals how I think and decide (would apply to most or all future briefs)

   If anything is ambiguous, ask me ONE clarifying question before logging. Don't log noise.

5. Write each feedback item to the right M-memory file.
   For learning-log.md and feedback-system.md entries:
   [YYYY-MM-DD] [one-time | pattern] [what I noticed or preferred] [short example from this session]

   For decisions.md (only if a decision was actually made):
   [YYYY-MM-DD] | Topic: [what] | Options considered: [A / B / C] | Chose: [X] | Reasoning: [1-2 lines] | Confidence: [Low / Medium / High]

6. Check promotion candidates (Memory to C-core).
   Re-read learning-log.md and feedback-system.md after logging. For any pattern that now appears 3+ times across entries, promote it:
   - Decision style insights ("I decide fast on reversible bets, slow on irreversible") / "how I work" → C-core/about-me.md
   - Framing or structure patterns ("always lead with recommendation, then options") → C-core/voice-dna.md
   - "How my company decides / what we won't risk" → C-core/company-context.md
   - Stakeholder insights (who reads briefs, what level of detail they expect) → C-core/icp-profile.md
   - Strategic precedents that should govern future decisions → C-core/project-brief.md or decisions.md
   The 3+ rule prevents one-off noise from becoming a permanent rule.

7. Sort B-brain/_INBOX/.
   Move any unsorted items to the right subfolder. Delete anything no longer relevant. Summarize what you sorted.

8. Show me a Loop Closure Report. Format:

   ## Loop Closure Report
   **Session shape:** [decision or document type, N drafts, X feedback rounds, what changed each round in one line]

   **What this session revealed about how I think / decide:**
   [1-2 lines. This is the gold. Example: "Prefer 3 options not 5. Push back when Devil's Advocate gets philosophical instead of concrete. Want recommendation first, then options, then risks."]

   **Top corrections I gave** (what I won't have to say next time):
   1. [most-impactful correction]
   2. [next]
   3. [next]

   **Logged to M-memory:**
   - learning-log.md: [N entries] → [brief summary]
   - feedback-system.md: [N entries] → [brief summary]
   - feedback-audience.md: [N entries or "none, no outcome logged yet"]
   - decisions.md: [decision logged, or "no decision finalized in this session"]

   **Promoted to C-core** (patterns that hit the 3+ threshold):
   - [file] ← [pattern] (appeared N times)
   - (or "Nothing ready to promote yet. Still gathering signal.")

   **B-brain/_INBOX sorted:** [N items moved | deleted]

   **One specific thing to try differently in the NEXT decision brief:**
   [Concrete, actionable, specific. Not generic. Example: "Have Strategist lead with the recommendation and confidence level, not the options. Three times in this session I asked for the bottom line first."]

This is The Loop. Every time you close it, the system learns my real decision style from how I corrected it. Next time, fewer rounds.
```

---

## Why The Loop Matters

Most AI systems are static. You set them up and they stay the same forever.

The ABC-TOM Loop is different. Every decision you make teaches the system something about how you weigh, frame, and choose. Every correction you give in a session reveals your real decision style. The Loop captures those signals and bakes them into the system permanently.

**Week 1:** Memory is empty. Briefs are generic. You give 10 corrections per session.
**Week 4:** Memory has patterns. Briefs improve. You give 5 corrections per session.
**Week 8:** Strong patterns get promoted to Core. Briefs fit your decision style. You give 2 corrections per session.
**Week 12:** The system runs itself. You just steer. Most briefs land on the first draft.

The Loop is the difference between "using AI" and "building an AI team."

---

## When to Use This

Run this prompt after:
- Producing a decision brief
- Producing a meeting summary or structured document
- Going through 2+ revision rounds (that's where the gold is)
- Making a real decision off the back of an analysis

Skip it for: outputs you accepted with zero feedback. Nothing for the system to learn yet.

---

> **© Tom Even**
> Workshops & future dates: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
