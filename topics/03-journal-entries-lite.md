---
title: "03. Journal entries, lite"
layout: default
nav_order: 4
---

# Journal entries, lite
{: .no_toc }

*~6 min read*

**Occasional**

## Why it matters

You do **not** need to be a bookkeeper for this guide, and you will never be asked to post a journal entry in an IB interview. You do need to understand one thing: **every reported number is the accumulated residue of paired entries**, and *which side of a transaction is an asset versus an expense* is a real judgment call that moves reported profit. This page gives you just enough to see inside a balance sheet and explain why certain "non-cash" items are non-cash.

## Core concepts

- **Double entry means every transaction has exactly two sides of equal value.** Either (a) value moves between two accounts on the same side of [the accounting equation](../01-accounting-equation/) (cash → equipment), or (b) it increases one side and offsets on the other (equipment up, debt up). The "debit" and "credit" labels are just the two sides of that entry; the mnemonic systems are arbitrary convention.
- **The one structural fact worth memorizing:** an entry is a debit to one account and a credit to another, and *debit ≠ bad*. A debit to cash means cash increased. A debit to an expense means the expense increased (which reduces profit and equity). A credit to revenue means revenue increased.
- **Accruals are the entries that most often surprise people.** Buying $10K of equipment cash creates an **expense**; buying the same $10K on credit creates a **liability**. Buying $10K of inventory creates an **asset** until the inventory is sold, at which point it becomes **COGS**. Same cash flow, wildly different income statements.
- **A cash payment can be a prepaid asset or an immediate expense depending on what it buys.** A one-year insurance premium paid today is a **prepaid expense** (an asset) amortized over twelve months, not a full-year expense hit today. This is a small example of a very large idea: **capitalization vs. expensing** is a timing choice with real earnings consequences, and it is the subject of most accounting-quality debates.
- **Book value is original cost minus accumulated adjustments.** Accumulated depreciation sits on the balance sheet as a *contra-asset* (a negative line), so `PP&E = gross PP&E − accumulated depreciation`. This is why you will sometimes see a company with tiny reported PP&E despite enormous replacement cost.

## Mental model

```
  Ask two questions about any transaction:

  1. Did CASH move?              ── no  →  at least one side is non-cash
  2. Did the benefit last >1 yr?  ── yes →  capitalize (asset, spread over time)
                                    ── no  →  expense (hits the P&L now)

  $50K delivery truck, cash        → PP&E asset, then $10K/yr depreciation   [profit smoothed]
  $50K delivery truck, financed    → PP&E asset + $50K debt liability       [same asset, more leverage]
  $50K used car for resale         → Inventory asset                        [profit awaits a buyer]
  $50K customer referral bonus     → Marketing expense, now                  [profit dented today]
```

## Interview questions

1. **Is depreciation an expense, an asset, or a cash outflow?**
   Answer: It's an **expense** on the income statement, and it is **not** a cash outflow in that period. The cash left when the asset was purchased (investing activity). Depreciation is the accounting recognition that the asset's cost is being consumed.

2. **Why do companies care whether a spend is capitalized or expensed?**
   Answer: Because expensing hits the current period's profit while capitalizing defers it. A company that wants to report higher near-term earnings has an incentive to capitalize anything it can defend (software development costs, commissions, "improvements" to equipment). The "accruals anomaly" literature and most classic accounting-fraud cases live in this gap.

3. **A company pays $120K cash for a 24-month maintenance contract. What's on each statement?**
   Answer: Balance sheet: a **$120K prepaid asset** today. Income statement: $5K per month of expense, so $60K in the first year. Cash flow: the full $120K is an **operating outflow in the period paid** — this is a common interview trap, since it makes early-period CFO look worse than the income statement suggests. Nothing is capitalized as a fixed asset, and nothing hits CFI.

4. **Explain a contra account. Why do they exist?**
   Answer: A contra account offsets a related account from the other side so a single balance sheet line can show a net figure without hiding the gross amounts. `Accumulated depreciation` is a contra-asset against `PP&E`; `Allowance for credit losses` is a contra-asset against `Receivables`. Analysts usually want the gross number (and the change in the allowance), so never stop reading at the net.

5. **Your friend says "the trial balance proves the numbers are right." Why is that a dangerous belief?**
   Answer: A balanced trial balance only proves that *entries were posted consistently* — arithmetic self-consistency, not economic accuracy. An entry can be balanced and completely wrong (recording a $1M sale that never happened, or misclassifying an operating expense as a capital expenditure). That's the whole premise behind the phrase "the books balance, the company is still broke." See [Interview hotspots](../14-interview-hotspots/) for how this plays out as an interview question.

## Watch

- [ACCOUNTING BASICS: a Guide to (Almost) Everything](https://www.youtube.com/watch?v=yYX4bvQSqbo) — Accounting Stuff. The 14-minute overview that hits the equation, debits/credits, and the six account types. Good orientation even though this guide deliberately skips the drills.
- [A Complete Guide to Adjusting Entries](https://www.youtube.com/watch?v=mrJdVh5MmKI) — Accounting Stuff. Prepaid expenses, deferred revenue, accrued expenses, accrued revenue — the four accrual entries that explain most of the gap between the income statement and the balance sheet.
- [The TRIAL BALANCE Explained](https://www.youtube.com/watch?v=3_PfoTzSCQE) — Accounting Stuff. Why a balanced trial balance can still be wrong, with five specific reasons.

## Further reading

- Any intro financial accounting text, the chapters on the accounting cycle and adjusting entries. Read the *concepts* and skip the problem sets — the goal is intuition about why numbers land where they do, not speed at posting entries.
