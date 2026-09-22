<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The researcher computed the [Pearson chi-squared statistic](../../../../../../pearson-chi-squared-statistic.md)

$$
X_P^2=\sum_i\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i}
$$

and compared it with a $\chi^2_{1305}$ distribution, using $1308-3=1305$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). Under an adequate large-sample [Poisson regression](../../../../../../poisson-regression.md), $X_P^2$ should be roughly the residual degrees of freedom. The reported tail probability rounds numerically to zero and gives strong evidence of [overdispersion](../../../../../../overdispersion.md).

Possible causes include unobserved heterogeneity or omitted covariates, dependence among respondents, excess zeros, or an incorrect mean function. The conclusion that the Poisson variance assumption fails is well supported, although this test alone does not identify the cause or establish that the [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) variance $\operatorname{Var}(Y_i)=\phi\mu_i$ is correct.

The reported [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md) is $\widehat\phi=X_P^2/1305=1.719346$, so

$$
X_P^2=1305(1.719346)=2243.75
$$

up to rounding.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
