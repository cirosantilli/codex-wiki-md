<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under a correctly specified [Poisson regression](../../../../../../poisson-regression.md) with adequate expected counts, the residual [Poisson deviance](../../../../../../poisson-deviance.md) is approximately [chi-squared distribution](../../../../../../chi-squared-distribution.md) with $n-p=107-5=102$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). The observed $D=319.86$ gives

$$
\boxed{\Pr(\chi^2_{102}\geq319.86)\approx2.62\times10^{-24}.}
$$

Thus the ordinary Poisson model gives a very poor fit under this goodness-of-fit approximation. This is consistent with [overdispersion](../../../../../../overdispersion.md), although a wrong mean model or dependence can also cause lack of fit; quasi-Poisson variance inflation alone does not establish that the mean model is adequate.

For [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md), $\operatorname{Var}(Y_i)=\phi\mu_i$. The [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) is

$$
\boxed{\widehat\phi=\frac1{102}\sum_{i=1}^{107}\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i}.}
$$

It uses squared [Pearson residuals](../../../../../../pearson-residual.md), not the residual deviance divided by 102. The fitted coefficients are unchanged, and their estimated [covariance matrix](../../../../../../covariance-matrix.md) is multiplied by $\widehat\phi$. With $\widehat\phi=3.24$, standard errors increase by $1.8$, so the main treatment coefficient has

$$
t=\frac{-0.3592068}{1.8(0.1117255)}\approx-1.7862,\qquad p=2\Pr(t_{102}\geq1.7862)\approx0.0770.
$$

**The main Progabide coefficient is not significant at 5% after this dispersion adjustment.** R uses a [Student's t-distribution](../../../../../../student-s-t-distribution.md) when dispersion is estimated, as described in [its GLM summary documentation](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/summary.glm.html); the large-sample normal approximation also gives the same decision.

Because an [interaction term](../../../../../../interaction-term.md) is present, this tests the treatment contrast at baseline zero. An overall absence of treatment influence requires the joint null $\beta_T=\beta_{TB}=0$. The printed marginal standard errors do not give their covariance, so they are insufficient to calculate that joint [Wald test](../../../../../../wald-test.md), or the treatment contrast test at an arbitrary nonzero baseline.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
