<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The zero means of both amplitudes give $\mathbb EX_t=0$. Their unit variances and zero [covariance](../../../../../../covariance.md) give, for arbitrary integer $s,t$,

$$
\mathbb E[X_sX_t]=\cos(\omega_0s)\cos(\omega_0t)+\sin(\omega_0s)\sin(\omega_0t)
=\cos(\omega_0(s-t)).
$$

Thus the [variance](../../../../../../variance-split.md) is one and the [covariance](../../../../../../covariance.md) depends only on lag, proving [weak stationarity](../../../../../../weakly-stationary-process.md). Independence or normality of the amplitudes is unnecessary. Since

$$
\cos(\omega_0k)=\tfrac12e^{ik\omega_0}+\tfrac12e^{-ik\omega_0},
$$

the [spectral measure of a random harmonic oscillation](../../../../../../spectral-measure-of-a-random-harmonic-oscillation.md) assigns mass $1/2$ to each of $-\omega_0,\omega_0$. The corresponding right-continuous [time-series spectral distribution](../../../../../../spectral-distribution-function-of-a-stationary-time-series.md) is

$$
\boxed{F(\lambda)=\begin{cases}0,&\lambda<-\omega_0,\\1/2,&-\omega_0\le\lambda<\omega_0,\\1,&\lambda\ge\omega_0.\end{cases}}
$$

These spectral atoms represent a persistent oscillation. There is no ordinary absolutely continuous spectral density for this process.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
