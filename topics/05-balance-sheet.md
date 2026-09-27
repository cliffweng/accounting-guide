---
title: "05. Balance sheet"
layout: default
nav_order: 6
---

# Balance sheet
{: .no_toc }

*~9 min read*

**🎯 Interview frequent**

## Why it matters

The balance sheet is a snapshot of what the company owns, owes, and has left for owners *at one instant* — and the snapshot is organized in a way that encodes risk. Reading it well means seeing the **maturity structure** (short-term debt funding long-lived assets is a classic early-warning signal), the **quality of the assets** (receivables and intangibles are worth less than cash), and the **flexibility** the company has (undrawn revolver, positive equity, low leverage). It is also the statement most often abused by non-GAAP framing: "we have $2B of cash" may be $2B of restricted or customer-owned cash.

## Core concepts

- **Assets = Liabilities + Equity**, sorted by likelihood of conversion to cash. **Current assets** (cash, receivables, inventory, prepaid) are expected to convert within a year; **non-current assets** (PP&E, intangibles, goodwill, long-term investments) are not.
- **Liabilities are split by when they're due, not by why.** The current/non-current split is the single most important structure on the statement: **the current ratio compares assets that convert to cash in a year against obligations that must be paid in a year.** If those don't line up, the company needs to refinance, and refinancing depends on credit markets and lender mood, not on management.
- **Quality of assets varies enormously.** Cash ≈ cash. Receivables are cash *minus* collection risk and timing. Inventory is cash *minus* obsolescence risk. Intangibles and goodwill are *not* cash at all — you can't pay a bill with them, and their carrying value is a historical allocation that a recession can permanently impair. Analysts increasingly subtract goodwill/intangibles when assessing "tangible book value."
- **Equity has three layers to know:** share capital (par value of shares issued), additional paid-in capital (what investors paid above par, plus treasury-stock effects), and **retained earnings** (cumulative net income minus cumulative dividends). Retained earnings is the only one that grows from operations — and it only grows if the company *retains* earnings rather than paying them out.
- **Debt is not all equal.** Long-term debt at a fixed coupon, convertible debt, leases, and revolving credit (often **undrawn**, appearing as a *facility* rather than a liability) have very different risk profiles. A company with no drawn revolver at a moment of stress is in a fundamentally different position from one that is fully drawn.
- **Negative equity has two very different causes**, and you must diagnose which: (a) cumulative losses or heavy buybacks (a warning), or (b) massive share-based comp / buybacks funded by debt, or large accumulated *deferred revenue* (a non-cash liability the company already holds cash for — often benign, see [Accrual vs. cash](../02-accrual-vs-cash/)). Amazon historically had huge negative book equity largely for this reason.

## Mental model

```
  ASSETS (quality ↓)                    LIABILITIES + EQUITY
  ────────────────                      ──────────────────────
  Cash & equivalents   ★★★★★          Accounts payable       (pay as you go)
  Receivables          ★★★★            Accrued expenses        (non-cash payables)
  Inventory            ★★★             Short-term debt         ← REFINANCE RISK
  Prepaid / other      ★★              Current portion of LTD
  ─────────────────────────             ─────────────────────────
  PP&E (net)           ★★★             Long-term debt          ← no near-term wall
  Intangibles/goodwill ★               Other long-term liabs
                                        ─────────────────────────
                                        Share capital + APIC
                                        Retained earnings       ← compounding engine
                                        = BOOK EQUITY

  Sanity checks, always:
    1. Does it balance?  (Assets = Liabilities + Equity)
    2. Is the current side funded by non-current assets?  → liquidity risk
    3. Is there undrawn revolver capacity?  → flexibility
    4. Is equity positive, and if not, why not?
```

## Interview questions

1. **A company has $100M of current assets, $60M of current liabilities, and $500M of net PP&E. Is it liquid?**
   Answer: Current ratio 1.67× looks fine, but the composition matters: if the $100M is mostly inventory (a fabricator with slow-moving stock) rather than cash or receivables, the company is far less liquid than the ratio suggests. Conversely, if a chunk of "current liabilities" is deferred revenue the company already holds cash for, the effective ratio is better than 1.67×. Always ask *what's inside* current assets and current liabilities before trusting the ratio.

2. **Why is a large current ratio not automatically good?**
   Answer: Because it can be achieved by stockpiling inventory or hoarding cash — both of which destroy returns on capital. A very high current ratio often signals a company that stopped reinvesting. DuPont makes this explicit: excess current assets drag down asset turnover, so ROE falls even with stable margins (see [Ratios](../11-ratios/)).

3. **A company has $2B of "cash" and $4B of debt. Net debt is $2B. Why might a credit analyst still be concerned?**
   Answer: Several reasons worth checking: (a) the cash may be **restricted**, **customer-owned** (e.g. fintech/payments, airline client funds), or held in foreign jurisdictions and not freely repatriable; (b) the debt may be **short-dated**, so net debt understates near-term refinancing risk; (c) gross debt matters for covenants and for how the company is treated in a downside case. "Net" debt is a liquidity concept; "gross" and maturity profile are solvency concepts. Know both.

4. **A company has negative shareholders' equity and is growing revenue 40% a year. Concerned?**
   Answer: Not automatically — first diagnose the cause. Negative equity driven by deferred revenue (customers prepaid) or by cumulative buybacks/stock comp is a different animal from negative equity driven by cumulative net losses. The real questions: is cash positive and growing? Is CFO positive? Are there covenant breaches or going-concern flags in the notes? Amazon ran negative book equity for years while growing; many companies run negative equity from real losses and die.

5. **What is goodwill, and why is it dangerous?**
   Answer: Goodwill is the excess paid over fair value in an acquisition — an accounting residual that used to be amortized and is now, under US GAAP, generally *not* amortized (subject to annual impairment testing). It's dangerous because (a) it doesn't represent anything you can sell or collect, (b) its carrying value is set by assumptions that can shift, and (c) impairments are how companies write off a bad acquisition years later — often in a "one-time" charge, which is the classic earnings-management pattern from [the income statement page](../04-income-statement/).

6. **Walk me through how you'd read a balance sheet in 3 minutes.**
   Answer: (1) **Liquidity**: cash level and trend, current ratio, undrawn revolver. (2) **Funding structure**: ST vs. LT debt, net debt / EBITDA, maturity wall, covenant headroom. (3) **Asset quality**: are receivables and inventory growing faster than revenue? How much is goodwill/intangibles? (4) **Equity**: positive, growing, or negative-and-why. (5) **Equity change**: retained earnings growth and buyback pace.

## Watch

- [The BALANCE SHEET: all the basics in 12 minutes](https://www.youtube.com/watch?v=_VS4ni14JHs) — Brian Feroldi. Walks a real balance sheet top to bottom, including what "the key number" is in each section.
- [Ultimate Financial Statement Summary: From Revenue to Cash](https://www.youtube.com/watch?v=pOZrylLwWS4) — Leila Gharani. A rapid tour of all three statements in sequence; good for building your "shape" of the statements before going deep on one.
- [Balance Sheet Red Flags (4 Warnings Signs)](https://www.youtube.com/watch?v=Uuy4xYJoh0w) — Brian Feroldi. A punchy short list of what actually kills companies, all of it visible on this statement.

## Further reading

- Khan Academy's [Interpreting the balance sheet](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme/financial-statements-tutorial/a/interpreting-the-balance-sheet) — free practice problems on a real set of statements.
- **Financial Shenanigans** (Palm Tree Publishing) or **The Intelligent Investor**'s "defensive investor" checklist — both teach you to read a balance sheet for *what it hides* rather than what it says.
