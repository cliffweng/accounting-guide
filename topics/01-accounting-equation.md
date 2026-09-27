---
title: "01. The accounting equation"
layout: default
nav_order: 2
---

# The accounting equation
{: .no_toc }

*~7 min read*

**🎯 Interview frequent**

## Why it matters

Everything in financial reporting hangs off one identity: **Assets = Liabilities + Equity**. It looks trivial, but it is the reason a balance sheet *balances*, the reason a company's book value of equity is a residual rather than a reported number, and the reason you can reverse-engineer a missing balance sheet from an income statement and a cash flow statement. In banking interviews this is often the first technical question precisely because it tests whether you understand accounting structurally or only procedurally.

## Core concepts

- **Assets** = things the company owns or controls that have future economic value, expected to be converted into cash. **Liabilities** = obligations to outsiders (suppliers, lenders, tax authorities) that will require an outflow. **Equity** = the residual claim held by owners, i.e. what would be left for shareholders if the company liquidated *everything* at book value and paid all creditors.
- **Equity is the plug, not an input.** It is `Assets − Liabilities`. When you buy $100 of equipment with $40 of cash and $60 of debt, assets rise by 100 and liabilities by 60, so equity is unchanged — the transaction is *financing-neutral* for equity.
- **The equation is definitional, which makes it a powerful consistency check.** Any time you see a balance sheet that doesn't balance, either a line is misclassified or you have misread one. It also means the *sign* of equity carries real information: negative book equity means liabilities exceed assets, which is a distress signal even if the company is profitable.
- **The expanded form** you should be able to write from memory: `Assets = Liabilities + Paid-in Capital + Retained Earnings`. Paid-in capital is what investors contributed; retained earnings is cumulative profit minus cumulative dividends. This is the bridge from the income statement to the balance sheet (see [Linking the three statements](../07-linking-three-statements/)).
- **Book value ≠ market value.** The equation is stated in *book* terms, based on historical cost less accumulated depreciation for most assets. Equity can be far below (or, with unrecognized intangibles, far above) economic value. That gap is exactly what a valuation exercise tries to capture.
- **Every transaction has two sides.** Double-entry bookkeeping is just the bookkeeping expression of the equation: something is either moved between two asset accounts, or offset on one side by a liability/equity account. Debits and credits are only labels for the two sides — you can ignore the mechanics and still reason correctly (see [Journal entries, lite](../03-journal-entries-lite/)).

## Mental model

```
      ASSETS                      =     LIABILITIES        +     EQUITY
  ─────────────                        ─────────────              ─────────────
  Cash, AR, Inventory,                  AP, accrued exp,           paid-in capital
  PP&E, intangibles                     debt, deferred tax         + retained earnings

  (what the firm owns)                      (what it owes OUTSIDE)      (what is left for owners)

  financed by:  creditors (liabilities)  +  owners (equity)

  Equity is the RESIDUAL. It is not independently reported — it is Assets − Liabilities.
```

Think of the left side as a portfolio of resources and the right side as the financing structure that funded it. Every growth decision shows up twice: once as an asset you bought, once as the liability or equity that paid for it.

## Interview questions

1. **A company buys a $1M factory with $300K cash and $700K of new debt. What happens to total assets, total liabilities, and equity?**
   Answer: Assets rise by $1M (cash falls $300K, PP&E rises $1M), liabilities rise $700K, equity is **unchanged**. This is the single most useful sanity check in the subject: if a financing transaction changed equity, something is wrong with your understanding.

2. **Why is equity described as a "plug"? Why does it matter?**
   Answer: Equity is whatever remains after liabilities, so it absorbs the effect of every operating and financing decision — it is where profits, dividends, buybacks, and share issuance all accumulate. It matters because book equity is a *reported balance* that grows only if the company retains profit, which is why "does this company compound value" reduces partly to "is it retaining earnings or paying them out."

3. **A company has $500K of assets and $700K of liabilities. Is it necessarily bankrupt?**
   Answer: No, but the *book* position is negative equity of −$200K, which is a serious flag. It may still be fine if assets are carried at conservative historical cost (or the liabilities include a large non-cash deferred revenue balance from a prepaid contract, which is cash the company already holds), or if the company is early-stage and asset-light. The correct answer is "negative book equity is a signal to investigate, not a verdict" — and investors should check the *composition* of the assets and liabilities before concluding anything.

4. **Your roommate says "equity is just market cap." Correct them.**
   Answer: Book equity is the accounting residual; market cap is the market's price for that claim. They differ whenever market value diverges from book value. Amazon, for example, has historically had enormous *negative* book equity (driven by share-based compensation and, earlier, accumulated losses) alongside a very large market cap. Equity on the balance sheet is a historical-cost accounting artifact, not a valuation.

5. **How does the accounting equation explain why balance sheets are organized by *liquidity*?**
   Answer: Because the equation requires the two sides to describe the same pool of resources, each side must be sorted consistently. Assets run from most liquid (cash) to least (intangibles); liabilities run from soonest due (accounts payable) to longest (long-term debt), and equity is the leftover. A firm that borrowed short-term to hold long-lived assets is exploiting a maturity mismatch, which is why the *composition* of the current side and the fixed-asset side is a real risk signal, not just a formatting convention.

## Watch

- [The ACCOUNTING EQUATION For BEGINNERS](https://www.youtube.com/watch?v=56xscQ4viWE) — Accounting Stuff. Five-minute walk from the equation to a balance sheet, with worked examples.
- [The BALANCE SHEET: all the basics in 12 minutes](https://www.youtube.com/watch?v=_VS4ni14JHs) — Brian Feroldi. A concrete tour of both sides of the equation on a real company (Chipotle), including the key number to look for in each section.
- [Accounting and financial statements (playlist)](https://www.youtube.com/playlist?list=PLSQl0a2vh4HAHUM1CLDf4YnxpX-WmxKZi) — Khan Academy. Sal Khan's full accounting unit; start here and work in order.

## Further reading

- Khan Academy's [Accounting and financial statements](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme) unit — the free text version of the same material, with practice problems on interpreting the balance sheet and income statement.
- Any intro financial accounting text, ch. 1–2 (Brealey/Myers/Marcus is the standard choice for finance students). The skill is structural reasoning, not memorization, so a single read is enough.
