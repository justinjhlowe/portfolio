# Tools & Stack — Answering "What Are You Actually Using"

This is a living FAQ. Add to it every time a prospect asks about a tool that isn't covered yet. The answer almost never changes shape, only the specific tool name does.

## The pattern behind every answer here

Split everything into two layers. The **input layer** is whatever produces a raw fact or signal: an enrichment tool, a transcription tool, an ad platform, a CRM, a job board. The **reasoning layer** is the repository, the scoring, the versioning, the change history. Input tools are replaceable by design. The reasoning layer isn't. Almost every "do you use X" question resolves to: yes, X can sit in the input layer, or it doesn't matter which tool sits there, because the repository is what decides whether the fact matters and what happens to it after.

## How is Clay leveraged in this process?

Lead with the real position, don't dodge it: Clay was dropped three months ago. It enriches data faster than any SDR team, but enrichment was never the actual problem, the problem was that whatever it found sat in a spreadsheet or CRM field with no memory and no connection to what actually converted. If a prospect already has a Clay contract, they don't need to cancel it, it can sit upstream as one input feeding a signal into the repository, same as a job posting or a G2 review would. It's replaceable, and that's the point. Clay finds a fact. It doesn't remember anything.

## We use Otter, not Zoom. Does that matter?

No. The mechanism behind a change-history entry like the week 3 BPO objection, a pattern spotted across multiple calls, doesn't care which tool produced the transcript. Whatever captures the raw text gets read the same way: a workflow scans it, flags a pattern, proposes a repository update, a human confirms it before it ships. The input layer is whatever's already in use. The reasoning layer doesn't change.

## Does this work for Google Ads and Meta, or just LinkedIn?

Yes, mechanically, for all three. The repository outputs a scored account or contact list and a creative angle, both platform-agnostic. What changes per platform is delivery: Google Customer Match, Meta Custom Audiences, LinkedIn Matched Audiences all want the list uploaded differently, and creative gets resized to spec. For this ICP specifically, mid-market finance buyers, LinkedIn is the sharper primary channel and Google/Meta are secondary, not because the mechanism doesn't work there but because that's where this buyer actually spends attention. Say that as a recommendation, not a hedge.

## What about HubSpot or Salesforce, and Breeze specifically?

Which CRM doesn't matter, same logic as Clay: pick whichever the client already runs, it's the input layer, and the repository doesn't care which one it is. It's where deals and activity live, permanently and necessarily, and nothing here is trying to replace that.

Breeze is the sharper version of the question, because it's not a passive enrichment tool, it's trying to be a reasoning layer inside the CRM. Draw the line directly: Breeze operates on one record at a time, the contact, the deal, the email, using whatever HubSpot can see about that record. It doesn't have a positioning file that a paid campaign, a newsletter segment, and an SEO brief all read from and write back to simultaneously. If a loss reason gets logged on a deal, Breeze doesn't reshape the ICP scoring weights that then change what the ad audience looks like and what the next piece of content leads with, the same day, across functions. That's the same tool-centric limitation as Clay, in the same shape, just with a UI that looks like reasoning instead of enrichment.

The repository can write into the CRM, push the fit score into a HubSpot property so a rep sees it without opening a separate file, and that's a good idea regardless of which CRM it is. But the reasoning that produced that score, and the memory of why it moved, lives in the repository, not in a CRM field or a Breeze suggestion scoped to one record. Breeze is a fine copilot for a rep working a single deal. It isn't a system that makes every channel smarter from what a different channel just learned.

## What about Notion, GitHub, or other tools that are a source of truth, not just an input?

This one's different in kind from Clay, Otter, or the CRM questions, because Notion and GitHub aren't replaceable inputs, they're genuine candidates for where the repository itself lives. Answer it that way instead of forcing it into the same box.

The repository is a discipline and an architecture, not a specific tool. It can live in GitHub, in Notion, anywhere that holds structured text with edit history. What doesn't count is pointing at an existing Notion wiki or GitHub repo of docs and calling the problem already solved. The test isn't whether a doc tool exists, it's whether anything in it changes because a deal was won or lost, and whether there's an entry that proves it. Most companies' Notion fails that test, it's a wiki written once during onboarding and never touched again, the static filter problem in nicer formatting.

GitHub is the strongest fit of anything on this list, worth saying directly rather than hedging toward whatever the prospect already uses. Version control is native to git, a commit message is a change-history entry for free, and a weekly update to a file reviewed and merged like a pull request is a more credible version of this pitch to a technical buyer than anything built by hand, because the discipline is enforced by the tool, not by someone remembering to log a reason. This repository is plain markdown files specifically because that's what a GitHub repo looks like.

Notion can house the same content, it just doesn't come with that discipline built in. Someone has to decide to build the scoring and the change-log habit into it on purpose. Fine as the home, not fine as the excuse, if their current Notion isn't versioned and isn't scored, it's the exact thing this replaces.

The interface is negotiable either way, raw GitHub, a Notion view, a chat interface, whatever the team is comfortable touching day to day. The versioning and the change history aren't.

## Add new questions below as they come up

*(next entry goes here)*
