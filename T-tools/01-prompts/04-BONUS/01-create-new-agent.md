# Prompt: Create a New Agent

Use this to add a new agent to your team.

Copy and paste this into your chat (fill in your agent idea first):

---

```
I want to create a new agent for my team. Here's what I need:

---
Agent name: [e.g., "researcher", "editor", "social-media-manager"]
Main responsibility: [What should this agent do?]
When to use: [In what situations should this agent be activated?]
---

Please do the following:

1. First, study the existing agents to understand the structure and style:
   - Read A-agents/copywriter-agent.md
   - Read A-agents/gatekeeper-agent.md
   - Notice the format: frontmatter, core identity, required reading, checklists, output format

2. Read the brand core so the new agent knows the user + the brand (all 7 files):
   - C-core/about-me.md
   - C-core/company-context.md
   - C-core/project-brief.md
   - C-core/voice-dna.md
   - C-core/icp-profile.md
   - C-core/team-roster.md
   - C-core/company-glossary.md

3. Create the new agent file in A-agents/ folder:
   - Use the same structure as existing agents
   - Include frontmatter (name, description)
   - Define core identity and mission
   - Add "Required Reading" section pointing to relevant C-core and M-memory files (and B-brain/02-my-samples as optional)
   - Create specific checklists for this agent's job
   - Define output format
   - Add collaboration instructions (who does this agent work with?)
   - Include a "The Loop" section explaining how this agent contributes to system learning

4. Create a slash command for the new agent at .claude/commands/[agent-name].md:
   - Study an existing command first (e.g., .claude/commands/copywriter.md) to match the pattern
   - Structure: Before Responding (mandatory reads) → Response Style → What You Do → "User's Request" section ending with $ARGUMENTS
   - Point "Before Responding" to the new agent file in A-agents/, all 7 C-core files (about-me, company-context, project-brief, voice-dna, icp-profile, team-roster, company-glossary), and M-memory
   - The slash command lets the user invoke this agent directly with /[agent-name] [request]

5. Update M-memory/learning-log.md:
   - Add an entry documenting the new agent
   - Note its role and how it fits with the team
   - Note the slash command name so the user remembers how to invoke it

6. Update A-agents/gatekeeper-agent.md:
   - Add the new agent to the "Your Team" section if relevant
   - Define how Gatekeeper should review this agent's work (if applicable)

7. Update A-agents/README.md:
   - Add the new agent to the appropriate section (base / deluxe / support)
   - Include its one-line description

8. Consider if any workflows need updating:
   - Should this agent be part of an existing workflow?
   - Should we create a new workflow for this agent?

Show me the new agent file, the new slash command, and confirm all updates are done.
```

---

> **© Tom Even**
> Workshops & future dates: [www.getagents.today](https://www.getagents.today)
> Newsletter: [www.agentsandme.com](https://www.agentsandme.com)
