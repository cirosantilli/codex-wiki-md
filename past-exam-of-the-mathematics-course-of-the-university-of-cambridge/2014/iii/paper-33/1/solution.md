<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [normal linear model](../../../../../normal-linear-model.md), the [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\beta,\sigma^2)=-\frac n2\log(2\pi\sigma^2)-\frac{(Y-X\beta)^T(Y-X\beta)}{2\sigma^2}.
$$

The full column rank of the [design matrix](../../../../../design-matrix.md) makes $X^TX$ invertible. Differentiating in $\beta$ gives the normal equations $X^TX\widehat\beta=X^TY$. With the minimized [residual sum of squares](../../../../../residual-sum-of-squares.md) substituted, differentiation in $\sigma^2$ gives

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY,\qquad\widehat\sigma^2=\frac{RSS}{n}.}
$$

These are the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md) almost surely; $RSS>0$ almost surely when $\sigma^2>0$ and $n>p$. The linear transformation of the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) yields

$$
\boxed{\widehat\beta\sim N_p\bigl(\beta,\sigma^2(X^TX)^{-1}\bigr).}
$$

Define the [hat matrix](../../../../../hat-matrix.md) $H=X(X^TX)^{-1}X^T$. The [fitted values](../../../../../fitted-values.md) are $\widehat Y=HY=X\widehat\beta$, the [regression residuals](../../../../../regression-residual.md) are $e=Y-\widehat Y=(I-H)Y$, and $RSS=e^Te$. The [orthogonal projection](../../../../../orthogonal-projection.md) $I-H$ has rank $n-p$ and annihilates $X\beta$. By [Cochran's theorem](../../../../../cochran-s-theorem.md),

$$
\boxed{RSS/\sigma^2\sim\chi^2_{n-p},\qquad\widehat\beta\ \text{is independent of }RSS.}
$$

Consequently $E(\widehat\sigma^2)=(n-p)\sigma^2/n$, with [bias](../../../../../bias-of-an-estimator.md) $-p\sigma^2/n$. The [unbiased estimator](../../../../../unbiased-estimator.md) is

$$
\boxed{\widetilde\sigma^2=\frac{RSS}{n-p}.}
$$

Its square root, the reported [residual standard error](../../../../../residual-standard-error.md), estimates $\sigma$; the assertion of unbiasedness applies to the variance, not generally to its square root.

For the paper-strength analysis, let $h_i$ be the measured percentage and $z_i=h_i-\overline h$. Both [normal linear models](../../../../../normal-linear-model.md) use independent errors of common [variance](../../../../../variance-split.md) $\sigma^2$. Their mean functions are $\beta_0+\beta_1z_i$ for `lm1`, and $\beta_0+\beta_1z_i+\beta_2z_i^2$ for `lm2`, with separately fitted coefficients. The reported [residual standard errors](../../../../../residual-standard-error.md) are **$11.82$ and $4.42$**, respectively.

For `lm1`, the estimated [conditional expectation](../../../../../conditional-expectation.md) at a new percentage $x$ is

$$
\boxed{\widehat m(x)=34.1842+1.7710(x-\overline h).}
$$

The original data mean $\overline h$ must be used for centering the new percentage; its numerical value is not supplied in the excerpt. Because $\sum_i z_i=0$, the two columns of this [design matrix](../../../../../design-matrix.md) are orthogonal, and $\operatorname{Cov}(\widehat\beta_0,\widehat\beta_1)=0$. Hence the coefficient [standard errors](../../../../../standard-error.md) in the output give

$$
\boxed{\widehat{\operatorname{Var}}\{\widehat m(x)\}=2.7108^2+(x-\overline h)^2\,0.6478^2.}
$$

This estimates uncertainty in the mean. Predicting an individual future batch would additionally require the new-error variance, estimated by $11.82^2$.

To compare the nested [normal linear models](../../../../../normal-linear-model.md), test $H_0:\beta_2=0$ against $H_1:\beta_2\ne0$ within the quadratic model. The [Student t-test](../../../../../student-s-t-test.md) statistic is

$$
T=\frac{-0.63455}{0.06179}\approx-10.27,
\qquad T\sim t_{16}\quad\text{under }H_0.
$$

Its two-sided [p-value](../../../../../p-value.md) is $1.89\times10^{-8}$. Equivalently $T^2$ is a partial [F-test](../../../../../f-test.md) statistic with null distribution $F_{1,16}$. **Reject the linear restriction and prefer `lm2` at the 5% level.** Its residual spread is much smaller; the increase in the [coefficient of determination](../../../../../coefficient-of-determination.md) from $0.3054$ to $0.9085$ supports the same conclusion, although the test is the relevant complexity-adjusted comparison.

For [regression diagnostics](../../../../../regression-diagnostics.md), inspect [regression residuals](../../../../../regression-residual.md) against fitted means and hardwood percentage for omitted curvature, a scale-location plot for nonconstant [variance](../../../../../variance-split.md), and a [quantile-quantile plot](../../../../../q-q-plot.md) against the [normal distribution](../../../../../normal-distribution.md) for departures from the error assumption. Check unusual observations using [regression leverage](../../../../../regression-leverage.md) and [Cook's distance](../../../../../cook-s-distance.md), and examine residuals in collection or batch order if dependence is plausible. Independence and a common [variance](../../../../../variance-split.md) require substantive justification as well as these plots; a small [p-value](../../../../../p-value.md) for a polynomial term does not itself check the error model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
