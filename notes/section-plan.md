---
title: Probability and Statistics I Sections
type: note
topic: teaching
created: 2026-09-25
tags: [ta, teaching, probability, statistics]
---
# Probability and Statistics I — Sections

> [!NOTE]
> Delivery plan, one block per section: the idea to land, what goes on the board, the problem I work, what they solve, and the mistakes I know are coming.
> Companions: [Probability and Statistics I Playbook](teaching-playbook.md) · [Probability and Statistics I Question Bank](../practice/question-bank.md) · the general teaching playbook (local reference).

## Contents
- [How I run a section](#how-i-run-a-section)
- [Section map](#section-map)
- [S00 — The three-step ritual](sections/00-the-three-step-ritual.md)
- [S01 — Describing data](sections/01-describing-data.md)
- [S02 — Counting](sections/02-counting.md)
- [S03 — Probability axioms](sections/03-probability-axioms.md)
- [S04 — Conditional probability and independence](sections/04-conditional-probability-and-independence.md)
- [S05 — Bayes](sections/05-bayes.md)
- [S06 — Discrete random variables](sections/06-discrete-random-variables.md)
- [S07 — Expectation and variance](sections/07-expectation-and-variance.md)
- [S08 — Named discrete distributions](sections/08-named-discrete-distributions.md)
- [S09 — Continuous random variables and the normal](sections/09-continuous-random-variables-and-the-normal.md)
- [S10 — Joint distributions and covariance](sections/10-joint-distributions-and-covariance.md)
- [S11 — Sampling distributions and the CLT](sections/11-sampling-distributions-and-the-clt.md)
- [S12 — Estimation, confidence intervals, and a first test](sections/12-estimation-confidence-intervals-and-a-first-test.md)
- [Stretch and fallback per section](#stretch-and-fallback-per-section)
- [The distribution chooser](#the-distribution-chooser)
- [Prep checklist — the night before](#prep-checklist--the-night-before)
- [Reusable closing drills](#reusable-closing-drills)

-----

## How I run a section

| Time | Part | What I do |
|---|---|---|
| 0–5 | Recap | 3 questions on last section, cold-called, never graded |
| 5–15 | Board | The picture: tree, Venn, or shaded density — before any formula |
| 15–30 | I solve | One problem end to end, narrating the three-step ritual |
| 30–45 | They solve | A near-twin problem; I walk the room instead of talking |
| 45–50 | Close | The sanity check + what to read before next week |

Rules I hold myself to:
- **The three-step ritual is written on the board before every problem.** Experiment → random variable in words with units → distribution plus its assumptions.
- **Draw and shade first.** No formula until the region is on the board.
- **Sanity-check out loud**, every answer: in [0,1]? variance non-negative? mean inside the data range?
- **Let them be wrong out loud first** on the counter-intuitive ones, then simulate. Arguing with intuition loses; data wins.
- **Say the direction we face today:** model → data (probability), or data → model (statistics).

-----

## Section map

| # | Section | Board focus | They leave able to |
|---|---|---|---|
| [00](sections/00-the-three-step-ritual.md) | The ritual | experiment, RV, model | set a problem up before touching a formula |
| [01](sections/01-describing-data.md) | Describing data | mean vs median, spread | choose and defend a summary statistic |
| [02](sections/02-counting.md) | Counting | ordered? repetition? | count outcomes for equally-likely problems |
| [03](sections/03-probability-axioms.md) | Axioms | Venn, complement rule | use the addition rule and complements |
| [04](sections/04-conditional-probability-and-independence.md) | Conditional, independence | tree diagram | tell `P(A\|B)` from `P(B\|A)`; test independence |
| [05](sections/05-bayes.md) | Bayes | the two-column table | do a base-rate problem correctly |
| [06](sections/06-discrete-random-variables.md) | Discrete RVs | PMF and CDF plotted | build a PMF and check it sums to 1 |
| [07](sections/07-expectation-and-variance.md) | Expectation, variance | the linearity rules | compute E and Var, including of aX + b |
| [08](sections/08-named-discrete-distributions.md) | Named distributions | assumption checklists | pick the right distribution from a story |
| [09](sections/09-continuous-random-variables-and-the-normal.md) | Continuous, normal | area under a density | standardise and use the z-table both ways |
| [10](sections/10-joint-distributions-and-covariance.md) | Joint distributions | the joint table, margins | get marginals, covariance, correlation |
| [11](sections/11-sampling-distributions-and-the-clt.md) | Sampling, CLT | the distribution of x̄ | say why x̄ is normal-ish and with what SE |
| [12](sections/12-estimation-confidence-intervals-and-a-first-test.md) | Estimation, CI, testing | the interval and the tail | build a CI and interpret it in one sentence |

-----

## The sections

One file each — open the file for the section you are about to teach.

- **S00** — [The three-step ritual](sections/00-the-three-step-ritual.md)
- **S01** — [Describing data](sections/01-describing-data.md)
- **S02** — [Counting](sections/02-counting.md)
- **S03** — [Probability axioms](sections/03-probability-axioms.md)
- **S04** — [Conditional probability and independence](sections/04-conditional-probability-and-independence.md)
- **S05** — [Bayes](sections/05-bayes.md)
- **S06** — [Discrete random variables](sections/06-discrete-random-variables.md)
- **S07** — [Expectation and variance](sections/07-expectation-and-variance.md)
- **S08** — [Named discrete distributions](sections/08-named-discrete-distributions.md)
- **S09** — [Continuous random variables and the normal](sections/09-continuous-random-variables-and-the-normal.md)
- **S10** — [Joint distributions and covariance](sections/10-joint-distributions-and-covariance.md)
- **S11** — [Sampling distributions and the CLT](sections/11-sampling-distributions-and-the-clt.md)
- **S12** — [Estimation, confidence intervals, and a first test](sections/12-estimation-confidence-intervals-and-a-first-test.md)

-----

## Stretch and fallback per section

| # | If we are ahead | If we are behind |
|---|---|---|
| 01 | skewness; why the median is robust | mean vs median with one outlier |
| 02 | stars and bars; the birthday problem | the ordered/repetition decision |
| 03 | inclusion–exclusion on three events | addition rule with one overlap |
| 04 | Simpson's paradox | one tree diagram, both stages |
| 05 | sequential/repeated updating | the counts table, once |
| 06 | functions of a random variable | one PMF built and verified |
| 07 | moment generating functions (if in syllabus) | E and Var of one small PMF |
| 08 | Poisson as a binomial limit, numerically | binomial vs hypergeometric only |
| 09 | exponential; memorylessness | one z-table lookup each direction |
| 10 | covariance of a linear combination | marginals from a table |
| 11 | how large must n be, really? | the three-panel CLT picture |
| 12 | t-intervals when σ is unknown; Type I/II errors | one CI plus its interpretation sentence |

-----

## The distribution chooser

Built live with them in S08, reused in every later section, and the single most exam-relevant page in this file.

| The story says | Model | The assumption you are accepting |
|---|---|---|
| one trial, yes/no | Bernoulli | — |
| "how many successes in n tries" | Binomial | fixed n, independent trials, constant p |
| "how many tries until the first success" | Geometric | independent trials, constant p |
| "how many events per hour/page/km" | Poisson | independent events, constant rate |
| "drawn without replacement from a finite group" | Hypergeometric | population size matters |
| "equally likely over a range" | Uniform | no preference inside the range |
| "measurement, symmetric, bell-shaped" | Normal | μ and σ known or estimated |
| "time until the next event" | Exponential | constant rate, memoryless |
| "the mean of a sample" | Normal via CLT | n large enough, independent observations |

-----

## Prep checklist — the night before

- [ ] Solve the problems I am assigning, with the three-step ritual written out — my own setup must be exemplary on the board.
- [ ] Sketches prepared: which curve/tree/table goes where, so I do not run out of board mid-problem.
- [ ] The simulation ready to run if intuition fights back (Monty Hall, birthday, base rates, CLT).
- [ ] Table/calculator mechanics rehearsed — fumbling the z-table on screen costs credibility.
- [ ] Three recap questions written down.
- [ ] One sanity-check question per problem, prepared: "what must be true of this answer?"

-----

## Reusable closing drills

- "What is the random variable, in words, with units?"
- "Which distribution, and what assumption did you just accept?"
- "Is your answer between 0 and 1? Should it be bigger or smaller than the last one?"
- "`P(A|B)` or `P(B|A)` — which did the question ask for?"
- "σ or σ/√n?"
- "Now say the answer in the problem's own words, without symbols."
