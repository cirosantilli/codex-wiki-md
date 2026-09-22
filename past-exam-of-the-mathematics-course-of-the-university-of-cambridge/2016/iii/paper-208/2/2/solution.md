<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

With angular frequency $\lambda$, the [periodogram](../../../../../../periodogram.md) is

$$
\boxed{I_T(\lambda)=\frac1{2\pi T}\left|\sum_{t=1}^TX_te^{-it\lambda}\right|^2.}
$$

At [Fourier frequencies](../../../../../../fourier-frequency.md) $2\pi j/T$ it is the squared modulus of the normalized [discrete Fourier transform](../../../../../../discrete-fourier-transform.md). If a nonzero mean is unknown, subtract the [sample mean](../../../../../../sample-mean.md) first.

For a zero-mean [stationary process](../../../../../../stationary-process.md), expanding the square gives

$$
EI_T(\lambda)=\frac1{2\pi}\sum_{|h|<T}\left(1-\frac{|h|}{T}\right)\gamma_X(h)e^{-ih\lambda}.
$$

Under absolute summability of the [covariances](../../../../../../covariance.md) this converges to the [spectral density of a stationary process](../../../../../../spectral-density-of-a-stationary-process.md). Thus the [periodogram](../../../../../../periodogram.md) is generally biased at finite $T$, but asymptotically unbiased under this [short-memory time series](../../../../../../short-memory-time-series.md) condition.

It is nevertheless **not a pointwise estimator with [statistical consistency](../../../../../../consistency-statistics.md) unless it is smoothed**. For Gaussian [white noise](../../../../../../white-noise.md), at a nonzero Fourier frequency other than the Nyquist frequency, the real and imaginary Fourier components are independent normal variables. Exactly,

$$
I_T(2\pi j/T)\overset d=f\,\operatorname{Exp}(1),\qquad\operatorname{Var}(I_T)=f^2,
$$

where $f=\sigma^2/(2\pi)$. The [variance](../../../../../../variance-split.md) does not decrease with $T$. Under usual [short-memory time series](../../../../../../short-memory-time-series.md) assumptions the same exponential limit is asymptotic for general processes. Averaging nearby frequencies or using a lag-window estimator reduces [variance](../../../../../../variance-split.md); a frequency bandwidth tending to zero while $T$ times that bandwidth tends to infinity can give [statistical consistency](../../../../../../consistency-statistics.md). The raw plot remains useful for detecting strong periodic peaks, but increasing the record length alone does not remove its pointwise noise.

## ↑ Ancestors (11)

1. [2](../2.md)
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
