<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $q=n-p$. In this [normal linear model](../../../../../normal-linear-model.md), the [ordinary least squares](../../../../../ordinary-least-squares.md) criterion is $\|Y-Xb\|^2$. Differentiating with respect to $b$ gives the [normal equations for linear least squares](../../../../../normal-equations-for-linear-least-squares.md), $X^TXb=X^TY$. Full column rank of the [design matrix](../../../../../design-matrix.md) makes $X^TX$ invertible, and completing the square proves that the unique minimum is

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Since $\widehat\beta=\beta+(X^TX)^{-1}X^T\epsilon$, its [sampling distribution](../../../../../sampling-distribution.md) is the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md)

$$
\widehat\beta\sim N_p\bigl(\beta,\sigma^2(X^TX)^{-1}\bigr).
$$

Let $H=X(X^TX)^{-1}X^T$ be the [hat matrix](../../../../../hat-matrix.md). It is symmetric and idempotent with rank $p$, and $HX=X$. The [regression residual](../../../../../regression-residual.md) vector is $(I-H)Y=(I-H)\epsilon$, so

$$
\operatorname{RSS}=\|Y-X\widehat\beta\|^2=Y^T(I-H)Y,\qquad \boxed{s^2=\frac{\operatorname{RSS}}{n-p}.}
$$

An [orthogonal projection of a Gaussian vector](../../../../../orthogonal-projection-of-a-gaussian-vector.md) onto the residual space gives $\operatorname{RSS}/\sigma^2\sim\chi^2_q$. The residual projection and fitted projection have zero cross-[covariance](../../../../../covariance.md), hence are [independent](../../../../../independent-random-variables.md) because they are jointly [normal](../../../../../normal-distribution.md). In particular, $s^2$ is an [unbiased estimator](../../../../../unbiased-estimator.md) of $\sigma^2$ and is [independent](../../../../../independent-random-variables.md) of $\widehat\beta$. The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) of $\sigma^2$ instead divides by $n$ and is not unbiased.

For the [null hypothesis](../../../../../null-hypothesis.md) $\beta_1=0$, put $v_{11}=((X^TX)^{-1})_{11}$. Under that [null hypothesis](../../../../../null-hypothesis.md), $\widehat\beta_1/(\sigma\sqrt{v_{11}})$ is standard [normal](../../../../../normal-distribution.md) and independent of $qs^2/\sigma^2$. Therefore the [Student t-test](../../../../../student-s-t-test.md) uses

$$
T=\frac{\widehat\beta_1}{s\sqrt{v_{11}}}\sim t_q.
$$

**A two-sided level-$\alpha$ test rejects when $|T|>t_{q,1-\alpha/2}$.** The denominator is the estimated [standard error](../../../../../standard-error.md) of the [regression coefficient](../../../../../regression-coefficient.md).

The fitted [linear regression](../../../../../linear-regression-split.md) includes an [intercept](../../../../../regression-intercept.md) and three [covariates](../../../../../covariate.md):

$$
\operatorname{NO2}_i=\beta_0+\beta_w\operatorname{wind}_i+\beta_t\operatorname{maxtemp}_i+\beta_s\operatorname{insol}_i+\epsilon_i,\qquad \epsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Thus $n=25$, $p=4$ and the residual [degrees of freedom](../../../../../degree-of-freedom.md) are $21$. The fitted [conditional mean](../../../../../conditional-expectation.md) is

$$
\widehat{\operatorname{NO2}}=3.784916-0.527410\operatorname{wind}+0.124991\operatorname{maxtemp}-0.005259\operatorname{insol}.
$$

Each slope measures a conditional association with the response while the other two [covariates](../../../../../covariate.md) are held fixed. Increasing wind speed by one mile per hour corresponds to a fitted decrease of $0.527410$ in the concentration units used. Its [standard error](../../../../../standard-error.md) is $0.224904$, giving $t=-2.345$ and a two-sided [p-value](../../../../../p-value.md) of $0.0289$: evidence of a negative conditional association at the 5% level. The temperature slope is $0.124991$ per degree Fahrenheit, with [standard error](../../../../../standard-error.md) $0.075173$, $t=1.663$ and [p-value](../../../../../p-value.md) $0.1112$. The insolation slope is $-0.005259$ per langley per day, with [standard error](../../../../../standard-error.md) $0.006637$, $t=-0.792$ and [p-value](../../../../../p-value.md) $0.4370$. Neither of these last two conditional effects is significant at 5%; that does not establish that either true slope is zero. These are associations, not a demonstration of causal effects.

The [intercept](../../../../../regression-intercept.md) estimates the mean at zero values of all three [covariates](../../../../../covariate.md). Its value $3.784916$ has a large [standard error](../../../../../standard-error.md) $7.979647$, giving $t=0.474$ and [p-value](../../../../../p-value.md) $0.6402$. The zero-covariate combination may be outside the observed range, so this test may have little practical relevance. Every coefficient test uses a [Student t-distribution](../../../../../student-s-t-distribution.md) with $21$ [degrees of freedom](../../../../../degree-of-freedom.md).

The reported residual [standard deviation](../../../../../standard-deviation.md) $s=1.844$ measures unexplained variation in concentration units; the subsequent table gives $\operatorname{RSS}=71.428$, consistent with $s=\sqrt{71.428/21}$ after rounding. The five-number residual summary describes the spread, from $-2.3052$ to $3.4033$, with median $-0.4990$. An [intercept](../../../../../regression-intercept.md) forces the residual sum to zero, not the residual median. These five numbers alone cannot establish [normal](../../../../../normal-distribution.md) errors, constant [variance](../../../../../variance-split.md) or [independence](../../../../../independent-random-variables.md); residual-versus-fitted and [quantile-quantile plots](../../../../../q-q-plot.md) would be more informative, and successive days also warrant checking serial dependence. The [coefficient of determination](../../../../../coefficient-of-determination.md) $R^2=0.6533$ means that 65.33% of the sample response sum of squares about its mean is explained by this fit. Its adjusted version is

$$
\overline R^2=1-\frac{\operatorname{RSS}/21}{\operatorname{TSS}/24}=0.6037,
$$

which accounts for the number of estimated [regression coefficients](../../../../../regression-coefficient.md).

The [stepwise selection by the Akaike information criterion](../../../../../stepwise-selection-by-the-akaike-information-criterion.md) searches between the intercept-only model and the specified model with all three main effects. For these [Gaussian](../../../../../normal-distribution.md) fits, the printed [Akaike information criterion](../../../../../akaike-information-criterion.md) is, up to a constant common to the candidates,

$$
\operatorname{AIC}=25\log(\operatorname{RSS}/25)+2p.
$$

The full model has $p=4$ and AIC $34.246$. Removing insolation increases the [residual sum of squares](../../../../../residual-sum-of-squares.md) by $2.136$ but decreases AIC to $32.982$, so that removal is chosen. Removing temperature or wind instead would give AIC $35.337$ or $38.060$ and is worse. In the next step the candidate models include deletions and restoration of insolation. Keeping wind and temperature has the smallest AIC: removing temperature gives $33.389$, restoring insolation gives $34.246$, and removing wind gives $37.960$. Hence the search stops, giving

$$
\boxed{\widehat{\operatorname{NO2}}=4.4368-0.5734\operatorname{wind}+0.1040\operatorname{maxtemp}.}
$$

The accompanying [F-tests](../../../../../f-test.md) compare a larger model with a one-parameter reduction: $F=\Delta\operatorname{RSS}/s^2$, where $s^2$ is estimated from the larger model. For example, removing insolation gives $2.136/(71.428/21)=0.628$, equal to the corresponding squared [test statistic](../../../../../test-statistic.md). Deletions from the second-stage model use $73.564/22$ in the denominator, whereas restoring insolation uses the full-model denominator. These tests describe the comparisons; they do not determine the AIC choice. In particular, temperature is retained despite its deletion-test [p-value](../../../../../p-value.md) $0.15016$. AIC balances fit and complexity, and a stepwise optimum need not be a global optimum over a richer model class. Ordinary coefficient inference after choosing a model does not account for the selection itself.

For positive responses, the [Box–Cox transformation](../../../../../box-cox-transformation.md) is $T_\lambda(y)=(y^\lambda-1)/\lambda$ for $\lambda\ne0$, and $T_0(y)=\log y$. Its [profile likelihood](../../../../../profile-likelihood.md) refits the [linear regression](../../../../../linear-regression-split.md) and [variance](../../../../../variance-split.md) at each $\lambda$ and includes the transformation Jacobian. The graph peaks at roughly $\lambda=0.3$–$0.4$. The approximate 95% [likelihood-ratio confidence interval](../../../../../likelihood-ratio-confidence-interval.md) contains values a little below zero through approximately one, using the cutoff $\ell_{\max}-\chi^2_{1,0.95}/2$. Thus a [logarithmic transformation](../../../../../logarithmic-transformation.md) ($\lambda=0$) and a square-root transformation ($\lambda=1/2$) are plausible, while leaving the response on its original scale ($\lambda=1$) is at or very near the upper confidence boundary. **The broad profile supports considering a mild power transformation; it does not determine a sharply estimated power.** The raster does not justify more precise endpoints or a decisive assertion about which side of the boundary $\lambda=1$ lies.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
