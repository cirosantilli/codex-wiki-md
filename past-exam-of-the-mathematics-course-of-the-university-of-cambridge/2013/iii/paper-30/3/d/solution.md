<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) retains the same conditional mean but permits

$$
E(Y_i\mid z_i)=\mu_i,\qquad \log\mu_i=\beta_0+\beta_1z_i,
\qquad \operatorname{Var}(Y_i\mid z_i)=\phi\mu_i.
$$

This is a mean–[variance function](../../../../../../variance-function.md) specification through [quasi-likelihood](../../../../../../quasi-likelihood.md); it does not assign a full [probability distribution](../../../../../../probability-distribution.md) to each count. For independent observations, the [quasi-score equation](../../../../../../quasi-score-equation.md) is proportional to $\sum_i x_i(Y_i-\mu_i)=0$, so the mean [statistical parameter](../../../../../../statistical-parameter.md) estimates equal those from [Poisson regression](../../../../../../poisson-regression.md). The output estimates $\widehat\phi=3.515351$ through the [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md), and inflates the [standard errors](../../../../../../standard-error.md) by approximately $\sqrt{\widehat\phi}=1.875$.

The large [residual deviance](../../../../../../residual-deviance.md) relative to 728 residual [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) also signals substantial [overdispersion](../../../../../../overdispersion.md). Daily weather, traffic and other omitted conditions may produce greater count variation than a homogeneous [Poisson distribution](../../../../../../poisson-distribution.md) allows. The [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) accounts for that extra marginal [variance](../../../../../../variance-split.md). It still requires a correct conditional mean and an appropriate independence assumption; a common [dispersion parameter](../../../../../../dispersion-parameter.md) alone does not repair [serial correlation](../../../../../../serial-correlation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
