---
title: "12. Depreciation & amortization"
layout: default
nav_order: 13
---

# Depreciation & amortization
{: .no_toc }

*~7 min read*

**Background**

## Why it matters

D&A is the largest and most predictable non-cash expense for most companies, and it sits at the intersection of three things you *do* need to know: why the income statement and cash flow statement disagree, why EBITDA is aggressive, and why "capex vs. D&A" is a hidden sustainability check. You don't need to build a depreciation schedule in an interview. You do need to know where D&A appears, why it's non-cash, and what accounting choices can do to it.

## Core concepts

- **Depreciation** is the allocation of the cost of a **tangible** long-lived asset (PP&E) over its useful life. **Amortization** is the same idea for **intangible** assets (patents, licenses, software, acquired intangibles). They are economically identical; only the asset class differs.
- **The standard methods:** **Straight-line** (equal charge each period), **declining balance / double-declining balance** (front-loaded charge, common for newer assets), and **units of production** (proportional to actual usage — often more economically accurate for equipment, and it means depreciation only happens when the asset is actually used).
- **Book depreciation is a policy, not an economics.** Total depreciation over the asset's life equals cost minus salvage value *regardless of method*, so method choice only shifts profit **between periods**. Straight-line is generally considered the most neutral; accelerated methods boost early-period earnings and boost reported ROA/ROE by keeping the asset base (and the equity denominator) smaller in later years. This is a legitimate choice, not fraud — but it is a lever.
- **D&A is non-cash but not free.** The cash left when the asset was bought (CFI). D&A is the recognition that the asset's productive capacity is being consumed. That's why it's added back in the CFO reconciliation (see [Cash flow statement](../06-cash-flow-statement/)) and why it's excluded from EBITDA — and why EBITDA overstates sustainable earnings for capital-intensive businesses, since the asset must eventually be replaced.
- **Accumulated depreciation is a contra-asset.** `PP&E (net) = gross PP&E − accumulated depreciation`. Analysts usually want the *gross* figure and the D&A rate. A rapidly-growing company that reports a small net PP&E relative to capex is telling you accumulated depreciation is eating the balance sheet.
- **Impairment is the reset.** If an asset's recoverable value falls below its carrying value, the company must write it down — often lumped into a "one-time" charge. This is how bad acquisitions and declining assets are finally acknowledged on the income statement, years after the fact (see [Income statement](../04-income-statement/) on "one-time" charges). Impairments are *non-cash*, which is why a company with a catastrophic write-down may still have fine cash flow that year.
- **The D&A → capex comparison is a real signal.** `Capex / D&A`: above ~1.2× is reinvesting for growth; below ~0.8× is harvesting / under-investing. A company generating attractive FCF *because* capex is well below D&A is not sustaining that FCF long-term.

## Mental model

```
  Buy a $500K machine, 5-year life, $50K salvage, straight-line:

  t=0   CASH −500K  (investing outflow, CFI)      PP&E +500K (gross)
  t=1   D&A −90K    (income statement expense)     Accum. Depr. +90K
  t=2   D&A −90K                                   Accum. Depr. +180K
  ...
  t=5   D&A −90K                                   Accum. Depr. +450K
        PP&E net = 500 − 450 = 50K (residual)

  EACH YEAR:  −90K on the income statement  (reduces profit, cash unaffected)
               +90K back in the CFO reconciliation (because no cash moved)

  TOTAL over life:  profit reduced by 450K   |   cash spent: 500K, all at t=0

  THE CHECK:   Capex / D&A > 1  →  asset base growing (investing)
                Capex / D&A < 1  →  asset base shrinking (harvesting)
```

## Interview questions

1. **Why is depreciation added back to net income in the cash flow statement?**
   Answer: Because it's a **non-cash** expense. The cash outflow happened when the asset was purchased, and it appears in CFI then, not in CFO now. The cash flow statement only records actual cash movements, so depreciation is removed from the starting net income figure and the capex is shown separately. Economically, the cost is real — it's just that the recognition and the payment happen in different periods.

2. **A company switches from straight-line to double-declining depreciation. What are the financial statement effects?**
   Answer: **Income statement**: higher depreciation in early years, lower in later years → higher early-year EBIT and net income, lower late-year. **Balance sheet**: faster accumulation of accumulated depreciation → smaller net PP&E, so later-year total assets and equity are both *smaller*, which paradoxically **raises** reported ROA and ROE in those later years. **Cash flow**: no effect at all — total depreciation over the asset's life is identical, and capex is unchanged. So the entire effect is on reported *accrual* profitability, and it flatters both early earnings and late-year return ratios.

3. **Why do analysts distrust EBITDA for capital-intensive businesses?**
   Answer: Because EBITDA ignores the cost of the assets required to sustain the business. D&A is a real, non-avoidable cost of staying in business, and for a manufacturer or utility, the capex bill is enormous relative to EBITDA. If capex consistently exceeds D&A, the company is *consuming* capital to maintain its asset base, and EBITDA-based multiples or leverage ratios will overstate the enterprise's earning power. Reserve EBITDA for cross-sector coarse comparisons, not valuation of a specific capital-intensive business.

4. **A company takes a $2B impairment charge. Its EBITDA "adjusted" figure jumps sharply. What's the concern?**
   Answer: The add-back is *arithmetically* fine (impairments are non-cash), but an impairment usually signals that management's prior forecasts were wrong or that an asset is genuinely worth much less — the write-down is information, not noise. And impairments are notorious for arriving in bad years under a "one-time" label, only to be followed by more "one-time" charges in a few years. Ask: what asset, what was the original thesis, and does the reduced (post-impairment) asset base change the company's future D&A? It usually does — and that lowers *future* reported earnings, so the add-back is only flattering if you ignore the ongoing effect.

5. **How do you distinguish maintenance capex from growth capex from public filings?**
   Answer: You often can't get a clean split — companies disclose total capex, and the "maintenance vs. growth" split is an **estimate**. Signals to use: (1) D&A as a floor estimate of maintenance capex (a company replacing assets at current prices typically spends more than D&A, since D&A is historical cost); (2) the capex note, which sometimes breaks out categories; (3) management's language in the MD&A about capacity additions; (4) asset turnover — if revenue is flat but PP&E is shrinking, it's harvesting. Be skeptical of a company that claims growth capex with no revenue impact for several years running.

6. **Explain why "net PP&E" understates how much a company actually owns.**
   Answer: Net PP&E is historical cost minus accumulated depreciation, so a company that bought its factories decades ago shows a small number even though the physical assets are worth far more today. A company that bought recently at high prices and accelerated the depreciation shows a large number for assets worth the same. This is why **asset-heavy companies look different depending on their vintage**, and why analysts sometimes use a replacement-cost or EV/replacement-capital framework instead of book value for such industries. Conversely, a company that has written off or depreciated heavily can show *negative* book equity while owning perfectly good productive assets.

## Watch

- [Depreciation vs Amortization Explained Simply](https://www.youtube.com/watch?v=IIGnbcICBSM) — Brian Feroldi. Six minutes covering the difference between the two and how all three statements account for them, with a worked company example.
- [Depreciation in cash flow](https://www.youtube.com/watch?v=uX2w0b8Qlss) — Khan Academy. Sal Khan on why depreciation is added back in the cash flow statement. Two minutes, and it resolves the most common confusion on this topic.
- [An In-Depth Guide to Depreciation in Accounting](https://www.youtube.com/watch?v=ndMPuMRusEs) — Accounting Stuff. Straight-line, declining balance, and units of production, plus the judgment calls around useful life and salvage value. Longer than this page, and the right depth if you want to actually build a schedule.

## Further reading

- Khan Academy's [Depreciation and amortization](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme/depreciation-amortization-tut) unit — the free written version, including the "expensing a truck produces inconsistent performance" example that motivates the whole principle.
- The **Property, Plant & Equipment** and **Goodwill & Intangible Assets** notes in any 10-K from an asset-heavy company. Useful lives, salvage values, and impairment-test methodology are all disclosed there.
