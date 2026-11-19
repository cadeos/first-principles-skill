# first-principles

A Claude skill for first principles thinking. It helps you take a problem or a decision apart: it names the frame the question arrives in, finds the assumptions it hides, separates what can be verified from what cannot, and rebuilds options from what survives.

## What it does

* **Triage.** Not every question deserves a deep analysis. The skill picks one of four depths: a one line answer when a single fact decides it, five lines, a standard pass of about a page, or a deep pass for irreversible decisions.
* **Two modes.** As an analyst it does the work and delivers a report that opens with "What this changes". As a coach it asks one question per message and closes in plain prose, never with a template.
* **Seven moves.** Name the frame, decompose the given number, find the load bearing assumptions, climb the ladder of whys, separate facts from values, rebuild from the surviving options, attack the result with a falsifier.
* **Bedrock test.** A claim counts as a first principle only if it is verifiable, irreducible and independent of convention.
* **No evidence, no pretending.** When data is missing it says so and builds a diagnostic tree: for each hypothesis, the cheapest observation that would tell it apart.
* **Values protocol.** On moral, political or cultural questions it grades the factual claims of each side, states the strongest version of each position, finds the crux and checks its own neutrality by swapping sides. The weighing of values stays with you.

## Install

Clone the repository into your Claude skills folder:

```bash
git clone https://github.com/cadeos/first-principles-skill ~/.claude/skills/first-principles
```

Start a new Claude Code session and ask Claude to look at a problem from first principles ("why do we do it this way?", "challenge my assumptions", "da zero").

## Files

* `SKILL.md`: the triage, the modes and the seven moves.
* `references/questions.md`: question banks for each move.
* `references/bedrock-test.md`: when a claim may be called a first principle.
* `references/pitfalls.md`: the usual ways the method goes wrong.
* `references/report-template.md`: report shapes for each depth.
* `references/values.md`: the protocol for contested questions.

## Background

The story behind the skill, with examples from Plato to the Wright brothers: *First Principles Thinking and a Skill to Use It* (Medium).
