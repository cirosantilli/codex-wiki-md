<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [scattering phase shift](../../../../../scattering-phase-shift.md) measures the change of a [partial wave](../../../../../partial-wave.md)'s outgoing phase relative to the free radial solution. For a real [central potential](../../../../../central-potential.md) and [elastic scattering](../../../../../elastic-scattering.md), [probability](../../../../../probability.md) conservation gives a unit-modulus [Partial-wave S-matrix](../../../../../partial-wave-s-matrix.md) $S_l=e^{2i\delta_l}$. Indeed

$$
e^{i\delta_l}\sin(z+\delta_l)
=\frac{e^{2i\delta_l}e^{iz}-e^{-iz}}{2i},
\qquad z=kr-l\pi/2,
$$

so the incoming amplitude is unchanged and the outgoing one acquires $S_l$.

Expanding an incident [plane wave](../../../../../plane-wave.md) in [Legendre polynomials](../../../../../legendre-polynomial.md) and comparing the outgoing [spherical wave](../../../../../spherical-wave.md) gives

$$
f(\theta)=\frac1k\sum_{l=0}^\infty
(2l+1)e^{i\delta_l}\sin\delta_l\,P_l(\cos\theta).
$$

Use $d\sigma/d\Omega=|f|^2$ and $\int d\Omega\,P_lP_{l'}=4\pi\delta_{ll'}/(2l+1)$ to remove cross terms:

$$
\boxed{\sigma=\frac{4\pi}{k^2}
\sum_{l=0}^\infty(2l+1)\sin^2\delta_l.}
$$

This is the elastic total [scattering cross-section](../../../../../scattering-cross-section.md) for the one-particle central-potential problem, with no identical-particle symmetrization factor.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
