<h1 id="section-a/a4/solution">Solution</h1>

↑ **Parent:** [A4](../a4.md)

The original PDF calls $\epsilon_r$ a relative [magnetic permeability](../../../../../permeability-electromagnetism.md) while also specifying a nonmagnetic [dielectric](../../../../../dielectric.md). These descriptions are inconsistent if read literally. The physically consistent interpretation of the notation is [relative permittivity](../../../../../relative-permittivity.md) $\epsilon_r=2$ and relative [magnetic permeability](../../../../../permeability-electromagnetism.md) $\mu_r=1$.

Let $a=3\,\mathrm{mm}$ and let $b=6\,\mathrm{mm}$ be the inner radius of the outer conductor. For line charge density $\lambda$, [Gauss's law](../../../../../gauss-s-law.md) gives $E_r=\lambda/(2\pi\epsilon r)$, hence

$$
V=\int_a^b E_r\,dr=\frac{\lambda}{2\pi\epsilon}\ln\frac ba,
\qquad C'=\frac\lambda V=\frac{2\pi\epsilon_0\epsilon_r}{\ln(b/a)}.
$$

The [magnetic field](../../../../../magnetic-field-split.md) in the [dielectric](../../../../../dielectric.md) is $H_\varphi=I/(2\pi r)$. Its [energy](../../../../../energy-split.md) per unit length gives

$$
\frac12L'I^2=\int_a^b\frac{\mu H_\varphi^2}{2}\,2\pi r\,dr,
\qquad L'=\frac{\mu_0\mu_r}{2\pi}\ln\frac ba.
$$

Using $b/a=2$,

$$
\boxed{C'=1.61\times10^{-10}\,\mathrm{F\,m^{-1}}=161\,\mathrm{pF\,m^{-1}},}
$$



$$
\boxed{L'=1.39\times10^{-7}\,\mathrm{H\,m^{-1}}=139\,\mathrm{nH\,m^{-1}}.}
$$

These are the [lossless coaxial line parameters](../../../../../lossless-coaxial-line-parameters.md), assuming negligible field penetration into the conductors. If the quoted radii instead referred to an outer diameter or if $\mu_r=2$ were intended, the data would need clarification; the stated [dielectric](../../../../../dielectric.md) and nonmagnetic assumptions support the interpretation above.

## ↑ Ancestors (14)

1. [A4](../a4.md)
2. [Section A](../../section-a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
