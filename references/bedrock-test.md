# Bedrock test

A statement qualifies as a **first principle** only if it passes all three checks.

| Check | Question | Fails when |
|---|---|---|
| Verifiable | Can I point to evidence, a measurement, or a proof? | It's repeated opinion, "everyone knows", or an authority claim |
| Irreducible | Does asking "why?" again reveal something deeper I can still use? | It is itself a conclusion built on other assumptions |
| Convention-independent | Is it still true if all habits, norms and tools are thrown out? | It depends on how things are currently done |

## Verdicts

- **Principle** — passes all three. Record confidence: high (proof or direct measurement), medium (strong
  indirect evidence), low (plausible, not yet checked).
- **Hypothesis** — plausible but not verified. May be used, but every conclusion that depends on it
  inherits the flag.
- **Discarded** — habit, preference, or inherited shape with no support.

## Examples of the difference

| Looks fundamental | Actually | Bedrock underneath |
|---|---|---|
| "Batteries are expensive" | Market price (convention) | Cost of the raw materials on the commodity market |
| "We need a weekly report" | Habit | The decision that report supports, and how often it is actually made |
| "Customers want feature X" | Inference | What customers do (observed behavior) when they hit the problem |
| "This must run on a microservice architecture" | Inherited shape | Required scale, team boundaries and deployment constraints |

## When the test does not fit

- **Empirical regularities** (e.g. induced demand, tail-latency amplification): not provable from a law, but
  they can still be *well established*. Label them "empirical, widely observed — check it applies here" and
  state what would show it doesn't.
- **Recalled numbers or "laws"** from memory: mark them *recalled*, not *verified*.
- **Values** ("what disparity is acceptable?"): they are not verifiable and can't be derived from facts.
  Don't promote them to principles. The "bedrock" of a value is **the choice the person or body must make**:
  name the value, make the trade-off concrete ("which error would you accept?"), and state what follows from
  each choice. That is more useful than just handing it back. See `values.md`.
- **Feelings and relationships:** apply the test to needs, interests and decision rules, not to feelings.
- **No evidence at all:** nothing can honestly pass the test. Use a diagnostic tree instead.

## Common mistakes

- Stopping at the first satisfying "why" — keep going until you hit a law, a measurement, a requirement
  with an owner, or an honest "unknown".
- Treating the opposite of a convention as a principle. Rejecting a norm proves nothing by itself.
- Counting a law of the *domain* as a law of *nature* (regulations and contracts are real requirements, not
  physics — they can sometimes be renegotiated, but at a cost).
