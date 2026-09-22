<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The probability of no recovery through month $M$ is the product of the conditional survival probabilities, so

$$
\boxed{\gamma=1-\prod_{t=1}^M(1-q_t)}.
$$

Under [quadratic loss](../../../../../../bayes-estimator-under-squared-error-loss.md), the [Bayes estimator](../../../../../../bayes-estimator.md) is the posterior mean. Posterior independence and the mean of a [Beta distribution](../../../../../../beta-distribution.md) give

$$
\mathbb E[1-q_t\mid X]
=\frac{1+r_t-d_t}{T+1+r_t}.
$$

Consequently

$$
\boxed{
\widehat\gamma_B
=1-\prod_{t=1}^M
\frac{1+r_t-d_t}{T+1+r_t}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
