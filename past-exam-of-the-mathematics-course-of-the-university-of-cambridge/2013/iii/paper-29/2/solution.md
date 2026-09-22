<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a real [weakly stationary process](../../../../../weakly-stationary-process.md), extend its [autocovariance](../../../../../autocovariance.md) by $\gamma_{-k}=\gamma_k$. The exact [existence of a time-series spectral density](../../../../../existence-of-a-time-series-spectral-density.md) condition is that its [spectral measure of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md) be [absolutely continuous with respect to](../../../../../absolute-continuity-of-measures.md) [Lebesgue measure](../../../../../lebesgue-measure.md). Absolute summability $\gamma_0+2\sum_{k\geq1}|\gamma_k|<\infty$ is a useful sufficient condition, not a necessary one.

We use the conventional angular-frequency density on $[-\pi,\pi]$, restricted to $[0,\pi]$ by symmetry. Under the absolute-summability condition, the [Fourier series](../../../../../fourier-series-split.md) and its inverse relation are

$$
\boxed{f(\omega)=\frac1{2\pi}\left(\gamma_0+2\sum_{k\geq1}\gamma_k\cos(k\omega)\right),\qquad
\gamma_k=2\int_0^\pi f(\omega)\cos(k\omega)\,d\omega.}
$$

Thus $2\int_0^\pi f=\gamma_0$. If a one-sided density is instead normalized to integrate to the full [variance](../../../../../variance-split.md), use $g=2f$ and omit the factor two in the inverse formula. This is the [positive-frequency spectral normalization](../../../../../positive-frequency-spectral-normalization.md) convention difference. With merely an integrable spectral density, the inverse relation remains valid; one must not assume pointwise convergence of the unweighted Fourier series. Its [Fejér sums](../../../../../fejer-sum.md) recover the density in $L^1$:

$$
f_N(\omega)=\frac1{2\pi}\left[\gamma_0+2\sum_{k=1}^N\left(1-\frac{k}{N+1}\right)\gamma_k\cos(k\omega)\right]\longrightarrow f.
$$

If $X$ and $Y$ are [independent](../../../../../independent-random-variables.md) stationary processes, the cross [covariances](../../../../../covariance.md) vanish, so

$$
\gamma_Z(k)=\operatorname{Cov}(X_{t+k}+Y_{t+k},X_t+Y_t)=\gamma_X(k)+\gamma_Y(k).
$$

Linearity of the inverse [Fourier series](../../../../../fourier-series-split.md) relation, or addition of the [spectral measures of a stationary time series](../../../../../spectral-measure-of-a-stationary-time-series.md), gives **$f_Z=f_X+f_Y$**. Independence can in fact be weakened to zero cross-covariances at every lag.

For the [ARMA](../../../../../autoregressive-moving-average-model.md)$(1,1)$ representation, away from an uncancelled unit root the transfer function gives

$$
\boxed{f_X(\omega)=\frac v{2\pi}\frac{1+\theta^2+2\theta\cos\omega}{1+\phi^2-2\phi\cos\omega}.}
$$

The usual causal case has $|\phi|<1$; the same expression holds for the two-sided stationary solution when $|\phi|>1$. We work in the nondegenerate case $v,w>0$ and $\phi\ne\pm1$; cancellations and zero-noise cases are obtained by the appropriate reduced representation or limits. Since [independent](../../../../../independent-random-variables.md) [white noise](../../../../../white-noise.md) of [variance](../../../../../variance-split.md) $w$ contributes $w/(2\pi)$, put

$$
A=v(1+\theta^2)+w(1+\phi^2),\qquad C=v\theta-w\phi.
$$

Then

$$
\boxed{f_Z(\omega)=\frac1{2\pi}\frac{A+2C\cos\omega}{1+\phi^2-2\phi\cos\omega}.}
$$

The [white-noise addition to an ARMA(1,1) process](../../../../../white-noise-addition-to-an-arma-1-1-process.md) problem is therefore the factorization

$$
A+2C\cos\omega=\lambda(1+\alpha^2+2\alpha\cos\omega).
$$

Define

$$
P=A+2C=v(1+\theta)^2+w(1-\phi)^2,\qquad
Q=A-2C=v(1-\theta)^2+w(1+\phi)^2.
$$

Both are positive under the stated nondegeneracy conditions. An invertible choice is

$$
\boxed{\alpha=\frac{\sqrt P-\sqrt Q}{\sqrt P+\sqrt Q},\qquad
\lambda=\frac{(\sqrt P+\sqrt Q)^2}{4}.}
$$

These satisfy $|\alpha|<1$, $\lambda(1+\alpha)^2=P$, and $\lambda(1-\alpha)^2=Q$. Hence

$$
\boxed{\left(\frac{1+\alpha}{1-\alpha}\right)^2=
\frac{v(1+\theta)^2+w(1-\phi)^2}{v(1-\theta)^2+w(1+\phi)^2}.}
$$

In particular, it is the autoregressive coefficient $\phi$ that enters the terms from the added observation noise.

To obtain a representation of the actual $Z$, define

$$
\xi_t=(1+\alpha B)^{-1}(1-\phi B)Z_t.
$$

The stable inverse exists because $|\alpha|<1$, and spectral filtering gives $f_\xi=\lambda/(2\pi)$. Thus $\xi$ is [weak white noise](../../../../../weak-white-noise.md), and

$$
\boxed{Z_t=\phi Z_{t-1}+\alpha\xi_{t-1}+\xi_t.}
$$

Its [variance](../../../../../variance-split.md) can equivalently be written

$$
\boxed{\lambda=\frac{v(1+\theta^2)+w(1+\phi^2)}{1+\alpha^2}
=\frac{A+\sqrt{A^2-4C^2}}2.}
$$

When $\alpha\ne0$, also $\lambda=(v\theta-w\phi)/\alpha$; when $\alpha=0$, necessarily $C=0$ and $\lambda=A$, so the latter quotient should not be used. The model may reduce in order through cancellation. Boundary limits with $P=0$ or $Q=0$ give $|\alpha|=1$ and need not be stably invertible; the displayed stable reconstruction applies to the nondegenerate case above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
