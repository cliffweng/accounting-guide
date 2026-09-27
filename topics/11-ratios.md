---
title: "11. Ratios (liquidity, profitability, leverage)"
layout: default
nav_order: 12
---

# Ratios (liquidity, profitability, leverage)
{: .no_toc }

*~10 min read*

**🎯 Interview frequent**

## Why it matters

Ratios are compression: they turn three statements into a handful of comparable numbers. The math is easy; the judgment is knowing **which ratio answers which question**, that most ratios are only meaningful against history and peers, and that the headline ROE is usually the least honest number on the page. DuPont is the tool that makes this explicit by decomposing a return into its three drivers — and interviewers like it because it's a fast test of whether you can reason structurally.

## Core concepts

- **Liquidity — can you meet near-term obligations?**
  - **Current ratio** = current assets / current liabilities. Crude; easily inflated by slow inventory.
  - **Quick ratio** = (current assets − inventory) / current liabilities. Removes the least liquid asset.
  - **Cash ratio** = cash & equivalents / current liabilities. The most pessimistic.
  - Interpretation: liquidity ratios are highly **industry-specific** and are almost meaningless in isolation. Banks have negative current liabilities and enormous "inventory." What matters is the *trend* versus the company's own history and versus the maturity of its debt.
- **Profitability — how efficiently does the business turn resources into profit?**
  - **Gross margin** = GP/Revenue; **operating margin** = EBIT/Revenue; **net margin** = NI/Revenue.
  - **ROA** = NI / average total assets. **ROE** = NI / average common equity.
  - **ROIC** = NOPAT / invested capital, where NOPAT = EBIT × (1 − tax rate). ROIC is the cleanest measure of operating quality because it removes capital structure and tax-distortion effects, and it can be compared across business models and over long histories without leverage flattering the number.
- **DuPont decomposes ROE into three drivers**: `ROE = Net margin × Asset turnover × Equity multiplier`, i.e. `NI/Revenue × Revenue/Assets × Assets/Equity`. **Profitability × efficiency × leverage.** The powerful use is not the number, it's the *bridge*: when ROE rises, you can say which of the three moved, and a rise driven only by leverage is a fundamentally different (and lower-quality) story than a rise driven by margin.
- **Leverage ratios measure how much of the asset base is creditor-funded**: debt/assets, debt/equity, **net debt / EBITDA**, and **interest coverage** (EBIT / interest). Interest coverage is the covenant-relevant one — it's the ratio that determines whether a downturn becomes a default.
- **Leverage mechanically inflates ROE.** If a business earns ROIC above its after-tax cost of debt, borrowing raises ROE; if ROIC is *below* the cost of debt, leverage destroys value while *raising* reported ROE. This is why ROE must always be read next to ROIC and net debt/EBITDA. A high-ROE, low-ROIC company is a leveraged bet, not a good business.
- **Cash-flow ratios exist and deserve more attention than they get**: CFO/net income (earnings quality), FCF/market cap or FCF yield (a valuation-adjacent quality measure), and capex/D&A (under-investment check, see [Cash flow statement](../06-cash-flow-statement/)). These are harder to manipulate than accrual-based ratios.

## Mental model

```
  DUPONT:  ROE  =  Net margin   ×   Asset turnover   ×   Equity multiplier
            (can they?)            (efficiently?)         (what's financed by?)

            NI/Revenue    ×    Revenue/Assets    ×    Assets/Equity
              e.g. 8%          e.g. 0.8x            e.g. 2.5x
                                    ↓
                                  = 16% ROE

  SAME 16% ROE, COMPLETELY DIFFERENT COMPANIES:
     A: 20% margin  ×  0.4x turnover  ×  2.0x  =  16%   luxury, asset-heavy, conservative
     B:  5% margin  ×  1.6x turnover  ×  2.0x  =  16%   retailer, volume, high leverage
     C:  8% margin  ×  0.8x turnover  ×  2.5x  =  16%   leverage doing the work

  THE QUESTION IS NEVER "WHAT IS ROE?" — IT'S "WHICH OF THE THREE MOVED, AND WHY?"
```

## Interview questions

1. **Two companies both report 18% ROE. One has 25% net margins and the other 6%. How do you decide which is better?**
   Answer: DuPont says both are getting there, but by completely different means, and the durability differs. High-margin/low-turnover businesses (luxury, software) are usually pricing-power businesses — the high margin is defensible but the business is more cyclical and asset-heavy. Low-margin/high-turnover businesses (retail, distribution) depend on volume, execution, and working capital discipline, and are far more sensitive to small margin shocks. Add leverage (equity multiplier) and the picture changes again. There's no answer without knowing the industry, growth, and capital intensity.

2. **A company raises ROE from 15% to 20%. ROIC is flat. What happened, and is it good news?**
   Answer: Since ROIC is flat, the operating business is unchanged, so the improvement came from **leverage** (equity multiplier rose) or from shrinking the equity base (buybacks). Both are financial rather than operating improvements. Leverage raises ROE only if ROIC > after-tax cost of debt; if ROIC is below the cost of debt, this is *value-destructive* despite the better-looking ROE. Buybacks raise ROE but are neutral-to-negative unless the shares were genuinely undervalued. So: probably not good news, and definitely not operational improvement.

3. **Why is ROIC considered the "cleanest" profitability measure, and what's the catch?**
   Answer: Because it strips out both capital structure (it sits above the interest line, using NOPAT rather than net income) and tax-distortion noise, so a leveraged and an unlevered version of the same business report roughly the same ROIC — which makes it comparable across time and across differently financed peers. The catches: (a) "invested capital" requires a judgment call (debt + equity, or net debt + equity less excess cash) and analysts differ; (b) it's less familiar to interviewers, so state the definition explicitly.

4. **A company's quick ratio is 0.9× but its current ratio is 2.2×. Why is that a problem?**
   Answer: Because the difference is **inventory** — the company is relying on selling inventory to meet near-term obligations. If demand is weak or the inventory is obsolete or slow-moving, the company cannot pay its bills. This is a classic early-warning configuration, and it's exactly what shows up in distressed retailers. Follow up by checking inventory turnover and whether there's a writedown or any LIFO reserve disclosure.

5. **Interest coverage is 4× and net debt/EBITDA is 5.5×. Walk through how a mild recession could produce a default.**
   Answer: EBITDA falls 25%. Coverage drops to ~3× — uncomfortable but survivable. Net debt/EBITDA rises to ~7.3×. If EBITDA falls 40%, coverage is ~2.4×, net debt/EBITDA is ~9×, and most high-yield documentation has **maintenance covenants at 4–5× total leverage** and a minimum interest coverage of ~2.0–2.5×. That's a technical default with no negotiation. The important structural point: leverage turns a *modest* operating shock into a *solvency* event, because the debt is fixed while the earnings are variable. (This is the same mechanism as the debt/cash feedback loop in [Linking the three statements](../07-linking-three-statements/).)

6. **How do you use ratios in a screen, given that all of them are backwards-looking and gameable?**
   Answer: Use them to *generate questions*, not to make decisions. Two stages: (1) **screen** on a small set that are hard to fake — CFO/net income, capex/D&A, ROIC trend over 5+ years, and share count trend (a persistent ROE propped up by shrinking equity is a red flag). (2) **investigate** whatever the screen flags, by reading the notes and the MD&A. Crucially, compare against the company's own **5–10 year history** before comparing to peers: a "cheap" ratio that has been falling for a decade is not cheap, it's deteriorating.

7. **Company A has a 4.0× current ratio; Company B has 1.2×. Which is safer?**
   Answer: You can't answer that from the ratio. B might be a business with negative working capital and a structurally superior cash position; A might be a capital-intensive manufacturer drowning in inventory. The follow-ups that matter: what's inside A's current assets, does B have an undrawn revolver, what's each one's near-term maturity schedule, and is CFO positive in a downturn? A high current ratio is only meaningful if the assets are liquid, and a low one is fine if it's a deliberate structural position backed by committed liquidity.

## Watch

- [FINANCIAL RATIOS: How to Analyze Financial Statements](https://www.youtube.com/watch?v=3W_LwpeG8c8) — Accounting Stuff. A single 24-minute pass over all five ratio families with formulas and worked numbers; heavily timestamped, so you can jump to the family you need.
- [DuPont analysis explained](https://www.youtube.com/watch?v=bhbDDSohJ84) — A short walkthrough of the ROE / ROA / asset-turnover / leverage chain, which is the fastest way to see the decomposition in one sitting.
- [Return on Equity (ROE) Explained via Dupont Analysis](https://www.youtube.com/watch?v=bs6wIc9fnJA) — A more applied treatment, including how interest and tax burden sit inside the margin leg.

## Further reading

- Wall Street Prep's free reference pages for [DuPont analysis](https://www.wallstreetprep.com/knowledge/dupont-analysis-template) and [working capital](https://www.wallstreetprep.com/knowledge/working-capital) — the 3-step and 5-step models laid out cleanly, and the standard reference on the site.
- **Financial Statement Analysis and Security Valuation** (Stephen Penman, free PDF version is widely posted on Columbia's site) — the rigorous version of ratio analysis, with a focus on why accounting multiples are deliberately built to be hard to manipulate. Longer than this guide, but it reframes the whole subject.
