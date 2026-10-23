---
title: Probability and Statistics I Question Bank
type: note
topic: teaching
created: 2026-09-25
tags: [ta, teaching, probability, statistics]
---
# Probability and Statistics I — Question Bank

> [!NOTE]
> Three kinds per topic: **Recap** (first 5 minutes, cold-called, ungraded) · **Exercise** (their turn, in-section) · **Exam-style**.
> Companions: [Probability and Statistics I Sections](../notes/section-plan.md) · [Probability and Statistics I Playbook](../notes/teaching-playbook.md) · the general teaching playbook (local reference).

## Contents
- [How to use this](#how-to-use-this)
- [Describing data](#describing-data)
- [Counting](#counting)
- [Axioms](#axioms)
- [Conditional and independence](#conditional-and-independence)
- [Bayes](#bayes)
- [Discrete random variables](#discrete-random-variables)
- [Expectation and variance](#expectation-and-variance)
- [Named distributions](#named-distributions)
- [Continuous and normal](#continuous-and-normal)
- [Joint distributions](#joint-distributions)
- [Sampling and the CLT](#sampling-and-the-clt)
- [Estimation and testing](#estimation-and-testing)
- [Name the distribution drill](#name-the-distribution-drill)
- [Find the flaw](#find-the-flaw)

-----

## How to use this

- Pick **three** recap questions the night before and write them down.
- Every exercise answer must arrive with the three steps (experiment, random variable in words with units, distribution + assumption). No bare numbers accepted, from week one.
- The **name the distribution drill** is the highest-value five minutes in this course — run it weekly once S08 has landed.
- Anything missed twice becomes a row in the misconception log in the general teaching playbook (local reference).

-----

## Describing data

**Recap**
1. Which is more affected by an outlier, mean or median?
2. Why do we divide by n − 1 for a sample?
3. Units of variance vs standard deviation?
4. Can SD be negative?
5. Two datasets, same mean — must they look alike?

**Exercise**
1. Mean, median, mode, variance, SD of `{2, 4, 4, 5, 10}` by hand.
2. Add the value 100 and recompute; state which statistic moved most and why.
3. Sketch a histogram and boxplot of the same data; say which question each answers better.

**Exam-style**
1. Given salary data, choose a summary statistic for a report and justify it in one sentence.
2. Two groups with equal means, different SDs — what would you tell a decision-maker?
3. Derive `Var(X) = E[X²] − (E[X])²` for a small dataset numerically.

-----

## Counting

**Recap**
1. Order matters, no repetition → which?
2. `C(n, k)` in terms of `P(n, k)`?
3. How do you count "at least one"?
4. When is `P = favourable/total` valid?
5. `C(5,2)` = ?

**Exercise**
1. From 10 people: a committee of 4; then president/VP/secretary. Which formula each, and why?
2. Probability a 5-card hand contains at least one ace — by the complement.
3. Count 4-digit PINs with no repeated digit.

**Exam-style**
1. Probability that two of 25 people share a birthday (setup + why the complement).
2. Distribute 10 identical prizes among 4 children.
3. A committee of 5 from 6 men and 4 women with at least 2 women — two ways, answers must agree.

-----

## Axioms

**Recap**
1. The three axioms, in your own words.
2. Addition rule for two events?
3. Mutually exclusive means what — and does it imply independent?
4. `P(Aᶜ)` = ?
5. Can `P(A∩B)` exceed `P(A)`?

**Exercise**
1. Given `P(A) = 0.5, P(B) = 0.4, P(A∩B) = 0.2`: find `P(A∪B)`, `P(Aᶜ)`, `P(A∩Bᶜ)`.
2. Probability of at least one six in four dice rolls.
3. Show that two mutually exclusive events with nonzero probability cannot be independent.

**Exam-style**
1. Three events with given pairwise overlaps — find `P(A∪B∪C)` by inclusion–exclusion.
2. A student claims `P(A∪B) = 1.2`. Diagnose the error without seeing the work.
3. Derive the complement rule from the axioms.

-----

## Conditional and independence

**Recap**
1. Definition of `P(A|B)`.
2. Does conditioning grow or shrink the sample space?
3. Independence test?
4. Along a tree branch — multiply or add?
5. Does replacement change independence?

**Exercise**
1. Two cards drawn without replacement: `P(both aces)`. Then with replacement; compare.
2. From a given contingency table: compute `P(A|B)` and `P(B|A)` and comment on the difference.
3. Verify or refute independence from that same table.

**Exam-style**
1. A two-stage machine problem; find the probability of a defect and then the probability it came from line 1.
2. Show that independence of A and B implies independence of A and Bᶜ.
3. A tree-diagram problem where the second stage's probabilities depend on the first.

-----

## Bayes

**Recap**
1. What is the prior?
2. What goes in Bayes' denominator?
3. If a test is 99% accurate and the disease is rare, is a positive result probably true?
4. `P(A|B)` vs `P(B|A)` — which does a test's "accuracy" describe?
5. Posterior means what?

**Exercise**
1. Disease prevalence 1%, sensitivity 99%, specificity 95%: find `P(disease | positive)` — with a counts table out of 100,000 first, then the formula.
2. Repeat with prevalence 20% and comment on what moved.
3. Two factories with different defect rates; given a defective item, find the probability of each source.

**Exam-style**
1. A spam-filter problem with three categories, using the law of total probability.
2. Sequential updating: a second independent positive test; find the new posterior.
3. Explain to a non-statistician, in three sentences, why a positive result from a very accurate test can still probably be wrong.

-----

## Discrete random variables

**Recap**
1. What is a random variable, formally?
2. Two requirements of a PMF?
3. What does the CDF at x give?
4. Is `P(X = 3)` ever the same as `P(X ≤ 3)`?
5. Shape of a discrete CDF?

**Exercise**
1. Build the PMF of the sum of two fair dice; verify it sums to 1; sketch it.
2. From it: `P(X > 9)`, `P(4 ≤ X ≤ 6)`, `P(X = 7)`.
3. Sketch the CDF and read `P(X ≤ 5)` off it.

**Exam-style**
1. A PMF given with an unknown constant k — find k, then compute two probabilities.
2. Given a CDF, recover the PMF.
3. Define a random variable for a described experiment, give its PMF, and justify each value.

-----

## Expectation and variance

**Recap**
1. `E[X]` in words?
2. `E[aX + b]` = ?
3. `Var(aX + b)` = ?
4. Computational form of variance?
5. When does `Var(X + Y) = Var(X) + Var(Y)`?

**Exercise**
1. E and Var for a 4-value PMF.
2. Then for `Y = 3X − 2`, both from the rules and by rebuilding the PMF — answers must agree.
3. A game costs 2 to play and pays according to a die; is it worth playing? Answer with `E` and a sentence.

**Exam-style**
1. Expected value of an insurance policy, with a recommendation in words.
2. Show `E[X²] ≥ (E[X])²` and say what the gap is.
3. Two dependent variables: compute `Var(X + Y)` and identify the extra term.

-----

## Named distributions

**Recap**
1. Binomial assumptions — all four.
2. With vs without replacement → which pair of models?
3. What does the Poisson λ represent, and what must match it?
4. Geometric counts what?
5. Mean and variance of a binomial?

**Exercise**
1. 20 items, 5% defective: `P(exactly 2 defective)`; name the model and the assumption.
2. The same, but drawing 20 from a box of 50 with 5 known defectives — which model now, and why?
3. Calls arrive at 3 per hour: `P(exactly 5 in two hours)`; watch λ.
4. `P(first success on the 4th trial)` with p = 0.3.

**Exam-style**
1. One story, two readings — argue for binomial and for hypergeometric, and say what makes one right.
2. Show numerically that a binomial with large n and small p is close to a Poisson.
3. Choose a distribution for a described quality-control process, state the assumption you accept, compute one probability, and sanity-check it.

-----

## Continuous and normal

**Recap**
1. `P(X = 5)` for a continuous variable?
2. Can a density exceed 1?
3. `z = ?`
4. `P(X > a)` from a table of `P(X ≤ a)`?
5. Roughly what fraction lies within 2σ?

**Exercise**
1. Heights `N(170, 8²)`: `P(X > 180)`, `P(165 < X < 175)` — each with a shaded sketch.
2. Find the cutoff for the top 10% (the reverse lookup).
3. A uniform density on `[2, 6]`: verify total area 1, then find `P(X > 5)`.

**Exam-style**
1. A two-sided symmetric interval containing 95% of the distribution; find both endpoints.
2. Two normal populations with different σ; compare the probability of exceeding one threshold and interpret.
3. Why can we use the normal for a *sum* of many small effects?

-----

## Joint distributions

**Recap**
1. How do you get a marginal from a joint table?
2. Independence test on a joint table?
3. Does zero covariance imply independence?
4. Range of the correlation coefficient?
5. What does a conditional distribution require after fixing a row?

**Exercise**
1. From a 3×3 joint table: both marginals, `P(X = 1 | Y = 2)`, and an independence verdict with justification.
2. Covariance and correlation for that table.
3. Construct a pair with zero covariance that is clearly dependent.

**Exam-style**
1. Compute `Var(X + Y)` from a joint table and identify the covariance contribution.
2. Given marginals only, say what you can and cannot conclude about the joint.
3. Interpret a correlation of −0.8 in the problem's own words, and state what it does *not* say.

-----

## Sampling and the CLT

**Recap**
1. Is x̄ a constant or a random variable?
2. `E[x̄]` = ?
3. Standard error of the mean?
4. To halve the SE, what must n do?
5. Does the CLT require a normal population?

**Exercise**
1. `σ = 10`, `n = 25`: SE, then `P(x̄ > 52)` with `μ = 50`.
2. Repeat with `n = 100`; state what changed and why.
3. Explain in two sentences why the histogram of sample means is narrower than the population.

**Exam-style**
1. A skewed population: justify using the normal for x̄ and state the condition you rely on.
2. Find the n needed so that x̄ is within 1 unit of μ with 95% probability.
3. A student used σ instead of σ/√n. Say what their answer over- or under-states, and why.

-----

## Estimation and testing

**Recap**
1. What is random in a confidence interval — the interval or the parameter?
2. The correct interpretation sentence for 95% confidence?
3. What happens to the width if confidence rises to 99%?
4. A p-value is the probability of what, given what?
5. Do we ever prove H₀?

**Exercise**
1. Build a 95% CI for μ from given x̄, σ, n; then write the interpretation sentence.
2. Recompute at 99% and with 4n; explain both movements.
3. A one-sample test at α = 0.05: state H₀ and H₁, compute the statistic, decide, and **write the conclusion in the problem's own words**.

**Exam-style**
1. Given a p-value of 0.03 at α = 0.01, state the decision and explain it to a non-statistician.
2. A report claims "95% probability μ is in [4.2, 5.1]." Correct the statement and explain why it matters.
3. Same data, one-tailed vs two-tailed: which is legitimate here, and why must that be decided before seeing the data?

-----

## Name the distribution drill

Ten stories, 10 seconds each, they call out the model **and the assumption**. Highest-value five minutes in the course after S08.

1. Defective items in a batch of 50 drawn from a large shipment.
2. Defective items in 5 drawn from a box of 20 with 3 defectives.
3. Typos per page.
4. Number of calls until the first complaint.
5. One coin flip.
6. Bus arrival time, equally likely in a 10-minute window.
7. Heights of adult men.
8. Time until the next arrival, constant rate.
9. Average of 100 measurements from a skewed population.
10. Number of heads in 10 flips of a bent coin with known p.

-----

## Find the flaw

The following statements are deliberately flawed. Identify and correct each mistake.

Projected on screen, 60 seconds each, hands down until time is up.

**F1** — "The coin landed heads five times in a row, so tails is now more likely."

**F2** — "`P(A) = 0.6`, `P(B) = 0.5`, so `P(A∪B) = 1.1`."

**F3** — "The test is 99% accurate and I tested positive, so I am 99% likely to have the disease."

**F4** — "A and B cannot both happen, so they are independent."

**F5** — "The expected value of the die is 3.5, so I expect to roll 3.5."

**F6** — "`Var(2X + 5) = 2Var(X) + 5`."

**F7** — "We're drawing 10 items from a box of 15 without replacement, so it's binomial with n = 10."

**F8** — "`P(x̄ > 52)` with `σ = 10` and `n = 25`: `z = (52 − 50)/10 = 0.2`."

**F9** — "The correlation is 0, so the two variables have nothing to do with each other."

**F10** — "The 95% CI is [4.2, 5.1], so there's a 95% chance μ is between 4.2 and 5.1."

**F11** — "p = 0.2 > 0.05, so we accept H₀ and conclude the means are equal."

-----
