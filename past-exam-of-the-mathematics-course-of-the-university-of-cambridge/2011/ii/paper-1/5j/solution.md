<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Write $u(y,\theta)=\partial_\theta\log f(y,\theta)$ for the single-observation [score function](../../../../../informant-function.md). Differentiating the normalization of the [probability density function](../../../../../probability-density-function.md) gives

$$
\mathbb E_\theta[u(Y,\theta)]
=\int f(y,\theta)\partial_\theta\log f(y,\theta)\,dy
=\partial_\theta\int f(y,\theta)\,dy=0.
$$

For discrete observations, use a sum instead. The allowed interchange of differentiation and integration is the usual regular-model assumption with common support. Adding these identities gives $\mathbb E_\theta U_n=0$.

Let $p_\theta$ be the joint density. Because $T$ is an [unbiased estimator](../../../../../unbiased-estimator.md) with no explicit dependence on the parameter, differentiating $\mathbb E_\theta T=\theta$ gives

$$
1=\int T\,\partial_\theta p_\theta
=\mathbb E_\theta[TU_n]
=\operatorname{Cov}_\theta(T,U_n).
$$

The scores are [independent random variables](../../../../../independent-random-variables.md) with mean zero, so [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md) gives $\operatorname{Var}_\theta(U_n)=n\operatorname{Var}_\theta(U_1)$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) applied to the centred estimator and the score now gives the [Cramér-Rao lower bound](../../../../../cramer-rao-bound.md):

$$
\boxed{\operatorname{Var}_\theta(T)\geq\frac1{n\operatorname{Var}_\theta(U_1)}.}
$$

The denominator is the sample [Fisher information](../../../../../fisher-information-matrix.md). This bound concerns regular models with positive finite information; the preceding covariance identity explains why a small estimator variance requires a sufficiently informative score.

## ↑ Ancestors (11)

1. [5J](../5j.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
