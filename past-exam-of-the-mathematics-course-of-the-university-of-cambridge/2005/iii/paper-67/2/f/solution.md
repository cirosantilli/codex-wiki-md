<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

In [single-photon emission computed tomography](../../../../../../single-photon-emission-computed-tomography.md), the unknown is an emitting source, rather than the absorption coefficient reconstructed by transmission [computed tomography](../../../../../../computed-tomography.md). Photons emitted at different points on the same ray are weighted by their probability of surviving the path to the detector. If the known attenuation is $a$ and the detector is at the positive end of the ray, the data are an [attenuated Radon transform](../../../../../../attenuated-radon-transform.md)

$$
R_af(\rho,\theta)=\int_{\mathbb R}f(\tau\boldsymbol d+\rho\boldsymbol n)
\exp\left[-\int_\tau^\infty a(s\boldsymbol d+\rho\boldsymbol n)ds\right]d\tau.
$$

The directional [transport equation](../../../../../../transport-equation.md) is $\boldsymbol d\cdot\nabla u+au=f$ with zero incoming intensity. An [integrating factor](../../../../../../integrating-factor.md) derives this attenuation weight. The same complexification, boundary-value and jump strategy gives [spectral reconstruction of an attenuated Radon transform](../../../../../../spectral-reconstruction-of-an-attenuated-radon-transform.md) when attenuation is known. **The unattenuated inverse from part (d) applies directly only when $a=0$**; for nonzero attenuation the weighted jump and inverse must be used. This distinction allows emission imaging of the source without confusing it with reconstruction of the absorbing medium.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
