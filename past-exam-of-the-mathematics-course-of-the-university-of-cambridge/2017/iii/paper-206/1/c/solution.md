<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [negative binomial regression](../../../../../../negative-binomial-regression.md) assumes [independent random variables](../../../../../../independent-random-variables.md) conditional on their recorded days, with

$$
Y_i\sim\operatorname{NB}(r,\lambda_i),\qquad \log\lambda_i=\beta_0+\beta_1d_i.
$$

The [logarithmic link function](../../../../../../logarithmic-link-function.md) applies to the conditional [expectation](../../../../../../expected-value.md), not to the observed count. The displayed [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) are

$$
\widehat\beta_0=2.778,\quad \widehat\beta_1=-0.003169,\quad \widehat r\simeq195525.9,
$$

and the [dispersion parameter](../../../../../../dispersion-parameter.md) for the fitted family is one. Thus the fitted [variance](../../../../../../variance-split.md) is $\widehat\lambda_i+\widehat\lambda_i^2/\widehat r$, practically the [Poisson distribution](../../../../../../poisson-distribution.md) [variance](../../../../../../variance-split.md) at these means.

Increasing the day by one multiplies the conditional [expectation](../../../../../../expected-value.md) by $e^{\widehat\beta_1}\simeq0.996836$, a decrease of about $0.3164\%$. Comparing days 365 and 1 gives $e^{364\widehat\beta_1}\simeq0.3155$. The negative slope has [Wald statistic](../../../../../../wald-test.md) approximately $-35.79$, so under the stated model assumptions there is very strong evidence of a decreasing conditional mean:

$$
\boxed{\widehat\lambda(d)=e^{2.778-0.003169d}.}
$$

This is an association with calendar day, not a [causal effect](../../../../../../causal-effect.md) established by the regression. The printed negative-binomial residual deviance is $7544.3$ on $1298$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md), which is a reason to investigate the adequacy of the assumed count model and dependence structure. In particular, the small reported slope [standard error](../../../../../../standard-error.md) cannot make a misspecified model reliable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
