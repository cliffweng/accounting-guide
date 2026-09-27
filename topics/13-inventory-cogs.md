---
title: "13. Inventory & COGS"
layout: default
nav_order: 14
---

# Inventory & COGS
{: .no_toc }

*~7 min read*

**Background**

## Why it matters

Inventory is the line item most likely to be **wrong on the balance sheet** and the one that most directly damages earnings when it is. It is also the clearest example in the subject of an accounting *choice* (FIFO, LIFO, average cost) that changes reported profit with no change in economics, and of the **COGS ↔ inventory** loop that makes gross margin move in ways you must understand rather than misread. This matters most for retail, consumer, pharma, and semiconductor roles; less so for banks or asset-light software.

## Core concepts

- **Inventory is an asset until it's sold, then it becomes COGS.** The moment of sale is the moment the cost moves from the balance sheet to the income statement. That's why inventory *builds* suppress COGS and *drawdowns* inflate it — and why a company can temporarily boost gross margin by slowing restocking, then pay for it later with writedowns.
- **The COGS loop.** `COGS = Beginning inventory + Purchases − Ending inventory`. Because COGS is a *plug* that depends on the inventory balance, anything that changes estimated inventory value changes reported gross profit one-for-one. If inventory is written down by $X, COGS rises by $X and gross profit falls by $X immediately.
- **The three cost-flow methods** (US GAAP allows all three; IFRS forbids LIFO):
  - **FIFO** — first in, first out. In a rising-cost environment, COGS reflects *older, cheaper* costs, so reported **gross margin is higher**.
  - **LIFO** — last in, first out. COGS reflects *recent, higher* costs, so reported **gross margin is lower** — a deliberate conservative choice, and one that creates a **LIFO reserve** on the balance sheet when prices fall.
  - **Average cost** — smooths across the period; margin moves with the average of old and new costs.
  - The economics are identical; only the reported COGS, gross margin, and inventory balance differ. In an inflationary period, FIFO also produces a lower *taxable* income, which is why the LIFO vs. FIFO choice often flips for tax reasons. (Note: the balance-sheet inventory and the tax basis can differ, giving you a deferred-tax line.)
- **Inventory is reported at the *lower* of cost and net realizable value** (LCNRV). If inventory is worth less than it cost — because it's obsolete, damaged, or selling below cost — it must be written down. Writedowns are the loudest early-warning signal in retail, and they are frequently *below* the operating line, so a company can show a "great" operating margin while quietly destroying inventory value.
- **Working capital is the strategic story.** Inventory days (DIO) is a direct cash commitment, and a company that lengthens DIO is funding its suppliers. Too *little* inventory risks stockouts and lost sales; too much ties up cash and raises obsolescence risk. The right level is a competitive decision, and the wrong one shows up in both the cash flow statement and the gross margin.
- **"Inventory" is not homogeneous.** Finished goods, work-in-progress, and raw materials have different turnover, different obsolescence risk, and — under LIFO — different cost layers. A company shifting toward older, slower-moving SKUs (a common retail trick when new product disappoints) quietly changes the mix and hides markdowns. Always check the inventory note and, where disclosed, reserves against slow-moving stock.

## Mental model

```
  THE COGS ↔ INVENTORY LOOP

  Beginning inventory
    +  Purchases
    −  Ending inventory
    =  COGS  →  Revenue − COGS = Gross profit
      ↑              ↓
      └──── writedowns flow straight through here

  CONSEQUENCE: if you estimate inventory $50M too HIGH,
  COGS is understated by $50M and gross profit is OVERSTATED by $50M.

  ─────────────────────────────────────────────
  INFLATING PRICES:  costs 10 → 12 → 14
  FIFO:  COGS uses  10, 12  →  gross margin HIGH
  LIFO:  COGS uses  12, 14  →  gross margin LOW (same cash, same business)
  ─────────────────────────────────────────────

  STRATEGIC LEVER:  Slow restocking → lower COGS → higher margin NOW,
  but less product on hand → lost sales, and a future writedown.
```

## Interview questions

1. **A retailer's gross margin expanded 200bps while revenue fell 3%. Why is that suspicious?**
   Answer: Falling revenue with rising margin is a hard combination to explain operationally, so I'd look for: (a) **LIFO or a rising-cost environment** inflating the gap, (b) a change in **product mix** toward higher-margin items, (c) **inventory drawdown** boosting COGS comparability, or (d) inventory **writedowns taken in a prior year** making this year's cost basis artificially low — the classic "taking the hit early to set up easy comps." Ask whether inventory levels and the LIFO reserve moved, and whether the writedown history is a pattern. A genuine margin expansion on falling sales is possible (price increases, cost deflation) but is the exception.

2. **Explain the "inventory reserve" and why a company might take a large writedown in a weak quarter.**
   Answer: The reserve (or allowance) reduces inventory to net realizable value. Companies take large writedowns in weak periods to "clean up" the balance sheet, front-load future costs, and set a lower base for future COGS — which mechanically *raises* future gross margins. It's an earnings-management pattern, and it's why analysts watch the inventory balance and writedown history rather than just the margin. If a company writes down inventory every 2–3 years, treat the "adjusted" gross margin as the real one and ignore the reported margin in the "bad" year.

3. **What is the difference between LIFO reserve and LIFO liquidation, and why does the second matter more?**
   Answer: A **LIFO reserve** is the gap between inventory on a LIFO basis and on a FIFO basis — a permanent balance sheet reconciliation, growing as prices rise. **LIFO liquidation** is when a company sells *more* than it replaces during a period, so older, cheaper cost layers flow into COGS. That produces a temporary *spike* in gross margin that is purely mechanical and non-repeatable. A company that liquidates LIFO in a year of good margins is borrowing profit from the past — and the margin will reverse once it must buy at current higher prices. Watch for this specifically in industrials and chemicals.

4. **A company has inventory of $800M on $5B of revenue. Days inventory is ~58. Its peers are at 90. What questions do you ask?**
   Answer: First: is 58 days *good*? Maybe — a business with shorter, more predictable demand (groceries, quick-turn manufacturing) legitimately runs lean. Second: is inventory valued aggressively? A low DIO with a big writedown history suggests they sold through excess stock and are now short. Third: is it a *mix* effect — is a high-margin, fast-moving SKU shrinking? Fourth: is the cost flow assumption (LIFO vs. FIFO) flattering the number? And fifth: does the low DIO come with high stockout risk? I'd want to see inventory by category and the 3-year trend before concluding it's efficiency.

5. **Why is COGS sometimes disclosed below the operating line?**
   Answer: Because companies can classify certain costs as "other operating expenses" rather than COGS, or present a combined "cost of revenue" line that includes items you wouldn't predict. The effect: gross margin becomes non-comparable across companies, and "operating income" stays the robust number (see [Expenses & matching](../09-expenses-matching/)). If you're comparing gross margins, check the policy note and confirm both companies classify costs the same way — a 500bp "gross margin improvement" that is entirely a reclassification is a reporting artifact.

6. **How does inventory affect the cash flow statement, and why can a company "grow" its CFO by liquidating inventory?**
   Answer: Inventory is an operating asset: an *increase* is a use of cash (negative CFO), a *decrease* is a source (positive CFO). So a company can generate cash in a tough year by selling down inventory — accepting lost future sales to fund current obligations. That's a real, and sometimes necessary, tactic, but it's finite: inventory can only be drawn down once, and after that the CFO benefit reverses while the lost-margin cost persists. This is why "CFO improved" must always be checked against inventory and receivables movements, not read as pure operational strength.

## Watch

- [INVENTORY & COST OF GOODS SOLD](https://www.youtube.com/watch?v=OB6RDzqvNbk) — Accounting Stuff. The link between inventory on the balance sheet and revenue/COGS on the income statement, with a worked example and manufacturing-vs-merchandising framing.
- [The Essential Guide to Inventory in Accounting](https://www.youtube.com/watch?v=vGPn_Oo7UBQ) — Accounting Stuff. A longer compilation covering perpetual vs. periodic systems and all three cost-flow methods (FIFO, LIFO, average cost). Heavily timestamped if you only need one section.
- [FINANCIAL RATIOS: How to Analyze Financial Statements](https://www.youtube.com/watch?v=3W_LwpeG8c8) — Accounting Stuff. The efficiency ratios — inventory turnover, DSI, DIO, DPO, and the cash conversion cycle — run from roughly the 10:29 mark.

## Further reading

- The **Inventories** note in any 10-K from a retail, industrial, or pharma company. It discloses cost-flow method, components of inventory, and any reserves — the three things that determine whether the reported number is trustworthy.
- Wall Street Prep's free reference on [inventory turnover](https://www.wallstreetprep.com/knowledge/days-inventory-outstanding-dio/) for the ratio math and how it feeds the cash conversion cycle.
