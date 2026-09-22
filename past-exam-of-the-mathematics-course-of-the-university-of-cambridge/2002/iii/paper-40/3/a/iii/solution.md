<h1 id="3/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Start with $v^{(0)}>0$ and any coefficient [vector](../../../../../../../vector.md). At sweep $m$, draw $a_k^{(m+1)}$ from the [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) above using $v^{(m)}$, then draw $v^{(m+1)}$ from the [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md) using the newly drawn coefficients. For the second step one may generate $1/v$ from a [gamma distribution](../../../../../../../gamma-distribution.md) with the same shape and rate equal to the displayed inverse-gamma scale.

Each block update uses an exact [conditional distribution](../../../../../../../conditional-distribution.md), so it preserves the joint [posterior distribution](../../../../../../../bayesian-posterior.md). The resulting pairs form a dependent [Gibbs sampler](../../../../../../../gibbs-sampler.md) sample. With proper priors, positive scale and positive-definite coefficient [covariance](../../../../../../../covariance.md), these conditionals have full [probability support](../../../../../../../support-of-a-probability-distribution.md) on $\mathbb R^{k+1}\times(0,\infty)$ and the usual posterior ergodicity applies. A burn-in reduces dependence on initialization; retained sweeps are still serially dependent and Monte Carlo errors should account for that dependence.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
