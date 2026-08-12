# Pattern 01: The Compounding GTM System

## The problem this solves

Most growth-stage B2B companies think they have a data or tooling problem. What they actually have is a context problem. GTM runs on scattered docs, SDR headcanon, and Slack messages that disappear in a week. When a signal fires, nobody agrees on who the ICP actually is today, so the response is generic, late, or both. Buying more enrichment or more outbound tooling doesn't fix this. The tools run the same way next month as they do today. The problem is architectural: nothing in the stack learns.

## The architecture

A repository the AI can reason against, running on a loop where every cycle makes the next one smarter. That's the center of this pattern, and everything else hangs off it.

**The repository** (`repository/`) is six files: `icp-file.md`, `persona-file.md`, `positioning-file.md`, `signal-library.md`, `competitor-radar.md`, and `change-history.md`. Read `icp-file.md` first. It opens with the static filter this replaces, side by side with the living version, so the difference is visible instead of asserted.

**Four spokes pull from the repository:**

1. *Signal-to-sequence*: outbound velocity without added headcount. A trigger fires, the workflow scores fit against the ICP file, pulls the right persona pain and positioning pillar, and writes a sequence grounded in accumulated context instead of a rep's memory.
2. *SEO/AEO content*: inbound growth for a company with no budget for an agency or paid research, generated from the same persona and positioning files instead of purchased separately.
3. *Paid*: targeting and creative informed by the same ICP and persona files instead of a media buyer optimizing in isolation.
4. *Newsletter*: the owned-audience channel, segmented by identity and lifecycle stage rather than a single trigger. Same persona and positioning files, applied to customers, engaged prospects, and cold subscribers differently, because the repository knows something different about each.

**The loop** is what makes the four spokes compound instead of running as four disconnected tools. `change-history.md` is the proof of this, not a description of it: five dated entries showing real reply rates, meeting outcomes, and win/loss reasons changing specific files with a stated reason each time. The strongest moment in any of the demos is running the same workflow before and after one of these updates, same input, visibly different output. That's the difference between tool-centric and learning-centric, shown instead of claimed.

## Status

- [x] Repository built (synthetic company: Ledgerly, Series B AP automation / spend intelligence, selling to Controllers and VP Finance at 200–2,000 employee companies)
- [x] Signal-to-sequence spoke (interactive demo: `demo/signal-to-sequence.html`, open directly in a browser, no server or dependencies required)
- [x] SEO/AEO spoke (interactive demo: `demo/seo-aeo-content.html`)
- [x] Paid spoke (interactive demo: `demo/paid-optimization.html`)
- [x] Newsletter spoke (interactive demo: `demo/newsletter-segmentation.html`)
- [x] Repository timeline (interactive demo: `demo/repository-live.html`). Replaces browsing raw markdown on GitHub during a live pitch. Fuses the static-filter-vs-living-file contrast with a five-week scrubber that updates `icp-file.md`, `signal-library.md`, `positioning-file.md`, and `competitor-radar.md` in place, with the `change-history.md` reasoning surfaced inline instead of requiring a tab switch.
- [ ] `results.md`: pull anonymized outcomes from where this pattern has actually run for clients

### On the signal-to-sequence demo

It already **is** the before/after proof moment for this one spoke, not just a sequence generator. Pick the "Controller LinkedIn post" trigger, run it against Week 2, then run the identical trigger against Week 5. Week 2 doesn't recognize the signal at all and falls back to generic outreach. Week 5 scores it at 96 and writes a sequence that references the actual post. Same input, same workflow, different output, because the repository underneath it changed. That's the whole argument in ninety seconds without a single slide.

The other two triggers are deliberately less dramatic. "Audit finding" barely changes between versions, because that signal's weight never moved. Worth keeping in the pitch, since a demo where every single input produces a dramatic before/after reads as staged. This one shows the system only rewrites what the data actually challenged.

### On the SEO/AEO demo

Same repository, same before/after mechanic, applied to inbound instead of outbound: `demo/seo-aeo-content.html`. The point being made here is specifically the budget one. The content angle, the SEO title, and the AEO direct-answer block (the tight, citable paragraph an AI assistant would actually lift) all come from files already owned, not a paid keyword tool or an agency brief.

Three topics, same three-tier contrast as the sequence demo. "AP automation vs. BPO" doesn't exist as a comparison at all in Week 2, since the BPO entry wasn't added to `competitor-radar.md` until week 3, so the workflow falls back to a generic category piece with no AEO block, because there's nothing specific enough to cite. "How to speed up month-end close" exists in both versions but sharpens: week 5 leads with the hard number (2.8 days) instead of burying it in a tools list. "Tipalti alternatives" barely moves, because that competitor entry was never touched. Same lesson as the sequence demo, different channel: proves this is a mechanism, not a one-off trick.

### On the paid demo

`demo/paid-optimization.html`. This is the one place the headline number isn't copy quality, it's spend efficiency, on purpose. Paid is the spoke where "no vanity metrics" bites hardest, and clicks or impressions would have been the easy, wrong thing to showcase. The ABM campaign is the one to lead with. Week 2 builds its audience from firmographic and funding filters only, before the budget-timing disqualifier existed, and an estimated 35% of spend lands on accounts with no current-quarter signal, the exact profile behind two of the three closed-lost deals logged in `change-history.md` week 4. Week 5 applies that disqualifier, the audience shrinks from 340 to 210 accounts, average fit score climbs from 71 to 89, and estimated waste drops to 8%. That's a real, defensible number pulled from an actual documented loss pattern, not a benchmark pulled from nowhere.

Search and retargeting hold the same moderate/flat range as the other two spokes: search adds outsourcing-comparison bidding once BPO gets tracked, retargeting barely changes since that persona pain was never in question.

### On the newsletter demo

`demo/newsletter-segmentation.html`. This one earns its place by reusing the exact same two pivot points from the other three spokes instead of inventing a new story. The week 3 BPO discovery and the week 4 timing disqualifier both show up again here. "Engaged prospects, Tier 1" is the dramatic case, same as the other spokes' sharpest example: week 2 can't address the outsourcing objection because the repository doesn't know it exists yet, week 5 leads with it. "Customers nearing renewal" is the moderate case, gaining one proof point. "Newly subscribed, unscored" is the honest flat case: no identifying signal means nothing to personalize, in either version, and the demo says so instead of faking a difference.

That repetition across all four spokes is the actual point worth making to a technical colleague: run all four demos back to back and the same two dated events in `change-history.md` ripple through outbound, content, paid, and newsletter identically. One repository, four channels, not four separate systems that happen to share a folder.

### On the repository-live demo

`demo/repository-live.html`. This is the one built around a single account, Fairmont Diagnostics, run through the real scoring formula at all five weeks instead of two endpoints. The fit score sits flat at 60 (Tier 2, nurture) for four straight weeks, then jumps to 80 (Tier 1, immediate outbound) in week 5 when the new signal lands, and it's the account that actually closed. Every file panel is a diff, old value struck through, new value highlighted, so the mechanism reads as a change to a specific line, not a refreshed card. Week 5's `icp-file.md` panel shows no edit at all on purpose: it sums whatever `signal-library.md` provides, so the score moves without this file being touched.

## What's actually left

The repository and all four spokes are built and internally consistent. Every number and claim in any demo traces to a specific file and, where relevant, a specific dated entry in `change-history.md`. What's not done: `results.md` with real anonymized outcomes once this pattern has run for an actual client. That's the right next step, not a before-you-can-pitch blocker. The demos as they stand are enough to run the full argument today.

## Why Ledgerly

The vertical is fintech, one of the four I work in, and the buyer (Controller / VP Finance at a mid-market company) is specific enough that a prospect in an adjacent vertical still recognizes the mechanic even though the company is fictional. Swap the repository files for a different vertical and the same architecture holds. That's the point of building by pattern instead of by client.
