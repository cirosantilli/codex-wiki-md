<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $k_D$ be the donor's total decay rate without acceptors, including radiative and nonradiative decay, and let $k_T$ be its transfer rate to one acceptor. In weak excitation, independent equivalent acceptors supply additive transfer rates, so [FRET efficiency](../../../../fret-efficiency.md) is

$$
E=\frac{k_T}{k_D+k_T},\qquad
E_n=\frac{nk_T}{k_D+nk_T}.
$$

Eliminating $k_T/k_D=E/(1-E)$ gives

$$
\boxed{E_n=\frac{nE}{1+(n-1)E}}.
$$

This assumes the same [Förster distance](../../../../forster-distance.md), equivalent donor–acceptor distances and unchanged donor decay, with no acceptor saturation or other transfer pathways affecting donor de-excitation.

For [Förster resonance energy transfer](../../../../forster-resonance-energy-transfer.md), $k_T/k_D=(R_0/R)^6$, hence

$$
E_n=\frac{n(R_0/R)^6}{1+n(R_0/R)^6},\qquad
\boxed{R=R_0\left[\frac{n(1-E_n)}{E_n}\right]^{1/6}
=6(2/3)^{1/6}\,\mathrm{nm}\simeq5.61\,\mathrm{nm}}.
$$

Here the single-pair [FRET efficiency](../../../../fret-efficiency.md) would be $E=0.60$, which indeed produces $E_2=0.75$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
