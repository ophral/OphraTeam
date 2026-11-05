# Prompt: Close The Loop

You just created your first output, and you almost certainly gave feedback during the session ("make it shorter", "that's not my voice", "I'd never write it that way"). Every one of those corrections is the system learning who you actually are. This prompt captures BOTH the output AND the session feedback so the next round needs fewer corrections.

This is The Loop. It's what makes week 10 better than week 1.

Copy and paste this into your chat:

---

```
I just created content output and we went through one or more rounds of feedback in this conversation. Now I want to close The Loop so the system learns from BOTH the final output AND the feedback I gave during the session.

Adam, please manage this:

1. Reconstruct this session.
   Scan our entire conversation in this chat. Identify:
   - The original brief I gave (what content I asked for)
   - The first draft the team produced
   - Each piece of feedback I gave you (every "change this", "I don't like X", "make it shorter", "this isn't my voice", every revision request)
   - Each revised version produced in response
   - The final version we landed on
   - How many revision rounds happened
   Show me a brief session recap (3-5 lines) before continuing.

2. Read what we created in O-output.
   Open the latest folder in O-output/ and review: researcher brief, copywriter draft, gatekeeper review, final output.

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
   - "I wouldn't say it that way" / "use this phrase, not that" / "shorter sentences" / voice corrections → feedback-system.md (my corrections to remember)
   - "The hook didn't grab me" / "The structure worked" / "Gatekeeper missed X" / execution patterns → learning-log.md
   - "I posted it and got reaction Y" / real audience response → feedback-audience.md
   - "I'm never doing that again" / "we don't talk about X this way" / precedent set → decisions.md

   (b) Is this a one-time fix or a likely pattern?
   - One-time: specific to this output's topic, won't apply elsewhere
   - Pattern: would apply to most or all future content I make

   If anything is ambiguous, ask me ONE clarifying question before logging. Don't log noise.

5. Write each feedback item to the right M-memory file.
   Format for learning-log.md and feedback-system.md entries:
   [YYYY-MM-DD] [one-time | pattern] [what I noticed or preferred] [short example from this session]

6. Check promotion candidates (Memory to C-core).
   Re-read learning-log.md and feedback-system.md after logging. For any pattern that now appears 3+ times across entries, promote it:
   - Voice / phrasing / hook patterns → C-core/voice-dna.md
   - "How I work / what I own / my style" insights → C-core/about-me.md
   - "How my company operates / brand voice" insights → C-core/company-context.md
   - Audience insights → C-core/icp-profile.md
   - Strategic precedents → C-core/project-brief.md (or decisions.md if still in flux)
   The 3+ rule prevents one-off noise from becoming a permanent rule.

7. Sort B-brain/_INBOX/.
   Move any unsorted items to the right subfolder. Delete anything no longer relevant. Summarize what you sorted.

8. Show me a Loop Closure Report. Format:

   ## Loop Closure Report
   **Session shape:** [N drafts, X feedback rounds, what changed each round in one line]

   **Top corrections I gave** (what I won't have to say next time):
   1. [most-impactful correction]
   2. [next]
   3. [next]

   **Logged to M-memory:**
   - learning-log.md: [N entries] → [brief summary]
   - feedback-system.md: [N entries] → [brief summary]
   - feedback-audience.md: [N entries or "none"]
   - decisions.md: [N entries or "none"]

   **Promoted to C-core** (patterns that hit the 3+ threshold):
   - [file] ← [pattern] (appeared N times)
   - (or "Nothing ready to promote yet. Still gathering signal.")

   **B-brain/_INBOX sorted:** [N items moved | deleted]

   **One specific thing to try differently in the NEXT content output:**
   [Concrete, actionable, specific. Not generic. Example: "Open with a contrarian take instead of a question. The question opener triggered 'too soft' twice in this session."]

This is The Loop. Every time you close it, the system learns my actual taste from how I corrected it. Next time, it should need fewer rounds.
```

---

## Why The Loop Matters

Most AI systems are static. You set them up and they stay the same forever.

The ABC-TOM Loop is different. Every project teaches you something. Every correction you give in a session reveals your real taste, your real voice, your real preferences. The Loop captures those signals and bakes them into the system permanently.

**Week 1:** Memory is empty. Output is rough. You give 10 corrections per session.
**Week 4:** Memory has patterns. Output improves. You give 5 corrections per session.
**Week 8:** Strong patterns get promoted to Core. Output sounds like you. You give 2 corrections per session.
**Week 12:** The system runs itself. You just steer. Most outputs ship without correction.

The Loop is the difference between "using AI" and "building an AI team."

---

## When to Use This

- Right after creating any output, especially if you gave feedback during the session.
- Whenever you went through 2+ revision rounds. That's where the gold is.
- At the end of each week (pair with bonus prompt 13: weekly review).
- When your output starts feeling stale.

Skip it for: outputs you accepted with zero feedback. There's nothing for the system to learn yet.

---

> **© Tom Even**
> Workshops & future dates: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
