---
title: "02. Accrual vs. cash"
layout: default
nav_order: 3
---

# Accrual vs. cash
{: .no_toc }

*~9 min read*

**🎯 Interview frequent**

## Why it matters

This is the highest-leverage concept in the subject for someone without an accounting background. GAAP requires **accrual** accounting: recognize revenue when earned and expenses when incurred, regardless of when cash moves. That single choice is why a company can report record profit while burning cash, why "adjusted" earnings exist, and why most of the analytical work in equity research is reconciling the accrual-based income statement back to actual cash. Expect a variant of "net income was up 20% — why is cash down?" on essentially any screen.

## Core concepts

- **Cash basis** records revenue when cash is received and expenses when cash is paid. **Accrual basis** records revenue when the *goods or services are delivered* and expenses when they are *incurred*. Public companies must use accrual (with a small-business exception, and cash-basis financials are close to uninterpretable).
- **The matching principle** is the other half: expenses are recognized in the same period as the revenue they helped generate. A machine bought in 2019 is not expensed in 2019 (which would make that year look terrible and later years look great) — it is depreciated over its useful life (see [Expenses & matching](../09-expenses-matching/)). Accrual accounting exists to make each period's profit a fair measure of that period's activity.
- **The wedge between profit and cash is entirely working capital and non-cash items.** The single indirect-method line that explains most of it: `CFO ≈ Net income + D&A − increase in net working capital`. Growing companies *consume* working capital (they pay for inventory and produce receivables before collecting), so profit and cash diverge precisely when growth accelerates.
- **Accruals are an estimate, and estimates are gameable.** Revenue recognized before cash arrives creates **receivables** (and, on the other side, deferred revenue when cash arrives first). If you want to see whether reported profit is real, follow the cash: rising receivables, rising deferred revenue, or a widening gap between net income and CFO are all reasons to be suspicious of the headline.
- **Accrual accounting is *not* a scam — it is information with noise.** It matches revenue and cost to the period that generated them, which is strictly more informative than cash timing for judging unit economics. The analyst's job is not to reject accruals but to identify which accruals reflect real economics and which reflect earnings management.
- **Cash is not a profit metric and profit is not a cash metric.** "This company is profitable" and "this company generates cash" are different claims, and the distinction is the reason the cash flow statement exists as a separate statement at all.

## Mental model

```
  PERIOD 1                                  PERIOD 2
  ─────────                                  ─────────
  Sells $100 on net-30 terms.               Collects the $100.

  ACCRUAL:  Revenue = $100   <── earned here (delivered)
            Cash    = $0
            (AR sits on the balance sheet)

  CASH:     Revenue = $0
            Cash    = $100   <── received here

  The company did identical work in both periods. Only the TIMING differs.
  Accrual accounting tries to put the work in the period it happened.
```

The cleanest single mental model: **accrual accounting is a timing convention applied on both sides of the income statement.** Every difference between profit and cash is a timing difference that will reverse — unless management is trying to hide something.

## Interview questions

1. **A company reports 20% net income growth and flat operating cash flow. What are the likely explanations, ranked?**
   Answer: In rough order of likelihood: (a) **working capital build** — receivables and/or inventory grew as the business scaled, so the growth was cash-hungry; (b) rising **accruals** — revenue recognized ahead of collection, or expenses deferred via capitalized costs; (c) **one-time non-cash charges** in the income statement (write-offs, stock comp, impairments) that don't repeat; (d) genuinely aggressive revenue recognition. The right follow-up is to check the cash flow statement's reconciliation and the receivables/inventory balances, not to conclude fraud from one data point.

2. **Why is depreciation added back on the cash flow statement when it's clearly a real economic cost?**
   Answer: Because the cash already left the business when the asset was purchased — it showed up as an investing cash outflow in the year of purchase. Depreciation is a non-cash allocation of that past outflow. The cash flow statement only counts cash movements, so it's added back. Economically the cost is real; it's just recognized on the income statement, not in the cash line.

3. **A software company has growing deferred revenue. Is that bad?**
   Answer: No — deferred revenue is generally *good*: customers paid cash up front, and the company has an obligation to deliver future service. It shows up as a current liability and a negative working capital position. The concerning version is the mirror image: receivables ballooning with no cash, or deferred revenue *declining* while reported revenue grows, which would suggest the company is pulling revenue forward rather than earning it.

4. **Your friend says a company with negative cash flow should be sold immediately. What's your response?**
   Answer: It depends on *why*. Negative CFO with rapid growth and a short cash conversion cycle is often an investment, not a warning — Amazon historically sacrificed cash flow to compound. Negative CFO at a mature, slow-growing company with heavy capex is more concerning. Always pair the cash flow statement with the growth rate and the balance sheet's debt maturity before judging.

5. **Explain the difference between an accrual and a deferral, and give one example of each.**
   Answer: **Accrued revenue** = you delivered the service but haven't been paid → record revenue now, sit the cash on the balance sheet as an **asset** (receivable). **Deferred revenue** = you were paid but haven't delivered → record cash now, sit the obligation on the balance sheet as a **liability**. Rule of thumb: cash before performance = liability; performance before cash = asset.

6. **Why do airlines and retailers have such different cash cycles than banks?**
   Answer: Airlines and retailers buy inventory (or capacity) and sell it before collecting, so they must finance a *negative* cash position through the operating cycle. Banks *are* the liquidity business — their "inventory" (cash lent out) is simultaneously their product, so working capital dynamics barely apply in the conventional sense. This is why working capital ratios are only comparable within an industry (see [Working capital](../10-working-capital/)).

## Watch

- [Accrual basis of accounting](https://www.youtube.com/watch?v=NNhyZFHAzaA) — Khan Academy. Sal Khan's cleanest minimal example, including how the same transaction looks different on cash vs. accrual basis.
- [Accrual Accounting Explained in 5 MINUTES!](https://www.youtube.com/watch?v=HqmmR4EMlP4) — THE CFO. Tight, focused walkthrough of the accrual method and the matching principle.
- [A Beginner's Guide to the Cash Flow Statement](https://www.youtube.com/watch?v=xbasHzq2fL0) — Accounting Stuff. Why we need a separate statement if we're already using accrual accounting, and the full indirect-method build.

## Further reading

- Khan Academy's [Cash versus accrual accounting](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme/cash-accrual-accounting) lessons — the free text version, with side-by-side examples.
- The MD&A ("disclosure by management's discussion and analysis") section of any 10-K. Reading how a company *explains* its own working capital and non-GAAP adjustments is the fastest way to build real intuition.
