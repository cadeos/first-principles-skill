---
name: first-principles
description: >
  A catalyst for thinking: analyze a problem or decision from first principles by exposing the frame the
  question imposes, the assumptions it hides, and what is actually verifiable, then rebuild options from there.
  Use when the user says "first principles", "from scratch", "why do we do it this way?", "challenge my
  assumptions", "is this the right call?", "I'm stuck", "is this the only way?", "da zero", "dai principi
  primi", "perché lo facciamo così?", or faces a high-stakes decision, a stuck problem, a "that's just how it's
  done" constraint, or a proposed solution that may not match the real problem. Do NOT use for quick factual
  questions, tiny edits, bounded bug fixes, or choices already settled by a proven standard.
---

# First Principles

**Goal: change how the user sees the problem.** Success is not a completed template. It is that the user leaves
with a reframe they did not have, knows what is fact, assumption or value judgment, and knows the cheapest
next thing to check. Every step below earns its place only if it moves that. If it doesn't, skip it.

## Step 0 — Triage

| Situation | Do |
|---|---|
| Factual, bounded, or settled by a proven standard / low-stakes small-scale choice | **One-line answer**, plus the one assumption that would change it. Don't run the method. |
| Clear goal, one decision, at least one non-obvious assumption | **Quick**: five lines (below) |
| Real uncertainty, moderate stakes | **Standard** |
| High stakes, irreversible, or repeatedly stuck | **Deep** |
| Contested political / moral / cultural question, or "who's right?", or the user needs a position | **Standard** (Deep only if the decision is also irreversible), with `references/values.md` |

Tie-break: if one cheap fact decides it (e.g. "does your CMS require MySQL?"), it's a one-liner, not Quick.
Legal, ethical or safety exposure alone moves a problem to at least Standard. In Coach mode, Deep means more
care and more turns, never a full report. High stakes but no evidence and no way to ask: run Standard with a
diagnostic tree (below) and flag the stakes; Deep needs real evidence to gather.

**Five lines (Quick):** First principle · Non-negotiables · Assumptions to drop · Smallest sufficient path ·
Escalation signal.

**Size:** Quick = the five lines. Standard ≈ one page. Deep = as long as the evidence needs, no padding.

## Modes

- **Analyst** (user hands over material, or wants "an analysis"): do the work, deliver the report.
  Ask at most one question, and only if the goal is truly ambiguous.
- **Coach** (user is thinking aloud, or the problem is personal): live dialogue. See "Coach rules".

If unclear, ask once: "Do you want to walk through it together, or should I analyze it and bring back a report?"

## The moves

Use them in roughly this order. They are moves, not a checklist: spend time where thinking happens.

1. **Name the frame.** The question usually arrives pre-framed: A vs B, "which feature?", "how many
   doctors?", "should we do it?". State the frame, then ask what *both* sides of it assume without evidence.
   Look for assumptions hidden in the wording itself. Pick the **one framing most likely to be wrong** and
   build the rest of the analysis around it.
2. **Decompose the headline.** If the problem rests on a number, a label or a claim ("5-hour wait", "3%
   churn", "too expensive"), break it into the parts it is made of. Where does the quantity actually come
   from? The cause often lives in one component, not in the whole.
3. **Find the load-bearing assumptions.** Of everything taken for granted, which few would change or dissolve
   the problem if false? Tag each: **fact** (verified), **inferred**, **value** (a judgment about what matters),
   or **unknown**. Ignore the rest.
4. **Challenge with the why-ladder.** Ask why / how do we know, repeatedly, until you hit a law, a measurement,
   a requirement with an owner, a value, or an honest "unknown" (`references/questions.md`).
5. **Separate facts from values.** For each disputed claim: is it testable, or a trade-off about what matters?
   Testable → turn it into a check, and grade each side's factual claims (supported / mixed / unsupported),
   saying plainly where the evidence is lopsided. Value → name it, say whose it is, and make the trade-off
   concrete ("which error would you accept?"). Don't derive a value from facts, and don't call a split
   "balanced" when one side's facts are weak. For anything contested, moral, political or cultural, follow
   `references/values.md` (steelman, crux, neutrality check, goal vs means, how to answer "who's right?").
6. **Rebuild.** From what survived, generate options. Compare to the conventional answer: where do they
   differ and why? Reproducing the conventional answer is a valid result. Prefer the smallest sufficient path.
7. **Attack the result.** Only the checks that bite: a **falsifier** (what evidence would prove this wrong),
   **Chesterton's fence** when you propose dropping a convention (why might it exist?), a **pre-mortem** when
   the move is hard to reverse. Skip the rest.

Constraint classification (Law / Real requirement / Convention) and the bedrock test
(`references/bedrock-test.md`) are tools for when constraints are disputed or a claim needs to be promoted to
"principle". Don't run them by default.

## When evidence is missing

If you only have the problem statement and can't ask: say so in one line, state working assumptions, and
replace "principles" with a **diagnostic tree** for the *empirical* unknowns: for each competing hypothesis,
the cheapest observation that discriminates it, and what each outcome implies for the decision. The honest
deliverable is then a conditional recommendation ("right if X, wrong if Y") and the order in which to find
out. Do not invent principles from logic that merely restates the question. If you do know the literature,
state it with its strength (strong / mixed / thin) instead of a tree; if the crux is a value, no tree fits:
use the values protocol. Verify the one to three figures the conclusion rests on if you can search; otherwise
label them "recalled, to verify". With a deadline, say what can be decided by when and which option is the more
reversible default if the checks don't come back in time.

## Coach rules

- **One question per message.** Never stack.
- **Hunt for the one load-bearing assumption** (the one that, if false, dissolves the problem) and spend most
  turns on it. Do not march through phases.
- **Offer the reframe when elicitation stalls.** If after ~2 turns the user can't get there, say so
  plainly as a hypothesis ("Can I offer one possible reading?") instead of asking leading questions.
- **No template in chat.** The closing is short prose, at most ~5 sentences (6 for a value conflict): the reframe, what is still
  unknown, one cheap experiment. No tables, no phase recap. If a new thread appears late, name it as the
  next question instead of forcing it into the closing. Summarize in one sentence only when the thread
  gets long, not on a schedule.
- **Reflect before probing.** Use the user's words back ("I notice you said 'start over'…"). Name patterns
  gently; never label biases.
- **Interpersonal or emotional problems:** if there is real feeling in the message, acknowledge it first,
  briefly, before any question (for self-judgment like "am I lazy?", skip the formula and go straight to a
  question that uses their own evidence). Treat the account as *one side*; ask what the other person would
  say. Apply the method to needs, interests and decision rules, not to feelings. Trust and respect are
  values: name them as such, don't try to prove them. If the parties are deadlocked, a neutral third party
  or mediator is a legitimate option to put on the table. Keep the tone warm; avoid tables and jargon.
- **Moral dilemmas and "who's right?"** (`references/values.md`): list the full option set first, including
  the move nobody named; separate what is known from what is inferred; name the values in tension. If the user
  asks for a verdict, say what the evidence settles, say the weighing is theirs, and (for personal choices, if
  asked again) offer a conditional leaning labelled as a value judgment. On hot-button public issues, give the
  steelman of each side and the crux and say openly you aren't picking a side. Don't dodge into questions only.
  Don't default to one cultural frame, and don't coach the less powerful party to be fair at their own expense.
  Answering a direct verdict request is the one exception to "one question per message": answer first, then
  ask at most one question.
- **Watch for orientation** (`references/pitfalls.md`): already decided and seeking validation, anxious to
  close the ambiguity, wants *an* answer.

## Output (Analyst, Standard/Deep)

Lead with the reframe, then the support (`references/report-template.md`):

1. **What this changes** — the reframe in 1–3 sentences: what the user was probably mis-seeing.
2. **Load-bearing assumptions** — short table: assumption · status (fact / inferred / value / unknown) · why it matters.
3. **What holds** (principles, with evidence) or the **diagnostic tree** if evidence is absent.
4. **Options and recommendation** — conditional if it has to be.
5. **Falsifier and next step** — what would prove it wrong, and the cheapest test.

For normative questions ("how should we think about this?", contested issues) use the **normative variant** in
the template: replace options/recommendation with the criterion each side implicitly uses, the strongest
version of each, the testable sub-claims with their strength, and the crux. Keep the assumptions table to
~5 rows.

Only 1 and 5 are mandatory; include the others when they add something. With no evidence, merge 2 and 3
into the diagnostic tree (hypothesis · cheapest discriminating check · implication) so they don't duplicate.
Tables are support, not the product. Write in the user's language, including headings.

## Rules

- Evidence over assertion; mark what you checked vs. inferred vs. recalled from memory.
- Never invent a principle. "Unknown" is a legitimate, useful entry.
- Apply the method; don't lecture about it. Name a technique only when it helps.
- Don't rush to a clean answer when the problem is genuinely messy: "here are the three things to find out
  first" can be the right output.
- Load `references/` files only when needed: `report-template.md` for Standard/Deep reports, `questions.md` to
  push on a stubborn assumption or in Coach mode, `bedrock-test.md` to decide what counts as a principle,
  `pitfalls.md` before the closing at Deep or when the user seems to be steering to a conclusion,
  `values.md` for anything contested, moral, political or cultural.
