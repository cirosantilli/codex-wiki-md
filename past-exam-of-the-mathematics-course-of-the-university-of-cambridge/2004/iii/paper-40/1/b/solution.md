<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a discrete-time [weakly stationary process](../../../../../../weakly-stationary-process.md), the [spectral density of a stationary process](../../../../../../spectral-density-of-a-stationary-process.md), when it exists, is a nonnegative function satisfying

$$
\gamma(h)=\int_{-\pi}^{\pi}e^{ih\omega}f_X(\omega)\,d\omega.
$$

If $\sum_h|\gamma(h)|<\infty$, then

$$
f_X(\omega)=\frac1{2\pi}\sum_{h\in\mathbb Z}\gamma(h)e^{-ih\omega}.
$$

A general second-order stationary process has a [spectral measure of a stationary time series](../../../../../../spectral-measure-of-a-stationary-time-series.md), which need not have a [spectral density](../../../../../../spectral-density-of-a-stationary-process.md): a centered random constant has an atom at zero. Thus the [spectral density](../../../../../../spectral-density-of-a-stationary-process.md) calculation below assumes that $f_X$ exists; the corresponding measure identity holds without that extra assumption.

Absolute summability of the filter coefficients gives [mean-square convergence](../../../../../../convergence-in-l2.md) because

$$
\left\|\sum_{s\in E}a_sX_{t-s}\right\|_2
\leq\|X_0\|_2\sum_{s\in E}|a_s|.
$$

Consequently the bilateral filtered process is well defined, with constant [mean](../../../../../../expected-value.md) $m\sum_sa_s$. Its [covariance](../../../../../../covariance.md) is

$$
\gamma_Y(h)=\sum_{r,s\in\mathbb Z}a_ra_s\gamma_X(h-r+s).
$$

The sum is absolutely convergent, since $|\gamma_X(j)|\leq\gamma_X(0)$ and $\sum|a_s|<\infty$. It depends only on lag, proving [weak stationarity](../../../../../../weakly-stationary-process.md) of $Y$.

Insert the spectral representation and interchange summation and integration using absolute summability and the finite total spectral mass. For real coefficients,

$$
\begin{aligned}
\gamma_Y(h)
&=\int_{-\pi}^{\pi}e^{ih\omega}
\left(\sum_ra_re^{-ir\omega}\right)
\left(\sum_sa_se^{is\omega}\right)f_X(\omega)\,d\omega\\
&=\int_{-\pi}^{\pi}e^{ih\omega}|A(e^{i\omega})|^2f_X(\omega)\,d\omega.
\end{aligned}
$$

Therefore the [spectral density transformation under a linear filter](../../../../../../spectral-density-transformation-under-a-linear-filter.md) is

$$
\boxed{f_Y(\omega)=|A(e^{i\omega})|^2f_X(\omega).}
$$

For a bilateral sequence, $A$ is guaranteed to converge on the unit circle. Its negative powers need not converge inside the disk: for example, $a_{-j}=2^{-j}$ makes the series diverge at $z=1/4$. Only the unit-circle values are used here, so the unnecessarily broad domain printed for $A$ does not affect the proof.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
