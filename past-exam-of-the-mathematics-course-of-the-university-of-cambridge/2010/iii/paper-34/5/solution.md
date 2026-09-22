<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the distinct observed event times $a_k$, let $i_k=\pi(a_k)$ and let $R_k$ be the [risk set](../../../../../risk-set.md) immediately before that event. The [Cox partial likelihood](../../../../../cox-partial-likelihood.md) is

$$
L_p(\beta)=\prod_{k=1}^d\frac{e^{\beta z_{i_k}}}{\sum_{i\in R_k}e^{\beta z_i}},\qquad
\ell_p(\beta)=\sum_{k=1}^d\left\{\beta z_{i_k}-\log S_0(a_k,\beta)\right\}.
$$

The different risk sets already incorporate each event and any intervening censoring. Differentiating this [log-likelihood](../../../../../log-likelihood.md) gives

$$
U(\beta)=\ell_p'(\beta)=\sum_{k=1}^d\left[z_{i_k}-\frac{S_1(a_k,\beta)}{S_0(a_k,\beta)}\right]
=\sum_{k=1}^d s(a_k,\beta).
$$

Therefore a finite interior [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) from the [Cox partial likelihood](../../../../../cox-partial-likelihood.md) satisfies the first-order condition

$$
\boxed{\sum_{k=1}^d s(a_k,\widehat\beta)=0.}
$$

Moreover

$$
-\ell_p''(\beta)=\sum_{k=1}^d\left[\frac{S_2(a_k,\beta)}{S_0(a_k,\beta)}-\left(\frac{S_1(a_k,\beta)}{S_0(a_k,\beta)}\right)^2\right]\geq0.
$$

Each summand is the conditional event-covariate [variance](../../../../../variance-split.md), so the [partial likelihood](../../../../../partial-likelihood.md) is log-concave. If some informative risk set has unequal covariates, the curvature is strictly negative and an existing finite root is the unique maximizer.

The finite-interior qualification is necessary. With two at-risk subjects having covariates zero and one, suppose the subject with covariate one is the sole observed event and the other is subsequently censored. Then $L_p(\beta)=e^\beta/(1+e^\beta)$ increases strictly and has its supremum only as $\beta\to+\infty$; the score $1/(1+e^\beta)$ has no finite zero. If every event risk set has identical covariates, the coefficient is instead unidentifiable and the score is identically zero. The displayed fitted-score equation applies to the regular case in which the proportional-hazards estimate is finite.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
