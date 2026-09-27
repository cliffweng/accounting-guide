---
title: "09. Expenses & matching"
layout: default
nav_order: 10
---

# Expenses & matching
{: .no_toc }

*~8 min read*

**Occasional**

## Why it matters

The matching principle is what makes an income statement a meaningful measure of a period's activity: **expenses are recognized in the same period as the revenue they helped generate.** Get it wrong and every period is distorted — which is why the interesting interview questions are all about *when* an expense belongs, and why "expense everything immediately" is not always conservative (see the truck example below, which is the single most counterintuitive idea in intro accounting).

## Core concepts

- **Matching has two halves:** (a) **revenue recognition** — record revenue when earned (see [Revenue recognition](../08-revenue-recognition/)); (b) **expense recognition** — record costs in the period the related revenue is earned. If there's no directly related revenue, match the expense to the period in which the benefit is received (the "economic benefits" principle).
- **The counterintuitive core: expensing a long-lived asset immediately distorts results badly, and so does capitalizing a short-lived one.** Khan Academy's truck example is the canonical illustration: buy a $30,000 truck and expense it in year 1, and year 1 shows a huge loss while years 2–5 look fantastic. Capitalizing and depreciating straight-line gives a smoother, more comparable series. Neither is "conservative" in the sense of being pessimistic — matching is about *comparability*.
- **Prepaid expenses (deferral) vs. accrued expenses (accrual)** are the two adjustments to memorize, and they are mirror images:
  - **Paid now, benefit later** → *asset* today, expense later (insurance, prepaid rent, annual software subscriptions). On the cash flow statement, the whole cash outflow hits in the period paid.
  - **Benefit now, paid later** → *expense* today, liability later (accrued payroll, accrued interest, rent accrued). Cash hits later.
- **Depreciation and amortization** (see [D&A](../12-depreciation-amortization/)) are the largest and most predictable expense for most asset-heavy companies, and they're non-cash. Depreciation method choice (straight-line vs. accelerated) shifts reported profit between periods without changing total cash over the asset's life — a permanent-reporting choice, not a timing trick.
- **Which costs go where matters for margins, not just totals.** Gross margin = revenue − **COGS**; OpEx is everything else. If a company reclassifies costs from OpEx to COGS, gross margin falls and operating margin is unchanged. Analysts should therefore always compare **operating income**, which is classification-robust, and treat gross margin comparisons with suspicion when a peer reclassifies.
- **Some costs are capitalized into the balance sheet and amortized, others are expensed immediately, and the line is genuinely judgmental.** Software development costs, sales commissions, and customer acquisition costs are the contested ones. This is a recurring source of "adjusted" earnings: capitalize more today and profit is higher today.

## Mental model

```
  A cost has one of three lives, and the life determines the treatment:

  ┌─ LONG life (years) ────────────────────────────────────────┐
  │  Capex → asset on the balance sheet → D&A expense over life │
  │  Truck, factory, software product, patents                 │
  │  "MATCH the cost to the periods that BENEFIT"             │
  └────────────────────────────────────────────────────────────┘
  ┌─ MEDIUM life (a few months) ───────────────────────────────┐
  │  Prepaid → asset today, expense ratably (prepaid rent)     │
  │  Or expense immediately if immaterial                      │
  └────────────────────────────────────────────────────────────┘
  ┌─ SHORT life (this month) ──────────────────────────────────┐
  │  Expense now. Salaries, utilities, COGS, marketing.        │
  └────────────────────────────────────────────────────────────┘

  THE MIRROR:
    CASH BEFORE BENEFIT  →  asset on BS   (deferral)  → expensed later
    BENEFIT BEFORE CASH  →  expense now   (accrual)    → liability on BS
```

## Interview questions

1. **A company has rising operating expenses relative to revenue. How do you decompose whether that's bad?**
   Answer: Split OpEx into (a) **fixed** (leases, salaried staff, D&A, most marketing commitments) and (b) **variable** (commissions, freight, some marketing, cloud costs that scale with usage). Rising fixed costs as a % of revenue in a *growing* company is a warning about future operating leverage, but a normal, deliberate investment phase. Rising *variable* costs per unit of revenue is a real unit-economics problem — you're paying more to serve each customer. Then ask: is this reflected in gross margin or below it, and is management investing deliberately or responding to competitive pressure?

2. **A company capitalizes customer-acquisition costs over three years instead of expensing them immediately. What's the impact?**
   Answer: Reported EBITDA and operating income are higher today (the expense is spread out), and there's a new asset on the balance sheet that will eventually run off. Total expense over the full life is the same, so this is a **timing** shift — but it inflates the "adjusted" numbers management reports and it creates a new amortization drag in future years. The correct skeptical move: ask what assumption the amortization period embeds, and note that this treatment is a choice, not a requirement. (Compare with the aggressive practices discussed on the [revenue page](../08-revenue-recognition/).)

3. **Why is operating income a more comparable metric than gross margin across companies?**
   Answer: Because classification between COGS and OpEx is somewhat discretionary, and companies reclassify for cosmetic reasons. Operating income is defined below that line, so it's robust to reclassification. Gross margin is only comparable if you know the costing policy. Always check the accounting-policy note for any reclassification, and prefer multi-year trend analysis over single-period cross-company comparison.

4. **A company pays $24M cash for a three-year software contract. What appears where?**
   Answer: **Balance sheet**: a $24M prepaid asset at signing (net of current portion). **Income statement**: $8M per year of expense. **Cash flow**: the entire $24M is an operating outflow in year one — so year-one CFO looks $8M worse than the income statement implies, purely as a timing artifact. This is a great "why do profit and cash diverge" example, and a reminder that the accrual wedge is not always growth-driven.

5. **Explain the difference between a prepaid expense and an accrued expense, with an example of each, and which way each pushes cash flow.**
   Answer: **Prepaid**: you paid for something you haven't consumed yet (a year of rent paid in advance) → asset now, expense later, cash out now. **Accrued**: you've consumed something you haven't paid for yet (incurred but unbilled legal fees) → expense now, liability later, cash out later. The first pulls cash *ahead* of the expense; the second pushes cash *behind* it. Together they're the two halves of why CFO ≠ net income.

6. **"Expensing a truck makes a company look worse this year, so it's conservative." What's wrong with that reasoning?**
   Answer: Conservatism isn't the goal — *comparability* is. If you expense a truck in year 1, year 1 is artificially depressed and years 2–5 artificially inflated, so no year's reported profit reflects that year's actual activity. Worse, it gives management an incentive to capitalize aggressively when they want to look good, and the two errors don't offset in any meaningful sense. The correct rule: match the cost to the periods that receive the benefit. This is exactly the point of the matching principle.

## Watch

- [Depreciation in cash flow](https://www.youtube.com/watch?v=uX2w0b8Qlss) — Khan Academy. Sal Khan on why depreciation is added back in the cash flow statement. Two minutes, and it resolves a question most people find confusing.
- [A Complete Guide to Adjusting Entries](https://www.youtube.com/watch?v=mrJdVh5MmKI) — Accounting Stuff. Prepaid expenses, deferred revenue, accrued expenses, accrued revenue in one pass — the four entries that constitute matching in practice.
- [An In-Depth Guide to Depreciation in Accounting](https://www.youtube.com/watch?v=ndMPuMRusEs) — Accounting Stuff. Straight-line, declining balance, units-of-production, and the judgment calls behind useful life and salvage value. Longer than this page, but it's the right depth for the topic.

## Further reading

- Khan Academy's [Depreciation and amortization](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme/depreciation-amortization-tut) unit — includes the truck example (why expensing a truck immediately produces inconsistent reported performance), expensing-vs-depreciating, and why depreciation is added back in the cash flow statement.
- The **Significant Accounting Policies** note in any 10-K. It is short, mandatory, and explicitly lists which costs the company capitalizes. Reading it changes how you read every other statement.
