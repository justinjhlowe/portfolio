# Signal Library — Ledgerly

**Version:** 4 | **Last updated:** week 5 | **Queried by:** signal-to-sequence workflow, paid targeting

Every signal below is a trigger a workflow can watch for. Weight feeds directly into the ICP file's fit score, is not static, and moves when `change-history.md` shows it should.

| Signal | Weight | Source | What it indicates | Status |
|---|---|---|---|---|
| Audit finding or restatement in press/filings | 25 | News, SEC filings | Active urgency, budget likely pre-approved internally | Stable |
| New Controller / VP Finance hire, last 6 months | 25 | LinkedIn | Highest-converting trigger to date — new hire reviews process in first 90 days | Stable |
| Controller posts about month-end close pain on LinkedIn | 20 | LinkedIn | Added week 5, high correlation with the one closed-won deal to date | New |
| Manual AP / invoice approval complaint on G2 or Glassdoor | 15 | Review sites | Named pain, not inferred | Stable |
| Recent funding round (Series B+), last 6 months | 15 | Crunchbase, press | Budget available, weak alone without a current-quarter signal | Downweighted |
| Job posting: AP Specialist / AP Clerk | 10 | Job boards | Scaling AP headcount manually — the exact wedge | Stable |
| ERP migration announced (job posting: "NetSuite admin") | 10 | Job boards | Finance stack in flux, window before new tooling decisions harden | Stable |
| Competitor review left recently (G2 review of Tipalti/Bill.com/Airbase) | 10 | Review sites | Active evaluation in category, timing signal for paid and outbound both | Stable |

## Notes on weighting

Weights aren't opinions, they're outcome-derived. "Recent funding round" was downweighted in v4 after two of three closed-lost deals had strong funding signal but no current-quarter budget signal — high firmographic fit, wrong timing. "Controller posts about close pain" was added in v5 directly from the pattern in the one deal that closed. Two data points isn't proof, it's a hypothesis the next ten sequences will test. That's the point: this file is supposed to be wrong sometimes and get corrected, not right once and frozen.
