<h1 id="26k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) $\hat\theta_n$ is a measurable maximizer of $\ell_n(\theta)=\sum_i\log f(X_i,\theta)$ over $\Theta$. Under identifiability, consistency conditions, an interior true parameter, sufficient differentiability and finite positive [Fisher information](../../../../../../fisher-information-matrix.md), the standard [limits](../../../../../../limit-of-a-function.md) are

$$
\boxed{\hat\theta_n\xrightarrow{\mathbb P}\theta_0,\qquad
 \sqrt n(\hat\theta_n-\theta_0)\xrightarrow{d}\mathcal N(0,I(\theta_0)^{-1}).}
$$

The [variance](../../../../../../variance-split.md) in the [normal distribution](../../../../../../normal-distribution.md) is the reciprocal of the per-observation [Fisher information](../../../../../../fisher-information-matrix.md), not of $nI$. Strong consistency needs additional hypotheses if it is to replace [convergence in probability](../../../../../../convergence-in-probability.md); the regular asymptotic result stated here does not require claiming it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
