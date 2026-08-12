# Pitch Guide — Walking a Prospect Through This Repo

Read this before the call, not during it. The sequence below is what turns a demo into proof instead of a feature tour. It's written generically so it holds up as new patterns get added to `/Portfolio/`, with `01-compounding-gtm-system` as the working example throughout.

## Before the call: pick one spoke

Match the spoke to what they told you was broken in discovery. Don't demo all four cold on a first call — one spoke, chosen because it's their stated pain, is the whole meeting.

- "We can't outbound at volume without hiring" → `demo/signal-to-sequence.html`
- "We're spending on ads with mediocre return" → `demo/paid-optimization.html`
- Budget-constrained content, stalled inbound → `demo/seo-aeo-content.html`
- Retention or expansion pressure → `demo/newsletter-segmentation.html`

If nothing in discovery points clearly at one, default to signal-to-sequence — it's the sharpest single before/after and the easiest to translate to a buyer who hasn't thought about this in systems terms yet.

## Phase 1 — Name the enemy before touching the screen

Don't open with the demo. Open with the diagnosis, in their language if you can pull it from discovery:

*"Most teams in your position think this is a data problem or a tooling problem. It's actually a context problem. Your GTM runs on scattered docs, headcanon, and Slack messages that disappear in a week, and when a signal fires, nobody agrees on who your ICP actually is today."*

This is what makes everything after this feel like the answer to a problem they already named, not a pitch for a tool they didn't ask for. Thirty seconds, no slides.

## Phase 2 — Show the repository as real files

Open `repository/icp-file.md` and point at the static filter sitting next to the living, scored version. Not a tour of all six files, just this one contrast. The point is making the architecture claim visible instead of asserted: this is what replaces a spreadsheet nobody updates.

## Phase 3 — Run the demo on Week 2 first, on purpose

Pick the trigger or topic with the sharpest before/after for that spoke (the linked signal-not-recognized case for signal-to-sequence, the missing comparison for SEO/AEO, the wasted-spend audience for paid, the objection-blind segment for newsletter). Let the Week 2 output be a little unremarkable. Don't apologize for it or rush past it — they've seen competent-but-generic AI output before, and that's exactly the point.

## Phase 4 — Toggle to Week 5 on the identical input

Let the sharper, grounded output sit on screen for a second before saying anything. Point at the retrieval trace so they see which specific file changed and why. This is the moment the meeting is built around. Don't talk over it.

## Phase 5 — Open `change-history.md` and preempt the objection

Show the actual dated entry that caused the difference: a real reply rate, an objection heard on a real call, a real loss reason. Say directly:

*"The data's synthetic because I can't show you a client's actual system. The mechanism generating it is the same one running live."*

A sharp prospect will ask if you scripted a good-looking demo. This answers it before they do.

## Phase 6 — Optional: show the same pivot in a second spoke

If they're engaged and there's time left, show the same week-3 or week-4 event rippling into a different channel — the BPO objection reshaping ad copy or the newsletter the same way it reshaped the first spoke. This is the strongest thing you can show a technical buyer: one repository moving four channels. It's a bonus round, not the core meeting. Don't force it if they're already sold or already out of time.

## Phase 7 — Turn it back on them

Ask what their ICP file, their signal library, their positioning file would actually need to say. Don't answer for them. Their answer is real discovery, not a rhetorical close, and whatever they say back is the first deliverable of working together:

*"This repository, built for you, is week one, not a sales prop I'm showing you."*

## When they ask about the tools underneath

Prospects will ask which specific tools power each spoke, Clay, transcription, ad platforms, a CRM. `tools-and-stack.md` in this same folder is the running answer key. The shape of every answer is the same: separate the input tool, which is replaceable, from the repository, which isn't. Add to that file after the call if a new tool question comes up that isn't covered yet.

## What not to do

Don't lead with the tool. Don't demo more than one spoke unless they ask for more. Don't let the fake-data question catch you off guard, Phase 5 exists so it doesn't. Don't rush Phase 4, the silence while the better output sits on screen is doing more work than anything you could say over it.
