---
title: PS S10 — Joint distributions and covariance
type: note
topic: teaching
subject: Probability and Statistics I
section: S10
created: 2026-09-25
tags: [ta, teaching, section, probability, statistics]
---
# S10 — Joint distributions and covariance

> [!NOTE]
> Probability and Statistics I, section 10. Index: [Probability and Statistics I Sections](../section-plan.md) · questions: [Probability and Statistics I Question Bank](../../practice/question-bank.md) · teaching notes: [Probability and Statistics I Playbook](../teaching-playbook.md).

**One idea to land:** marginals come from **summing the other variable away**; covariance measures joint movement, and **zero covariance is not independence**.

**Board:**
1. A joint PMF as a table. Compute both marginals by summing rows and columns — literally, with a pen, in the margins. That is where the name comes from and it makes the idea stick.
2. Conditional distribution from the table: fix a row, renormalise it.
3. Independence tested cell by cell (`p(x,y) = p(x)p(y)` for **every** cell, not one).
4. Covariance, then correlation as its scale-free version, with the −1..1 range and what the sign means.
5. A concrete pair with zero covariance and obvious dependence — the counterexample that prevents a whole class of exam errors.

**They solve:** from a given joint table: marginals, one conditional, independence verdict with justification, covariance and correlation.

**Mistakes I expect:** checking independence on one cell; confusing conditional with joint; forgetting to renormalise a conditional; reading "correlation 0" as "unrelated"; correlation outside [−1, 1] and no sanity check.

-----
[← S09](09-continuous-random-variables-and-the-normal.md) · [All sections](../section-plan.md) · [S11 →](11-sampling-distributions-and-the-clt.md)
