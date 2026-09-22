<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [connected generating functional](../../../../../../connected-generating-functional.md) is $W_0[J]=\log Z_0[J]$. Its second functional source derivative gives the [connected correlation function](../../../../../../connected-correlation-function.md); the source-independent determinant drops out. Translational invariance therefore gives

$$
\langle\widetilde\phi(p)\widetilde\phi(q)\rangle_c=(2\pi)^D\delta^{(D)}(p+q)\widetilde G_0(p),\qquad
\boxed{\widetilde G_0(p)=\widetilde\Delta(p)^{-1}=\frac{\alpha}{p^2+\mu^2},\quad \mu^2=\alpha m^2.}
$$

This covariance is independent of the source in a purely Gaussian theory; at zero source the mean field vanishes.

Fourier inversion can be evaluated with the [Schwinger parameterization](../../../../../../schwinger-parameterization.md). Since $(p^2+\mu^2)^{-1}=\int_0^\infty ds\,e^{-s(p^2+\mu^2)}$, the elementary [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md) gives

$$
G_0(r)=\alpha\int_0^\infty\frac{ds}{(4\pi s)^{D/2}}
\exp\left[-\mu^2s-\frac{r^2}{4s}\right]
=\frac{\alpha}{(2\pi)^{D/2}}\left(\frac\mu r\right)^{D/2-1}K_{D/2-1}(\mu r),
$$

where $K$ is the [Modified Bessel function of the second kind](../../../../../../modified-bessel-function-of-the-second-kind.md). This integral formula also gives both asymptotic regimes directly.

For $\mu r\ll1$, set $u=r^2/(4s)$. The integral tends to the [gamma function](../../../../../../gamma-function.md) integral $\int_0^\infty u^{D/2-2}e^{-u}du=\Gamma(D/2-1)$; this is finite for $D>2$. Hence, at distances larger than the microscopic cutoff,

$$
\boxed{G_0(r)\sim\frac{\alpha\Gamma(D/2-1)}{4\pi^{D/2}}\frac1{r^{D-2}},\qquad \Lambda^{-1}\ll r\ll\xi.}
$$

For $\mu r\gg1$, the exponent $\mu^2s+r^2/(4s)$ has its minimum at $s=r/(2\mu)$, with value $\mu r$. Gaussian expansion about that saddle, or the [large-argument asymptotic expansion of a modified Bessel function](../../../../../../large-argument-asymptotic-expansion-of-a-modified-bessel-function.md), gives $K_\rho(z)\sim\sqrt{\pi/(2z)}e^{-z}$. Therefore

$$
\boxed{G_0(r)\sim\frac{\alpha}{2(2\pi)^{(D-1)/2}}
\frac{\xi}{(r\xi)^{(D-1)/2}}e^{-r/\xi},\qquad r\gg\xi,\quad \xi=\frac1{\sqrt{\alpha m^2}}.}
$$

This is the [massive Gaussian field correlation tail](../../../../../../massive-gaussian-field-correlation-tail.md) with its normalization displayed. For example $D=3$ gives exactly $G_0(r)=\alpha e^{-r/\xi}/(4\pi r)$, verifying both regimes and the exponential length scale.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
