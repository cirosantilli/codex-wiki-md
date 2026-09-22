<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The second analysis is an exposure-adjusted [Poisson regression](../../../../../../poisson-regression.md) for case counts:

$$
\boxed{C_{gj}\sim\operatorname{Poisson}(\lambda_{gj}),\qquad\log\lambda_{gj}=\log N_{gj}+\alpha_P+a_{P,j}+\gamma_Pg,\qquad a_{P,15\text{–}24}=0.}
$$

Cell counts are independent, and their conditional [variance](../../../../../../variance-split.md) equals their conditional mean. The population term is an [offset](../../../../../../generalized-linear-model-offset.md) with coefficient fixed at one. Thus the fitted case rate is $\lambda_{gj}/N_{gj}=\exp(\alpha_P+a_{P,j}+\gamma_Pg)$; treating $\log N_{gj}$ as a free [covariate](../../../../../../covariate.md) would fit a different model. Age multipliers and the adjusted city rate ratio are exponentials of the corresponding [regression coefficients](../../../../../../regression-coefficient.md).

The fitted model again has nine parameters and six residual [degrees of freedom](../../../../../../degree-of-freedom.md). Sequential additions of age and city reduce the [Poisson deviance](../../../../../../poisson-deviance.md) by $2095.56$ on seven [degrees of freedom](../../../../../../degree-of-freedom.md) and $226.52$ on one, respectively. The residual [deviance](../../../../../../exponential-family-deviance.md) is $5.21$, close to the six residual [degrees of freedom](../../../../../../degree-of-freedom.md). The city [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) is overwhelmingly significant, as in the binomial analysis. The table provides no Poisson coefficient estimates, so an exact Poisson city rate ratio cannot be read from it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
