<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [weakly stationary process](../../../../../weakly-stationary-process.md) with mean $m$, the [autocovariance function](../../../../../autocovariance.md) is $\gamma_k=\mathbb E[(X_{t+k}-m)(X_t-m)]$, independent of $t$. The positive definiteness of these covariances gives a unique finite positive [spectral measure of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md) on the frequency circle. Its cumulative function is the [time-series spectral distribution](../../../../../spectral-distribution-function-of-a-stationary-time-series.md) $F$, with total mass $\gamma_0$, and

$$
\boxed{\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}\,dF(\lambda).}
$$

Use one representative of the identified endpoints $-\pi$ and $\pi$ when specifying atoms. For a real-valued process the measure is symmetric, so the imaginary part integrates to zero. If it has a [time-series spectral density](../../../../../spectral-density-of-a-stationary-process.md), then

$$
\boxed{\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}f(\lambda)d\lambda,\qquad
f(\lambda)=\frac1{2\pi}\sum_{k\in\mathbb Z}\gamma_k e^{-ik\lambda}.}
$$

The second identity is pointwise for an absolutely summable [covariance](../../../../../covariance.md) sequence, as will apply to part (a). Existence of a density alone does not guarantee ordinary pointwise convergence of its [Fourier series](../../../../../fourier-series-split.md); in general the reconstruction can be interpreted by its [Cesaro means](../../../../../cesaro-mean.md) in $L^1$. This fixes the frequency normalization for all three calculations below.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
