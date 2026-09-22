<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An unknown [variance](../../../../variance-split.md) requires a joint [prior distribution](../../../../prior-probability.md) for $(\alpha,\beta,\sigma^2)$. **The analysis is not determined until a prior for the unknown variance, and its relation to the coefficients, is specified.** A [maximum-likelihood estimate](../../../../maximum-likelihood-estimator.md) substituted for $\sigma^2$ does not by itself account for its posterior uncertainty.

For example, retain the independent coefficient [prior distributions](../../../../prior-probability.md) from part (b) and independently assign $s=\sigma^2$ an [inverse-gamma distribution](../../../../inverse-gamma-distribution.md) with shape $a_0>0$ and scale $b_0>0$, whose [probability density function](../../../../probability-density-function.md) is proportional to $s^{-a_0-1}e^{-b_0/s}$. Then the joint [posterior density](../../../../posterior-density.md) is proportional to

$$
s^{-a_0-1-n/2}\exp\left\{-\frac{b_0+\frac12\sum_i(y_i-\alpha-\beta x_i)^2}{s}
-\frac{(\alpha-\alpha_0)^2}{2\tau_0^2}
-\frac{(\beta-\beta_0)^2}{2\tau_1^2}\right\}.
$$

Conditional on $s$, the two coefficient [posterior distributions](../../../../bayesian-posterior.md) are still the independent [normal distributions](../../../../normal-distribution.md) in part (b), with $s$ substituted for $\sigma^2$. The other [full conditional distribution](../../../../full-conditional-distribution.md) is

$$
s\mid\alpha,\beta,\boldsymbol y\sim
\operatorname{InvGamma}\left(a_0+\frac n2,
b_0+\frac12\sum_i(y_i-\alpha-\beta x_i)^2\right).
$$

The marginal coefficient [posterior distribution](../../../../bayesian-posterior.md) requires [marginalization](../../../../marginalization.md) over $s$; it is generally nonnormal and the two coefficients need not remain independent. In particular, the posterior [cumulative distribution function](../../../../cumulative-distribution-function.md) of the requested [mean](../../../../expected-value-split.md) becomes

$$
\mathbb P(M_0\leq t\mid\boldsymbol y)
=\int_0^\infty
\Phi\left(\frac{t-m_\alpha(s)-x_0m_\beta(s)}
{\sqrt{v_\alpha(s)+x_0^2v_\beta(s)}}\right)
\pi(s\mid\boldsymbol y)\,ds.
$$

Its shortest 95% [credible interval](../../../../credible-interval.md) must be found from this marginal [posterior distribution](../../../../bayesian-posterior.md), for example by numerical [integration](../../../../integral-split.md) or posterior simulation. This is [normal regression with independent coefficient and variance priors](../../../../normal-regression-with-independent-coefficient-and-variance-priors.md).

A different, convenient choice is a [normal-inverse-gamma prior](../../../../normal-inverse-gamma-prior.md), in which the conditional coefficient prior [covariance matrix](../../../../covariance-matrix.md) is proportional to $\sigma^2$. That choice gives a multivariate [Student's t-distribution](../../../../student-s-t-distribution.md) after [marginalization](../../../../marginalization.md), so the interval uses its univariate [Student's t-distribution](../../../../student-s-t-distribution.md) [quantiles](../../../../quantile-function.md). It changes the coefficient prior specification; a Student interval does not follow automatically from retaining the fixed-$\tau_0,\tau_1$ priors in part (b).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
