<h1 id="13j/solution">Solution</h1>

↑ **Parent:** [13J](../13j.md)

Let $\ell_{\rm sat}$ denote the maximized [log-likelihood](../../../../../log-likelihood.md) in the saturated model, with one fitted mean per observation. With known dispersion, define the [deviance](../../../../../exponential-family-deviance.md) of a fitted model as $D=2(\ell_{\rm sat}-\ell_{\rm fitted})$; for an exponential-dispersion convention that scales deviance by the dispersion $\phi$, divide that scaled quantity by $\phi$ in the following test.

Let $D_0,D_1$ be the fitted deviances under the null and full models. Their difference is the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md)

$$
\boxed{D_0-D_1=2(\ell(\widehat\beta)-\ell(\widehat\beta_0,0)).}
$$

Under the regular identifiable interior null hypothesis, [Wilks theorem](../../../../../wilks-theorem.md) gives the limiting $\chi^2_{p-p_0}$ distribution. Reject for an observed difference above its chosen upper-tail critical value. This concerns the difference of fitted model deviances, not simply the full-model deviance compared with zero.

For a [Poisson regression](../../../../../poisson-regression.md), the means are $\mu_i=e^{x_i^T\beta}$ and $\ell=\sum_i(y_i\log\mu_i-\mu_i-\log y_i!)$. Saturation sets $\mu_i=y_i$, taking the limiting value at $y_i=0$. Consequently the [Poisson deviance](../../../../../poisson-deviance.md) is

$$
\boxed{D=2\sum_i\left[y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right],}
$$

with $0\log0=0$. The intercept score implies $\sum_i(y_i-\widehat\mu_i)=0$ at a finite fit, although retaining that term makes the individual deviance contributions clear.

For $y_i=\widehat\mu_i+\delta_i$ with $|\delta_i|/\widehat\mu_i$ small, expand $(\widehat\mu_i+\delta_i)\log(1+\delta_i/\widehat\mu_i)-\delta_i$. The linear term cancels and the result is $\delta_i^2/(2\widehat\mu_i)+O(|\delta_i|^3/\widehat\mu_i^2)$. Therefore

$$
D\simeq\sum_i\frac{(y_i-\widehat\mu_i)^2}{\widehat\mu_i},
$$

the [Pearson chi-squared statistic](../../../../../pearson-chi-squared-statistic.md). The approximation requires adequately large fitted counts and small relative residuals; it is not an identity for sparse observations.

## ↑ Ancestors (10)

1. [13J](../13j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
