<h1 id="10j/solution">Solution</h1>

↑ **Parent:** [10J](../10j.md)

The [Poisson regression](../../../../../poisson-regression.md) uses independent counts with mean $m_i$ and [logarithmic link function](../../../../../logarithmic-link-function.md). Writing $c$ for concentration, the fitted predictors for strains $0,1,2$ are respectively

$$
\log m_0=4.47171-0.28700c,\quad
\log m_1=4.56552+0.05515c,\quad
\log m_2=4.59328-0.26315c.
$$

The interaction formula includes concentration, strain indicators and their products. The intercept is the baseline log mean at zero toxin; exponentiating it gives about $87.5$ fleas. Strain coefficients compare log means at zero concentration. Interaction coefficients compare concentration slopes with the common strain. A unit concentration increase multiplies the three means by about $0.751$, $1.057$ and $0.769$ respectively.

For design [matrix](../../../../../matrix.md) $X$, the fitted expected [Fisher information](../../../../../fisher-information-matrix.md) is $X^TWX$, $W=\operatorname{diag}(\hat m_i)$, since a Poisson count has variance equal to its mean. Standard errors are square roots of diagonal entries of $(X^TWX)^{-1}$. Each reported [Wald test](../../../../../wald-test.md) divides its coefficient estimate by its standard error and compares with an approximate standard normal distribution under a zero-coefficient null, conditional on the other terms. Concentration has strong evidence of a negative baseline effect. At zero concentration strain 1 is not significant at 5% ($p=0.087$), while strain 2 is ($p=0.030$). The strain-1 slope differs strongly from the baseline ($p=0.000193$); the strain-2 slope has no detected difference ($p=0.808$). A nonsignificant difference is not proof of equality. The very significant intercept is a test of mean one at zero toxin, with little scientific relevance.

Relabelling factor levels merges strains 0 and 2 into one group and leaves strain 1 separate. Model $M_2$ retains three intercepts but allows only two slopes: strain 1 versus the common slope of strains 0 and 2. Thus it has five parameters, compared with six in $M_1$. Model $M_3$ merges both intercepts and slopes for strains 0 and 2, retaining only four parameters. The natural nesting is $M_3\subset M_2\subset M_1$.

For these nested [generalized linear models](../../../../../generalized-linear-model.md), the difference in [Poisson deviance](../../../../../poisson-deviance.md) is an asymptotic [likelihood-ratio test](../../../../../likelihood-ratio-test.md) statistic with degrees of freedom equal to the parameter difference. Comparing $M_2$ with $M_1$ gives $56.93-56.87=0.06$ on one degree of freedom, far below $3.84$: the additional strain-2 slope is unnecessary. Comparing $M_3$ with $M_2$ gives $76.98-56.93=20.05$ on one degree of freedom, far above $3.84$: merging the strain-0 and strain-2 intercepts is rejected. Comparing $M_3$ with $M_1$ uses $20.11$ on two degrees of freedom and requires a two-degree-of-freedom threshold, about $5.99$, rather than the supplied $3.84$.

**$M_2$ is the most appropriate of the three models**: retain different strain baselines and the special strain-1 slope, but pool the unsupported strain-2 slope difference. Residual degrees of freedom are $74,75,76$; deviances of this magnitude give no obvious evidence of overdispersion from these summaries alone.

## ↑ Ancestors (10)

1. [10J](../10j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
