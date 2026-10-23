---
title: PS S08 — Named discrete distributions
type: note
topic: teaching
subject: Probability and Statistics I
section: S08
created: 2026-09-25
tags: [ta, teaching, section, probability, statistics]
---
# S08 — Named discrete distributions

> [!NOTE]
> Probability and Statistics I, section 08. Index: [Probability and Statistics I Sections](../section-plan.md) · questions: [Probability and Statistics I Question Bank](../../practice/question-bank.md) · teaching notes: [Probability and Statistics I Playbook](../teaching-playbook.md).

**One idea to land:** the distribution is chosen by **checking assumptions against the story**, not by pattern-matching on numbers.

**Board — an assumption checklist per distribution, in this fixed format:**

| Distribution | The story | Must be true | Parameters |
|---|---|---|---|
| Bernoulli | one trial, success/failure | — | p |
| Binomial | count of successes in n trials | fixed n, independent, constant p | n, p |
| Geometric | trials until the first success | independent, constant p | p |
| Poisson | count of events in an interval | independent, constant rate | λ |
| Hypergeometric | count of successes, drawn *without* replacement | finite population, no replacement | N, K, n |

1. Two stories that differ only by "with replacement" → binomial vs hypergeometric. This is the discrimination exams love.
2. Poisson as the rare-event limit of the binomial, shown numerically rather than proved.
3. Mean and variance of each, in a table they build.

**They solve:** four stories, and for each they name the distribution **and the assumption they had to accept**, then compute one probability.

**Mistakes I expect:** binomial for sampling without replacement; mismatched λ and the interval length (per hour vs per day); geometric off-by-one on the counting convention; "independent" asserted with no justification.

-----
[← S07](07-expectation-and-variance.md) · [All sections](../section-plan.md) · [S09 →](09-continuous-random-variables-and-the-normal.md)
