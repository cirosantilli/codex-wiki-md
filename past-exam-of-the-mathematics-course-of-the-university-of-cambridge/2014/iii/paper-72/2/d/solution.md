<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the stationary height have [covariance function](../../../../../../covariance-function.md) $C_h(\xi)=\langle h(x)h(x+\xi)\rangle$, with $C_h(0)=\sigma^2$. Define the [power spectrum of surface height](../../../../../../power-spectrum-of-surface-height.md) by

$$
S_h(q)=\int C_h(\xi)e^{-iq\xi}d\xi,\qquad C_h(\xi)=\frac1{2\pi}\int S_h(q)e^{iq\xi}dq.
$$

For real stationary heights this spectrum is even and nonnegative. The [Fourier multiplier](../../../../../../fourier-multiplier.md) identity in part (c) gives

$$
\langle h(x)\mathcal B h(x)\rangle=\frac1{2\pi}\int\beta(q)S_h(q)dq.
$$

Thus [coherent reflection from a stationary rough surface](../../../../../../coherent-reflection-from-a-stationary-rough-surface.md) at normal incidence is

$$
\boxed{\langle\psi_s(x,0)\rangle_{\text{through second order}}=-1+\frac{k}{\pi}\int_{\mathbb R}\beta(q)S_h(q)dq.}
$$

Require the corresponding weighted spectral moment to exist. If the stationary process has a spectral measure rather than a density, the same formula uses that measure with the matching normalization.

Splitting the propagating and evanescent parts makes the effect clear:

$$
\langle\psi_s(x,0)\rangle=-1+\frac{k}{\pi}\int_{|q|<k}\sqrt{k^2-q^2}\,S_h(q)dq+\frac{ik}{\pi}\int_{|q|>k}\sqrt{q^2-k^2}\,S_h(q)dq
$$

through second order. The positive real correction reduces the magnitude of the initially negative unit coherent reflection at this order, as some reflection becomes diffuse. The evanescent part produces a coherent [wave phase](../../../../../../phase-waves.md) correction. In contrast, the first-order mean was exactly the flat reflected wave.

The [height-correlation dependence of coherent reflection](../../../../../../height-correlation-dependence-of-coherent-reflection.md) cannot generally be determined from $\sigma$ alone: the quadratic term weights the whole spectrum by $\beta(q)$, while $\sigma^2=(2\pi)^{-1}\int S_h(q)dq$ is unweighted. If the roughness varies only on scales much longer than the wavelength, so its spectrum is concentrated at $|q|\ll k$, then $\beta\simeq k$ and

$$
\langle\psi_s(x,0)\rangle\simeq-1+2k^2\sigma^2.
$$

This is a useful limiting formula, not the general second-order answer under only small-height assumptions. Also the mean field sampled at the moving physical boundary is $-1+k^2\sigma^2/2$ through second order, from part (c), and is a different observable.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
