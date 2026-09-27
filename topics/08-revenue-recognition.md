---
title: "08. Revenue recognition basics"
layout: default
nav_order: 9
---

# Revenue recognition basics
{: .no_toc }

*~8 min read*

**Occasional**

## Why it matters

Revenue is the single largest line in most income statements and the most aggressively managed. *When* you record revenue determines *when* you record profit, and every form of aggressive revenue recognition ultimately runs through the same small number of judgments. You don't need to memorize ASC 606 for an interview — you need to know the question to ask, which is: **has the company delivered, and has it been paid?**

## Core concepts

- **The core principle: record revenue when the goods or services are delivered**, not when the contract is signed, not when the cash arrives, and not when the invoice is sent. Everything else is mechanics to get the timing right in hard cases.
- **The 5-step model (ASC 606 / IFRS 15)** collapses to three questions you actually need: (1) Is there an **enforceable contract**? (2) What **performance obligations** are in it, and have they been satisfied? (3) What is the **transaction price**, and how is it **allocated** to those obligations? If the answer to any of these is "not yet," revenue is deferred.
- **Deferral is normal and often healthy.** A SaaS company collecting a year up front records **deferred revenue** (a liability) and recognizes it ratably as it delivers. A construction company recognizes revenue **percentage of completion** as work is done. A software company with a perpetual license and separate support arrangement allocates the price between them. These are not aggressive — they're the framework working.
- **The classic "premature revenue" patterns** to recognize instantly: recognizing revenue on a signed contract before delivery; extending payment terms to book a sale; shipping product to a customer's own warehouse ("channel stuffing") and booking the sale; bill-and-hold arrangements; bundling low-margin services into a contract to hit a target; booking sales in a weak quarter to meet a consensus number. All of them show up later as **rising receivables, rising returns/refunds, or a gap between net income and CFO**.
- **Bundled vs. stand-alone selling price is the fiddly part.** If you sell a device for $1,000 with a one-year support plan and the standalone prices are $900 and $300, you don't book $1,200 revenue — you allocate, here to $750 and $250. The "standalone selling price" judgment is where analysts argue real money, so it shows up in the notes.
- **Related-party and channel revenue deserve a second look.** Revenue from the CEO's other company, or from a "customer" that is really a distributor, is the highest-risk revenue. Also check the **customer-concentration** disclosure: if one customer is >10% of revenue, that revenue is less durable than the headline suggests.

## Mental model

```
  Ask three questions, in order:

  1. IS THERE A CONTRACT?
     No  →  no revenue. Period. (Signed-but-not-delivered = nothing.)

  2. HAVE THE PERFORMANCE OBLIGATIONS BEEN SATISFIED?
     "Build and deliver 100 servers by Q3"  → recognize as delivered (percentage of completion)
     "Install software, then 12 months of support"  → separate obligations,
         recognize the license up front, the support ratably
     "Upfront annual fee"  → deferred revenue (liability) on the balance sheet,
         recognized ratably over the year

  3. WHAT PRICE, ALLOCATED TO WHAT?
     Bundle total $1,200 across two obligations → allocate by standalone selling price.
     Do NOT book $1,200 on day one.

  RESULT ON THE BALANCE SHEET:
     Delivered, unpaid  →  Accounts RECEIVABLE  (asset)      → earnings
     Paid, not delivered→  Deferred REVENUE     (liability)  → not yet earnings
```

## Interview questions

1. **A software company jumps from quarterly to annual billing and revenue accelerates. Is anything wrong?**
   Answer: Maybe. Annual prepay creates a **deferred revenue** balance, and recognizing that upfront would pull revenue forward. So I'd check: (a) did the deferred revenue balance *fall*? (b) is revenue recognized ratably or upfront? (c) did receivables or DSO fall suspiciously? Annual billing itself is a **cash flow** event more than a revenue event — a company can collect annual cash and report the same revenue, which is a good outcome, not a bad one. The real question is whether the *timing of recognition* changed, not whether cash came in earlier.

2. **Why do SaaS companies care so much about deferred revenue growth?**
   Answer: Because deferred revenue is a forward-looking, contracted, cash-collected indicator of future revenue. Growing deferred revenue is one of the highest-quality growth signals available: the customer already paid, so there's no collection risk and no receivable. Watch the "remaining performance obligation" (RPO) disclosure too — it's contracted future revenue and often more informative than the income statement. The flip side: a *decline* in deferred revenue can be an early warning even if reported revenue still grows.

3. **Revenue grew 15% but accounts receivable grew 40%. What are the likely explanations?**
   Answer: (a) **Looser payment terms** (DSO up) — the classic aggressive-revenue signal; (b) a shift in **customer mix** toward larger, slower-paying customers or the public sector; (c) **recent acquisitions** bringing in receivables; (d) a **new financing/subsidization program** (e.g., vendor financing of the customer's own purchases) that flatters sales; (e) straight-up premature recognition. I'd check DSO in isolation, the allowance for credit losses, and any disclosure about extended terms.

4. **Your cousin says "recognized revenue must be cash collected." Why are they wrong?**
   Answer: Under accrual accounting those are two different things, and the difference is the *entire reason* the balance sheet has receivables (see [Accrual vs. cash](../02-accrual-vs-cash/)). Recognized revenue means *delivered*. Cash collected on a prepaid contract is deferred revenue, not revenue at all. Being able to explain this crisply is a fast credibility win — interviewers are listening for exactly this distinction.

5. **What is a "bill-and-hold" arrangement and why is it on the fraud checklist?**
   Answer: The seller invoices the buyer but retains physical possession of the goods until the buyer needs them. It's legitimate when the buyer has requested it and lacks space or capability to store the product. It becomes aggressive when it's used to pull sales into a weak quarter — the company "sold" product nobody took. Signs: rising inventory *and* rising receivables, unusual revenue in the last week of a period, and a subsequent return spike. Always check the notes.

6. **How do you test whether reported revenue is real, using only public filings?**
   Answer: Triangulate: (1) compare revenue growth to **receivables, deferred revenue, and returns** growth; (2) compare net income growth to **CFO**; (3) check **DSO** trend; (4) look at the **critical accounting estimates** note for any revenue-recognition language; (5) check **customer concentration** and **related-party** disclosures; (6) read the **MD&A** for management's own explanation of the change. If revenue growth is only explained by acquisitions or FX, it's not organic. If five of those six line up and management's explanation is specific and plausible, it's probably fine.

## Watch

- [Revenue recognition explained](https://www.youtube.com/watch?v=816Q6pOaGv4) — a compact walk through the 5-step model with the key judgments highlighted.
- [ASC 606 Revenue Recognition in Plain English: A CPA's Walkthrough of the 5-Step Model](https://www.youtube.com/watch?v=I8dBdXuT7cA) — longer but systematic, with worked examples of the judgment calls.
- [Revenue toolkit: Step five—Recognize revenue](https://www.youtube.com/watch?v=OG9Lai0AMb8) — PwC. A Big Four perspective on when to recognize and when to defer; useful for seeing the "why" behind the rule.

## Further reading

- The **Revenue Recognition** section of the notes to any recent 10-K from a company in the sector you're covering. The policy note is written in plain language and is the fastest way to see how the framework applies in practice.
- Investopedia's free explainer on [revenue recognition](https://www.investopedia.com/terms/r/revenuerecognition.asp) as a reference for the specific jargon (RPO, ASC 606, stand-alone selling price).
