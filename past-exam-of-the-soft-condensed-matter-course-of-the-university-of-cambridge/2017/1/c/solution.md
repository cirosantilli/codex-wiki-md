<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the membrane height above its mean plane as a sum of [Fourier modes](../../../../fourier-mode.md), $h(\mathbf r)=\sum_{\mathbf q}h_{\mathbf q}e^{i\mathbf q\cdot\mathbf r}$. The supplied average is a thermal mean-squared modal height; for complex Fourier coefficients it is understood as $\langle|h_{\mathbf q}|^2\rangle$, with $h_{-\mathbf q}=h_{\mathbf q}^*$ for a real height field. The terms are:

- $k_BT$ is the thermal energy, with [Boltzmann constant](../../../../boltzmann-constant.md) $k_B$ and absolute [temperature](../../../../temperature-split.md) $T$.
- $A$ is the projected membrane [area](../../../../surface-area.md) used in the Fourier normalization.
- $q=|\mathbf q|$ is the in-plane [wavenumber](../../../../wavenumber.md); the corresponding [wavelength](../../../../wavelength.md) is $2\pi/q$.
- $\sigma$ is the [membrane tension](../../../../membrane-tension.md), in $\mathrm{N\,m^{-1}}=\mathrm{J\,m^{-2}}$.
- $\kappa$ is the [membrane bending modulus](../../../../membrane-bending-modulus.md), in joules.

In the small-slope approximation, [Helfrich membrane energy](../../../../thermal-membrane-undulation.md) contains

$$
F=\frac12\int_A[\sigma|\nabla h|^2+\kappa(\nabla^2h)^2],d^2r
=\frac A2\sum_{\mathbf q}(\sigma q^2+\kappa q^4)|h_{\mathbf q}|^2.
$$

The [equipartition theorem](../../../../equipartition-theorem.md), with the independent real modes counted consistently, gives the stated [membrane fluctuation spectrum under tension](../../../../membrane-fluctuation-spectrum-under-tension.md). Its units are length squared: $\sigma q^2$ and $\kappa q^4$ both have units $\mathrm{J\,m^{-4}}$, so $k_BT/[A(\sigma q^2+\kappa q^4)]$ has units $\mathrm{m^2}$.

At small length scales, $q$ is large and the bending term dominates:

$$
\boxed{\langle|h_{\mathbf q}|^2\rangle\simeq\frac{k_BT}{A\kappa q^4}
\quad\text{for }q\gg\sqrt{\sigma/\kappa}.}
$$

The fluctuation [amplitude](../../../../wave-amplitude.md) is controlled mainly by the [membrane bending modulus](../../../../membrane-bending-modulus.md) and thermal energy, rather than tension. The crossover occurs when $\sigma q_c^2=\kappa q_c^4$, hence

$$
\boxed{q_c=\sqrt{\frac\sigma\kappa},\qquad
\ell_c\equiv q_c^{-1}=\sqrt{\frac\kappa\sigma},\qquad
\lambda_c=2\pi\sqrt{\frac\kappa\sigma}.}
$$

The bending-dominated regime extends up to the [membrane elastic length](../../../../membrane-elastic-length.md) when scale means $1/q$, or up to $\lambda_c$ when it means [wavelength](../../../../wavelength.md). At still larger scales tension gives a $q^{-2}$ spectrum. At the opposite end, the continuum formula requires [wavelengths](../../../../wavelength.md) larger than the microscopic membrane thickness or molecular cutoff. Without numerical $\kappa$ and $\sigma$, no numerical crossover scale is determined.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
