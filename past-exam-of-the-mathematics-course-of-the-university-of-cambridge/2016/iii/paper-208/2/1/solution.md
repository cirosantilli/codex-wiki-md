<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a causal [autoregressive model](../../../../../../autoregressive-model.md) of order $p$, the population [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) cuts off after lag $p$, whereas the [autocorrelation function](../../../../../../autocorrelation.md) generally decays. For an invertible [moving-average model](../../../../../../moving-average-model.md) of order $q$, the [autocorrelation function](../../../../../../autocorrelation.md) cuts off after lag $q$, whereas the partial [correlation coefficients](../../../../../../pearson-correlation-coefficient.md) generally decay. For a mixed [autoregressive moving-average model](../../../../../../autoregressive-moving-average-model.md), both generally decay. Exponential decay may alternate in sign or show damped oscillations. Sample [correlation coefficients](../../../../../../pearson-correlation-coefficient.md) only approximate these patterns, so isolated crossings of the significance bands are not exact order tests.

In PDF Figure 1, the [autocorrelation function](../../../../../../autocorrelation.md) alternates sign, with a large negative lag-one [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) and geometrically decreasing magnitude. The [partial autocorrelation function](../../../../../../partial-autocorrelation-function.md) has essentially one substantial spike, negative at lag one and about $-0.8$; later values mostly lie within the displayed bands. Thus **a stationary [AR(1)](../../../../../../autoregressive-process-of-order-one.md) with a negative coefficient is the natural first model**, with $\widehat\phi$ initially near $-0.8$. The trace fluctuates around an approximately constant mean and shows no evident deterministic trend.

Fit that model, compare nearby low-order alternatives using [likelihood function](../../../../../../likelihood-function.md) and an [Akaike information criterion](../../../../../../akaike-information-criterion.md) or [Bayesian information criterion](../../../../../../bayesian-information-criterion.md), and inspect the residual [autocorrelation function](../../../../../../autocorrelation.md) and residual [variance](../../../../../../variance-split.md). A few small later [PACF](../../../../../../partial-autocorrelation-function.md) spikes are expected in a plot with many lags. The roughly $\pm1.96/\sqrt T$ [white noise](../../../../../../white-noise.md) bands are a guide, rather than simultaneous guarantees for every lag.

The sign alternation also suggests concentration of spectral power near the high-frequency end: the [AR(1)](../../../../../../autoregressive-process-of-order-one.md) denominator $1+\phi^2-2\phi\cos\lambda$ is smallest near $\lambda=\pi$ when $\phi<0$. From estimated $\gamma(0)$ and lag-one [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) one can estimate innovation [variance](../../../../../../variance-split.md) as $\widehat\sigma_\varepsilon^2\approx\widehat\gamma(0)(1-\widehat\phi^2)$. The persistence parameter controls the decay rate and [long-run variance of a stationary process](../../../../../../long-run-variance-of-a-stationary-process.md). These plots do not establish a [normal distribution](../../../../../../normal-distribution.md), [independence](../../../../../../independent-random-variables.md), or the absence of nonlinear dependence; [correlation coefficients](../../../../../../pearson-correlation-coefficient.md) of squared residuals can provide a separate [variance](../../../../../../variance-split.md) diagnostic.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
