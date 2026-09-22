<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each substudy define the log-odds treatment effect

$$
d_j=\theta_{1j}
=\operatorname{logit}(p_{j1})-\operatorname{logit}(p_{j0}).
$$

The normal random-effects log-likelihood, up to an additive constant, is

$$
\ell(\mu,\sigma^2)
=-\frac J2\log\sigma^2
-\frac1{2\sigma^2}\sum_{j=1}^J(d_j-\mu)^2.
$$

Its [score equations](../../../../../../../score-equation.md) give

$$
\widehat\mu=\frac1J\sum_{j=1}^Jd_j,
\qquad
\widehat\sigma^2=\frac1J\sum_{j=1}^J(d_j-\widehat\mu)^2.
$$

These are the [maximum-likelihood estimators](../../../../../../../maximum-likelihood-estimator.md) rather than the unbiased sample-variance estimator. At an interior solution with $\widehat\sigma^2>0$, the Hessian in $(\mu,\sigma^2)$ is negative definite, which is the required second-order condition.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
