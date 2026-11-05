# Prompt: Close The Loop

You just produced a professional communication (an email, a proposal, an internal update, an HR message, a community post, a follow-up). And almost certainly you gave feedback during the session ("too formal", "this isn't how I'd say it to them", "soften the ask", "tighten the close"). Every one of those corrections is the system learning how YOU communicate with this specific kind of recipient. This prompt captures BOTH the message AND the session feedback so the next round needs fewer corrections.

This is The Loop. It's what makes week 10 better than week 1.

Copy and paste this into your chat:

---

```
I just created a professional communication and we went through one or more rounds of feedback in this conversation. Now I want to close The Loop so the system learns from BOTH the final message AND the feedback I gave during the session.

Adam, please manage this:

1. Reconstruct this session.
   Scan our entire conversation in this chat. Identify:
   - Who the recipient was and what the communication type was (proposal / email / update / HR / community / outreach / follow-up)
   - The first draft the team produced
   - Each piece of feedback I gave (every "too formal", "wrong tone for this recipient", "soften the ask", "I'd never write that to them", every revision request)
   - Each revised version produced in response
   - The final version we landed on
   - How many revision rounds happened
   Show me a brief session recap (3-5 lines) before continuing.

2. Read what we created in O-output.
   Open the latest folder in O-output/ and review: strategist analysis, copywriter draft, gatekeeper review, final message.

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
   - "I wouldn't say it that way" / "use this phrase, not that" / "shorter sentences" / voice corrections → feedback-system.md
   - "The opening hit wrong for this recipient" / "the CTA was buried" / "Gatekeeper missed X" / execution patterns → learning-log.md
   - "They replied with reaction Y" / real recipient response after sending → feedback-audience.md
   - "I'm never opening cold like that" / "we don't make promises like this on email" / precedent set → decisions.md

   (b) Is this a one-time fix or a likely pattern?
   - One-time: specific to this recipient on this topic
   - Pattern: would apply to all future communications of this type (e.g., all proposals, all customer follow-ups)

   If anything is ambiguous, ask me ONE clarifying question before logging. Don't log noise.

5. Write each feedback item to the right M-memory file.
   Format for learning-log.md and feedback-system.md entries:
   [YYYY-MM-DD] [comm-type] [one-time | pattern] [what I noticed or preferred] [short example from this session]

6. Check promotion candidates (Memory to C-core).
   Re-read learning-log.md and feedback-system.md after logging. For any pattern that now appears 3+ times across entries, promote it:
   - Tone / phrasing / signature opening or sign-off patterns → C-core/voice-dna.md
   - "How I work / what I own / my decision style" insights → C-core/about-me.md
   - "How my company operates / brand voice for external comms" insights → C-core/company-context.md
   - Recipient insights (what this type of recipient cares about, how they respond) → C-core/icp-profile.md
   - Strategic precedents (pricing line, positioning line, "we don't do X") → C-core/project-brief.md or decisions.md
   The 3+ rule prevents one-off noise from becoming a permanent rule.

7. Sort B-brain/_INBOX/.
   Move any unsorted items to the right subfolder. Delete anything no longer relevant. Summarize what you sorted.

8. Show me a Loop Closure Report. Format:

   ## Loop Closure Report
   **Session shape:** [comm-type, N drafts, X feedback rounds, what changed each round in one line]

   **Did the approach match the type?** [Yes / No / Partially, with one-line reason. e.g., "Started too formal for a community post, corrected on draft 2."]

   **Top corrections I gave** (what I won't have to say next time):
   1. [most-impactful correction]
   2. [next]
   3. [next]

   **Logged to M-memory:**
   - learning-log.md: [N entries] → [brief summary]
   - feedback-system.md: [N entries] → [brief summary]
   - feedback-audience.md: [N entries or "none, no recipient response logged yet"]
   - decisions.md: [N entries or "none"]

   **Promoted to C-core** (patterns that hit the 3+ threshold):
   - [file] ← [pattern] (appeared N times)
   - (or "Nothing ready to promote yet. Still gathering signal.")

   **B-brain/_INBOX sorted:** [N items moved | deleted]

   **One specific thing to try differently in the NEXT communication of this type:**
   [Concrete, actionable, specific. Not generic. Example: "Open follow-up emails with the previous decision restated in one line. Twice in this session I asked for the context to be reattached."]

This is The Loop. Every time you close it, the system learns how I communicate with each kind of recipient. Next time, it should need fewer rounds.
```

---

## Why The Loop Matters

Most AI systems are static. You set them up and they stay the same forever.

The ABC-TOM Loop is different. Every message you draft teaches the system something. Every correction you give in a session reveals how you talk to this kind of recipient. The Loop captures those signals and bakes them into the system permanently.

**Week 1:** Memory is empty. Messages are rough. You give 10 corrections per session.
**Week 4:** Memory has patterns. Messages improve. You give 5 corrections per session.
**Week 8:** Strong patterns get promoted to Core. Messages sound like you. You give 2 corrections per session.
**Week 12:** The system runs itself. You just steer. Most messages ship without correction.

The Loop is the difference between "using AI" and "building an AI team."

---

## When to Use This

Run this prompt after:
- Drafting (or sending) a client proposal
- Drafting a sales or outreach email
- Posting a community message
- Delivering an internal update
- Handling an HR or sensitive conversation
- Any communication where the recipient's response matters

Skip it for: drafts you didn't send, throwaway notes, internal scratchpads. Or any output you accepted with zero feedback. Nothing for the system to learn yet.

---

> **© Tom Even**
> Workshops & future dates: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
