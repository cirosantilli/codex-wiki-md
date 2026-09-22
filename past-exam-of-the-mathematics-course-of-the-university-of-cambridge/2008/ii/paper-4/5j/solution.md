<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

These are nested [Poisson regression](../../../../../poisson-regression.md) models with [independent](../../../../../independent-random-variables.md) counts and the default log [link function](../../../../../link-function.md). If $x_i$ is biomass and $g_i$ is the three-level pH group, model 1 specifies $\log\mu_i=\alpha+\beta x_i$: one common intercept and slope. Model 2 specifies $\log\mu_i=\alpha_{g_i}+\beta x_i$: three group-specific intercepts and a common slope. Model 3 specifies $\log\mu_i=\alpha_{g_i}+\beta_{g_i}x_i$: three intercepts and three slopes, because the multiplication syntax includes both main effects and their interaction. The parameter counts are therefore $2,4,6$.

The [analysis of deviance](../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) compares model 1 against model 2 by testing equality of the three intercepts, conditional on a common biomass slope. The [likelihood-ratio test](../../../../../likelihood-ratio-test.md) statistic is $407.67-99.24=308.43$ with two additional parameters, giving the reported tiny [p-value](../../../../../p-value.md). The next test compares model 2 against model 3 by testing equality of their three slopes. Its statistic is $99.24-83.20=16.04$, again with two degrees of freedom and reported $p=3.288\times10^{-4}$. Both restrictions are rejected. Thus **model 3 is the supported choice: both baseline richness and its biomass dependence vary with pH**. Under the Poisson assumptions, residual deviance $83.20$ on $84$ residual degrees of freedom is also consistent with a satisfactory fit, although these nested tests themselves establish improvement rather than every possible aspect of model adequacy.

The prediction from model 2 is on its linear-predictor scale. Exponentiating gives its fitted means. The final expression is twice the saturated log likelihood minus the model-2 log likelihood, i.e. the [Poisson deviance](../../../../../poisson-deviance.md) of model 2. Consequently

$$
\boxed{\text{The returned value is }99.24\text{, up to the table's rounding}.}
$$

In the saturated model each mean equals the corresponding observed count, with the usual continuous convention for a zero count.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
