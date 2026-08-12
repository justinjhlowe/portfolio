# Signal Library — Ledgerly

**Version:** 3 | **Last updated:** week 5 | **Queried by:** signal-to-sequence workflow, paid targeting, `icp-file.md`'s scoring

Every signal below is a trigger a workflow can watch for. This is the only file that owns weights — `icp-file.md` reads this list to score an account, it doesn't keep its own copy. Weight is not static and moves when `change-history.md` shows it should.

| Signal | Weight | Source | What it indicates | Status |
|---|---|---|---|---|
| Audit finding or restatement in press/filings | 25 | News, SEC filings | Active urgency, budget likely pre-approved internally | Stable since v1 |
| New Controller / VP Finance hire, last 6 months | 25 | LinkedIn | Highest-converting trigger to date — new hire reviews process in first 90 days | Stable since v1 |
| Controller posts about month-end close pain on LinkedIn | 20 | LinkedIn | Added v3 (week 5), high correlation with the one closed-won deal to date | New |
| Manual AP / invoice approval complaint on G2 or Glassdoor | 15 | Review sites | Named pain, not inferred | Stable since v1 |
| Recent funding round (Series B+), last 6 months | 15 | Crunchbase, press | Budget available, weak alone without a current-quarter signal | Downweighted v2 |
| Job posting: AP Specialist / AP Clerk | 10 | Job boards | Scaling AP headcount manually — the exact wedge | Stable since v1 |
| ERP migration announced (job posting: "NetSuite admin") | 10 | Job boards | Finance stack in flux, window before new tooling decisions harden | Stable since v1 |

## Notes on weighting

Weights aren't opinions, they're outcome-derived. "Recent funding round" was downweighted in v2 (week 4) after two of three closed-lost deals had strong funding signal but no current-quarter budget signal — high firmographic fit, wrong timing. "Controller posts about close pain" was added in v3 (week 5) directly from the pattern in the one deal that closed. Two data points isn't proof, it's a hypothesis the next ten sequences will test. That's the point: this file is supposed to be wrong sometimes and get corrected, not right once and frozen.

## Why this file exists separately from `icp-file.md`

Every signal and its weight live here, once. `icp-file.md` owns the gate, the disqualifiers, and the tiers, and sums whatever this file currently says a given account qualifies for. Keeping weights in one place instead of two means a weight change here updates every account's score immediately, without anyone having to remember to edit a second file that duplicates the same numbers.
