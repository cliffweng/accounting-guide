---
title: "14. Interview hotspots"
layout: default
nav_order: 15
---

# Interview hotspots
{: .no_toc }

*~10 min read*

**🎯 Interview frequent**

## Why it matters

You now have the content. This page is about *delivery* — how to say it out loud in 8–12 minutes, what the follow-ups are, and which mistakes cost you the most. "Walk me through the three statements" is the canonical technical question in investment-banking and markets loops, and the reason it keeps coming back is that it is unusually good at separating people who have read about accounting from people who can use it. The good news: it is a *learned* answer, and the structure below is the whole thing.

## Core concepts

- **Deliver in a fixed order, every time.** Consistency is what buys you thinking time. Six beats: (1) **frame** the three statements and the equation, (2) **income statement**, (3) **balance sheet**, (4) **cash flow statement**, (5) **the links**, (6) **one forward-looking implication**. Never improvise the structure; improvise only the examples.
- **Never recite a definition without a "so what."** Every line you describe should be followed by a consequence, an example, or a risk. "Inventory is a current asset" is worth nothing; "inventory is a current asset that becomes COGS on sale, which means COGS is a function of the inventory *estimate*, so a writedown hits gross profit one-for-one" is worth a lot.
- **The three links are the payoff and the most-tested part.** `Ending RE = Beginning RE + NI − Dividends`; `Ending cash = Beginning cash + CFO + CFI + CFF`; and the umbrella version — *Δ balance sheet = income statement activity + cash flows*. If you get nothing else out of this guide, get these.
- **The forward-looking consequence is what separates a recital from understanding.** The single best thing to land at the end: **profitable growth can consume cash**, because receivables and inventory grow with revenue. So when revenue accelerates, expect net income up and cash down — which is where the funding requirement, the revolver draw, and the interest-expense feedback loop come from.
- **Answer as a *process*, not a list.** For any "how would you assess this" or "your model doesn't balance" question, the ordering *is* the answer. Interviewers are grading your judgment about what to check first, not your recall of a checklist.
- **Be honest about what you don't know.** "I haven't worked with ASC 606 in detail, but here's how I'd think about it: contract, obligations, delivery, price allocation" scores far better than a confident wrong answer. The scoring rubric for these loops explicitly rewards sound reasoning over completeness.

## Mental model

```
  THE 10-MINUTE WALKTHROUGH
  ═══════════════════════════

  [1] FRAME (30s)        Three statements. IS = period, BS = date, CFS bridges.
                        Assets = Liabilities + Equity, at every date.
                              │
  [2] INCOME STMT (2m)   Revenue → COGS → GP → OpEx → EBIT → interest/tax → NI
                        "So what": recurring vs one-time; margins over levels
                              │
  [3] BALANCE SHEET (2.5m)  Assets by LIQUIDITY · Liabilities by MATURITY
                        Equity = residual.  "So what": current vs non-current
                        mismatch is real risk; asset quality ≠ face value
                              │
  [4] CASH FLOW (2.5m)   CFO (operations) · CFI (capex/M&A) · CFF (debt/equity/divs)
                        CFO = NI + D&A − ΔNWC        FCF = CFO − capex
                        "So what": capex vs D&A sustainability check
                              │
  [5] THE LINKS (1.5m)   End. RE   = Beg. RE + NI − Divs
                        End. cash = Beg. cash + CFO + CFI + CFF
                        ΔBS = IS activity + cash flows
                              │
  [6] IMPLICATION (1m)    Growth up → AR + Inventory up → CASH DOWN.
                        → funding need → revolver → interest → CFO
                        └────────────────────────────────────────┐
                                                                 ▼
                                                     "…which means a modest
                                                      operating shock can become
                                                      a solvency event if
                                                      leverage is high."
```

## The answer, in order

| Beat | Time | The one thing that must land |
|---|---|---|
| Frame | 30s | IS = period, BS = date, CFS bridges them; the equation holds at every date |
| Income statement | 2m | Structure, plus recurring-vs-non-recurring and margin *trend* |
| Balance sheet | 2.5m | Liquidity vs. maturity split; asset quality; equity is the residual |
| Cash flow | 2.5m | CFO/CFI/CFF with one example each; CFO = NI + D&A − ΔNWC; FCF = CFO − capex |
| The links | 1.5m | The three identities, stated explicitly and slowly |
| Implication | 1m | Growth consumes cash → funding → interest loop |

## Interview questions

1. **Walk me through the three financial statements.**
   Answer: Use the six-beat structure above, out loud, in about 10 minutes, without checking notes. Do *not* recite definitions at length — every time you describe a line, follow it with a "so what." Close on the growth-uses-cash implication.

2. **Why is net income not the same as cash? Give me the complete list of reasons.**
   Answer: Three families, enumerable without notes: (a) **non-cash items** — D&A, stock comp, impairments, deferred taxes; (b) **accrual timing on the way in** — revenue recognized before collection (receivables up) and expenses recognized before payment (accrued liabilities up), or the reverse (prepaids, deferred revenue); (c) **investing and financing flows**, which never touch net income at all — capex, acquisitions, debt issuance, buybacks, dividends. Only (a) and (b) appear in the CFO reconciliation; (c) is what the other two sections are for.

3. **A company has rising net income and falling cash. Walk me through the diagnostic.**
   Answer: Go to the cash flow statement and read the reconciliation. Is it non-cash add-backs (impairments, SBC) inflating net income? Is `ΔNWC` negative — specifically, are receivables or inventory growing faster than revenue? Confirm on the balance sheet: are AR and inventory growing faster than revenue, and is DSO/DIO deteriorating? Then check the credit view: is there a debt maturity inside 12 months, and is the revolver drawn? Finish with the growth rate — if growth is decelerating *and* working capital is building, it's a demand problem, not an investment.

4. **Why do capital-intensive companies look more levered than they are?**
   Answer: Because of the D&A add-back. EBITDA excludes D&A, so two identical businesses — one owning its factories, one leasing them — produce different EBITDA and therefore different apparent leverage on an EBITDA basis. The correct lens: `net debt / EBITDA` alongside **EBIT-based interest coverage** (`EBIT / interest`), and for a lease-heavy company treat the lease liability as debt and add rent back to EBIT before computing coverage. Also note that EBITDA multiples make asset-heavy businesses look *cheaper* than they are, because you must subtract maintenance capex to get real earnings power.

5. **What is the difference between an expense and an asset, and why does the choice matter?**
   Answer: An asset provides a future benefit and is expensed over that benefit's life; an expense is consumed now. It matters because the choice determines *when* profit is recognized, with no change in total economics — so it's a pure earnings-timing lever, and a strong incentive to capitalize. Real cases to name: software development costs, customer-acquisition costs, sales commissions, "improvements" to existing equipment. The test: is there a future benefit, and can you support a defensible useful life?

6. **Explain ROE to me, and then tell me why I shouldn't trust it.**
   Answer: ROE = net income / average common equity, the return earned on owners' capital. Don't trust it alone because it is the product of three very different things (DuPont: margin × asset turnover × equity multiplier) and the **equity denominator is small and manipulable** — buybacks, stock comp, and impairments all shrink it and mechanically raise ROE. Compare **ROIC** (NOPAT / invested capital) as the cleaner operating measure, and check **net debt / EBITDA** and **interest coverage** for the leverage reality. A company whose ROE rose because it bought back stock is not a better business.

7. **A company's balance sheet shows negative equity. Are they in trouble?**
   Answer: Not necessarily, and the right answer diagnoses rather than concludes. Negative equity can come from (a) cumulative losses or buybacks — a genuine concern; (b) large **deferred revenue** — a non-cash liability for services not yet delivered, with the cash already in hand, often benign; (c) massive **stock-based compensation** credited to APIC; (d) large non-cash write-downs. So: is cash positive and growing? Is CFO positive? Are there going-concern or covenant disclosures? Negative book equity is a signal to investigate and is meaningless alone.

8. **What would make you change your mind about a company you're bullish on?**
   Answer: Interviewers are testing judgment, not a list. Strong answers name *specific, observable* tripwires: (1) receivables or inventory growing materially faster than revenue for 2+ periods; (2) CFO/net income persistently below ~0.8; (3) a rising DSO combined with flat-to-declining gross margin; (4) "one-time" charges recurring on a 2–3 year pattern; (5) capex persistently below D&A while growth claims continue; (6) leverage rising against a softening revenue trend; (7) a growing gap between reported and contract-basis backlog or RPO. Naming tripwires shows you know what evidence would change your mind — which is precisely the question.

9. **Your model doesn't balance. Where do you look?**
   Answer: Give it as an ordered process, because the process is the answer. (1) Does the cash flow statement's ending cash equal the balance sheet cash? (2) Does ending retained earnings equal beginning + NI − dividends? (3) Is the balance sheet itself off-balance — if so, is it the retained-earnings line (usually a missing NI or dividend) or the cash line (usually a missing cash flow item)? (4) Are you double-counting across sections — e.g. modeling PP&E through the capex line *and* through the D&A schedule? (5) Is a circular reference (interest on average debt balance) failing to iterate? The habit of "check the three links first" is worth more than any single fix.

10. **How would you assess this company in 10 minutes? Here are the statements.**
    Answer: Give an explicit *ordered* process — the ordering is the point. (1) **Income statement, 3 years**: margin trend, what's recurring, growth quality (organic vs. M&A/FX). (2) **Cash flow**: CFO vs. net income, capex vs. D&A, FCF trend. (3) **Balance sheet**: liquidity, undrawn revolver, debt maturity, net leverage, equity sign. (4) **Working capital**: DSO/DIO/DPO and whether the CCC is improving or deteriorating. (5) **Ratios**: DuPont bridge to see where the returns come from. (6) **Read the notes**: accounting policies, revenue recognition, covenant language. Then state the two or three things you'd want to verify next. Interviewers reward the discipline far more than the individual numbers.

## Traps to avoid

- **Saying EBITDA is "the" profit measure.** It's a cross-sector rough comparison, and it's wrong for capital-intensive businesses. Default to operating income / EBIT.
- **Confusing a dividend with an expense.** Dividends are a *distribution*, funded by CFF, reducing equity without touching net income.
- **Forgetting that stock comp is a real cost.** It hits the income statement *and* dilutes, so "adjusted EBITDA excluding SBC" overstates economics for any software or tech company.
- **Treating book value as valuation.** Book equity is a historical-cost residual. It says nothing about a brand-light business with no tangible assets.
- **Quoting a ratio without a comparison.** "Current ratio is 1.4×" is meaningless alone. Pair it with the trend and a peer.
- **Over-explaining the basics.** If you've covered accrual vs. cash once, don't re-derive it. Answer, then stop.
- **Failing to connect to a consequence.** The strongest answers end with "…which means X" — the funding need, the margin pressure, the covenant risk. The weakest stop at the definition.

## How to actually practice

1. **Rehearse out loud, from a blank page, on a timer.** Not in your head. Target 10 minutes for the three-statement walkthrough and 3 minutes per ratio definition.
2. **Do it against a real company.** Pick a well-known filer, pull the three statements from the 10-K, and talk through them as if presenting. This is the highest-ROI hour of prep available.
3. **Do one toy 3-statement model in Excel.** Two years of history, a simple forecast, and force it to balance. It is the standard first-week exercise for banking hires and it will make the links on [page 07](../07-linking-three-statements/) permanent.
4. **Have someone ask the follow-ups.** The content isn't the hard part; being asked "but *why*?" six times in a row is.

## Watch

- [Connecting the Income Statement, Balance Sheet, and Cash Flow Statement](https://www.youtube.com/watch?v=f3T0tCjw1k8) — Brian Feroldi. The closest thing to a rehearsed version of the full walkthrough, with a worked example whose structure you can imitate.
- [How to Read Financial Statements w/ Brian Feroldi (TIP752)](https://www.youtube.com/watch?v=vIameomgKMQ) — The Investor's Podcast. Longer, and worth it: it's about *how to think* while reading statements, and it closes with a red-flag checklist covering all three.
- [Basic cash flow statement](https://www.youtube.com/watch?v=Mioqyv_IW3E) and [Accrual basis of accounting](https://www.youtube.com/watch?v=NNhyZFHAzaA) — Khan Academy. Re-watch these two the night before; they are the foundation of the two most common follow-up questions.

## Further reading

- [The Ultimate Guide to Financial Statements](https://www.youtube.com/watch?v=eorpdJUWfTA) (Accounting Stuff) — a single 35-minute pass over all three statements, useful as one consolidated revision session.
- Khan Academy's [Accounting and financial statements](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme) unit — free, short, and the cleanest free written treatment of the whole subject.
- The **first 20 pages of any 10-K** (financial statements plus the notes index) — the fastest way to convert all of this from abstract to concrete. Do it once with a company you know and the numbers will stick.
