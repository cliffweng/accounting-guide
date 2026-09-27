---
title: "06. Cash flow statement"
layout: default
nav_order: 7
---

# Cash flow statement
{: .no_toc }

*~9 min read*

**🎯 Interview frequent**

## Why it matters

The cash flow statement answers the only question that actually matters in a crisis: **did cash actually move, and where did it go?** While the income statement is subject to accrual estimates and the balance sheet is a snapshot, the cash flow statement is largely arithmetic on real bank movements — which makes it the hardest statement to manipulate and the one most likely to tell you the truth about a business. In banking interviews, "walk me through the cash flow statement" is almost always followed by "why is it different from net income?"

## Core concepts

- **Three sections, and you should be able to define each by example:**
  - **Operating (CFO)** — cash from running the business: collections from customers, payments to suppliers and employees, taxes paid. *This is the profit measure you should care about.*
  - **Investing (CFI)** — cash to long-lived assets and investments: **capex**, acquisitions, purchases/sales of investments. *This is where growth is funded.*
  - **Financing (CFF)** — cash to/from capital providers: debt issued or repaid, equity issued, buybacks, **dividends**.
  - Ending cash = beginning cash + CFO + CFI + CFF. That last line ties directly to the cash on the balance sheet — a hard internal consistency check (see [Linking the three statements](../07-linking-three-statements/)).
- **The indirect method is the reconciliation you must be able to do.** `CFO = Net income + D&A + other non-cash items − increase in net working capital`. Every line is there for a reason: add back non-cash expenses, then adjust for revenue/expense recognized but not yet settled in cash. The *only* real reason CFO differs from net income is non-cash items and working capital timing.
- **Capex is the number to find and the number to distrust.** Maintenance capex keeps the business running; growth capex expands it. Reported "capital expenditures" is the total, and separating the two requires reading the notes. FCF = CFO − capex. A company that reports strong FCF while capex is well below D&A is **under-investing** and harvesting, not compounding.
- **CFO should roughly track net income over a full cycle.** Persistent divergence is the signal: CFO far below NI suggests earnings aren't converting (rising receivables/inventory); CFO far above NI suggests collection of previously booked receivables or a big non-cash add-back (impairments, SBC). One year of divergence is noise; three is a story.
- **Working capital movements dominate CFO in growth companies.** A company growing 50% is investing cash in receivables and inventory every year, so CFO lags net income structurally. This is why "CFO < net income" is not automatically bad — you need growth context.
- **Accrued and non-recurring items live here too.** Cash restructuring payments, cash taxes vs. book taxes, and the SBC add-back all show up in the reconciliation. This is where you can verify whether a "non-cash, non-recurring" charge actually involved cash.

## Mental model

```
  Net income                                          <- accrual profit
    + D&A (non-cash)                                  <- add back
    + SBC / impairments / other non-cash              <- add back
    − Δ Receivables        (grew  →  cash not yet in) <- usually a DRAG in growth
    − Δ Inventory          (grew  →  cash not yet out) <- usually a DRAG in growth
    + Δ Payables / accrued (grew  →  kept the cash)   <- usually a BOOST
  = CFO                                                <- REAL operating cash

  − Capex (PP&E + intangibles)                         <- maintenance + growth
  = Free Cash Flow                                     <- cash left after staying alive
  − Interest, taxes, dividends, debt service, buybacks
  = Cash available to fund growth or return to owners


  HEALTHY PATTERN (mature, steady):
     NI  ≈  CFO      FCF > 0        CFI < 0 (capex only)   CFF ≈ 0

  HEALTHY PATTERN (compounder):
     NI  >  CFO      FCF > 0 and growing    CFI < 0 (capex > D&A)

  WARNING SIGNS:
     CFO << NI for 3+ yrs (receivables/inventory build)  |  NI > 0 but CFO < 0
     FCF positive only because capex << D&A            |  CFF > 0 forever (funded by debt/equity, not operations)
```

## Interview questions

1. **A company's net income is $500M every year but CFO is only $80M and falling. What's your read?**
   Answer: Red flag. Either (a) **receivables and/or inventory are ballooning** — revenue recognized ahead of collection, growth that's cash-hungry or possibly not real; (b) large **non-cash charges** are flattering net income (impairments, SBC) while operations genuinely generate little cash; or (c) genuine structural problems. I would immediately check the receivables/inventory balances versus revenue growth on the balance sheet, and check the reconciliation lines. Persistent CFO/NI far below 1 is one of the strongest single indicators of earnings quality problems.

2. **Company A has 25% EBITDA margins and Company B has 8%, but B's EBITDA converts to cash at 95% and A's at 40%. Which is the better business?**
   Answer: Hard to say without context, but B is meaningfully more interesting. EBITDA margin is an *estimate-laden* accounting output; cash conversion is closer to fact. A's 40% conversion suggests accrual revenue, inventory build, or heavy working capital absorption. I'd want to know A's growth rate and whether the gap is explained by investment (capex, inventory for a ramp) or by collection problems.

3. **Why is CFO the right "profit" measure for valuing a business, and why isn't it perfect?**
   Answer: Because it's the cash actually generated by operations, it's hard to manipulate, and it's what funds interest, capex, and dividends. Imperfections: it's *lumpy* (one working-capital swing can dominate a year), it's *after cash interest and taxes* (so it's a levered measure — a levered company looks worse even if the underlying business is identical), and it doesn't capture accrual-estimated items like SBC cleanly. For unlevered valuation you typically re-derive from EBITDA and reinvestment instead.

4. **A company reports negative CFO, positive net income, and revenue growing 50% a year. Bull or bear?**
   Answer: Neither, yet. Negative CFO with rapid growth can be a deliberate, rational investment (Amazon, grocery delivery, marketplaces) — you're funding customer acquisition and inventory. The tests are: (1) is the working capital *recoverable* (receivables will convert; inventory will sell)? (2) how much external funding does it need, and from whom, on what terms? (3) is there a credible path to positive FCF, and by when? If a 50%-growth company with structurally negative cash conversion needs a new capital raise every 12 months, it's a funding risk, not a growth story.

5. **Explain the difference between "capex of $500M" and "capex of $500M against D&A of $300M." Why does the comparison matter?**
   Answer: Because D&A is roughly the historical cost of consuming the asset base. Capex > D&A means the asset base is *growing* (investing for expansion); capex < D&A means it's *shrinking* (harvesting, under-investing, or asset-lite-ing via outsourcing/leases). A company with FCF that looks great because capex is far below D&A is not sustainable indefinitely — it will eventually not be able to maintain its competitive position. Analysts flag this as "under-investment."

6. **Where in the cash flow statement would you look to see if a restructuring charge was really non-cash?**
   Answer: The CFO reconciliation. If the company added back a restructuring charge, look at whether the corresponding "change in liabilities" line shows a big increase (accrued but unpaid → genuinely non-cash this period) or whether there's an actual restructuring cash outflow in CFO. Also check the investing section for asset sale proceeds from closing facilities. This is exactly the kind of verification that separates a real answer from a rehearsed one.

## Watch

- [Basic cash flow statement](https://www.youtube.com/watch?v=Mioqyv_IW3E) — Khan Academy. Sal Khan builds the indirect-method reconciliation from scratch; short and completely mechanical, which is exactly what you want here.
- [The CASH FLOW STATEMENT: all the basics in 9 minutes](https://www.youtube.com/watch?v=b41Jo8CtQec) — Brian Feroldi. The three sections explained intuitively, with free cash flow as the payoff concept.
- [Cash Flow Statement Basics Explained](https://www.youtube.com/watch?v=hMBN6yTIDb0) — Leila Gharani. Focused on *why* the statement exists and why you shouldn't stop at the income statement.
- [The CASH FLOW STATEMENT for BEGINNERS](https://www.youtube.com/watch?v=DiVPAjgmnj0) — Accounting Stuff. Builds the indirect method line by line with a worked example.

## Further reading

- Khan Academy's [Basic cash flow statement](https://www.khanacademy.org/economics-finance-domain/core-finance/accounting-and-financial-stateme/financial-statements-tutorial/v/basic-cash-flow-statement) — the free text version with the same example laid out in steps.
- Any 10-K's cash flow statement with the notes open. Reading one real statement with the notes is worth more than any textbook chapter for building fluency.
