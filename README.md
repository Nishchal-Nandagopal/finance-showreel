# Ten desks. One answer key each.

> Finance runs on models. Most of them never get checked. These do.

### **[▶ Watch the reel](https://nishchal-nandagopal.github.io/finance-showreel/)**

Ten projects, one for each seat on the Street, from the M&A desk to the trading pod. Each one does that seat's real work on free public data, and is then graded against something it couldn't see: the bankers' own fairness opinion, the price a buyer actually paid, the next earnings print, the tape.

## The house rules

1. **Public data only.** SEC filings, FRED, IMF ship tracking, satellite imagery. Nothing paid.
2. **Lock it before you look.** Every prediction gets a SHA-256 fingerprint before the outcome exists, so it can't be edited after the fact.
3. **Grade it against reality.** Each desk has an answer key it never saw.
4. **Publish the misses.** Three of these ideas failed. They're in the reel, next to the wins.

## The desks

Click any desk to jump to it in the reel.

| | Desk | The work | What happened |
|---|---|---|---|
| P0 | **[LedgerLens](https://nishchal-nandagopal.github.io/finance-showreel/#p0)** · research tooling | A filing robot that answers from SEC filings, shows its page, and says "I don't know" when it can't prove it | 50/50 benchmark questions (in-sample); right page in the top 5 **70%** of the time vs 43% for keyword search |
| P1 | **[Kimberly-Clark / Kenvue](https://nishchal-nandagopal.github.io/finance-showreel/#p1)** · investment banking | Rebuilt four banks' fairness opinions on the $48.7B deal from the merger proxy | Overlapped all 10 of their analyses; Centerview's DCF matched within **0.3%** |
| P2 | **[Jamf · Hologic buyouts](https://nishchal-nandagopal.github.io/finance-showreel/#p2)** · private equity | Priced two take-privates blind, locked the answers, then compared | Came in **16% and 35% low**, because the sponsors used 1.8x more debt. Rules rewritten |
| P3 | **[Amkor Technology](https://nishchal-nandagopal.github.io/finance-showreel/#p3)** · equity research | Full initiation: 3-statement model, DCF, reverse DCF, geopolitical scenarios | **SELL, $39 target** vs a $76 Street average. Live |
| P4 | **[$400M foundation](https://nishchal-nandagopal.github.io/finance-showreel/#p4)** · asset management | Investment policy and five portfolio builds, with market views drawn from Fed statements | The 60/40's return at less risk. The Fed-statement views didn't help, and the reel says so |
| P5 | **["Priya", H-1B engineer](https://nishchal-nandagopal.github.io/finance-showreel/#p5)** · wealth management | Goals-based plan for a tech employee with 40% of her net worth in one stock | Found a **$17,121** tax bill her payroll never withheld |
| P6 | **[Annual-report text changes](https://nishchal-nandagopal.github.io/finance-showreel/#p6)** · quant research | Pre-registered signal, 6,842 10-Ks, all 46 attempts counted | **Killed by its own rules.** It was value investing in a trench coat |
| P7 | **[Teradyne](https://nishchal-nandagopal.github.io/finance-showreel/#p7)** · FP&A | Locked a budget, then explained the $139.1M first-half beat line by line | Bias-corrected guidance (**2.2%** error) beat my ML model (4.8%) |
| P8 | **[Hormuz, satellites & oil](https://nishchal-nandagopal.github.io/finance-showreel/#p8)** · macro | Counted ships through the strait (68 → 5 a day), ran event studies with placebos | Brent **+32%** in five days. The satellite NO₂ signal was a null |
| P9 | **[Pod-style paper book](https://nishchal-nandagopal.github.io/finance-showreel/#p9)** · trading | Risk rules locked before trade one, a ticket validator, weekly P&L attribution | The desk is set. The live clock hasn't started |

## Still open

Calls on the record that the market hasn't scored yet: whether the Kenvue deal closes, the Amkor price target, Amkor's and Teradyne's next quarters, the Hormuz scenarios, and one honest live retry of the killed quant idea. The scoreboard at the bottom of the reel updates as each one settles, hits and misses alike.

## Under the hood

**Data:** SEC EDGAR & XBRL, FinanceBench, FRED, Damodaran, SEC N-PORT, IMF PortWatch, CFTC, Sentinel-5P and Sentinel-1 imagery, public price history.
**Built with:** Python (pandas, statsmodels, scikit-learn, LightGBM), Excel models with check tabs, and a hand-built motion reel (GSAP + SVG).

---

<sub>Nishchal Nandagopal · Tempe, AZ · [Medium](https://medium.com/@nishchalnandagopal) · [LinkedIn](https://www.linkedin.com/in/nishchal-nandagopal-730105253) · Also: **[Ten cases, the consulting reel →](https://github.com/Nishchal-Nandagopal/consulting-showreel)**<br>Personal projects on public data. Not investment advice; no positions held. The P4 and P5 clients are fictional; the data is real.</sub>
