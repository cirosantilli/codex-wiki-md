<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the medium's [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md) and [power spectrum](../../../../../../power-spectrum.md) use the explicit convention

$$
 C(\mathbf s)=\langle W(\mathbf r+\mathbf s)W(\mathbf r)\rangle,\qquad
 S_W(\mathbf q)=\int_{\mathbb R^3}C(\mathbf s)e^{-i\mathbf q\cdot\mathbf s}\,d^3s,
$$



$$
 C(\mathbf s)=\frac1{(2\pi)^3}\int_{\mathbb R^3}S_W(\mathbf q)e^{i\mathbf q\cdot\mathbf s}\,d^3q.
$$

Since $n^2-1=2\mu W+\mu^2W^2$, only the linear term in $\mu$ is needed to obtain the cross-section through second order:

$$
 f_\infty^{(1)}=\frac{\mu k^2}{2\pi}\int_VW(\mathbf r)e^{-i\mathbf k_s\cdot\mathbf r}\,d^3r+O(\mu^2).
$$

Squaring and taking the [expectation](../../../../../../expected-value.md) gives

$$
\boxed{\langle\sigma_d\rangle=
\frac{\mu^2k^4}{4\pi^2}\int_V\!\int_V
 C(\mathbf r-\mathbf r')e^{-i\mathbf k_s\cdot(\mathbf r-\mathbf r')}\,d^3r\,d^3r'
 +O(\mu^3).}
$$

This is the finite-volume formula in the [Born approximation for scalar wave scattering](../../../../../../born-approximation-for-scalar-wave-scattering.md); the zero mean of $W$ does not make its squared scattered amplitude vanish. For a jointly centered [Gaussian random field](../../../../../../gaussian-random-field.md), the third-order contribution is zero, so the next perturbative contribution is fourth order when that expansion is valid.

Introduce the overlap volume $H_V(\mathbf s)=|V\cap(V-\mathbf s)|$. Changing variables rewrites the double integral as

$$
 \int_{\mathbb R^3}H_V(\mathbf s)C(\mathbf s)e^{-i\mathbf k_s\cdot\mathbf s}\,d^3s.
$$

When the linear dimensions of a regular scattering volume are large compared with the [correlation length](../../../../../../correlation-length.md), and $C$ is integrable, $H_V(\mathbf s)\simeq|V|$ over the significant covariance range. This gives the [finite-volume random scattering spectrum](../../../../../../finite-volume-random-scattering-spectrum.md) result

$$
\boxed{\langle\sigma_d(\widehat{\mathbf r},\widehat{\mathbf r}_0)\rangle
 \simeq\frac{\mu^2k^4|V|}{4\pi^2}S_W(\mathbf k_s),\qquad
 \mathbf k_s=k(\widehat{\mathbf r}-\widehat{\mathbf r}_0).}
$$

There are two distinct approximations here: the weak-scattering expansion in $\mu$ and the negligible-boundary-overlap approximation in the volume-to-correlation-scale ratio. If $S$ instead denotes the [power spectrum](../../../../../../power-spectrum.md) of the index fluctuation $n-1=\mu W$, then $S=\mu^2S_W$ and the external factor $\mu^2$ is absorbed into $S$.

[Statistical homogeneity](../../../../../../statistical-homogeneity.md) alone allows an anisotropic spectrum, so its argument is generally the vector $\mathbf k_s$. If [statistical isotropy](../../../../../../statistical-isotropy.md) is additionally assumed, $S_W$ depends only on

$$
\boxed{k_s=|\mathbf k_s|=2k\sin(\theta/2),\qquad
 \cos\theta=\widehat{\mathbf r}\cdot\widehat{\mathbf r}_0.}
$$

The scalar notation $S(k_s)$ is valid in that isotropic case. For the alternative convention $S_{\mathrm{norm}}=(2\pi)^{-3}S_W$, the bulk formula is $2\pi\mu^2k^4|V|S_{\mathrm{norm}}(\mathbf k_s)$. Changing the sign of the scattering vector does not change the spectrum of a real stationary scalar field; changing the [Fourier transform](../../../../../../fourier-transform.md) normalization does change the displayed $2\pi$ factors. Both conventions have therefore been stated explicitly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
