---
title: "04. Income statement"
layout: default
nav_order: 5
---

# Income statement
{: .no_toc }

*~9 min read*

**🎯 Interview frequent**

## Why it matters

The income statement is the only statement that describes a **period** rather than a point in time, and it is the one most often quoted out of context ("revenue grew 30%!"). Real skill is not memorizing line items — it's reading *quality of earnings*: which revenue is recurring, which costs are fixed, what management left out, and how the reported number relates to cash. On a banking screen this is usually where you're asked to open a real 10-K.

## Core concepts

- **Structure: Revenue − COGS = Gross profit; − operating expenses (OpEx) = Operating income (EBIT); − interest & taxes = Net income (bottom line).** The "operating" cutoff is the important part: it separates results of running the business from results of how the business is financed and taxed.
- **Margins are the product, not just the level.** Gross margin = GP/Revenue, operating margin = EBIT/Revenue, net margin = NI/Revenue. A company with 20% margins that falls to 15% can be more worrying than one growing 15% → 20%, because margin compression suggests pricing power or cost problems.
- **SG&A is mostly *fixed* in the short run** (salaries, leases, marketing commitments). That creates **operating leverage**: once you cover the fixed base, incremental revenue drops to gross profit, so small revenue surprises produce outsized EBIT changes. Fixed cost also means margin *expands* as revenue scales — which is exactly why a high-growth, high-fixed-cost model is both more profitable and more fragile.
- **Recurring vs. non-recurring is the whole ballgame.** Management labels "one-time" charges (restructuring, impairments, M&A costs, litigation) — and this label is used defensively. Ask whether the item is *really* one-time, whether it recurs every few years, and whether the "adjusted" number replaces GAAP for the rest of the industry's history. Recurring "one-time" charges are a sign of low-quality earnings.
- **Stock-based compensation (SBC) sits in operating expense but is a non-cash item** and is a real economic cost (dilution). Many investors add it back for "adjusted" EBITDA — be aware of who benefits from that adjustment.
- **EPS is not a measure of performance.** Basic EPS is net income divided by weighted-average shares; because buybacks shrink the denominator, EPS can grow while net income falls. A classic screen: net income down, EPS up → the "growth" is a capital-structure artifact. See [Ratios](../11-ratios/).

## Mental model

```
  Revenue  .....................................................  100.0
    − COGS .....................................................   (60.0)
  = Gross profit .................................................   40.0   ← 40% gross margin
    − SG&A / R&D  (mostly FIXED) .................................  (25.0)
  = Operating income (EBIT) ......................................   15.0   ← 15% operating margin
    − Interest .................................................   (3.0)
    − Taxes ....................................................   (2.4)
  = Net income ..................................................    9.6   ← 9.6% net margin

  WHAT TO CHECK, in order:
    1. Gross margin trend        — pricing power? mix shift? input costs?
    2. OpEx as % of revenue      — operating leverage: is it scaling?
    3. Non-recurring items       — is "adjusted" EBIT the new baseline?
    4. SBC as % of revenue       — real cost, dilutive
    5. Net income vs. CFO        — is the profit arriving in cash?
```

## Interview questions

1. **A company's revenue is growing 25% but gross margin fell from 45% to 38%. What are the plausible causes, and which worry you most?**
   Answer: Plausible causes: input-cost inflation (gross-margin squeeze), a shift in mix toward lower-margin products, price cuts to defend share, or channel/product ramp costs. Most worrying: price cuts, because they're hard to reverse and signal the market is tightening. Also always ask whether prior-period figures were *restated* — a "recast" segment can look like a margin collapse that's really a reclassification.

2. **Net income fell 5% but EPS rose 12%. Explain.**
   Answer: Share count fell — buybacks and/or net issuance to employees was more than offset by the buyback. Net income / average shares = EPS, so shrinking the denominator raises EPS even as profit declines. This is not company improvement; it's financial engineering. Ask whether the buyback was funded with debt (which is just equity-plus-leverage) and whether share-based comp is offsetting the reduction.

3. **What is EBIT, why is it useful, and how does it differ from EBITDA?**
   Answer: EBIT = earnings *before interest and taxes*, i.e. operating income. It's useful because it measures operating performance before financing choices (capital structure) and tax jurisdiction distort it. EBITDA adds back D&A as well, giving a rough proxy for cash operating profit — but D&A is a real cost (the asset must be replaced eventually), so EBITDA overstates sustainable economics for capital-intensive businesses. Use EBIT for comparability, EBITDA for cross-sector coarse comparisons, and be suspicious of either being used as the headline.

4. **A company reports "adjusted EBITDA" up 30% while GAAP net income is flat. What questions do you ask?**
   Answer: (a) What exactly was added back, and is it genuinely non-recurring? (b) Is SBC excluded? (c) Was the prior-year figure restated so the growth isn't an apples-to-oranges comparison? (d) Does the add-back reflect a real cash cost — restructuring often comes with severance and severance is cash. The right default is to anchor on GAAP and treat adjusted figures as a supplement.

5. **How do you identify a company with pricing power from the income statement alone?**
   Answer: Look for **stable or rising gross margin through a period of input-cost inflation or competitive intensity**, plus low promotional intensity (not a line item you can see, but inferable from low D&A-to-revenue or flat marketing spend as % of sales). A firm that can raise prices and hold margin during a cost shock has structural pricing power. Contrast with a business whose margin tracks input costs almost one-for-one — it's a price-taker with no buffer.

6. **Why is the income statement described as "for a period" and the balance sheet "at a point in time," and why does that distinction cause real errors?**
   Answer: The income statement aggregates flows over a window; the balance sheet aggregates stocks at the date the window closes. Analysts err by treating a stock (e.g. year-end cash) as if it were a flow (e.g. "cash was up 30% so performance was strong"), or by comparing a trailing-twelve-month revenue to a single balance sheet date without realizing the dates must match. Every growth-rate calculation must specify the period, and every balance sheet item must be dated.

## Watch

- [The INCOME STATEMENT: all the basics in 9 minutes](https://www.youtube.com/watch?v=abh1PzKDAK0) — Brian Feroldi. Line-by-line tour with a worked example and a clear statement of what each section actually tells you.
- [The INCOME STATEMENT Explained (Profit & Loss / P&L)](https://www.youtube.com/watch?v=hrSUq4wcd0g) — Accounting Stuff. The most literal walkthrough of the structure, useful if you want the terminology nailed down.
- [Financial Statements Explained | Balance Sheet | Income Statement | Cash Flow Statement](https://www.youtube.com/watch?v=e8qbynFb4Zc) — 365 Financial Analyst. Good on why sales on the income statement don't equal cash in the bank.

## Further reading

- Khan Academy's [Introduction to the income statement](https://www.khanacademy.org/economics-finance-domain/core-finance/stock-and-bonds/valuation-and-investing/v/introduction-to-the-income-statement) — a short, free primer with the accounting mechanics made explicit.
- **A Rule of Thumb for Management** (Mulford & Comiskey) and **Financial Shenanigans** (Schilit) — the practical guides to spotting earnings management; both are freely available online. Read one of these before your first real 10-K.
