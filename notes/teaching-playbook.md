---
title: Probability and Statistics I Playbook
type: note
topic: teaching
created: 2026-09-25
tags: [ta, teaching, probability, statistics]
---
# Probability and Statistics I — Playbook delta

> [!NOTE]
> The universal TA method lives in the general teaching playbook (local reference). This file is only what is **different about this subject**.

## What makes this subject hard for them

**Intuition that is confidently wrong.** In data structures a misconception produces a crash; here it produces a plausible number, and nothing pushes back. Their gambler's-fallacy instincts are older and louder than the axioms.

- **The arithmetic is easy; the modelling is the course.** Most lost marks are not computation — they are the wrong distribution, a forgotten independence assumption, or a misread question.
- **Notation is load-bearing and they treat it as decoration.** `P(A|B)` vs `P(B|A)` vs `P(A∩B)` — confusing these *is* the mistake, not a symptom of one.
- **Simulation beats argument.** When intuition and the axioms disagree, a 20-line simulation settles it in seconds and they believe it. I keep one ready.

## Section-specific moves

- **Three-step ritual, every single problem, all term:**
  1. What is the experiment / sample space?
  2. Define the random variable **in words, with units**: "let X = the number of defective items in a sample of 20."
  3. Name the distribution and *check its assumptions* before writing a formula.
  A student who does this cannot write `n` and `p` into the wrong model.
- **Draw before computing** — tree diagram, Venn, or number line for a continuous variable. Shade the region the question asks for. Most "which formula?" panic is a missing picture.
- **Sanity-check every answer aloud:** is it between 0 and 1? Does it exceed a probability it must be smaller than? Is a variance negative? Is the mean inside the range of the data?
- **Estimate before computing.** Guess the answer's order of magnitude first; it turns a wrong keystroke into a caught error.
- **Simulate the counter-intuitive ones** — Monty Hall, the birthday problem, base-rate/Bayes cases. Do not argue with intuition; outvote it with data.
- **Distinguish probability from statistics out loud.** First half: model known, predict data. Second half: data known, infer the model. Say which direction we are facing today.

## Grading, subject-specific

Use the 10-point rubric in the general teaching playbook (local reference), adapted:

- **Weight the setup as heavily as the answer.** A correct `Binomial(20, 0.05)` identification with a slipped arithmetic step deserves most of the marks; a right number from a wrong model deserves few.
- **Standing deductions, published:** no units or no definition of the random variable −1, an assumption (independence, identical distribution) used silently −1, a probability outside [0,1] left unremarked −1 (it means they never checked).
- **Interpretation is graded.** A confidence interval or p-value with no sentence in the problem's own language is incomplete — that sentence is the entire point of statistics.
- **Never give full marks for a bare number**, even a correct one, and say this in week one so it is a rule and not a surprise.

## The question I ask all term

> "What is the random variable, in words, with units — and what has to be true for this distribution to apply?"

If they can answer that, the formula sheet does the rest.

## Misconception log — seeded

Format and rules in the general teaching playbook (local reference). Add a row the same day it happens.

| Misconception | Where it shows up | The move that fixes it |
|---|---|---|
| "After five heads, tails is due" | S03 → S04 | simulate 10,000 flips and look at the runs |
| "Mutually exclusive means independent" | S03 | both definitions on the board, side by side |
| "`P(A\|B)` is `P(B\|A)`" | S04, S05 | the medical-test story where they differ hugely |
| "A 99% accurate test means 99% likely ill" | S05 | the counts table out of 100,000 |
| "`E[X]` is the outcome I should expect" | S07 | E = 3.5 on a die, which is unrollable |
| "`Var(aX + b) = aVar(X) + b`" | S07 | rebuild the PMF of the transform and compare |
| "Without replacement is still binomial" | S08 | the assumption checklist, read line by line |
| "Use σ for the sample mean" | S11 | the three-panel picture; SE = σ/√n |
| "Correlation 0 means unrelated" | S10 | a clearly dependent pair with zero covariance |
| "95% chance μ is in this interval" | S12 | the pinned interpretation sentence, both versions |
| "p > α means H₀ is true" | S12 | "fail to reject", plus one power example |

**The layer usually missing underneath:** the setup, not the arithmetic — no defined random variable, no stated assumption. Send them back to the three-step ritual.
