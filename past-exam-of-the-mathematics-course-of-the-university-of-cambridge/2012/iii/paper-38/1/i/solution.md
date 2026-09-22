<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the one-sided convention: integrating the [one-sided spectral density](../../../../../../one-sided-spectral-density-of-a-real-stationary-time-series.md) over $[0,\pi]$ gives the [variance](../../../../../../variance-split.md). A standard sufficient hypothesis is absolute summability of the [autocovariance sequence](../../../../../../autocovariance.md):

$$
\boxed{\gamma_0+2\sum_{k=1}^{\infty}|\gamma_k|<\infty.}
$$

For a real [weakly stationary process](../../../../../../weakly-stationary-process.md), extend the sequence by $\gamma_{-k}=\gamma_k$. The Fourier pair is

$$
\boxed{f_X(\omega)=\frac1\pi\sum_{k\in\mathbb Z}\gamma_ke^{ik\omega}
=\frac1\pi\left(\gamma_0+2\sum_{k\ge1}\gamma_k\cos(k\omega)\right),\qquad
\gamma_k=\int_0^\pi f_X(\omega)\cos(k\omega)\,d\omega.}
$$

Absolute summability makes the series uniformly convergent and continuous; cosine orthogonality gives the inverse relation. Nonnegativity follows from the [spectral measure of a stationary time series](../../../../../../spectral-measure-of-a-stationary-time-series.md), or from the nonnegative Fejér approximations obtained by taking [variances](../../../../../../variance-split.md) of finite Fourier sums.

For precision, absolute summability is sufficient, not necessary. The exact general condition is that the spectral measure be [absolutely continuous with respect to](../../../../../../absolute-continuity-of-measures.md) [Lebesgue measure](../../../../../../lebesgue-measure.md). For example, a density constant on $[0,\pi/2]$ and zero elsewhere has $\gamma_k$ proportional to $\sin(k\pi/2)/k$, which is not absolutely summable. Thus the displayed absolutely convergent Fourier formula answers the usual covariance-summability version; an arbitrary density need only have the integral inverse relation and Fejér-mean Fourier recovery in $L^1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
