<h1 id="34c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real short-range [spherically symmetric potential](../../../../../../spherically-symmetric-potential.md), the stationary [wavefunction](../../../../../../wave-function.md) must solve the [Schrödinger equation](../../../../../../schrodinger-equation.md), be regular at the origin whenever the potential is finite there, and satisfy the scattering boundary condition

$$
\psi(\mathbf r)\sim e^{ikz}+f(\theta)\frac{e^{ikr}}r
\qquad(r\to\infty).
$$

Here $e^{ikz}$ is the incident [plane wave](../../../../../../plane-wave.md), the second term is an outgoing spherical wave, and its coefficient $f(\theta)$ is the [scattering amplitude](../../../../../../scattering-amplitude.md).

Comparing the stated asymptotic expression with the [partial-wave expansion of a scattering amplitude](../../../../../../partial-wave-expansion-of-a-scattering-amplitude.md) gives

$$
f(\theta)=\frac1k\sum_{l=0}^{\infty}(2l+1)f_lP_l(\cos\theta),
$$

where $P_l$ is a [Legendre polynomial](../../../../../../legendre-polynomial.md). The outgoing-to-incoming coefficient in channel $l$ is

$$
S_l=1+2if_l.
$$

[Partial-wave unitarity](../../../../../../partial-wave-unitarity.md) requires

$$
|S_l|=1,
$$

or equivalently

$$
\operatorname{Im}f_l=|f_l|^2.
$$

The real [scattering phase shift](../../../../../../scattering-phase-shift.md) $\delta_l$ is defined modulo $\pi$ by

$$
\boxed{S_l=e^{2i\delta_l},
\qquad
f_l=\frac{e^{2i\delta_l}-1}{2i}
=e^{i\delta_l}\sin\delta_l.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34C](../../34c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
