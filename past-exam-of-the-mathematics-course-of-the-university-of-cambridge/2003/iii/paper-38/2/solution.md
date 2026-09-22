<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The prose names a second year that differs from the table label. The calculations use the four supplied counts, interpreting the first and second rows as the two displayed periods; no numerical conclusion depends on resolving that label discrepancy.

The first [generalized linear model](../../../../../generalized-linear-model.md) treats the four counts as independent [Poisson random variables](../../../../../poisson-distribution.md), with a [log link](../../../../../logarithmic-link-function.md) and both row and column [regression factors](../../../../../regression-factor.md). The row-by-column interaction makes the [log-linear model](../../../../../log-linear-model.md) saturated. With $r,c\in\{0,1\}$, write

$$
\log\mu_{rc}=\alpha+\beta r+\gamma c+\delta rc.
$$

Its four [maximum-likelihood fitted values](../../../../../maximum-likelihood-fitted-value.md) equal the observed counts. Thus $\widehat\alpha=\log20$, $\widehat\beta=\log(12/20)$, $\widehat\gamma=\log(9/20)$, and

$$
\widehat\delta=\log\frac{20\cdot11}{9\cdot12}=0.711496.
$$

The interaction is the [log odds ratio](../../../../../log-odds-ratio.md) measuring association of row and column. Under independent Poisson sampling, the delta-method [variances](../../../../../variance-split.md) are $1/20$ for the intercept, $1/12+1/20$ for the row contrast, $1/9+1/20$ for the column contrast, and $1/20+1/9+1/12+1/11$ for the interaction. Their square roots reproduce the printed [standard errors](../../../../../standard-error.md). Although the software labels the standardized ratios as t values, these are asymptotic normal [Wald statistics](../../../../../wald-test.md), with known [Poisson](../../../../../poisson-distribution.md) dispersion one, not exact finite-df Student tests.

The [statistical saturated model](../../../../../saturated-statistical-model.md) has zero [residual deviance](../../../../../residual-deviance.md) and zero [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md); this is a perfect interpolation, not evidence of predictive adequacy. The null deviance $5.016056$ compares the four observed counts with an intercept-only model, whose four fitted means are $52/4=13$. [Fisher scoring](../../../../../scoring-algorithm.md) is the numerical score/information iteration used to fit the model; the iteration count is a convergence report, not a test statistic.

Dropping the interaction gives the [independence log-linear model for a two-way contingency table](../../../../../independence-log-linear-model-for-a-two-way-contingency-table.md), $\log\mu_{rc}=\alpha+\beta r+\gamma c$. Its [Poisson regression margin-matching score equations](../../../../../poisson-regression-margin-matching-score-equations.md) match the row and column totals, so

$$
\widehat\mu_{rc}=\frac{r_r c_c}{N},\qquad \widehat\mu=\begin{pmatrix}17.846154&11.153846\\14.153846&8.846154\end{pmatrix},\qquad N=52.
$$

Here $r_r$ and $c_c$ denote the observed row and column totals. In particular the fitted row multiplier is $23/29$, the column multiplier is $20/32$, and the intercept is $\log(29\cdot32/52)=2.881788$. These produce the second coefficient table. Their [standard errors](../../../../../standard-error.md) follow from the inverse [Fisher information matrix](../../../../../fisher-information-matrix.md); for the row and column contrasts their squared values are $1/29+1/23$ and $1/32+1/20$, while the intercept [variance](../../../../../variance-split.md) is $1/29+1/32-1/52$.

The [Poisson deviance](../../../../../poisson-deviance.md) relative to the saturated fit is

$$
G^2=2\sum_{r,c}y_{rc}\log\frac{y_{rc}}{\widehat\mu_{rc}}=1.527855.
$$

The linear terms cancel because fitted and observed totals agree. The additive model has three coefficients, leaving one [degree of freedom](../../../../../degree-of-freedom.md). [Wilks theorem](../../../../../wilks-theorem.md) calibrates this [likelihood-ratio test](../../../../../likelihood-ratio-test.md) approximately by $\chi^2_1$, giving $p\simeq0.2164$. The interaction [Wald test](../../../../../wald-test.md) instead gives $p\simeq0.2192$; the two are only asymptotically equivalent.

[Fisher's exact test](../../../../../fisher-s-exact-test.md) conditions on both margins under independence. If $X$ is the upper-left count, then

$$
P(X=x)=\frac{\binom{32}{x}\binom{20}{29-x}}{\binom{52}{29}},\qquad9\le x\le29.
$$

Its usual two-sided [p-value](../../../../../p-value.md) sums the probabilities of all tables no more probable than the observed $X=20$. That sum is $0.259724$, reproducing the output without an asymptotic approximation. It tests the same absence of row-column association, but conditioning and discreteness explain the numerical difference from the [likelihood-ratio test](../../../../../likelihood-ratio-test.md).

In ordinary language, the male proportion among the cases is $20/29\simeq69.0\%$ in the first row and $12/23\simeq52.2\%$ in the second. The estimated case-sex [odds ratio](../../../../../odds-ratio.md) is $2.037$, but its approximate 95-percent [confidence interval](../../../../../confidence-interval.md) is wide, $(0.655,6.338)$. **These small samples do not give convincing evidence that the sex composition of cases changed between the two periods.** Failure to reject is not evidence that the compositions are exactly equal. Nor do these counts establish a male-to-female disease-incidence ratio or an incidence trend: population denominators and comparable ascertainment would be needed for those interpretations.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
