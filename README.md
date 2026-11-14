# Fifteen finance projects. Every forecast sealed, then graded.

> Finance runs on models. Most of them never get checked. These do.

### **[▶ Open the showreel](https://nishchal-nandagopal.github.io/finance-showreel/)**

Fifteen projects, one for each seat from the M&A desk to the options desk. Each does that seat's real work on free public data and is then graded against something it could not see: the bankers' own fairness opinion, the price a buyer paid, the next earnings print, the tape. Every project on the page opens an interactive lab.

## The house rules

1. **Public data only.** SEC filings, FRED, exchange feeds, IMF ship tracking, satellite imagery. Nothing paid.
2. **Seal it before you look.** Every forecast gets a SHA-256 fingerprint and joins a hash-chained ledger before the outcome exists.
3. **Grade it against reality.** Each project has an answer key it never saw.
4. **Publish the misses.** Nulls, kills and misses are on the page next to the wins.

## The projects

| | Seat | The work | What happened |
|---|---|---|---|
| P0 | **[LedgerLens](https://nishchal-nandagopal.github.io/finance-showreel/#p0)** · research tooling | A filing Q&A engine that cites its page and refuses what it cannot prove | 50/50 FinanceBench metric questions in-sample (39/50 first pass); keyword baseline 0/50 |
| P1 | **[Kimberly-Clark / Kenvue](https://nishchal-nandagopal.github.io/finance-showreel/#p1)** · investment banking | Rebuilt four banks' fairness opinions from the merger proxy | All 10 ranges overlap the banks'; 5 of 10 midpoints within 10% |
| P2 | **[Jamf and Hologic](https://nishchal-nandagopal.github.io/finance-showreel/#p2)** · private equity | Two take-privates priced blind, then compared with the deal | **Missed:** $11.00 vs $13.05 paid; $49.75 vs $76.00 paid. I assumed too little debt both times |
| P3 | **[Amkor Technology](https://nishchal-nandagopal.github.io/finance-showreel/#p3)** · equity research | Full initiation with a reverse DCF | SELL, target $39 against a Street mean of $76.40. Sealed until September 2027 |
| P4 | **[$400M foundation](https://nishchal-nandagopal.github.io/finance-showreel/#p4)** · asset management | Policy, allocation and a test of language-model market views (fictional client) | **Null, published:** Sharpe 0.63 with the views, 0.60 without (p = 0.52) |
| P5 | **["Priya"](https://nishchal-nandagopal.github.io/finance-showreel/#p5)** · wealth management | A plan for an H-1B engineer with concentrated stock (fictional client) | Found a $17,121 withholding gap before April |
| P6 | **[10-K rewrites](https://nishchal-nandagopal.github.io/finance-showreel/#p6)** · quant research | A pre-registered text signal, all 46 trials counted | **Killed by its own rules** (development t of 0.5) |
| P7 | **[Teradyne](https://nishchal-nandagopal.github.io/finance-showreel/#p7)** · FP&A | A frozen budget, variance analysis and capital allocation | **Null, published:** my ML forecast lost to guidance (4.8% vs 4.4% error); bias-corrected guidance 2.2% |
| P8 | **[Hormuz and oil](https://nishchal-nandagopal.github.io/finance-showreel/#p8)** · macro | Ship counts through the strait and event studies with placebo dates | Brent +32% in the first five days (placebo p = 0.026). The satellite signal was a null |
| P9 | **[Paper long-short book](https://nishchal-nandagopal.github.io/finance-showreel/#p9)** · trading | Pod-style risk rules enforced in code before trade one | Dry run only. No track record yet |
| P10 | **[Order books](https://nishchal-nandagopal.github.io/finance-showreel/#p10)** · market making | One full Nasdaq day and one crypto hour rebuilt from the raw feeds | Zero broken references in 9.6 million updates. Order flow does not predict the next move; a taker loses on all eight symbols |
| P11 | **[Factor risk model](https://nishchal-nandagopal.github.io/finance-showreel/#p11)** · portfolio risk | Does a one-in-twenty loss happen one day in twenty? | 4.91% of 134,750 days at the 95% limit. The 99% limit fails at 1.75% |
| P12 | **[Who files?](https://nishchal-nandagopal.github.io/finance-showreel/#p12)** · credit | A bankruptcy screen graded on every bankruptcy 8-K, plus a credit memo | AUC 0.87 out of sample; 60% of bankruptcies in the riskiest tenth. Its probabilities did not beat a constant |
| P13 | **[The Treasury curve](https://nishchal-nandagopal.github.io/finance-showreel/#p13)** · rates | Duration sheets and forward-rate forecasts, graded | Explains 92–94% of Treasury fund moves and 8% of high yield. "No change" beat the forward rate on 6 of 6 horizons |
| P14 | **[What options charge](https://nishchal-nandagopal.github.io/finance-showreel/#p14)** · volatility | Implied against realised volatility over 441 months | Implied was higher in 84% of months. Selling it had a Sharpe of 1.14 before costs; its worst month cost 25 average months |

## The record so far

Nine calls are sealed on the ledger. Four have been graded (as of 10 November 2026):

| Call | Mine | Benchmark | Actual | Result |
|---|---|---|---|---|
| Teradyne Q3 revenue | $1,316M | Guidance $1,250M | $1,306M | Off 0.7% against 4.3% |
| Amkor Q3 revenue | $2,004M | Street $2,041M | $1,991M | Off 0.7% against 2.5% |
| Amkor Q3 EPS | $0.78 | Street $0.78 | $0.76 | **Miss:** off 2.6% against 2.2% |
| Kenvue deal closes | 85% | Market 98% | Closed | **Miss:** the market was better calibrated |

Still open: the Amkor price target (September 2027), Brent's Q4 average (January 2027), ten earnings moves (late November 2026), a 25-name bankruptcy list and a 9-year Treasury rate (both November 2027).

## Under the hood

**Data:** SEC EDGAR and XBRL, FinanceBench, FRED, Nasdaq ITCH, Kraken, Damodaran, SEC N-PORT, IMF PortWatch, Sentinel imagery, public price history.
**Built with:** Python (pandas, statsmodels, scikit-learn, LightGBM), Excel models with check tabs, 352 automated tests, and a hand-built page (GSAP, canvas and SVG).

---

<sub>Nishchal Nandagopal · Tempe, AZ · [Medium](https://medium.com/@nishchalnandagopal) · [LinkedIn](https://www.linkedin.com/in/nishchal-nandagopal-730105253) · Also: **[Fifteen consulting cases →](https://github.com/Nishchal-Nandagopal/consulting-showreel)**<br>Personal projects on public data. Not investment advice; no positions held. The P4 and P5 clients are fictional; the data is real.</sub>
