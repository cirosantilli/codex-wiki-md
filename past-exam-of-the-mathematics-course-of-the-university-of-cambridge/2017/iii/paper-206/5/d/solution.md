<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The selected model is a [moving-average process of order one](../../../../../../moving-average-process-of-order-one.md), with the plus-sign convention used by R:

$$
\boxed{Y_t=\mu+\varepsilon_t+\theta\varepsilon_{t-1},\quad \widehat\mu=15.0133,\quad \widehat\theta=0.6727,\quad \widehat\sigma_\varepsilon^2=4.634.}
$$

The Gaussian [likelihood function](../../../../../../likelihood-function.md) models innovations as independent $N(0,\sigma_\varepsilon^2)$. Its [autocovariance](../../../../../../autocovariance.md) is $\gamma(0)=\sigma_\varepsilon^2(1+\theta^2)$, $\gamma(1)=\sigma_\varepsilon^2\theta$, and zero at larger lags, with [autocorrelation](../../../../../../autocorrelation.md) $\rho(1)=\theta/(1+\theta^2)\simeq0.4631$. The estimated coefficient has modulus less than one, giving [invertibility of a moving-average model](../../../../../../invertibility-of-a-moving-average-model.md); a finite moving-average process is stationary regardless of this invertibility restriction.

The original plots show fluctuations around a roughly constant level, no persuasive deterministic trend, and a conspicuous positive lag-one correlation with the other plotted correlations within the approximate sampling bands. They make a stationary nonseasonal working model reasonable for this short series. `stationary=TRUE` excludes differenced alternatives, and `seasonal=FALSE` excludes seasonal ARIMA terms. Neither option is proved by a 60-day plot: annual temperature seasonality cannot be excluded from two months, and a longer record or residual diagnostics might require a different model. The options are reasonable local simplifications, not universal statements about temperature dynamics.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
