# Top 20 Claude skills for finance

A weekly curated list for retail investors and traders. Ranked by outcomes, not checklists.

Last updated Nov 15, 2026 (v1). 19 of 20 slots filled. One slot left open on purpose: nothing else passed the bar, and we do not pad.

Star counts checked Nov 15, 2026. They move daily. Treat them as an adoption signal, not proof of quality.

## The honest part first

No skill on this list has a verified performance record. Not one publishes an audited track record or an independently replicated backtest. That is the state of this whole category in November 2026.

So the ranking runs on what can be checked: disclosed methodology, real risk controls, paper-first defaults, maintenance, and adoption. Where a skill is one person's method or a vendor's front door, the entry says so. Research only, not financial advice.

## Scope

In: investing research, trading tooling that is paper-first, personal finance.
Out: crypto pump bots, guaranteed-returns hype, signal-selling, anything that places real-money orders without human approval. Full rules in [../CURATION.md](../CURATION.md).

## The list

| # | Skill | Lane | Stars | What it does |
|---|---|---|---|---|
| 1 | [Claude for Financial Services](https://github.com/anthropics/financial-services) | Investing research | 41.3k | Anthropic's official finance plugins: comps, DCF, LBO, earnings, 3-statement models, plus named research agents |
| 2 | [Claude Trading Skills](https://github.com/tradermonty/claude-trading-skills) | Investing process | 5.4k | 74 skills for individual investors: regime checks, screeners, position sizing, trade planning, journaling, postmortems |
| 3 | [Day Trader Skill](https://github.com/Jakeschincariol/day-trader-skill) | Trading | 8.0k | 11 skills: chart scanner, news monitor, entry timer, exit planner, a 10,000-replay setup tester, risk and budget gates |
| 4 | [Finance Skills](https://github.com/himself65/finance-skills) | Investing research | 3.6k | Analysis library: correlation, liquidity, market analysis, TradingView reader |
| 5 | [Trader Skill](https://github.com/Jakeschincariol/trader-skill) | Investing research | 1.8k | 13F copycat portfolios from SEC filings, Congress trade tracker, earnings analyst, tax lots, rebalancing |
| 6 | [A-Stock Data](https://github.com/simonlin1212/a-stock-data) | Data layer | 11.8k | Full China A-share data stack in one SKILL.md: 87 endpoints, 34 sources, almost no API keys |
| 7 | [Trading Skills](https://github.com/staskh/trading_skills) | Trading, options | 411 | About 25 skills: options advisor with Greeks and roll candidates, insider tracker, stock reports |
| 8 | [OpenMobius Skill](https://github.com/MobiusQuant/OpenMobius-skill) | Trading methodology | 726 | 2,008 curated ICT/SMC knowledge cards, live data, chart generation. Analysis only |
| 9 | [Claude Equity Research](https://github.com/quant-sentiment-ai/claude-equity-research) | Investing research | 759 | Generates full equity research reports: fundamentals, technicals, risk |
| 10 | [OpenAccountants](https://github.com/openaccountants/openaccountants) | Personal finance, tax | 492 | 2,132 tax skills across 249 jurisdictions, every rate and deadline cited to its legal source |
| 11 | [FinLab AI Skill](https://github.com/koreal6803/finlab-ai) | Trading, backtesting | 427 | Backtest Taiwan and US stocks on FinLab's real engine and adjusted data, no hand-rolled code |
| 12 | [Agentii Investment Intelligence](https://github.com/agentii-ai/agentii-investment-intelligence) | Investing research | 210 | 25 skills: SEC filings and XBRL financials, earnings, volatility analysis |
| 13 | [InvestSkill](https://github.com/yennanliu/InvestSkill) | Investing research | 285 | US stock analysis frameworks, no API keys, no subscriptions |
| 14 | [Finance Assistant](https://github.com/googlarz/finance-assistant) | Personal finance | 53 | Local-first money copilot: real tax statute on your numbers, bank statement parsing, Monte Carlo FIRE planning |
| 15 | [Stock Skill](https://github.com/xiongcp/stock-skill) | Trading, technicals | 119 | Deterministic K-line structure analysis for A-shares, HK, and US. Same input, same output |
| 16 | [Longbridge Skills](https://github.com/longbridge/skills) | Broker data | 71 | Official Longbridge skills: market data, fundamentals, valuation, your own portfolio across HK, US, A-share, Singapore |
| 17 | [Anti-Gambling Trader](https://github.com/mars-tw/anti-gambling-trader-tw) | Trading, risk | 1.2k | Discipline toolkit: paper broker by default, local trade statistics. Built to stop bad trades, not find more |
| 18 | [Serenity Stock Choke](https://github.com/fadewalk/serenity-stock-choke) | Investing, screening | 535 | Screening by the Serenity supply-chain bottleneck theory across A-shares, HK, US |
| 19 | [Portfolio123 Skill](https://github.com/cmoralesm/P123-Claude-Skill) | Investing, quant | 23 | Portfolio123 from an agent: 464 functions, 4,456 factors, reference checked line by line against the official docs |
| 20 | Open | - | - | Nothing else passed the bar this week |

## Notes and caveats

- **1, Financial Services:** built for professionals. Its data connectors (CapIQ, FactSet, Morningstar) need paid subscriptions. Agents draft work for human sign-off, they do not recommend or execute.
- **2, Trading Skills:** explicitly not a signal service, places no orders. Many screeners need an FMP API key. The starter path runs on free data.
- **3, Day Trader Skill:** paper trading is the default and no order goes through without your yes. One reviewer rates it high risk if you connect the broker. The 10,000-replay tester is a disclosed Monte Carlo method, not a track record.
- **6, A-Stock Data:** a data layer, not a strategy. It makes no decision claims. US-only investors may prefer the watchlist's global-stock-data instead.
- **7, Trading Skills (options):** one stop-loss skill can place orders, only with an explicit flag. Approval-gated, not autonomous.
- **8, OpenMobius:** ICT/SMC is a contested methodology. Listed as a knowledge base, not as proof of anything.
- **10, OpenAccountants:** AGPL-3.0 license, the one licensing caveat on this list. Its verification method is the strongest here: answers sourced to law, not model memory.
- **11, FinLab:** no LICENSE file found in the repo as of Nov 15. Vendor platform, full use needs a FinLab account.
- **14, Finance Assistant:** tiny adoption (53 stars). It is here because the personal finance lane is nearly empty and this one is genuinely built: deterministic calculators, data never leaves your machine, 1,630 tests claimed by the author.
- **16, Longbridge:** portfolio features need a Longbridge account. A data and access layer, not advice.
- **17, Anti-Gambling Trader:** Traditional Chinese, Taiwan-market focused.
- **18, Serenity Stock Choke:** one named investor's public method distilled into a skill. A method label, not an endorsement.
- **19, Portfolio123:** needs a paid Portfolio123 subscription. 23 stars is minimal adoption, the weakest pass on this list. It passes on verifiability and a job nothing else does.

## Watchlist for next Saturday

Did not make v1. First in line if a slot opens:

- global-stock-data (simonlin1212/global-stock-data): US/global sibling of 6, 1.9k stars. One of the two belongs; 6 has 6x the adoption
- Kansoku (kansoku-trade/kansoku): trading discipline skills inside a Mac stock app. License unclear, app-first
- MAIA Skill (Hainrixz/maia-skill): multi-agent market analysis, multi-asset including crypto, overlaps 4
- Fadacai Portfolio (PatrickSUDO/fadacai-portfolio): research framework with a thesis ledger. Traditional Chinese
- Alpha Skills (mphinance/alpha-skills): backtesting and edge research, 32 stars, edge claims unverified
- Oddly (KorroAi/oddly): SEC odd-lot tender offer scanner with backtest. 18 stars, AGPL
- claude-finance-skills (andreworia/claude-finance-skills): IB/PE valuation skills, but 1 covers the same jobs officially
- Excel Analyst Pro (jeremylongshore/excel-analyst-pro-skill-md): DCF and modeling toolkit, overlaps 1

## Left out on purpose

See archive/ARCHIVED.md. Short version: autonomous real-money trading harnesses, crypto execution tooling, everything-dump collections, full apps that are not skill packs, stale repos, and prediction-market bots.
