# AI Agent Team - Project Instructions (v11)

## Session Start Protocol (MANDATORY)

When starting ANY new conversation from this folder, ALWAYS read these files first before responding.

### Canonical Read Order (TOKEN EFFICIENCY)

Read files in THIS EXACT ORDER, every time. Anthropic's prompt cache hits identical prefixes, so consistent ordering = significant token savings across the session.

### 1. Core Files (C-core/) - read in this exact sequence
1. `C-core/about-me.md` (Who YOU are: role, ownership, goals, personal voice)
2. `C-core/company-context.md` (The COMPANY: what it does, stage, priorities, brand voice)
3. `C-core/project-brief.md` (What you produce in this role at this company)
4. `C-core/voice-dna.md` (How you communicate: blends personal + brand voice)
5. `C-core/icp-profile.md` (Who reads or receives your work)

Read `C-core/team-roster.md` and `C-core/company-glossary.md` only if the task references named people or product terms. They are not in the default load.

**Why about-me.md and company-context.md are separate:** You as a person are not the company. The agents need both. For internal Slack messages, personal LinkedIn posts, and 1:1 communication, your personal voice and ownership matter. For sales decks, brand content, and external proposals, the company identity leads. Keep them in sync, but separate.

### 2. Memory Files (M-memory/)
- `M-memory/learning-log.md` (What we've learned together)
- `M-memory/feedback-audience.md` (Audience reactions and signals)
- `M-memory/feedback-system.md` (Your corrections and preferences for the agents)
- `M-memory/decisions.md` (Strategic choices made)

### 3. Agent Definitions (A-agents/)
- `A-agents/adam-agent.md` (Your COO - manages the team and workflows)
- `A-agents/copywriter-agent.md` (Content creation agent)
- `A-agents/gatekeeper-agent.md` (Quality review agent)
- `A-agents/researcher-agent.md` (Research and web intelligence agent)
- `A-agents/analyst-agent.md` (Turns raw material into structured documents)
- `A-agents/strategist-agent.md` (Strategic analysis from business/growth perspective)
- `A-agents/devils-advocate-agent.md` (Challenges assumptions and finds blind spots)
- `A-agents/chief-of-staff-agent.md` (Synthesizes multiple perspectives into decision briefs)
- `A-agents/tom-agent.md` (Your guide to the ABC-TOM system)

---

## Token Efficiency Rules (System-Wide)

These four techniques minimize cost without changing output quality.

### 1. Canonical Read Order (already specified above)
Read files in the same order every time. Maximizes prompt cache hits.

### 2. Context Packet Pattern (within pipelines)
When an agent runs Stage 1 of a pipeline, it outputs a "Context Packet" at the top of its draft:
```
<!-- CONTEXT PACKET -->
- Me: [name, role, what I own that's relevant here]
- Company: [name and stage]
- Voice cues: [3-5 bullets, note personal vs brand if it matters]
- Audience: [primary reader]
- Key people: [relevant names]
- Banned terms: [from glossary]
- Domain notes: [department-specific facts used]
<!-- END PACKET -->
```
Stages 2-N (Copywriter, Compliance, Gatekeeper) read the Packet instead of re-reading C-core. Same quality, ~50% fewer tokens for downstream stages.

### 3. Skill-by-Trigger Loading
When the user picks a Type in the create-output prompt, the agent reads ONLY the matching skill file. It does NOT scan the other skill options. The Type-to-skill mapping is in each prompt.

### 4. Memory Decay
Active memory files stay lean. Entries older than 90 days move to `M-memory/archive/[YYYY-MM].md`. Patterns worth keeping forever get promoted to `C-core/voice-dna.md` instead of accumulating in learning-log.

---

## How This Works

Your AI coding agent (Claude Code, Codex, Cursor, Cline, anything that respects AGENTS.md or CLAUDE.md) automatically reads this file when you open a conversation from this folder.

The files above are your "memory". They persist between sessions. When you update them, future sessions will have that context.

**IMPORTANT:** Actually read these files before responding. Don't just acknowledge them. Scan C-core to understand the brand, check what's in A-agents, and review M-memory for context. This makes your responses relevant to THIS user's system.

---

## The 3 Workshop Tracks

| Track | Folder | What It Creates | Agents Involved |
|-------|--------|----------------|-----------------|
| **Content** | `T-tools/01-prompts/01-content/` | Publishable content: social posts, newsletters, blog posts | Adam → Researcher → Copywriter → Gatekeeper |
| **Communication** | `T-tools/01-prompts/02-communication/` | Professional text to a recipient: emails, Slack messages, internal updates, community, education | Adam → Strategist → Copywriter → Gatekeeper |
| **Thinking** | `T-tools/01-prompts/03-thinking/` | Decision briefs: multiple agents debate your question, you get a brief with different perspectives | Adam → Strategist → Devil's Advocate → Chief of Staff → Gatekeeper |

---

## The ABC-TOM Loop (v11)

After completing significant work, close The Loop:

1. **New insight about what works?** Update `M-memory/learning-log.md`
2. **Received audience feedback?** Update `M-memory/feedback-audience.md`
2b. **User corrected an agent?** Log it in `M-memory/feedback-system.md`
3. **Made a strategic decision?** Update `M-memory/decisions.md`
4. **Pattern strong enough to become a rule?** Promote it to `C-core/voice-dna.md`
5. **Research worth keeping?** Move it from `B-brain/_INBOX/` to the right subfolder

The Loop is what makes the system compound. Every project that closes The Loop makes the next project better.

Run `04-close-the-loop.md` from your track folder (`01-content/`, `02-communication/`, or `03-thinking/`) to close The Loop explicitly.

---

## Quick Commands

- "כתוב פוסט על [נושא]" - Creates content using your voice
- "תכתוב הצעה ל[לקוח]" - Creates a client proposal
- "תסכם את [הישיבה/הראיון]" - Creates a structured summary
- "תבדוק את האיכות" - Runs gatekeeper review
- "מה למדנו?" - Shows learning log summary
- "סגור את הלופ" - Runs The Loop (updates memory + promotes insights)
- `/tom [question]` - Get help from Tom on the ABC-TOM system
- `/adam [what you want to build]` - Your COO helps you build agents, skills, connect tools

---

## Deluxe: Department-Specific Tracks

| # | Track | Folder | What It Creates | Agents Involved |
|---|-------|--------|----------------|-----------------|
| 01 | **HR** | `T-tools/01-prompts/05-BONUS/_deluxe/01-hr/` | JDs, onboarding, reviews, employer brand | Adam → HR Specialist → Copywriter → Compliance → Gatekeeper |
| 02 | **Finance** | `T-tools/01-prompts/05-BONUS/_deluxe/02-finance/` | Board reports, budgets, investor updates | Adam → Financial Analyst → Strategist → Compliance → Gatekeeper |
| 03 | **Legal** | `T-tools/01-prompts/05-BONUS/_deluxe/03-legal/` | Contracts, policies, risk assessments | Adam → Legal Counsel → Compliance → Gatekeeper |
| 04 | **Product** | `T-tools/01-prompts/05-BONUS/_deluxe/04-product/` | PRDs, specs, release notes, competitive intel | Adam → Product Strategist → Devil's Advocate → CoS → Gatekeeper |
| 05 | **Management** | `T-tools/01-prompts/05-BONUS/_deluxe/05-management/` | OKRs, decisions, board narratives | Adam → Management Advisor → Strategist → DA → CoS → Gatekeeper |
| 06 | **Support** | `T-tools/01-prompts/05-BONUS/_deluxe/06-support/` | KB articles, playbooks, troubleshooting | Adam → Support Specialist → Copywriter → Gatekeeper |
| 07 | **Customer Success** | `T-tools/01-prompts/05-BONUS/_deluxe/07-customer-success/` | QBRs, success plans, expansion proposals | Adam → CS Agent → Strategist → Copywriter → Gatekeeper |

### Cross-Department Workflows

For business events that span multiple departments: `T-tools/03-workflows/_deluxe/` (the numbered files `01-` through `07-`)

7 orchestrated workflows that coordinate multiple agents across departments to produce coherent output bundles.

### Deluxe Navigation

Start here: `_deluxe/README.md` (the full menu card with quick start guide)

---

## Need Help?

**Want to understand the system?** Type `/tom` and ask.
Tom explains how ABC-TOM works, what each folder does, and answers questions about the framework.

**Want to build something?** Type `/adam` and tell him what you need.
Adam manages the team, creates agents, builds skills, connects external tools, organizes your system, and sets up workflows.

Both work in Hebrew and English.

---

> **© Tom Even**
> Workshops: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
