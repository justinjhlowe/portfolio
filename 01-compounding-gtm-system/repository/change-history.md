# Change History — Ledgerly GTM Repository

This is the loop. Every entry below is a real weekly cycle: performance data came in, a specific file changed, and the reason is stated. This is the file that proves the difference between tool-centric and learning-centric. A tool runs the same campaign next month as it does today. This repository doesn't let it.

---

## Week 1 — Baseline

Repository built from discovery calls and market research. No performance data yet, so no weighting decisions to defend — this version is a hypothesis, not a result.

- `icp-file.md` v1: firmographic filter only, no scoring.
- `persona-file.md` v1: Controller and VP Finance personas drafted from discovery call notes.
- `positioning-file.md` v1: three value pillars drafted, no priority order, no proof points yet.
- `signal-library.md` v1: six signals listed, weights assigned by judgment, not data.
- `competitor-radar.md` v1: Tipalti, Bill.com, Ramp/Airbase only.

---

## Week 2 — First sequence data

Signal-to-sequence sent 40 sequences across two hooks pulled from `positioning-file.md`: "close faster" (Pillar 2) and "audit-ready" (Pillar 1).

**Data:** "Close faster" hook: 6% reply rate. "Audit-ready" hook: 14% reply rate.

**Changes made:**
- `positioning-file.md` → v2: audit-ready promoted to primary pillar, close-faster demoted to secondary. Reason logged: audit-ready outperformed by more than 2x on identical send volume.
- `icp-file.md` → v2: no change yet, insufficient signal-level data.

---

## Week 3 — First meetings, first objection pattern

5 meetings held from Tier 1 accounts. Recurring objection across 4 of 5 calls: "we already have a BPO handling overflow AP."

**Changes made:**
- `competitor-radar.md` → v2: BPO/outsourced AP added as a fourth competitive alternative. It hadn't been tracked because it isn't software, but it was blocking more deals than any actual software competitor that week.
- `persona-file.md` → v2: Controller objection list updated with BPO-specific rebuttal.
- `positioning-file.md` → v3: proof point added directly countering the BPO frame (cost scaling + audit trail comparison), since existing proof points didn't address it.

---

## Week 4 — First closed deals

1 closed-won, 2 closed-lost. Both losses had strong firmographic fit (Tier 1 on the old scoring) but the same stated reason: "no urgent budget trigger this quarter."

**Changes made:**
- `icp-file.md` → v3: new disqualifier added — no budget/funding signal in current fiscal quarter, even at high firmographic fit. This single factor explained both losses independently of anything else in the file.
- `icp-file.md` → v4: "recent funding round" signal weight reduced from 15 to lower priority after review, since it correlated with fit but not with timing, and timing is what the losses were actually about.

---

## Week 5 — Pattern from the win

Reviewing the one closed-won account for anything not yet captured: the Controller had posted about month-end close pain on LinkedIn nine days before the sequence went out. Not currently a tracked signal.

**Changes made:**
- `signal-library.md` → v4: new signal added, "Controller posts about month-end close pain on LinkedIn," weight 20. Flagged explicitly as a hypothesis from a single data point, not a proven weight — the next ten sequences targeting this signal are the actual test.
- `icp-file.md` → v5: fit scoring table updated to include the new signal.

---

## What this proves

Five weeks, five files, zero weeks where the system ran the same way it did the week before. Nothing here was updated because someone remembered to; it was updated because the data forced the question and the file was the place the answer got written down. That's the repository compounding. A static ICP spreadsheet from week 1 would still be running the "close faster" hook today, still targeting funding rounds with no budget-timing check, and would have never heard of the BPO objection until it lost the fifth deal to it instead of the third.
