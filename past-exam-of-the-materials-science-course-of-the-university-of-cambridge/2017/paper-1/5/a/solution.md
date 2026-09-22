<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Measure $x$ from the clamped end and let downward deflection $y$ be positive. In the small-slope [elastic beam](../../../../../elastic-beam.md) model, the [bending moment](../../../../../bending-moment.md) has magnitude $M(x)=F(l-x)$ and $EIy''=M(x)$. Integrating with $y(0)=y'(0)=0$ gives

$$
y'(x)=\frac F{EI}\left(lx-\frac{x^2}{2}\right),\qquad y(x)=\frac F{EI}\left(\frac{lx^2}{2}-\frac{x^3}{6}\right).
$$

For the rectangular cross-section, $I=wh^3/12=6.75\times10^{-7}\,\mathrm{m^4}$, and therefore

$$
\boxed{\delta=y(l)=\frac{Fl^3}{3EI}=\frac{4mgl^3}{Ewh^3}.}
$$

Requiring $\delta\le0.2\,\mathrm m$ with $F=1079.1\,\mathrm N$ yields

$$
E\ge\frac{4(110)(9.81)(3)^3}{(0.3)(0.03)^3(0.2)}=\boxed{71.94\,\mathrm{GPa}.}
$$

This calculation neglects beam self-weight as stipulated, and also transverse shear deformation and geometric nonlinearities. The end slope at the limit is $3\delta/(2l)=0.10$, so the small-slope approximation is reasonable for the intended estimate. Meeting a stiffness specification alone does not establish safe strength or fatigue life.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the materials science course of the University of Cambridge](../../../../split.md)
6. [Materials science course of the University of Cambridge](../../../../../materials-science-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
