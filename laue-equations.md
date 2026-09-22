# Laue equations

↑ **Parent:** [X-ray diffraction](x-ray-diffraction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laue_equations)

For incident and outgoing unit propagation vectors $\mathbf s_{\rm in}$ and $\mathbf s_{\rm out}$, [wavelength](wavelength.md) $\lambda>0$, and [primitive lattice translation vectors](primitive-lattice-translation-vector.md) $a_1,a_2,a_3$, the [Laue equations](laue-equations.md) are

$$
a_1\cdot(\mathbf s_{\rm out}-\mathbf s_{\rm in})=h\lambda,\qquad
a_2\cdot(\mathbf s_{\rm out}-\mathbf s_{\rm in})=k\lambda,\qquad
a_3\cdot(\mathbf s_{\rm out}-\mathbf s_{\rm in})=l\lambda,
\qquad (h,k,l)\in\mathbb Z^3.
$$

All three must hold for the same [wavelength](wavelength.md) and outgoing direction. The integers label a [reciprocal lattice](reciprocal-lattice.md) vector; they need not be coprime. For [wavevectors](wavevector.md) $\mathbf k_{\rm in,out}=(2\pi/\lambda)\mathbf s_{\rm in,out}$, equivalently

$$
\mathbf G=\mathbf k_{\rm out}-\mathbf k_{\rm in}=h b_1+k b_2+l b_3,\qquad a_i\cdot b_j=2\pi\delta_{ij}.
$$

This uses angular [wavenumbers](wavenumber.md); the crystallographic convention without $2\pi$ instead uses $\mathbf s/\lambda$.[Online Dictionary of Crystallography by International Union of Crystallography; Definition: three scalar conditions and reciprocal form](online-dictionary-of-crystallography-by-international-union-of-crystallography/laue-equations.md)

For a short proof, translate a scatterer through $a_i$. Its incident [wave phase](phase-waves.md) changes by $\mathbf k_{\rm in}\cdot a_i$ and propagation to the same distant observation direction contributes $-\mathbf k_{\rm out}\cdot a_i$. The relative [wave phase](phase-waves.md) factor is therefore $\exp(-i\mathbf G\cdot a_i)$. It equals one for all [lattice translations](lattice-translation.md) exactly when $\mathbf G$ belongs to the [reciprocal lattice](reciprocal-lattice.md). A finite [crystal lattice structure factor](crystal-lattice-structure-factor.md) broadens the ideal maxima; the [crystal basis structure factor](crystal-basis-structure-factor.md) can cancel them. Geometric phase matching is necessary for a sharp reflection, but does not guarantee a visible spot.

For [elastic scattering](elastic-scattering.md), the additional constraint is

$$
|\mathbf k_{\rm in}+\mathbf G|^2=|\mathbf k_{\rm in}|^2,
\qquad 2\mathbf k_{\rm in}\cdot\mathbf G+|\mathbf G|^2=0.
$$

It is an [Ewald sphere](ewald-sphere.md) centered at $-\mathbf k_{\rm in}$ in the space of transfer vectors $\mathbf G$. The parent [elastic Bragg scattering condition](elastic-bragg-scattering-condition.md) uses $q=\mathbf k_{\rm in}-\mathbf k_{\rm out}=-\mathbf G$, so its displayed condition has the opposite sign. Both give [Bragg's law](bragg-s-law.md) for the same [lattice planes](lattice-plane.md).

## ↑ Ancestors (8)

1. [X-ray diffraction](x-ray-diffraction.md)
2. [Crystal scattering](crystal-scattering.md)
3. [Scattering amplitude](scattering-amplitude.md)
4. [Quantum scattering](quantum-scattering-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Calculated transmission Laue pattern](calculated-transmission-laue-pattern.md)
- [Lattice translation](lattice-translation.md)
- [Laue equations](laue-equations.md)
- [Laue method](laue-method.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-2/section-c/c11/solution.md)
- [X-ray diffraction](x-ray-diffraction.md)
