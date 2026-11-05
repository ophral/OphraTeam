### Preparation: Installing the Project Files

1. Download the ZIP file and extract it.
2. Drag the extracted folder into your Obsidian Vault.
3. On Windows? It sometimes creates an extra ".obsidian" folder inside the Vault. Ignore it.
4. Make sure you can see all folders (A-agents, B-brain, C-core, T-tools, etc.) in the left sidebar in Obsidian. They're inside the the-system folder you extracted from the ZIP file.

### Preparation: Opening Your AI Coding Agent

This system works with both **Claude Code** and **OpenAI Codex** (and any tool that reads AGENTS.md or CLAUDE.md, including Cursor and Cline).

1. Open a new session in your agent of choice.
2. **Important:** Select the the-system folder as your working directory. This is how the agent knows where to read, edit, and create files.
3. **Slash commands:** Claude Code reads them from `.claude/commands/`. Codex reads them from `.codex/prompts/`. Both folders ship with this system. Same commands, same content.

---

### Step 1: Choose Your Track

Before you start, pick the track that fits your work:

**Content** (תוכן)
Publishable content that people read: social posts, newsletters, blog posts, articles.
*For: marketers, creators, founders, anyone who publishes content. Also great for thought leadership.*

**Communication** (תקשורת)
Professional text to a specific recipient: emails, Slack messages, internal updates, community messages, and more.
*For: founders, freelancers, consultants, HR, managers, anyone who writes professional messages.*

**Thinking** (חשיבה)
Decision briefs: you bring a decision you need to make, multiple agents debate it from different angles, and you get a structured brief with different perspectives.
*For: CEOs, PMs, business owners, managers, team leads, anyone who makes decisions.*

**Not sure which to pick?** Ask yourself:
- Do you publish things people read? → **Content**
- Do you write professional text to specific people? → **Communication**
- Do you need help making a decision? → **Thinking**

---

## Phase 1: Feed the Brain

*Do this in Obsidian first. before running any prompts. Just fill in the two files below.*

### Step 2: Fill in Your Information

Open the file `B-brain/01-context/01-context.md`

The file is split into four parts:
- **Part A. About Me** (you as a person: name, role, what you own, goals, how you work, personal voice)
- **Part B. Company Context** (the company: what it does, stage, industry, priorities, brand voice)
- **Part C. Audience (ICP)** (who reads or receives your work)
- **Part D. Anything else** (catch-all)

Fill in the text with your information (copy-paste from the document you filled in beforehand). When the prompt runs, the agent splits Part A into `C-core/about-me.md` and Part B into `C-core/company-context.md`, plus populates the rest of C-core.

**Don't have a "business"?** No problem. This works for anyone:
- If you work at a company: write about your role, your team, and the company you sit inside
- If you're a freelancer: Part A is you, Part B is your practice (positioning, niche, client mix)
- If you're exploring: Part A is you, Part B is the venture you want to build

**Do not change file names.** The prompts are linked to them.

### Step 3: Add Your Writing Samples

Open the samples folder that matches your track:
- **Content** → `B-brain/02-my-samples/01-content/`
- **Communication** → `B-brain/02-my-samples/02-communication/`
- **Thinking** → `B-brain/02-my-samples/03-thinking/`

Each folder has a README explaining exactly what to paste. Read it first.

Paste your text (Hebrew or English) into each of the 3 files: `sample-01`, `sample-02`, `sample-03`.

**Pro tip:** The better your samples, the better the output. Pick pieces you're proud of.

✋ **Finish both steps above before moving on. Don't run any prompts yet.**

---

## Phase 2: Run Your New Team

*Now go to your agent (Claude Code or Codex). Run one prompt at a time. Wait for it to finish before pasting the next one.*

All 4 prompts are inside your track folder under `T-tools/01-prompts/`:
- Content track → `T-tools/01-prompts/01-content/`
- Communication track → `T-tools/01-prompts/02-communication/`
- Thinking track → `T-tools/01-prompts/03-thinking/`

**Prompt 1. Learn From Context**

- Copy the entire content of `01-learn-from-context.md`
- Paste it in your agent and send.
- The agent reads your answers and splits them across the C-core files: `about-me`, `company-context`, `project-brief`, `icp-profile`, `voice-dna`.

**Prompt 2. Learn From Samples**

- Copy `02-learn-from-samples.md` and paste it.
- The agent reads the 3 samples and updates the Core documents, the agents, and Memory.

**Prompt 3. Create Your Output**

- Copy the `03-...` file from your track folder and paste it.
- Fill in the details:
  - **Content:** your topic or idea for a post/newsletter/article
  - **Communication:** who you're writing to and what about
  - **Thinking:** the decision you need to make and the options you're considering
- Adam (your COO agent) manages the entire team to create the output. The result is saved in `O-output/`.

What each track produces:

- **Content** A piece of publishable content (social post, blog post, or newsletter). 3 agents collaborate: Researcher finds angles → Copywriter writes in your voice → Gatekeeper reviews quality.
- **Communication** Professional text to a specific recipient (email, Slack message, internal update, community message). 3 agents collaborate: Strategist analyzes the situation → Copywriter writes in your voice → Gatekeeper reviews quality.
- **Thinking** A decision brief. You bring the decision you need to make, and 4 agents debate it from different perspectives (Strategist → Devil's Advocate → Chief of Staff → Gatekeeper). You get a structured brief with options and recommendations.

**Prompt 4. Close The Loop**

- Copy `04-close-the-loop.md` and paste it.
- Adam reviews what was just created, logs what worked and what didn't to M-memory, and promotes strong insights to C-core.
- This is what makes the system get smarter over time.

---

## Phase 3: Deep Dive (Workshop Hours 3 and 4)

*By now you have agents that produce real output in your voice. The second half of the workshop is about EXTENDING the system: building your own agents, skills, and workflows.*

All 5 deep-dive prompts live in `T-tools/01-prompts/04-deep-dive/`.

**Prompt 1. Create a New Agent**

- Copy `01-create-new-agent.md` and paste it.
- Fill in: agent name, main responsibility, when to use.
- The agent creates the agent file in A-agents/, the slash command in `.claude/commands/` (Claude Code) and `.codex/prompts/` (Codex), and wires it into the team.
- Use this to add a specialist that doesn't exist yet (e.g., a Recruiter Agent, a Board Reporter Agent, a Sales Researcher).

**Prompt 2. Enhance an Agent with Research**

- Copy `02-enhance-agent-with-research.md` and paste it.
- Fill in: which agent, its role, the domain.
- The agent generates a research prompt you paste into Google Gemini Deep Research (or any deep research tool).
- The results come back as expert-level knowledge. You paste them back into your agent, and the new agent goes from "follows instructions" to "thinks like a top-1% practitioner."

**Prompt 3. Create a New Skill**

- Copy `03-create-new-skill.md` and paste it.
- Fill in: skill name, what it teaches, when to use.
- The agent creates a new skill folder in T-tools/02-skills/ and wires it into the agents that need it.
- Use this when you keep producing the same kind of output and want a reusable template (e.g., newsletter-skill, weekly-update-skill, performance-review-skill).

**Prompt 4. Enhance a Skill with Research**

- Copy `04-enhance-skill-with-research.md` and paste it.
- Fill in: which skill, what it produces, who reads the output.
- The agent generates a research prompt you paste into Google Gemini Deep Research.
- The results come back as world-class structures, hook formulas, sentence patterns, and quality checks for that specific output format. You paste them back into the agent, and your skill goes from generic to top-1% playbook.
- Same mechanic as Prompt 2. Different target. Prompt 2 upgrades a thinker. Prompt 4 upgrades a craft.

**Prompt 5. Create a New Workflow**

- Copy `05-create-new-workflow.md` and paste it.
- Fill in: workflow name, what it does, which agents, trigger.
- The agent builds a multi-agent process in T-tools/03-workflows/ that you can invoke as one command.
- Use this for any multi-step process worth codifying (e.g., onboarding a client, preparing a board meeting, launching a feature).

✋ **Don't try all 5 in one session.** Pick the one that solves your biggest current pain. The others stay in your system, ready when you need them.

---

### Important Tip: Permissions

When the agent asks for permission to read or edit files, approve broadly for the session so you don't have to confirm each action.
- **Claude Code:** click "Allow always for session"
- **Codex:** run with `--auto-edit` (or pick "Auto" approval mode), or trust this folder when prompted

---

### What Happens Next? (After the Workshop)

- Your output is saved in the `O-output/` folder as a new file. You can read it both in Obsidian and in the agent's chat.
- **Keep extending:** The deep-dive prompts in `04-deep-dive/` are reusable forever. Every time you spot a new specialty, build the agent. Every time a process repeats, codify it as a workflow.
- **11 more bonus prompts:** `T-tools/01-prompts/05-BONUS/` (prompts 05-15) covers content calendars, API connections, competitor analysis, hook banks, self-audits, client onboarding flows, and more. For ongoing use after the workshop.
- **B2B / company users:** `05-BONUS/_deluxe/` has 7 department tracks (HR, Finance, Legal, Product, Management, Support, Customer Success) with department-specific 4-step pipelines.
- You can also try a different track. Pick a different track folder and run Prompt 3 again to see the same system produce a completely different output.
- **Tip:** Got a file and not sure where it goes? Drop it in `B-brain/_INBOX/`. It's your junk drawer. Sort it later, or ask the agent to sort it for you.

Yalla, good luck.
