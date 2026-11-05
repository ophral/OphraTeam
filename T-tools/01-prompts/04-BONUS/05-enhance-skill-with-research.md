# Prompt: Enhance Your Skill with Deep Research

You just created a skill (or you have one that feels generic). Now make it world-class.

This prompt generates a deep research query you can copy into Google Gemini Deep Research (or any AI research tool). The research will come back with everything your skill needs to become a top 1% playbook for that specific output format: proven structures, hook formulas, sentence patterns, world-class examples, frequent mistakes, and quality checks that elite practitioners actually use.

You paste the research back into your skill file, and suddenly your newsletter-skill writes like the top 50 Substacks, your sales-proposal-skill closes like a 7-figure rep, and your PRD-skill drafts like an Amazon principal PM.

Same mechanic as `02-enhance-agent-with-research.md`. Different target. The agent prompt upgrades a thinker. This prompt upgrades a CRAFT.

Copy and paste this into your chat (fill in the skill details first):

---

```
I want to make one of my skills significantly better by feeding it expert-level knowledge about its specific output format.

---
Skill name: [e.g., "newsletter-skill", "sales-proposal-skill", "prd-skill", or a new skill you just created]
What this skill produces: [The actual output format. e.g., "weekly email newsletters for SaaS founders", "B2B sales proposals for $50K+ deals", "internal product requirement documents for engineering"]
Audience for the output: [Who reads or receives what this skill produces. e.g., "newsletter subscribers (mostly product people)", "VP-level buyers at enterprise tech companies", "my engineering team"]
---

Please do the following:

1. Read the skill file in T-tools/02-skills/[skill-name]/[skill-name].md to understand its current structure and contents.

2. Read the C-core files to understand WHO uses this skill and WHERE the output lands:
   - C-core/about-me.md (my role and how I work)
   - C-core/company-context.md (the company, brand voice, constraints)
   - C-core/project-brief.md (what I produce in this role)
   - C-core/voice-dna.md (voice rules the skill must respect)
   - C-core/icp-profile.md (who reads or receives the output)

3. Generate a deep research prompt I can paste into Google Gemini Deep Research (or any AI research tool).

   The research must come back organized into THESE EXACT SECTIONS, because each section maps to a section of my skill file:

   (A) **Fundamentals.** What separates a world-class [output format] from an average one? Length conventions, frequency, structural norms, what "great" actually looks like in this format.

   (B) **Proven structures.** 3 to 5 named structural templates the best practitioners use (e.g., "PAS framework", "Pyramid Principle", "Amazon PR-FAQ"). For each: name, when to use it, the skeleton, one short example.

   (C) **Hook and opening patterns.** 8 to 12 proven opening formulas for this format, with one-line examples each. The kind of openers that earn the read.

   (D) **Sentence patterns and language.** Phrases, transitions, and sentence structures top practitioners reach for. What word-level moves separate amateur from elite.

   (E) **Common mistakes and anti-patterns.** The 5 to 7 mistakes even experienced people make in this format. The "if you do this, you lose them" list.

   (F) **Quality checks.** A 7 to 10 item checklist a top-1% practitioner runs before shipping. Specific, testable, not vague.

   (G) **Best-in-class examples.** 3 to 5 specific real-world examples of this format done at the highest level. Include the creator/source, why it works, and the one move worth stealing. URLs if available.

   (H) **Where this format is heading (2024-2026).** What's changing. What used to work and stopped. What's emerging.

   Make the research prompt specific to MY context. Reference my role from about-me.md, my company stage from company-context.md, and my audience from icp-profile.md. The research should come back tuned to MY use case, not a generic textbook version.

4. Format the research prompt as a clean block I can copy-paste directly into Gemini Deep Research. No extra formatting, no instructions around it. Just the prompt itself, ready to paste.

5. After I paste the research results back here, help me integrate the best findings into the skill file. Update these sections of T-tools/02-skills/[skill-name]/[skill-name].md:

   - "Fundamentals" or equivalent intro → use (A)
   - "Structures" or "Proven Structures" → use (B)
   - "Hook / Opening Formulas" → use (C) as a new or expanded section
   - "Sentence Patterns / Language" → use (D) as a new or expanded section
   - "Rules" or "Anti-Patterns" → use (E) as the things-to-avoid list
   - "Quality Checklist" → use (F), replacing any vague existing checklist
   - "Examples" → use (G), with the source and "one move worth stealing" preserved
   - Add a "What's Changing (2024-2026)" callout at the top of the skill file → use (H)

   Also:
   - Check if any cross-cutting voice rules from the research should be promoted to C-core/voice-dna.md (e.g., "use one number per paragraph"). Promote anything that applies to MORE than this one format.
   - Log a M-memory/learning-log.md entry noting the skill was upgraded, when, and the source of the research.

Show me the research prompt first. I'll run it externally and come back with the results.
```

---

## How to Use This

1. Run the prompt above in Claude Code. You'll get a research query.
2. Copy the research query and paste it into [Google Gemini Deep Research](https://gemini.google.com/) (or any AI research tool that does deep research).
3. Wait for the research to finish (usually a few minutes).
4. Copy the research results back into Claude Code and say: "Here are the research results. Please integrate them into my skill."
5. Claude updates your skill file with expert-level structures, hooks, language patterns, and quality checks.

**The result:** A skill that doesn't just describe the format, but writes it like a top-1% practitioner.

---

## Examples

**Newsletter skill:**
"What makes a top 1% email newsletter for product people? Best structures (PAS, Sequence, One Big Idea), opening formulas that earn the open, sentence-level moves the best Substacks use, common mistakes that kill engagement, and 5 real newsletters worth studying."

**Sales proposal skill:**
"What makes a top 1% B2B sales proposal for $50K+ enterprise deals? Proven structures (Challenger, Mutual Action Plan), executive summary patterns, pricing-page conventions, mistakes that lose deals, and 3 real-world proposals worth studying."

**PRD skill:**
"What makes a top 1% PRD for engineering teams at growth-stage SaaS? Proven structures (Amazon PR-FAQ, Stripe-style), how to write the problem statement, common PM-to-eng failure patterns, and 3 PRDs worth studying."

**Hebrew newsletter skill:**
"What makes a top 1% Hebrew-language newsletter for Israeli tech founders? Cultural conventions, opener patterns that work in Hebrew specifically, length norms for Israeli inboxes, and 3 Hebrew newsletters worth studying."

---

## When to Use Enhance-Skill vs Enhance-Agent

| Question | Use |
|----------|-----|
| "How does this PERSON think?" | `02-enhance-agent-with-research.md` (upgrades a thinker) |
| "How is this OUTPUT FORMAT done at the highest level?" | This prompt (upgrades a craft) |

You can run both. An expert thinker armed with an expert craft is the combo that produces world-class output.

---

> **© Tom Even**
> Workshops & future dates: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
