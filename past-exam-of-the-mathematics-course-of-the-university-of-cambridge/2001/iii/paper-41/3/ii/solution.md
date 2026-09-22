<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the specified [Fourier transform](../../../../../../fourier-transform.md) convention, the inverse is $\delta(\mathbf x)=\int d^3k\,\delta_{\mathbf k}e^{-i\mathbf k\cdot\mathbf x}/(2\pi)^3$. Inserting both inverse transforms into the [cosmological two-point correlation function](../../../../../../correlation-function-astronomy.md) and applying the given [Dirac delta](../../../../../../dirac-delta-function.md) covariance yields

$$
\begin{aligned}
\xi(\mathbf r)
&=\int\frac{d^3k\,d^3k'}{(2\pi)^6}
e^{-i\mathbf k\cdot\mathbf x-i\mathbf k'\cdot(\mathbf x+\mathbf r)}
\langle\delta_{\mathbf k}\delta_{\mathbf k'}\rangle\\
&=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
\end{aligned}
$$

For an isotropic [matter power spectrum](../../../../../../matter-power-spectrum.md), align the polar axis with $\mathbf r$. The angular integral is $2\pi\int_{-1}^1e^{ikr\mu}\,d\mu=4\pi\sin(kr)/(kr)$. Hence the [isotropic cosmological correlation-power-spectrum relation](../../../../../../isotropic-cosmological-correlation-power-spectrum-relation.md) is

$$
\boxed{\xi(r)=\frac1{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin(kr)}{kr}\,dk.}
$$

The angular kernel is the order-zero [Spherical Bessel function](../../../../../../spherical-bessel-function.md) $j_0(kr)$. At $r=0$, replace it by its [limit](../../../../../../limit-of-a-function.md) one, giving the unsmoothed [variance](../../../../../../variance-split.md) when the integral converges. The argument assumes an ordinary integrable spectrum, or an explicitly specified [distributional Fourier transform](../../../../../../fourier-transform-of-a-tempered-distribution.md) interpretation otherwise.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
