# Changelog

## 2026-11-14 - v3, one swap

- Dropped ECC (slot 20): active and maintained, but no published outcome evidence, and its harness-tuning job is partly covered by #1 (Superpowers harness bootstrap) and #4 (gstack process roles). Replaced by globalmpc/backendskills: three backend-convention skills (api-endpoint, data-integrity, db-migration), MIT licensed, install with `npx skills add globalmpc/backendskills`. Test-installed Nov 14: the repo clones and all three skills are found. Evidence is an author-run 150-run stress test with hidden checks: critical mistakes 25 to 2 (Sonnet 5.5 13/75 to 0/75). Read the caveats in the README before trusting the headline: 20 of the 25 came from two tasks, 10 of 15 tasks had no critical mistake either way, runs cost about twice as much, and there is no independent replication yet. The raw runs and rerun instructions are in the repo, which is what earned it the slot.
- The other 19 entries were rechecked: every source repo had a commit Nov 6-14, no breaking changes. anthropics/skills had two commits this week: Nov 6 moved the Office skills to Apache 2.0, Nov 14 updated docx, pptx, xlsx, pdf. Still 19 folders, no new engineering skill. mcp-builder (#8) got a TypeScript SDK v2 guide Oct 28, so #8 stays current.
- Watchlist: Karpathy Skills (multica-ai) dropped from the watchlist, last commit Apr 20, 2026, fails the 90-day maintained rule. Added Graphify as an alternative to #15. MCode Stack, Unslop, and react-best-practices rechecked, all still waiting on evidence. Hallmark, GitNexus, open-gsd, Context Engineering, Pristine, playwright-cli unchanged.
- Evidence note: a Nov 2026 independent test on a 72,000-line codebase found code maps did not make answers more accurate. Graphify cut reading about 12 percent, Understand Anything helped only when asked through /understand-chat. Added as a caveat under #15.
- Candidates evaluated this week are all in archive/ARCHIVED.md: backendskills (in), Graphify, lot-map, claude-model-router, claude-config, REA, Agent Reach, Last 30 Days, Career Ops, cinematic-skill, guizang-game-skill, line-art-animation, spine-hero-skill, claude-3d-animated-shorts, MCode Stack recheck, Unslop recheck, react-best-practices recheck, Karpathy Skills (dropped from watchlist, unmaintained).
- The Pages site (docs/index.html) was rebuilt to match the README.

## 2026-11-07 - v2, no swaps

- No swaps. All 20 sources rechecked: every repo had a commit in the last 7 days, no breaking changes. Superpowers shipped v7.0.2 (Nov 3), Caveman 4.1.0 (Nov 7), Planning with Files v3.28.1 (Nov 7). anthropics/skills still has the same 19 folders, no new engineering skill; its Nov 6 commit only moved the Office skills to Apache 2.0.
- Accuracy fixes: #11 renamed to web-artifacts-builder, the exact folder name in anthropics/skills. #15 pinned to Egonex-AI/Understand-Anything (about 91k stars). #20 pinned to affaan-m/ecc. The "check the owner" warning is gone now that both are linked.
- Claude-Mem stays at #17 with a new caveat in the README: browser installs Oct 25-Nov 2 uploaded 30 days of prompts without asking. Fixed in v15.8.3 on Nov 2 with a consent panel. Installs after the fix ask first. The entry stays because the fix is shipped and there is no better memory skill on the list.
- Watchlist: driving-seat dropped, its repo now returns 404. Added vercel-labs/agent-skills (react-best-practices), Karpathy Skills (multica-ai), and Unslop. MCode Stack rechecked at 545 stars, still no published evals.
- Evidence note: a Subframe test in Oct 2026 found impeccable the only one of four design skills that changed the look. That backs the Oct 31 swap of Taste for Impeccable.
- Candidates evaluated this week are all in archive/ARCHIVED.md: Karpathy Skills, react-best-practices, Unslop, T3 Code, TradingAgents, tuicr, discernment-nudge, academy-guide, doc-coauthoring, driving-seat, MCode Stack recheck.
- The Pages site (docs/index.html) was rebuilt to match the README. It was still on v1, listing GSD, the dead Karpathy repo, and Taste Skill. It now matches v2.

## 2026-10-31 - v2, three swaps

- Dropped GSD (slot 4): gsd-build/get-shit-done was archived by its maintainer; last commit May 2026, so it fails the 90-day rule. Replaced by garrytan/gstack (was watchlist #1): team-in-a-box process with slash-command roles for design, review, QA, security, and release. Install path verified by cloning the repo.
- Dropped Karpathy Skills (slot 6): the linked source repo was deleted (404) and every known mirror is stale. Replaced by claude-api from anthropics/skills: the official API and SDK reference. SKILL.md verified in the repo.
- Dropped Taste Skill (slot 14): superseded by pbakaus/impeccable, which shipped v4.8.0 this week with 62 deterministic anti-slop detector rules. The npm package resolves at 4.8.0. Taste ranked last in the Oct blind test this README cited.
- Planning with Files moved from the old Thinking section into Workflow (slot 6). The Thinking and discipline section is gone; its other entry is archived.
- Watchlist: gstack, impeccable, and claude-api promoted out. Hallmark is now first in line. Added open-gsd/gsd-core, driving-seat, Pristine, and the playwright-cli skill as new names to watch.
- The other 17 entries were rechecked: every source repo has a commit in the last 90 days. No breaking changes found.

## 2026-10-28 - Plain human rewrite

- Rewrote all files in a human voice: keyboard characters only, short sentences, no AI-style symbols. No list changes.
- Added a "How we write" section to the curation rules so every future update follows it.

## 2026-10-27 - v1, initial Top 20

- Started the repo: software engineering only, Top 20, one in one out, archive instead of delete.
- Initial Top 20: Superpowers, Matt Pocock Skills, Addy Osmani Agent Skills, GSD, BMAD-METHOD, Karpathy Skills, Planning with Files, skill-creator, mcp-builder, frontend-design, artifacts-builder, webapp-testing, UI-UX Pro Max, Taste Skill, Understand-Anything, Context7, Claude-Mem, Diagram Design, Caveman, ECC.
- Archived on day 1 (not software engineering): algorithmic-art, canvas-design, brand-guidelines, internal-comms, slack-gif-creator, theme-factory, docx, pdf, pptx, xlsx.
- Watchlist: gstack, Hallmark / Impeccable, GitNexus, Context Engineering / Context Mode, claude-api.
- Next curation: Saturday 2026-10-31, around 9am PT.
