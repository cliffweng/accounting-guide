# Accounting & Financial Statements Study Guide

A practical study guide for reading the three financial statements — built for investment-banking and markets interview prep, and for self-study.

**Live site:** https://cliffweng.com/accounting-guide/

## Audience

Written for builders and interview candidates. The assumption is that you are analytically strong and *have never had an accounting course*. So this guide is biased toward **interview rigor on the three statements** — why a number moved, how the statements link, how to read a 10-K — and deliberately **not** toward bookkeeping drills, debits and credits mechanics, tax, or consolidation accounting.

If you can already post a balanced journal entry, you can skip [Journal entries, lite](topics/03-journal-entries-lite/) and start at the statements.

## Roadmap

14 topics, one file each under [`topics/`](topics/), ordered foundational → applied:

1. The accounting equation
2. Accrual vs. cash
3. Journal entries, lite
4. Income statement
5. Balance sheet
6. Cash flow statement
7. Linking the three statements
8. Revenue recognition basics
9. Expenses & matching
10. Working capital
11. Ratios (liquidity, profitability, leverage)
12. Depreciation & amortization
13. Inventory & COGS
14. Interview hotspots

## Interview hotspots

Every topic page carries a badge (🎯 Interview frequent / Interview occasional / Background) so you know where to spend prep time. If you're short on time, prioritize these:

- **The accounting equation** — the identity the whole field hangs from, and the fastest way to check whether a set of statements is internally consistent.
- **Accrual vs. cash** — the single most-missed concept. Expect "net income was up, why is cash down?" and "is this company actually profitable?" with zero setup.
- **Journal entries, lite** — just enough concept to see *why* depreciation is a non-cash expense and why receivables can be good news. Not a drill.
- **Income statement** — structure, the recurring vs. non-recurring distinction, and reading growth *quality* rather than growth rate.
- **Balance sheet** — assets = liabilities + equity, what a deficit actually means, and reading operating leverage off a fixed-cost base.
- **Cash flow statement** — CFO vs. CFI vs. CFF, why CFO should roughly track net income over a cycle, and capex.
- **Linking the three statements** — the retention roll-forward, the debt/cash loop, and the indirect-method reconciliation from net income to CFO. If you only prep one page for a banking screen, prep this one.
- **Working capital** — NWC, the CCC, and cash conversion as a driver of both growth and funding needs.
- **Ratios** — DuPont, ROIC vs. ROE, and what leverage does to reported returns.
- **Interview hotspots** — how to actually deliver "walk me through the three statements" out loud in 8–12 minutes, including the traps.

**Occasional/Background**: journal-entry mechanics, revenue recognition edge cases, expense-matching detail, D&A schedules, and inventory/COGS accounting mechanics. These matter but rarely anchor a loop on their own.

This split is a judgment call based on what shows up in banking and markets interviews, not a guarantee for any specific process — adjust your prep if a role is unusually FP&A-, audit-, or quant-research-flavored.

## How to use this guide

Each topic page is designed to be read in **~10 minutes** and follows the same structure: why it matters, core concepts, a mental model, 3–6 interview questions with brief answer keys, and a short list of verified YouTube videos. Read them in order, or jump straight to what you need. No backend, no login, no paid data — just read the pages.

## How to contribute

See [CONTRIBUTING.md](CONTRIBUTING.md). In short: one topic per file, keep it under ~10 minutes to read, and only link to sources (especially YouTube videos) you've personally verified exist. Open an issue before proposing new topics or restructuring the curriculum.

## Decisions

These are the product locks this guide was built against — echoed here so future contributors don't accidentally relitigate them:

- **Audience**: builders and interview candidates, targeting investment-banking and markets interviews. Not a CPA crash course, not a tax guide, not a consolidation text.
- **Interviews-first, not bookkeeping-first**: three-statement fluency, not voucher-to-ledger drills. Accounting mechanics appear only where they explain a reported number.
- **Time-boxed**: every topic is readable in 10 minutes or less. Depth is sacrificed for scannability; "further reading" links are where depth lives.
- **Learning + interview prep in one page**: each topic pairs core concepts with interview questions, rather than splitting them into separate tracks.
- **Real links only**: every YouTube link is verified to exist before being added. No invented URLs, ever.
- **Static site, GitHub Pages, Just the Docs**: no backend, no auth, no quizzes, no consolidation modules. Cheap to host, cheap to maintain, easy to contribute to via plain Markdown + front matter.

## Enabling GitHub Pages

Just the Docs is configured via `_config.yml` (remote theme). After this lands on `main`:

1. Repo **Settings → Pages**.
2. **Build and deployment → Source**: **Deploy from a branch**.
3. Branch: `main` / folder: `/ (root)`.
4. Save. Site publishes to https://cliffweng.com/accounting-guide/

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## License

[MIT](LICENSE)
