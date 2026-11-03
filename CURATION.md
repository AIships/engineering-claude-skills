# Curation rules

## Goal

A Top 20 list of Claude skills a software engineer must have, kept current every week. Not a dump of everything on GitHub.

## Scope: in

- Software engineering only: planning, coding, testing, debugging, refactoring, code review, architecture, docs for code, deployment, MCP, API and SDK work, frontend engineering, developer tooling.
- Skills that work in Claude Code, ideally also in Codex, Cursor, or compatible agents.
- Skills with a clear install path: plugin marketplace, npx skills add, or a SKILL.md folder you can copy.

## Scope: out

- Creative work for its own sake: generative art, posters, GIFs.
- Brand, internal comms, marketing, SEO, general writing.
- Document production (docx, pdf, pptx, xlsx) unless it is part of a dev workflow. Those live in archive.
- Skills with no maintained source, no README, or a broken install.

## How a skill gets in

All four must hold:

1. Useful on a real task. It solves a concrete pain: losing track on long tasks, generic UI, outdated docs, no tests, flaky debugging, token waste, forgotten context.
2. Maintained. A commit, release, or maintainer activity in the last 90 days, or an official Anthropic source that is still current.
3. Verifiable. Source repo, license, and install command can be checked. Star count is noted but proves nothing.
4. Distinct. It does not duplicate a Top 20 skill already in the list. If two skills do the same job, keep the better maintained one and archive the other.

## How we rank: outcomes, not checklists

Textbook criteria (clean README, installs fine, maintained) only get a skill through the door. The ranking itself is outcome-based: what does this skill actually do for the person using it?

- Engineering: does it help ship more, ship better, debug faster, waste less time and fewer tokens? Evidence that counts: benchmarks, head-to-head tests, real team adoption, documented before-and-after.
- Finance: does it help a retail investor make better decisions and better risk-adjusted returns? Does it give a trader a real edge? Evidence that counts: backtested or paper-traded records, disclosed methodology, real risk controls. Stars and marketing copy count for nothing.

When outcome evidence is thin, we say so plainly and rank accordingly. A polished skill with no proof of outcomes sits below an ugly one with proof. No skill is ranked on promises.

## How a skill gets dropped

- Unmaintained for 90+ days, broken install, or replaced by a better skill.
- A new skill beats it on the same job in a head-to-head test.
- It drifts out of software engineering scope.

When dropped: move it to archive/ARCHIVED.md with date, reason, and what replaced it. Never delete the record.

## The archive rule

Every skill we evaluate gets an entry in archive/ARCHIVED.md, whether it makes the Top 20 or not. In the list, dropped from the list, watchlist, or rejected: all of it, with a date and a reason. Anyone browsing the archive sees everything we looked at and why we decided what we did.

The only things that skip the archive are trash: dead repos with no README, broken installs that cannot be fixed, spam, or duplicates with nothing new. Those are not worth the bytes.

## How we write

- Write like a person, not an assistant. Short sentences. Plain words.
- Keyboard characters only. No em dashes, no special symbols, no decorative unicode. A hyphen does the job.
- Minimalism: say it once, say it short. Essentialism: every line earns its place. Craftsmanship: get the details right, check the links, spell things correctly.

## Weekly process, every Saturday around 9am PT

1. Check the Top 20: stars, last commit, open issues, breaking changes.
2. Check the watchlist and new contenders from the past week: GitHub trending, Reddit r/ClaudeAI and r/programming, Dev.to, Hacker News.
3. Test-install any candidate before adding. Do not add untested skills.
4. Swap at most 3 per week, usually 0 to 1. Stability matters.
5. Update README.md (date, table, watchlist), CHANGELOG.md (what changed and why), archive/ARCHIVED.md (dropped skills AND every candidate evaluated this week with its verdict: in, watchlist, or rejected).
6. Commit with a plain human message. Example: "Weekly curation Oct 31: swapped X for Y".
