<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y_i$ be passenger count and use a [Poisson regression](../../../../../../poisson-regression.md) with log mean, initially treating the response as a working daily count:

$$
\log\mu_i=\beta_0+\beta_B\log(\mathrm{Bmiles}_i)+\beta_F\mathrm{Fare}_i
+\beta_P\log(\mathrm{Pop}_i)+\beta_O\frac{\mathrm{Older}_i}{\mathrm{Pop}_i}
+\beta_L\mathrm{LIH}_i+\beta_V\mathrm{Poverty}_i+\beta_R\mathrm{MedRent}_i.
$$

Center and scale the continuous predictors before fitting, and compare a small set of defensible reduced models rather than saturating twenty observations. Household counts should not be called household proportions without a household denominator; population-scaled counts are alternative intensity covariates. Bus miles can be an estimated elasticity term rather than an [offset](../../../../../../generalized-linear-model-offset.md), since proportionality of passenger numbers to bus miles has not been established.

For actual counts, the log-likelihood score is $X^T(Y-\mu)=0$, with $\mu_i=e^{x_i^T\beta}$. Fitting by [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md) uses weights $\mu_i$ and working response $\eta_i+(Y_i-\mu_i)/\mu_i$. Compare nested means by a [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) only if the Poisson variance assumption is plausible; check the [Poisson deviance](../../../../../../poisson-deviance.md), Pearson dispersion $\sum_i(Y_i-\widehat\mu_i)^2/\widehat\mu_i/(20-p)$, residuals, leverage and sensitivity to influential providers. Consider [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) or [negative binomial regression](../../../../../../negative-binomial-regression.md) if variance exceeds the mean.

The recorded response is actually a daily average, so [Poisson working models for averaged counts](../../../../../../poisson-working-models-for-averaged-counts.md) need special care. If a provider was observed for $T_i$ days and total passengers were $C_i$, fit $C_i\sim\operatorname{Poisson}(T_i\mu_i)$ with [offset](../../../../../../generalized-linear-model-offset.md) $\log T_i$. If only the average and no observation duration are available, a Poisson mean model can still be explored, but its likelihood and standard errors are not automatically justified by integer-looking averages.

A one-unit increase in an untransformed predictor has fitted multiplicative mean effect $e^{\beta_j}$; a bus-mile elasticity $\beta_B$ gives a doubling effect $2^{\beta_B}$. **No numerical coefficient estimates or selected twenty-provider model are identifiable from the printed excerpt.** The full provider file and, ideally, the averaging periods are needed to execute these model comparisons.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
