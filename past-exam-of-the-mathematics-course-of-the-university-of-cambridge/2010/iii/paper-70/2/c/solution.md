<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the given Gaussian radial spectrum, the only needed [integral](../../../../../../integral.md) is

$$
\int_0^\infty \mu^2L^3e^{-\nu^2L^2/4}\nu\,d\nu=2\mu^2L.
$$

If $S$ is interpreted with the self-reciprocal Hankel pair in the supplied hint, the coherent field is

$$
\boxed{m(x,\mathbf r)=e^{-k^2\mu^2Lx}(U_xE_0)(\mathbf r).}
$$

In this convention $B_n(r)=2\mu^2L e^{-r^2/L^2}$ and hence $B_n(0)=2\mu^2L$, directly verifying the attenuation coefficient. If instead the stated spectrum is the unnormalized Cartesian [Fourier transform](../../../../../../fourier-transform.md), use its inverse normalization and obtain

$$
\boxed{m(x,\mathbf r)=e^{-k^2\mu^2Lx/(2\pi)}(U_xE_0)(\mathbf r).}
$$

Its transverse [covariance](../../../../../../covariance.md) coefficient is then $B_n(r)=\mu^2L\,e^{-r^2/L^2}/\pi$. The apparent difference is precisely the inconsistent Fourier/Hankel normalization in the printed hint, not a difference in stochastic propagation. For a unit constant entrance field the Fresnel factor is one; coherent intensity is the square of the displayed mean amplitude.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
