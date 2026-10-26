# ESCO Skills Map — a free agent skill by ReLoop.me

**Map any job ad or CV to ESCO, the European Commission's official classification of occupations and skills.** A free SKILL.md for Claude, Claude Code, Cursor, Codex CLI, Gemini CLI, GitHub Copilot and other agents that read SKILL.md skills.

Built by [ReLoop.me](https://www.reloop.me/?utm_source=github&utm_medium=esco_skills_map&utm_campaign=readme), the capability intelligence platform for nonlinear careers and skills-based hiring.

## What it does

Paste a job ad or a CV. The skill returns a neutral, standardised ESCO skills map:

- the **1–3 closest ESCO occupations**, with official labels and URIs
- each requirement or claimed skill mapped to an **ESCO skill or knowledge concept**
- for each item: **essential or optional** for the occupation, **reuse level** (transversal, cross-sector, sector-specific, occupation-specific) and **type**
- the items with **no ESCO match**, listed as written, never forced
- a short, neutral **coverage** note

When the agent has web access, every label and URI is verified against the public [ESCO API](https://esco.ec.europa.eu/en/use-esco/use-esco-services-api). Without web access, items are marked `unverified`. It works in all EU languages, Romanian and French included, and can output JSON for ATS and HR-tech workflows.

### Example requests

- "Map this job ad to ESCO."
- "Which ESCO skills does my CV evidence?"
- "Which ESCO occupation is closest to this role, and which of its essential skills does the ad leave out?"
- "Give me this job ad as an ESCO skills map in JSON."

## What it deliberately doesn't do

ESCO describes what a role or profile is made of. It doesn't judge seniority, the scope a role really supports, requirement inflation, pay or fit, so neither does this skill.

Those are **capability intelligence** questions, answered by ReLoop.me:

- [Role Intel](https://www.reloop.me/role-intel?utm_source=github&utm_medium=esco_skills_map&utm_campaign=readme) reads a job ad: the level its scope really supports, how inflated its requirements are, and the likely pay range.
- [Profile Intel](https://www.reloop.me/profile-intel?utm_source=github&utm_medium=esco_skills_map&utm_campaign=readme) is a candidate-led read of a CV for nonlinear careers: distinctive capabilities, where the professional signal is likely to be misread, and market value.
- The [Role Intel API and MCP server](https://api.reloop.me/?utm_source=github&utm_medium=esco_skills_map&utm_campaign=readme) brings the Role Intel read to job boards, ATS tools and AI agents (free quick check, paid full reads).

## Install

**Claude (web or app):** get `esco-skills-map.zip` free from [Agensi](https://www.agensi.io/skills/esco-skills-map), then upload it in Claude under Settings → Capabilities → Skills.

**Claude Code and other file-based agents:** copy the [`esco-skills-map`](esco-skills-map/) folder into your agent's skills directory. For Claude Code that is `~/.claude/skills/` (all projects) or `.claude/skills/` (one project).

More about the skill: [reloop.me/esco-skills-map](https://www.reloop.me/esco-skills-map?utm_source=github&utm_medium=esco_skills_map&utm_campaign=readme).

## Network use

When web access is available, the skill calls the public ESCO API (`ec.europa.eu/esco/api`) to verify occupation and skill labels. It sends only the search terms it is checking. It makes no other network calls.

## Licence

© 2026 ZORRI S.R.L. (ReLoop.me). Free to use in your own agents, for personal or business work. Redistribution, resale or republishing of this skill, in whole or in part, is not permitted. See [LICENSE](LICENSE).

This service uses the ESCO classification of the European Commission. ESCO data is © European Union, reused under the European Commission's reuse policy, and is not covered by this licence. The European Commission does not endorse ReLoop.me.

---

**ReLoop.me** — capability intelligence for nonlinear careers and skills-based hiring. Built in the EU by [Ligia Adam](https://www.linkedin.com/in/ligiaadam). Operated by ZORRI S.R.L., Bucharest, Romania. Contact: hello@reloop.me
