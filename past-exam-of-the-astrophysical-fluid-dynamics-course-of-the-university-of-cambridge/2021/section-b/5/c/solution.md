<h1 id="section-b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The particle count is the enclosed mass divided by the particle mass $m$:

$$
N(\xi)=\frac{4\pi\rho_ca^3}{m}\int_0^\xi s^2e^{-\Psi(s)}\,ds.
$$

Integrating the [isothermal Lane-Emden equation](../../../../../isothermal-lane-emden-equation.md) gives

$$
\int_0^\xi s^2e^{-\Psi(s)}\,ds
=\left[s^2\Psi'(s)\right]_0^\xi=\xi^2\Psi'(\xi),
$$

where regularity makes the lower endpoint vanish. Thus

$$
\boxed{N(\xi)=\frac{4\pi\rho_c}{m}
\left(\frac{K}{4\pi G\rho_c}\right)^{3/2}\xi^2\Psi'(\xi).}
$$

The prefactor is a mass divided by a mass, and the remaining factor is dimensionless. In particular, at fixed $K$ the dependence on central [mass density](../../../../../density.md) is $N\propto\rho_c^{-1/2}f(\xi)$, with $f(\xi)=\xi^2\Psi'(\xi)$. Both changes must be retained when comparing equilibria at fixed $N$.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
