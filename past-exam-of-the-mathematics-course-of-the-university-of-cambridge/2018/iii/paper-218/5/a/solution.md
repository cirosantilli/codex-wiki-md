<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the stationary [autoregressive process of order one](../../../../../../autoregressive-process-of-order-one.md)

$$
X_t-\mu=\phi(X_{t-1}-\mu)+\varepsilon_t,\qquad\varepsilon_t\overset{\mathrm{iid}}\sim N(0,\sigma^2),\quad|\phi|<1.
$$

Multiplication by $X_{t-1}-\mu$ and expectation, using independence of the innovation from the past, gives the [autocovariance](../../../../../../autocovariance.md) equation $\gamma(1)=\phi\gamma(0)$. With $\bar X=n^{-1}\sum_tX_t$, define the sample autocovariances using the same denominator:

$$
\widehat\gamma(h)=\frac1n\sum_{t=h+1}^n(X_t-\bar X)(X_{t-h}-\bar X),\qquad h=0,1.
$$

Substitution into that equation gives the [Yule–Walker estimator for an autoregressive process of order one](../../../../../../yule-walker-estimator-for-an-autoregressive-process-of-order-one.md)

$$
\boxed{\widehat\phi_{YW}=\frac{\widehat\gamma(1)}{\widehat\gamma(0)}=\widehat\rho(1).}
$$

This is exactly the lag-one [sample autocorrelation function](../../../../../../sample-autocorrelation-function.md) under the divisor-$n$ convention, provided the sample has positive variance. Using different divisors for different lags would change the estimator.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
