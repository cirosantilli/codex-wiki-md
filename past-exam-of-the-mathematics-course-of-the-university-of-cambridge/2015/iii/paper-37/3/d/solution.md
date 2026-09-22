<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [cycles-per-time spectral density](../../../../../../cycles-per-time-spectral-density.md), with frequency $\omega\in[-1/2,1/2]$. The [spectral representation theorem for a stationary time series](../../../../../../spectral-representation-theorem-for-a-stationary-time-series.md) gives the centered [white noise](../../../../../../white-noise.md) representation

$$
\varepsilon_t=\int_{-1/2}^{1/2}e^{2\pi it\omega}\,dZ_\varepsilon(\omega),\qquad
\mathbb E|dZ_\varepsilon(\omega)|^2=\sigma^2\,d\omega,
$$

where disjoint increments are orthogonal. Put $\theta_0=1$. Since the filter is finite, substitute each noise representation and interchange the finite sum with the integral:

$$
X_t=\int_{-1/2}^{1/2}e^{2\pi it\omega}\Theta(e^{-2\pi i\omega})\,dZ_\varepsilon(\omega).
$$

The new orthogonal increment measure is $dZ_X=\Theta(e^{-2\pi i\omega})dZ_\varepsilon$. Its [variance](../../../../../../variance-split.md) measure is therefore $\sigma^2|\Theta(e^{-2\pi i\omega})|^2d\omega$. The coefficients are real, so conjugation changes the sign of the exponent without changing the modulus. Hence

$$
\boxed{f_X(\omega)=\sigma^2|\Theta(e^{2\pi i\omega})|^2.}
$$

With angular frequency $\lambda=2\pi\omega$, the [spectral density of a stationary process](../../../../../../spectral-density-of-a-stationary-process.md) instead contains the factor $1/(2\pi)$. The convention explains its absence here. Invertibility is not needed for this finite-filter spectral calculation.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
