---
title: PS S07 — Expectation and variance
type: note
topic: teaching
subject: Probability and Statistics I
section: S07
created: 2026-09-25
tags: [ta, teaching, section, probability, statistics]
---
# S07 — Expectation and variance

> [!NOTE]
> Probability and Statistics I, section 07. Index: [Probability and Statistics I Sections](../section-plan.md) · questions: [Probability and Statistics I Question Bank](../../practice/question-bank.md) · teaching notes: [Probability and Statistics I Playbook](../teaching-playbook.md).

**One idea to land:** expectation is a **weighted average, not a prediction** — and linearity is the most useful fact in the course.

**Board:**
1. `E[X] = Σ x·p(x)` computed on the two-dice sum PMF; then note that 7 is expected and never "typical" of a single roll.
2. Linearity: `E[aX + b] = aE[X] + b`, and `Var(aX + b) = a²Var(X)` — the missing `b` in the variance is the lesson; ask why before telling them.
3. `Var(X) = E[X²] − (E[X])²`, derived, and immediately used because it is the computational form.
4. Variance of a sum: additive **only** under independence. Say the condition every time.
5. Expected value of a game: is it worth playing? A real decision makes the abstraction stick.

**They solve:** E and Var of a small PMF; then of a linear transform; then of a simple bet, with a recommendation in words.

**Mistakes I expect:** forgetting to square the constant in variance; adding a constant to the variance; treating E[X] as the most likely value; adding variances of dependent variables; `E[X²] ≠ (E[X])²` confusion.

-----
[← S06](06-discrete-random-variables.md) · [All sections](../section-plan.md) · [S08 →](08-named-discrete-distributions.md)
