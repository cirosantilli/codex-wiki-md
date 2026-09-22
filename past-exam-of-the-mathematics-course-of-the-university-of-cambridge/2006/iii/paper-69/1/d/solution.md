<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Invert the two-dimensional [Fourier transform](../../../../../../fourier-transform.md) from part (c):

$$
H(k)=\frac1{a_0^2n_e^2L}\int_{\mathbb R^2}C_{\mathrm{RM}}(s)e^{-i\mathbf k_\perp\cdot\mathbf s}\,d^2s.
$$

In [polar coordinates](../../../../../../polar-coordinates.md), the angular integral is $2\pi J_0(ks)$, where $J_0$ is a [Bessel function of the first kind](../../../../../../bessel-function-of-the-first-kind.md). The [Fourier-Hankel normalization for an isotropic spectrum](../../../../../../fourier-hankel-normalization-for-an-isotropic-spectrum.md) therefore yields

$$
\boxed{H(k)=\frac{2\pi}{a_0^2n_e^2L}\int_0^\infty s\,J_0(ks)C_{\mathrm{RM}}(s)\,ds.}
$$

This [Hankel inversion of a rotation-measure correlation](../../../../../../hankel-inversion-of-a-rotation-measure-correlation.md) recovers the scalar [spectral tensor](../../../../../../spectral-tensor.md) coefficient. To obtain the shell-integrated [magnetic energy spectrum](../../../../../../magnetic-energy-spectrum.md), take the [trace](../../../../../../matrix-trace.md) of the three-dimensional tensor:

$$
\mathbb E|\mathbf B|^2=\int\frac{d^3k}{(2\pi)^3}\,2H(k)=\frac1{\pi^2}\int_0^\infty k^2H(k)\,dk.
$$

With [magnetic energy](../../../../../../magnetic-energy.md) density $B^2/(8\pi)$ in [Gaussian units](../../../../../../gaussian-units.md), the one-dimensional convention $\int_0^\infty E_B(k)\,dk=\mathbb E|\mathbf B|^2/(8\pi)$ gives $\boxed{E_B(k)=k^2H(k)/(8\pi^3)}$. A spectrum normalized instead to $\mathbb E|\mathbf B|^2/2$ has coefficient $k^2H(k)/(2\pi^2)$; the physical normalization must be stated.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
