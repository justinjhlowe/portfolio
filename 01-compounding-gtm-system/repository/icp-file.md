# ICP File — Ledgerly

**Version:** 2 | **Last updated:** week 4 | **Owner:** GTM repository | **Change log:** see `change-history.md`

This file's own version hasn't moved since week 4, even though the scores it produces keep changing. That's not staleness, it's the design: this file owns the gate, the disqualifiers, and the tiers. It doesn't own the signal weights. See "How scoring actually works" below.

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

### How scoring actually works

This file used to keep its own copy of the signal list. It doesn't anymore, on purpose. `signal-library.md` is the only place signal weights live. This file's job is to sum whichever of those signals apply to a given account, then run the total through the gate, the disqualifiers, and the tiers below.

That split matters more than it sounds like it should: when a signal's weight changes, or a new signal gets added, every account's score updates automatically, without this file being touched. `icp-file.md`'s version only moves when the gate, a disqualifier, or a tier threshold itself changes. If you see a score change between two weeks but this file's version number is the same, that's not a bug, that's the dependency working correctly. See `signal-library.md` for the current weights.

### Disqualifiers

- Tipalti, Bill.com, or Airbase deployed for 6+ months with no public complaints (switching cost too high, no wedge)
- Finance team of 15+ with a dedicated AP function (headcount problem already solved a different way)
- No budget or funding signal in current fiscal quarter, even at high firmographic fit (added v4 — see change history: this alone explained two of three losses)

### Tiering

- **Tier 1 (score 80–100):** immediate outbound, signal-to-sequence eligible
- **Tier 2 (score 50–79):** nurture, revisit if a new signal fires
- **Tier 3 (below 50):** deprioritize

This file is a query target, not a reference doc. Every workflow that touches outbound, content, or paid reads this before it does anything else.
