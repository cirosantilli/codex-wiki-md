<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) is $\widehat\phi=3.099079$, well above the Poisson value one. A [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) retains the logarithmic mean model but uses

$$
\mathbb E Y_i=\mu_i,\qquad\operatorname{Var}(Y_i)=\phi\mu_i,\qquad
\log\mu_i=\beta_0+\beta_aa_i.
$$

This is a [quasi-likelihood](../../../../../../quasi-likelihood.md) specification; it does not by itself identify a count probability distribution. For a common $\phi$, the [quasi-score equation](../../../../../../quasi-score-equation.md) is the Poisson score divided by $\phi$, so its roots and fitted means are unchanged. Thus

$$
\boxed{\widehat\mu(a)=e^{3.24926+0.01898a},\qquad
\widehat{\operatorname{Var}}(Y\mid a)=3.099079\,\widehat\mu(a).}
$$

Coefficient [standard errors](../../../../../../standard-error.md) are multiplied by $\sqrt{\widehat\phi}$. The altitude [standard error](../../../../../../standard-error.md) becomes $0.00447\sqrt{3.099079}\approx0.0078691$, giving the requested approximate normal [confidence interval](../../../../../../confidence-interval.md)

$$
\boxed{0.01898\pm1.96(0.0078691)=(0.003557,\,0.034403).}
$$

It excludes zero, so **retain altitude on this approximate 5% test**. Its test statistic is about $2.412$ after allowing for [overdispersion](../../../../../../overdispersion.md), rather than the Poisson value $4.245$. Rescaling uncertainty cannot repair a systematically misspecified mean; the diagnostics in part (e) motivate reconsidering that mean as well.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
