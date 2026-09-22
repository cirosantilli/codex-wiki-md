<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Integrating the conditional mean in the [gamma random-intercept Poisson model](../../../../../../gamma-random-intercept-poisson-model.md) gives

$$
\mathbb E(Y_{ij}\mid x_{ij})
=\mathbb E(e^{b_i})\exp(\beta_0+\beta^{\mathsf T}x_{ij})
=\tau\exp(\beta_0+\beta^{\mathsf T}x_{ij}),
$$

and hence

$$
\boxed{\log\mathbb E(Y_{ij}\mid x_{ij})
=(\beta_0+\log\tau)+\beta^{\mathsf T}x_{ij}}.
$$

The marginal model's logarithmic mean family is therefore correctly specified, with a shifted intercept and identical slopes. Under the usual [independent](../../../../../../independent-random-variables.md)-cluster and estimating-equation regularity conditions, fitting that marginal mean consistently estimates

$$
\boxed{\beta_{0,\mathrm{marginal}}=\beta_0+\log\tau,
\qquad\beta_{\mathrm{marginal}}=\beta}.
$$

Thus the treatment and other slopes estimate the intended marginal log [rate ratios](../../../../../../rate-ratio.md); indeed they also coincide with the conditional slopes under the stated common random-effect distribution. The intercept consistently estimates the marginal baseline, but not the conditional $b_i=0$ intercept unless $\tau=1$. If the first investigator interprets the intercept as a conditional latent-student baseline without recognizing this shift, that interpretation is incorrect.

The assumed Poisson marginal [variance](../../../../../../variance-split.md) and constant correlation generally fail under this random-effect law. They need not invalidate mean-coefficient consistency for a suitable [generalized estimating equation](../../../../../../generalized-estimating-equation.md), because the expected residual vector is still zero at the true marginal mean. They do invalidate naive [standard errors](../../../../../../standard-error.md) based only on that assumed [covariance](../../../../../../covariance.md); robust inference requires the correction in part (iv). The simple unchanged-slope result relies on the random multiplier distribution not changing with covariates, rather than on a universal equivalence of marginal and conditional regression models.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
