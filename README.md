# Portfolio

This is the repo I pull from when I need to show a prospect or a colleague how I actually build, not just what I've argued for on LinkedIn.

## Why this exists

Anyone can write a case study. A case study proves you can narrate a system after the fact. It doesn't prove you can build one. This repo is organized around proof instead: real architecture, running on synthetic data, that a prospect can click through live on a call and a technical colleague can inspect line by line.

## How it's organized

The unit here is the problem pattern, not the client. A client engagement is one instance of a pattern I've solved more than once or expect to solve again. Organizing by client means rebuilding the same demo every time a new prospect has the same problem. Organizing by pattern means I build it once and it pays out three times: proof for prospects, a live tool I pull up mid-pitch, and the starting point I actually build from once the deal closes.

Each pattern folder holds:

- **`README.md`** — the problem this pattern solves, generalized to the shape a prospect would recognize, and the architecture decision behind it.
- **`repository/`** — the actual context files the system runs on: ICP, personas, positioning, signal library, competitor radar, and a change history that logs how the repository evolved based on real performance data. This is the proof that it's a system and not a mockup.
- **`demo/`** *(added as each pattern gets built out)* — a working interactive artifact that reproduces the real mechanics on synthetic data.
- **`results.md`** *(added once a pattern has real deployment history)* — outcomes tied to pipeline, reply rate, meeting rate, or revenue, anonymized enough not to breach confidentiality, specific enough to be evidence.

## Why the data is fake

Client work can't be shown as the literal artifact. The demo has to be a rebuilt, genericized version using synthetic data that proves the same mechanic without exposing a client's actual system. The synthetic data is built industry-flavored per pattern rather than generic, so a prospect can still see their own situation in it.

## Using this in a live pitch

`pitch-guide.md` is the call script: which spoke to pick based on what the prospect told you was broken, the order to walk through the repository and the before/after toggle, and how to preempt the "is this data even real" objection before it's asked. Read it before the call, not during it.

## Current patterns

- **`01-compounding-gtm-system/`** — the repository-and-loop architecture: why static ICP filters can't compound, and what a system that gets smarter every cycle looks like instead. In progress.
