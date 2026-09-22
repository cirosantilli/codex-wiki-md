<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [Fourier transform](../../../../../../fourier-transform.md) convention of equation 3, insert the given [power spectrum](../../../../../../power-spectrum.md) as $S_F$. With $t=\nu L/2$,

$$
\int_0^\infty S_F(\nu)\nu\,d\nu
=4\mu^2L\int_0^\infty te^{-t^2}\,dt=2\mu^2L.
$$

The [Fourier transform of a Gaussian](../../../../../../fourier-transform-of-a-gaussian.md), or the order-zero [Hankel transform](../../../../../../hankel-transform.md), also gives

$$
Q(r)=\frac1{2\pi}\int_0^\infty\mu^2L^3e^{-\nu^2L^2/4}J_0(\nu r)\nu\,d\nu
=\frac{\mu^2L}{\pi}e^{-r^2/L^2}.
$$

Thus the [coherent attenuation in a white-noise random medium](../../../../../../coherent-attenuation-in-a-white-noise-random-medium.md) is

$$
\boxed{m(x,\mathbf z)=e^{-k_0^2\mu^2Lx/(2\pi)}(U_xE_0)(\mathbf z).}
$$

For a unit incident [plane wave](../../../../../../plane-wave.md), the [Fresnel propagator](../../../../../../fresnel-propagator.md) leaves the initial envelope unchanged, so the answer reduces to $\boxed{m=e^{-k_0^2\mu^2Lx/(2\pi)}}$. If instead the given numerical function is interpreted as the self-reciprocal [Hankel transform](../../../../../../hankel-transform.md) spectrum suggested by the printed equations 4 and 5, then $Q(r)=2\mu^2Le^{-r^2/L^2}$ and the alternative is

$$
\boxed{m(x,\mathbf z)=e^{-k_0^2\mu^2Lx}(U_xE_0)(\mathbf z).}
$$

The factor $2\pi$ ambiguity is present in the original PDF. No unique numerical attenuation coefficient follows until the [power spectrum](../../../../../../power-spectrum.md) convention is fixed. The covariance strength $Q(0)$ has units of length in this longitudinal [white noise](../../../../../../white-noise.md) model, making both attenuation exponents dimensionless.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
