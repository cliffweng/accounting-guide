---
title: "10. Working capital"
layout: default
nav_order: 11
---

# Working capital
{: .no_toc }

*~8 min read*

**🎯 Interview frequent**

## Why it matters

Working capital is where a business model shows its economics in days. It determines how much cash a company must fund before it gets any back, which is why fast-growing businesses often need external financing *despite being profitable*, and why the difference between a good and a great business is often just a 20-day improvement in the cash conversion cycle. In a 3-statement model, the change in working capital is a line item you must forecast explicitly, and interviewers do ask about it.

## Core concepts

- **Working capital = current assets − current liabilities.** **Net working capital (NWC)**, the more useful modeling version, excludes cash and marketable securities: `NWC = (AR + Inventory + Prepaids) − (AP + Accrued expenses)`. Cash is excluded because it's the *output* of the operating cycle, not an input to it.
- **Only the *change* in NWC matters for cash.** A company with $500M of NWC growing revenue 5% barely notices. A company with $50M of NWC growing 50% is *consuming* $25M of cash a year. This single fact explains most of the "profitable but cash-burning" cases — the growth rate, multiplied by the working capital intensity, is your funding requirement.
- **The operating cycle** = the days between paying for inputs and collecting cash from customers: `Operating cycle = DIO + DSO`, where **DIO** (days inventory outstanding) is how long inventory sits and **DSO** (days sales outstanding) is how long customers take to pay.
- **The cash conversion cycle (CCC) = DIO + DSO − DPO.** Subtracting days payable outstanding (DPO) is the key step: if you buy inventory on 60-day terms and sell in 30, suppliers finance 30 of your days. **Negative CCC** means you're *paid* before you pay — suppliers and customers fund you. Amazon runs a large negative CCC; most manufacturers run positive. Negative CCC is a structural advantage and one of the strongest signals of a business model with real negotiating power.
- **Working capital *quality* matters as much as size.** CCC can be "improved" by stretching payables (risking supplier relationships and losing discounts) or by pushing inventory to channel partners. Watch the trend in each of the three components separately, not just the CCC total.
- **The normal seasonal pattern**: most businesses build working capital into a peak season and release it after. So a single year's NWC change is nearly meaningless — use trailing averages or normalize for seasonality. A persistent NWC build is the real signal.
- **"Other current assets" and "other current liabilities" hide things.** Lines like deferred revenue, current portion of long-term debt, and "other accrued liabilities" can each be large. Deferred revenue is a *non-cash* liability (good for liquidity), while the current portion of LTD is a hard maturity wall (bad). Always disaggregate the current section.

## Mental model

```
  THE CASH CLOCK (days)

  Day 0        Pay suppliers ──────────► Receive customer cash
  │            (DIO days)   (DPO days)     (DSO days)
  ▼            │                         │
  Buy/hold     ▼                         ▼
  inventory  Sell it                Collect the cash

  Operating cycle = DIO + DSO
  CCC = DIO + DSO − DPO        ← negative CCC = customers/suppliers fund you

  ─────────────────────────────────────────────────────────────
  WHY GROWTH CONSUMES CASH:

     ΔCash from working capital  ≈  − (Revenue growth) × (NWC / Revenue)
                                   =  − (Revenue growth) × (CCC / 365)

  20% revenue growth  ×  60-day CCC  ≈  3.3% of revenue, in cash, every year.
  Double that growth rate and you double the funding need.
  ─────────────────────────────────────────────────────────────
```

## Interview questions

1. **A retailer's CCC is 90 days. Its main supplier offers 60-day terms. What happens if they switch, and what's the risk?**
   Answer: DPO goes from (say) 30 to 60 days, so CCC falls by 30 days — from 90 to 60. That releases roughly 8% of annual revenue in cash immediately, with zero change to the income statement. It's a free liquidity win. The risks: losing early-payment discounts, straining a supplier relationship, and the supplier responding with a price increase (which is the more common outcome over time). This is a standard value-creation lever in PE.

2. **How do you know if a company's rising CCC is a problem or an investment?**
   Answer: Look at the **components and the drivers**. Rising DIO with stable demand = potential obsolescence risk, especially in fast-moving consumer goods or tech, where old inventory gets written down. Rising DSO = either looser credit terms (a sales-pressure signal) or a genuinely newer, lower-credit-quality customer base. Falling DPO = paying faster, which is either healthier relationships or suppliers tightening terms on a weak balance sheet. And always check whether the CCC change is *seasonal* by comparing to prior years, not just last quarter.

3. **Amazon has negative working capital. Is that a red flag?**
   Answer: No — it's a structural advantage. Amazon collects from customers before it pays many of its costs, and its scale and market position let it extract long payment terms. Negative working capital means **suppliers and customers fund the business**, so growth is *less* cash-hungry, not more. The comparison to make is against peers: a retailer with a *less* negative CCC than Amazon, growing faster, is in a much worse funding position.

4. **A company has a current ratio of 2.5× and a CCC of 120 days. What's your read?**
   Answer: Two conflicting signals, and I want to know why. A 2.5× current ratio can be an artifact of slow-moving inventory — exactly the same problem the 120-day CCC reveals. So the high current ratio may be *illiquid assets*, not strength. The diagnosis: how much of the current assets is inventory, and is the current ratio stable or was it inflated by a recent cash raise? High current ratio plus long CCC is often a warning, not a comfort.

5. **Why does an increase in NWC show up as a *negative* in the cash flow statement?**
   Answer: Because the cash has already left (paid to suppliers, employees) but hasn't come back in (customers haven't paid), so it's sitting on the balance sheet as a receivable or inventory rather than as cash. Rising NWC is a use of cash. Conversely, a *release* of NWC — shrinking inventory, collecting receivables faster, stretching payables — is a **positive** CFO item, which is why a company can have a good year of cash flow purely by harvesting working capital. Never assume a positive working-capital line means good operations.

6. **How would you model working capital in a 3-statement model?**
   Answer: Drive each component off a **days metric** rather than a percentage of revenue, because days are more stable across growth rates and make the seasonality visible. Typical structure: `AR = DSO/365 × Revenue`, `Inventory = DIO/365 × COGS`, `AP = DPO/365 × COGS` (or of purchases, which is more accurate), then `ΔNWC` flows into CFO as a negative. Sanity-check the resulting DSO/DIO/DPO against the company's historical range and its peers — if your model implies DSO falling for five straight years, you're not modeling management's actual practice.

## Watch

- [Working Capital and the Change in Working Capital in Valuation and Financial Modeling](https://www.youtube.com/watch?v=tMgty8jwmHI) — Mergers & Inquisitions / Breaking Into Wall Street. Directly aimed at modeling: why we care about the change, how to compute it, and real-company examples (Best Buy, Zendesk).
- [Cash Conversion Cycle Explained](https://www.youtube.com/watch?v=ePdSit175iQ) — Corporate Finance Academy. A short, clean derivation of DSO + DIO − DPO, with a cash timeline diagram.
- [FINANCIAL RATIOS: How to Analyze Financial Statements](https://www.youtube.com/watch?v=3W_LwpeG8c8) — Accounting Stuff. Timestamped: efficiency ratios (including DSI/DSO/DPO and the cash conversion cycle) start around the 11-minute mark; profitability ratios around 2:39.

## Further reading

- Wall Street Prep's free [Working Capital](https://www.wallstreetprep.com/knowledge/working-capital) reference — the cleanest written treatment of NWC vs. working capital, the working capital cycle, and how to reconcile the change in NWC on the cash flow statement.
- McKinsey's *Uncovering cash and insights from working capital* — the deeper, more strategic treatment of why CCC is a competitive weapon, including real case studies.
