<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the longitudinal delta [covariance](../../../../../../covariance.md) as a white-noise limit. It is a generalized random field, not a pointwise unit-variance [function](../../../../../../function-split.md). Let $B_x(\mathbf r)$ have independent longitudinal increments with

$$
\langle dB_x(\mathbf r)dB_x(\mathbf r')\rangle=A(\mathbf r-\mathbf r')dx.
$$

The smooth-medium limit gives the Stratonovich equation $dE=DE\,dx+iaE\circ dB$. Conversion to Itô form contributes the local [variance](../../../../../../variance-split.md) drift:

$$
dE=\left(DE-\frac{a^2A(0)}2E\right)dx+iaE\,dB.
$$

The Itô [stochastic integral](../../../../../../stochastic-integral.md) has zero mean, so [coherent attenuation in a white-noise random medium](../../../../../../coherent-attenuation-in-a-white-noise-random-medium.md) satisfies

$$
\boxed{m_x=\frac{i}{2k}\Delta_\perp m-\gamma m,\qquad\gamma=\frac{k^2\mu^2A(0)}2,\qquad
m(x,\mathbf r)=e^{-\gamma x}(U_xE_0)(\mathbf r).}
$$

Here $U_x=e^{ix\Delta_\perp/(2k)}$ is the [Fresnel propagator](../../../../../../fresnel-propagator.md). Equivalently,

$$
m(x,\mathbf r)=e^{-\gamma x}\frac{k}{2\pi ix}\int_{\mathbb R^2}\exp\left(\frac{ik|\mathbf r-\mathbf r'|^2}{2x}\right)E_0(\mathbf r')d\mathbf r'.
$$

For a constant entrance envelope this is simply its constant value times $e^{-\gamma x}$.

Put $B_n(r)=\mu^2A(r)$, the transverse [covariance](../../../../../../covariance.md) coefficient of the refractive-index fluctuations. The spectrum required here is the transverse spectrum of that longitudinal [covariance](../../../../../../covariance.md) coefficient, or equivalently the longitudinal-zero-frequency slice of a prelimit stationary medium. Radial symmetry refers to the transverse plane; exact [white noise](../../../../../../white-noise.md) in one direction is not full three-dimensional isotropy. With the Cartesian Fourier convention,

$$
S_F(\boldsymbol\nu)=\int_{\mathbb R^2}B_n(\mathbf r)e^{-i\boldsymbol\nu\cdot\mathbf r}d\mathbf r,
$$

angular integration gives $S_F(\nu)=2\pi\int_0^\infty B_n(r)J_0(\nu r)r\,dr$. Its inverse gives

$$
B_n(0)=\frac1{2\pi}\int_0^\infty S_F(\nu)\nu\,d\nu,\qquad
\boxed{m(x)=\exp\left[-\frac{k^2x}{4\pi}\int_0^\infty S_F(\nu)\nu\,d\nu\right]U_xE_0.}
$$

The printed transform hint mixes two different normalizations. Its radial transform and inverse constitute the self-reciprocal Hankel pair, whose spectrum is $S_H=S_F/(2\pi)$, rather than the unnormalized Cartesian transform also displayed there. Using that Hankel convention consistently yields instead

$$
\boxed{m(x)=\exp\left[-\frac{k^2x}{2}\int_0^\infty S_H(\nu)\nu\,d\nu\right]U_xE_0.}
$$

These are the same physical solution after converting spectra. The distinction is [Fourier-Hankel normalization for an isotropic spectrum](../../../../../../fourier-hankel-normalization-for-an-isotropic-spectrum.md); $J_0(0)=1$ fixes the zero-separation [covariance](../../../../../../covariance.md) in either convention.

## ↑ Ancestors (11)

1. [B](../b.md)
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
