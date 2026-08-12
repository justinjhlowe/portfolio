# ICP File — Ledgerly

**Version:** 5 | **Last updated:** week 5 | **Owner:** GTM repository | **Change log:** see `change-history.md`

## The static filter this replaces

Most companies write this once, put it in a spreadsheet, and never touch it again:

> 200–2,000 employees. $20M–$250M revenue. SaaS, healthcare services, or logistics. Uses NetSuite or Sage Intacct. Series B or later.

That filter is dead the day it's written. It tells a rep who *might* fit and nothing about who's actually likely to respond, buy, or close. It doesn't get smarter when a deal is won or lost. It's a list, not a system.

## The living version

Same firmographic core, but every signal below carries a weight, every weight is set by outcome data, and the file has a version number because it's expected to change. This is what a rep or a workflow actually queries against.

### Firmographic core (qualifying, not scoring)

- Employee count: 200–2,000
- Revenue: $20M–$250M
- Industry: SaaS, healthcare services, logistics (in that priority order as of v5 — see change history for why logistics moved up)
- ERP: NetSuite or Sage Intacct (disqualify if custom-built ERP or QuickBooks — deal cycle data shows these accounts aren't ready)
- Funding stage: Series B or later, OR profitable with $20M+ revenue

### Scored signals (fit score, 0–100)

| Signal | Weight | Source | What it indicates |
|---|---|---|---|
| Audit finding or restatement mentioned in press/filings | 25 | News, SEC filings | Active urgency, budget likely already approved internally |
| New Controller or VP Finance hire in last 6 months | 25 | LinkedIn | New hire reviews process in first 90 days — highest-converting trigger to date |
| Manual AP / invoice approval complaint on G2 or Glassdoor | 15 | Review sites | Named pain, not inferred pain |
| Recent funding round (Series B+) in last 6 months | 15 | Crunchbase / press | Budget available, but weak alone — see disqualifiers |
| Job posting for AP Specialist / AP Clerk | 10 | Job boards | Scaling AP headcount to cover volume manually — the exact problem we solve |
| ERP migration announced (job posting for "NetSuite admin") | 10 | Job boards | Finance stack in flux, window to get in before new tooling decisions harden |

### Disqualifiers

- Tipalti, Bill.com, or Airbase deployed for 6+ months with no public complaints (switching cost too high, no wedge)
- Finance team of 15+ with a dedicated AP function (headcount problem already solved a different way)
- No budget or funding signal in current fiscal quarter, even at high firmographic fit (added v4 — see change history: this alone explained two of three losses)

### Tiering

- **Tier 1 (score 80–100):** immediate outbound, signal-to-sequence eligible
- **Tier 2 (score 50–79):** nurture, revisit if a new signal fires
- **Tier 3 (below 50):** deprioritize

This file is a query target, not a reference doc. Every workflow that touches outbound, content, or paid reads this before it does anything else.
