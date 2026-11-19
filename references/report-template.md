# Report template (Analyst mode, Standard / Deep)

Write it in the user's language, headings included. Aim for Standard ≈ one page. Tables are support: drop any
section that doesn't change the thinking. The reframe comes first. Mandatory: "What this changes" and
"Falsifier and next step". With no evidence, skip the assumptions table and "What holds": the diagnostic tree
replaces both.

```markdown
# <short title>

## What this changes
<1–3 sentences: the framing the user was probably mis-seeing, and what the question becomes instead.
Example: "'Hire 6 doctors?' may be the wrong question: the 5-hour wait may be an output problem (beds), not an
input problem (doctors). The question becomes: where in the journey does the time accumulate?">

## Load-bearing assumptions
| Assumption | Status (fact / inferred / value / unknown) | Why it matters |
|---|---|---|

**Key challenge:** the short why-chain that moved the most important one, e.g.
"Management needs it" → who reads it? → what decision follows? → none named → unknown.

## What holds        (use when there is evidence)
1. <principle> — basis: <measurement / law / requirement with an owner> — confidence: high/medium/low

## Diagnostic tree   (use INSTEAD when evidence is absent)
| Hypothesis | Cheapest observation that discriminates it | If true → decision implication |
|---|---|---|

## Facts vs values   (include when the question is partly normative)
- Testable: <claim → check>
- Value trade-off: <what each side prices, returned to the decision owner>

## Options and recommendation
- **Option A:** <...> — follows from <what holds>
- **Option B:** <...>
- **Conventional answer:** <...> — differs / matches because <...>
- **Recommendation:** <conditional if needed: "right if X, wrong if Y">

## Falsifier and next step
- I'm wrong if: <specific evidence>
- Cheapest next test: <one concrete step, owner if known>
- (Optional, only if they bite) Dropped convention and why it may have existed · Pre-mortem for irreversible moves
```

## Normative variant (contested, moral, political, cultural questions)

Use instead of "Options and recommendation". Keep "What this changes" first and "Falsifier and next step" last.
Skip the general assumptions table: the testable sub-claims table below replaces it. Keep each section to a few
lines; drop "whose standing is missing" or "if a decision is needed" when they add nothing.

```markdown
## The criterion each side uses
- Side A implicitly assumes: <criterion/value>   · Side B implicitly assumes: <criterion/value>

## Strongest honest version of each
- A: <...>   · B: <...>

## Testable sub-claims (with strength)
| Claim | Whose it supports | Evidence: supported / mixed / unsupported | Basis (recalled → to verify) |
|---|---|---|---|

## The crux
<the one factual or evaluative question that would move each side; for a value crux, a concrete trade-off
("which error would you accept?")>

## Whose standing is missing / conflicts of interest
<affected people not in the room; anyone judging their own case>

## If a decision is needed
<a rule you'd accept applied symmetrically to the opposing case; what can be decided by when; the more
reversible default>
```

If the user asked for an advocacy position: draft the strongest honest version and mark which lines rest on
values or contested facts. Do not hand down a personal verdict on hot-button issues; say openly that you aren't
choosing a side and why.

## Optional appendix: constraint classification
Only when constraints are disputed.
| Constraint | Law / Real requirement / Convention | Note |
|---|---|---|

## Five lines (Quick depth)
```
First principle:
Non-negotiables:
Assumptions to drop:
Smallest sufficient path:
Escalation signal:
```

## Coach-mode closing (chat, no template)
Short prose, 3–5 sentences: the reframe in the user's own words where possible, what is still unknown, and one
cheap experiment. No tables, no phase recap.
