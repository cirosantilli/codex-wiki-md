<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The multidimensional [Itô formula](../../../../../../ito-s-lemma.md) includes a mixed second derivative multiplied by the [quadratic covariation](../../../../../../quadratic-covariation.md), with no extra factor $1/2$. Here

$$
d[\sigma]_t=B(\sigma_t)^2dt,\qquad d[X]_t=\sigma_t^2dt,\qquad d[\sigma,X]_t=\rho\sigma_tB(\sigma_t)dt.
$$

Consequently the [Itô formula](../../../../../../ito-s-lemma.md) for $M_t=U(t,\sigma_t,X_t)$ has drift equal to the left side of the stated backward [partial differential equation](../../../../../../partial-differential-equation-split.md). That drift vanishes, leaving

$$
\boxed{dM_t=B(\sigma_t)U_\sigma(t,\sigma_t,X_t)dW_t^\sigma
+\sigma_tU_X(t,\sigma_t,X_t)dW_t^X.}
$$

A [stochastic integral](../../../../../../stochastic-integral.md) against [Brownian motion](../../../../../../brownian-motion-split.md) with locally square-integrable predictable integrand is a continuous [local martingale](../../../../../../local-martingale.md). The smoothness of $U$ and localization of the diffusion and its coefficients give this integrability on the model's lifetime. Thus $M$ is a [local martingale](../../../../../../local-martingale.md), as required. The [partial differential equation](../../../../../../partial-differential-equation-split.md) cancellation alone does not establish a true [martingale](../../../../../../martingale-split.md) or justify replacing $U$ by a terminal-payoff expectation without an additional integrability argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
