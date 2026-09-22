<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In winding sector m write the lifted path as

$$
\phi(\tau)=\phi_0+\frac{2\pi m\tau}{\beta}+\eta(\tau),\qquad \eta(0)=\eta(\beta)=0.
$$

The cross term vanishes since $\int_0^\beta\dot\eta\,d\tau=0$. The action separates into $I(2\pi m)^2/(2\hbar^2\beta)$ and the same fixed-endpoint [Gaussian path integral](../../../../../gaussian-path-integral.md) for every m. Neither term depends on the initial angle, so its integral supplies $2\pi$:

$$
\boxed{Z=2\pi Z_0\sum_m e^{-I(2\pi m)^2/(2\hbar^2\beta)},\qquad
Z_0=\int_{\eta(0)=\eta(\beta)=0}\mathcal D\eta\,
e^{-I\int_0^\beta\dot\eta^2d\tau/(2\hbar^2)}.}
$$

The [fixed-endpoint rotor fluctuation normalization](../../../../../fixed-endpoint-rotor-fluctuation-normalization.md) is

$$
\boxed{Z_0=\sqrt{\frac{I}{2\pi\hbar^2\beta}}.}
$$

It is the diagonal free-particle thermal kernel on the lifted line, or the amplitude density for a zero-displacement fluctuation bridge. It is not by itself the circle partition function or a separately countable angular zero mode. The integration over $\phi_0$ has already counted that mode. Quadraticity makes the saddle-plus-fluctuation evaluation exact.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter Field Theory course of the University of Cambridge](../../../../../quantum-condensed-matter-field-theory-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
