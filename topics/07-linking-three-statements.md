---
title: "07. Linking the three statements"
layout: default
nav_order: 8
---

# Linking the three statements
{: .no_toc }

*~10 min read*

**🎯 Interview frequent**

## Why it matters

This is the single most important page in the guide. If you can explain how the three statements **feed each other** — and do it out loud in under ten minutes — you can handle essentially any accounting question an investment-banking or markets interview will throw at you. "Walk me through the three statements" is the canonical technical question, and the follow-ups ("okay, now what happens to the balance sheet if revenue grows 20%?") are all variations on the same few loops.

## Core concepts

- **The income statement is a period, the balance sheet is a date, and the difference between the two dates is the cash flow statement.** That one sentence is the whole idea. Change in balance sheet = income statement activity + cash flows. If you can state that, you can derive any statement from the other two.
- **Loop 1 — the retained earnings link (income statement → balance sheet).** `Ending RE = Beginning RE + Net income − Dividends`. This is the most-tested identity in the subject, and the dividends term is where candidates lose points. It connects the income statement directly to a balance sheet equity line, and it's why buybacks (which reduce equity without touching net income) are a *capital allocation* decision rather than a performance one.
- **Loop 2 — the cash link (cash flow statement → balance sheet).** `Ending cash = Beginning cash + CFO + CFI + CFF`. Every dollar in the cash flow statement lands in a balance sheet account: capex → PP&E, debt issued → debt payable, buyback → treasury stock/equity reduction. This loop is what makes the statements reconcile.
- **Loop 3 — the working capital link (balance sheet → cash flow statement).** Changes in *operating* balance sheet accounts (receivables, inventory, payables, accrued expenses) are exactly the working-capital lines in the CFO reconciliation. An increase in receivables is a *negative* CFO item. An increase in payables is a *positive* CFO item. This is the mechanism behind "growing companies consume cash."
- **The debt/cash feedback loop is the subtle one.** Interest expense flows income statement → net income → cash. Debt issuance is a financing inflow that increases cash, which increases interest income, which increases net income. Refinancing a maturing bond can produce a one-time gain/loss depending on extinguishment accounting. This loop is why a company with a near-term maturity wall is genuinely fragile, and why "leverage" is not a static ratio but a dynamic process.
- **Interest expense classification is a real accounting trap.** Under US GAAP, interest on *operating* leases is an operating expense, while interest on most other debt sits below the operating line. This is why operating margin is not perfectly comparable across capital structures — two identical businesses with different debt loads report different operating margins.
- **Building a simple three-statement model is the check for understanding.** If you can project revenue → COGS → net income → retained earnings → balance sheet → CFO, you understand the system. A 3-statement model is the foundational deliverable in banking, and the mechanics come straight from this page.

## Mental model

```
  THE THREE LOOPS
  ═════════════════

  ┌──────────────────────┐
  │   INCOME STATEMENT   │──── Net income ────┐
  │   (a PERIOD)         │                    │
  └──────────────────────┘                    ▼
                              ┌──────────────────────────┐
  ┌──────────────────────┐     │  RETAINED EARNINGS       │
  │    BALANCE SHEET     │◄────│  Beg. RE + NI − Divs     │  LOOP 1
  │    (a DATE)          │     │  = End. RE               │
  │                      │     └──────────────────────────┘
  │  Assets                              ▲
  │    ↑ Δ Cash, AR, Inv, PP&E          │ Net income
  │  Liabilities + Equity               │
  │    ↑ Debt, AP, Equity  ─────────────┘
  └──────────┬───────────────────────────┘
             │  every change in a balance sheet account
             │  is explained by a cash flow (or by net income)
             ▼
  ┌──────────────────────────────────┐
  │      CASH FLOW STATEMENT         │  LOOP 2
  │   ΔAR → CFO     Capex → CFI     │  LOOP 3
  │   ΔInv → CFO    Debt → CFF       │
  │   ΔAP → CFO     Divs → CFF       │
  │   PP&E, ΔCash → CFI / CFF        │
  └──────────────────────────────────┘

  RULE OF THUMB:  Δ Balance Sheet = (Income Statement activity) + (Cash Flows)
```

## Interview questions

1. **Revenue grows 20% next year. What changes, and in which order, across the three statements?**
   Answer: (1) **Income statement** first: revenue up; COGS up if the business carries inventory, and gross margin may shift if operating leverage kicks in. (2) **Balance sheet**: receivables up if terms are unchanged (same DSO → 20% more AR); inventory up if the business is inventory-carrying; payables up if purchases scale; cash may be *down*. (3) **Cash flow**: because AR and inventory grow, working capital consumes cash, so CFO typically *falls* relative to net income — despite higher profit. (4) **Equity**: retained earnings up by the incremental net income minus any dividend change. (5) Optionally PP&E up if growth needs capacity. The punchline interviewers want: **profit goes up, cash often goes down.**

2. **Company issues $500M of new debt and pays a $200M special dividend. What's the effect on each statement?**
   Answer: **Balance sheet**: cash +$500M, debt +$500M, retained earnings −$200M (the dividend is a direct reduction of equity, not an expense). **Cash flow**: CFF = +$500M − $200M = +$300M net inflow; net income **unchanged** (dividends are not expenses). **Income statement**: only the interest on the new debt hits below the line. This is the classic test of whether you know that a dividend is not an expense.

3. **Net income is $300M, dividends were $100M, and no new equity was issued. Equity on the balance sheet rose $200M. Retained earnings rose $150M. What else explains the difference?**
   Answer: **Other comprehensive income (OCI)** and/or stock-based compensation credits to APIC — plus any share issuances. A common real-world case: positive currency translation gains on overseas subsidiaries, or the tax-effected portion of pension/benefit-plan remeasurement, flow through OCI and hit equity without ever touching net income. This is why the income statement alone can't reconcile equity. (Also check: share-based compensation increases APIC.)

4. **You only have a company's income statement and balance sheet. Can you build the cash flow statement?**
   Answer: Yes, for the *summary* version. `CFO ≈ NI + D&A + other non-cash − Δ operating working capital`, `CFI ≈ −capex + net investment purchases`, `CFF ≈ net debt issuance + equity issuance − dividends − buybacks`. In practice: Δcash (from the two balance sheet dates) must equal CFO + CFI + CFF, which gives you a check. What you *can't* reliably recover is the gross detail — acquisitions vs. capex splits, buybacks vs. option exercises, and which specific working-capital accounts moved.

5. **What breaks if a company has negative cash flow for several years? Walk the chain.**
   Answer: Cash balance falls → **current ratio falls** → **revolver or working-capital line gets drawn** → **CFF turns positive** (new borrowing) → **interest expense rises** → **net income falls** → **covenants on leverage or interest coverage get tighter** → **refinancing at a higher rate or with more restrictive terms**, or in the extreme, a covenant breach and restructuring. The key insight: the damage compounds through the interest expense loop, which is why a company with a modest cash shortfall can end up in a spiral rather than a smooth recovery.

6. **A company's CFO is $400M, capex is $120M, and D&A is $200M. FCF is $280M. What's the concern?**
   Answer: Capex ($120M) is well below D&A ($200M), so the asset base is shrinking — the company is under-investing relative to what it consumes. The FCF number is *flattered* right now but not sustainable: eventually capacity or competitiveness degrades, or the asset base becomes too small to support the revenue base. Always compare capex to D&A before admiring a free cash flow number, and check whether the "low capex" is actually outsourced/leased spending showing up elsewhere (e.g., in OpEx or as a lease liability).

7. **Why does the balance sheet's cash line have to equal the cash flow statement's ending cash?**
   Answer: Because it's the same physical quantity described twice. Any mismatch means one of the three statements has an error — which is exactly what makes this a powerful *consistency test* in diligence. In practice, real filings sometimes show small differences due to restricted cash classification, but the identity is exact in substance and is the basis of the "does this model tie out?" check every modeler runs.

## Watch

- [Connecting the Income Statement, Balance Sheet, and Cash Flow Statement](https://www.youtube.com/watch?v=f3T0tCjw1k8) — Brian Feroldi. A worked tutorial example where one business's transactions flow through all three statements, which is exactly the mental model above.
- [The Ultimate Guide to Financial Statements](https://www.youtube.com/watch?v=eorpdJUWfTA) — Accounting Stuff. A single deep dive covering all three in order; good consolidation read.
- [How to Read Financial Statements w/ Brian Feroldi (TIP752)](https://www.youtube.com/watch?v=vIameomgKMQ) — The Investor's Podcast. Longer, but excellent on *how to think* when reading statements rather than just where the lines are.

## Further reading

- **Reading Financial Statements For Dummies** (Charles M. Jones) — short, genuinely readable, and the closest thing to a comprehensive beginner-to-intermediate bridge.
- Khan Academy's [Accounting and financial statements](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme) unit — covers the balance sheet ↔ income statement relationship explicitly, with exercises.
- Building a small 3-statement model in Excel from scratch (even a toy one with two years of data) is the single best way to make this page stick. It's the standard "first week" exercise for banking new hires.
