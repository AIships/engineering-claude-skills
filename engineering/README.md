# Top 20 Claude skills for software engineering

A weekly curated list. Software engineering only, no fluff.

Last updated: 2026-11-21 (v3, no swaps)
Next curation: Saturday 2026-11-28, around 9am PT
Rule: always 20. One in, one out. Dropped skills move to archive, never deleted.

Browse it as a simple site: https://aiships.github.io/engineering-claude-skills/

This is an index, not a copy. Each entry links to its source repo. Read the source README and license before you install anything. Star counts below are from Oct 27-31 and change daily. Treat them as a popularity signal, not proof of quality.

## How to use this list

1. Start with one workflow framework from 1-6, not all six.
2. Add the official Anthropic skills you actually need from 7-12.
3. Add one skill per real pain point after that: UI, understanding code, context, tokens, backend safety.
4. Install only what you will use. Every enabled skill costs context.

Install patterns (check the source repo first, commands change):

```bash
# Anthropic official marketplace
/plugin marketplace add anthropics/skills
/plugin install example-skills@anthropic-agent-skills
/plugin install document-skills@anthropic-agent-skills

# Most community skills: copy the skill folder, or use the repo's installer
# Global (all projects):
cp -r <skill-folder> ~/.claude/skills/
# Project only:
cp -r <skill-folder> .claude/skills/
```

## The Top 20

### Workflow and methodology

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 1 | Superpowers | [obra/superpowers](https://github.com/obra/superpowers), about 306k stars, checked Oct 28 on GitHub | Plan first, test-driven development, systematic debugging, subagent-driven work, verify before finishing | You want Claude Code to act like a disciplined senior engineer instead of jumping straight to code |
| 2 | Matt Pocock Skills | [mattpocock/skills](https://github.com/mattpocock/skills) | Small composable skills for real engineering work | You want bite-size skills you can adopt one at a time |
| 3 | Addy Osmani Agent Skills | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills), about 101k stars | Production-grade spec, build, test, ship workflows | You want a shipping workflow, not just a coding helper |
| 4 | gstack | [garrytan/gstack](https://github.com/garrytan/gstack), about 138k stars, checked Oct 31 on GitHub | Team-in-a-box process: slash-command roles for design, eng management, review, QA, security, and release | You want a full engineering-team process around your agent, not just a coding helper |
| 5 | BMAD-METHOD | [bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) | Agile AI-driven development method | You want an agile, role-based method for bigger builds |
| 6 | Planning with Files | [OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files) | Breaks tasks into steps and tracks progress in files | Any coding task longer than a few minutes, where Claude loses track |

### Official Anthropic, software engineering only

Source: [anthropics/skills](https://github.com/anthropics/skills), about 184k stars, 19 skill folders, checked Oct 31 on GitHub. Only the engineering ones made the Top 20. Document, brand, art, and comms skills are in archive.

| # | Skill | What it does | When to use it |
|---|---|---|---|
| 7 | skill-creator | A skill that writes skills, following Anthropic's own authoring practice | Every time you catch yourself explaining the same procedure twice |
| 8 | mcp-builder | Guide for building good MCP servers | You need Claude to reach an API, database, or outside service |
| 9 | claude-api | Reference for the Claude API and SDKs: model ids, pricing, params, streaming, tool use, caching | You build with the Claude API and want current facts, not the model's memory |
| 10 | frontend-design | Distinctive, production-grade UI direction | You build web interfaces and want to avoid generic-looking pages |
| 11 | web-artifacts-builder | Build complex HTML artifacts with React, Tailwind, shadcn | You build interactive artifacts or web apps in Claude |
| 12 | webapp-testing | Test local web apps with Playwright for UI checks and debugging | You need browser-driven QA before shipping a web app |

### Frontend and UI

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 13 | UI-UX Pro Max | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Design intelligence: styles, palettes, UX rules | Your UI looks AI-made and you want a real design system |
| 14 | Impeccable | [pbakaus/impeccable](https://github.com/pbakaus/impeccable), about 98k stars, checked Oct 31 on GitHub | Design vocabulary for agents: polish, critique, audit commands plus 62 deterministic anti-slop detector rules | Your agent-built UI looks generic and you want concrete, checkable design feedback |

Honest caveat: independent blind tests in Oct 2026 ranked UI-UX Pro Max first on one test, and a Subframe test the same month found impeccable the only one of four design skills that changed the look. Impeccable uses deterministic detectors instead of LLM judgment. Some design skills burn a lot of tokens. Use one design skill at a time and judge on your own brief.

### Understanding, docs, context

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 15 | Understand-Anything | [Egonex-AI/Understand-Anything](https://github.com/Egonex-AI/Understand-Anything), about 91k stars, checked Nov 7 on GitHub | Turns a codebase into an interactive knowledge graph you can explore and ask about | You are onboarding to an unfamiliar codebase |

Honest caveat: an independent Nov 2026 test on a 72,000-line codebase found code maps did not make answers more accurate. Graphify cut reading about 12 percent, and Understand Anything helped only when asked through `/understand-chat`. Maps save reading time. They do not fix hard answers, so ask "where else could this be decided?" yourself.
| 16 | Context7 | [upstash/context7](https://github.com/upstash/context7) | Keeps current library docs in front of the model | Claude keeps using outdated library APIs |
| 17 | Claude-Mem | [thedotmack/claude-mem](https://github.com/thedotmack/claude-mem) | Persistent memory across sessions. Note: browser installs Oct 25-Nov 2 uploaded 30 days of prompts without asking; fixed in v15.8.3 (Nov 2) with a consent panel. Check the consent screen on install | Claude forgets your project between sessions |
| 18 | Diagram Design | [cathrynlavery/diagram-design](https://github.com/cathrynlavery/diagram-design), about 53k stars | Architecture, flow, org, and timeline diagrams, 44 types, exports to HTML, SVG, PNG | You need clean architecture diagrams from a codebase or a brief |

### Efficiency, harness, and backend

| # | Skill | Source | What it does | When to use it |
|---|---|---|---|---|
| 19 | Caveman | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Cuts output tokens hard while keeping technical accuracy | You are hitting usage limits and want shorter output |
| 20 | Backendskills | [globalmpc/backendskills](https://github.com/globalmpc/backendskills), 61 stars, created Nov 5, checked Nov 21 on GitHub | Three skills (api-endpoint, data-integrity, db-migration) that force caller-scoped queries, locks and idempotency keys, and expand-then-contract migrations | Your agent writes backend code that passes the demo and breaks in production: auth holes, money bugs, bad migrations |

Honest caveat: Caveman's author corrected the README Nov 17, dropping the 76 percent working-day claim (3 sessions, run once). Terminal-Bench 4 against Claude Code is level within noise; the tagline now reads 21 percent less than Codex per solved task. The claim got smaller and more honest, which is why it stays.

Honest caveat: the evidence is a 150-run stress test run by the author, not an independent replication. Critical mistakes fell from 25 to 2, but 20 of the 25 came from two tasks (login rate-limiting and column renames), 10 of 15 tasks had no critical mistake either way, and runs with the skills cost about twice as much ($0.11 vs $0.06). The raw runs and rerun instructions are in the repo's bench folder, which is why it earned the slot over ECC. Install with `npx skills add globalmpc/backendskills` (test-installed Nov 14: repo clones, all three skills found).

Both names have many mirrors. Use the linked repos. Do not install a fork without reading it.

## Watchlist for next Saturday

Did not make v3. First in line if a Top 20 slot opens:

- Context Mode (mksglu/context-mode): MCP server plus hooks that shrink tool output before it reaches the context window. 34,357 stars, v2.2.1 released Nov 17. One independent test (yoDEV, Nov 19) cut a 174 KB log to 6.5 KB with all three failures kept, but it measured the plumbing only, no live model session, and no compaction test. The author's own 98 percent headline counts bytes, not tokens, and the scripts were hand-written for files already seen. License is Elastic 2.0, not open source, and the Gateway routes requests through the vendor's server and keeps session records. Closest challenger to 19. Stays watchlist until a live-session replication lands. Install path verified Nov 21: plugin manifest and marketplace file exist in the repo
- Claude-BugHunter (elementalsouls/Claude-BugHunter): 83 skills and 15 commands for bug hunting, patterns from 681 disclosed HackerOne reports. 15,553 stars, up 9,300 in a week, number one trending Nov 18. Evidence is thin: self-reported red-team experience, no measured outcomes. Offense framing sits awkwardly in a general list
- spec-kit (github/spec-kit): GitHub's official spec-driven development toolkit, 150,916 stars, active Nov 20. Big adoption, no independent outcome evidence, and it duplicates the workflow jobs in 1, 3, 5, and 6
- cloudflare/security-audit-skill: six-phase security audit skill from Cloudflare's internal vuln-hunting harness, 76,573 stars. Last commit Sep 14, 68 days ago, inside the rule but quiet for 8 weeks. Overlaps 4's security role and 1's verification
- ponytail (DietrichGebert/ponytail): one skill that makes the agent write less code. 196,168 stars, last commit Oct 29. Author claims only: minus 53 percent code, minus 41 percent time, minus 26 percent cost. No independent replication
- emilkowalski/skills: design-engineering skills, 58,599 stars, active Nov 15. Overlaps 13 and 14, no outcome evidence
- Hallmark (Nutlope/hallmark): anti-slop design with 50 themes and a browser lint, alternative to 13. 58,944 stars, up 4,100 in a week, still no head-to-head vs 13 and 14
- react-best-practices (vercel-labs/agent-skills): 40+ React and Next.js performance rules from Vercel Engineering, 34,654 stars. Distinct from 10: performance, not design. No benchmarks yet, last commit Nov 20
- GitNexus (abhigyanpatwari/GitNexus): client-side knowledge graph with built-in RAG, alternative to 15. Very active, last commit Nov 21, still no head-to-head vs 15
- open-gsd/gsd-core: the official successor to the archived GSD, install with npx @opengsd/gsd-core. Active Nov 21, still no published evals vs 4 and 5
- Graphify (Graphify-Labs/graphify): codebase knowledge graph with a /graphify skill, alternative to 15. The Nov 2026 head-to-head found it cut reading about 12 percent but did not improve answer accuracy, so it stays a watchlist alternative, not a swap
- Unslop (heydamir/unslop): staged UI review, 19,649 stars. Overlaps 13 and 14, no comparative evaluation yet. Active Nov 15
- MCode Stack (MiniMax-AI/mcode-stack): harness engineering skills from the MiniMax Code team, MIT, 740 stars, 10 days old, no published evals. Standouts: independent-review, long-command-check, subagent-split-check. Active Nov 11, still no evals
- Pristine: UI critique skill, no verified repo yet
- playwright-cli skill: browser QA through an npm package, overlaps 12

## Left out on purpose

See archive/ARCHIVED.md. Short version: algorithmic-art, canvas-design, brand-guidelines, internal-comms, slack-gif-creator, theme-factory, docx, pdf, pptx, xlsx, discernment-nudge, academy-guide, doc-coauthoring. Real Anthropic skills, just not software engineering.

## Curation rules

Full rules in [../CURATION.md](../CURATION.md). Short version:

- Software engineering only.
- Maintained: a commit or release in the last 90 days, or an official Anthropic source that is still current.
- Installable and tested on a real task, not just starred.
- Stars help, they do not decide.
- Max 20. One in, one out. Archive, do not delete.
- Updated every Saturday morning, around 9am PT.
- Written like a human wrote it. Keyboard characters only, no AI-style symbols.

## License and attribution

This repo is a curated index with links. Each skill keeps its own license and owner. Do not copy a skill's files here without checking its license.
