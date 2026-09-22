<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Y_i$ be the number of maintenance jobs, $t_i$ average temperature and $p_i$ average precipitation. The fitted [Poisson regression](../../../../../../poisson-regression.md) assumes independent conditional responses with

$$
Y_i\mid t_i,p_i\sim\operatorname{Poisson}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_Tt_i+\beta_Pp_i.
$$

The logarithm is the [Poisson canonical link](../../../../../../poisson-canonical-link.md), so fitted means are always positive. The estimated [regression coefficients](../../../../../../regression-coefficient.md) are

$$
\boxed{(\widehat\beta_0,\widehat\beta_T,\widehat\beta_P)=(4.079374,-0.006162,-0.002922).}
$$

At fixed precipitation, one unit of temperature multiplies the fitted mean by $e^{-0.006162}\simeq0.99386$, a decrease of about $0.614\%$. The fitted precipitation multiplier is $e^{-0.002922}\simeq0.99708$ per unit, but its large [p-value](../../../../../../p-value.md) gives little evidence for that effect. These are conditional associations, not established causal effects.

The intercept-only model has $n-1=23$ residual degrees of freedom, and the full model has $n-3=21$. Both imply **$n=24$ months**.

For an approximate [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) of the full [Poisson regression](../../../../../../poisson-regression.md), compare residual deviance $23.527$ with $\chi^2_{21}$. Its upper-tail [p-value](../../../../../../p-value.md) $0.3165361$ supplies **no evidence of lack of fit**. The ratio $23.527/21\simeq1.120$ also gives no striking indication of [overdispersion](../../../../../../overdispersion.md), though deviance per degree of freedom is only a rough dispersion check. Fitted count means around fifty make the usual chi-squared approximation plausible. Independence between months, the conditional variance-equals-mean assumption and the absence of residual structure still need diagnostics. Failure to reject is not proof that the model is correct.

The null deviance $37.969$ on $23$ degrees of freedom has $p=0.02566753$, suggesting the constant-mean model is inadequate. In the sequential [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md), adding temperature to that model reduces deviance by $14.204$ on one degree of freedom, giving $p=0.000164$. Adding precipitation after temperature reduces it by only $0.238$, with $p=0.625677$. Therefore **retain temperature; these data give no reason to retain precipitation after temperature**. The temperature-only residual deviance is $23.765$ on $22$ degrees of freedom. This prediction-oriented reduced model should be refitted before reporting its coefficients: the printed temperature coefficient belongs to the full model. The [Wald test](../../../../../../wald-test.md) results, $p=0.000833$ and $0.625582$, broadly support the same conclusion, while the sequential deviance tests answer the stated nested-model questions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
