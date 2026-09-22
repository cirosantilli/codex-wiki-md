<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $z$ increase down the pipe, $a=0.015\,\mathrm m$ be its radius and $r$ the distance from its axis. For steady, fully developed [laminar flow](../../../../laminar-flow.md) of a [Newtonian fluid](../../../../newtonian-fluid.md), the axial [Navier-Stokes equations](../../../../navier-stokes-equation.md) reduce to

$$
0=-\frac{dp}{dz}+\eta\frac1r\frac d{dr}\left(r\frac{du}{dr}\right)+\rho g\sin20^\circ.
$$

Write $K=-dp/dz+\rho g\sin20^\circ$. Integrating twice, regularity at $r=0$ excludes a logarithmic term, and the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) $u(a)=0$ gives the [Hagen-Poiseuille flow](../../../../hagen-poiseuille-equation.md) profile

$$
\boxed{u(r)=\frac{K}{4\eta}(a^2-r^2).}
$$

The [volumetric flow rate](../../../../volumetric-flow-rate.md) follows by integrating over the circular cross-section:

$$
Q=2\pi\int_0^a u(r)r\,dr
=\frac{\pi Ka^4}{8\eta},\qquad
\overline u=\frac{Q}{\pi a^2}=\frac{Ka^2}{8\eta}=\frac{u(0)}2.
$$

For the intended gravity-driven case with no imposed axial [pressure gradient](../../../../pressure-gradient.md), $dp/dz=0$. Substitution gives

$$
\boxed{u(r)\simeq0.2095\left[1-\left(\frac{r}{0.015\,\mathrm m}\right)^2\right]\mathrm{m\,s^{-1}},}
$$

and

$$
\boxed{Q\simeq7.40\times10^{-5}\,\mathrm{m^3\,s^{-1}}
=74.0\,\mathrm{mL\,s^{-1}}\simeq4.44\,\mathrm{L\,min^{-1}}.}
$$

The corresponding mean speed is about $0.1047\,\mathrm{m\,s^{-1}}$ and the diameter-based [Reynolds number](../../../../reynolds-number.md) is $\rho\overline u(2a)/\eta\simeq3.49$, consistent with [laminar flow](../../../../laminar-flow.md). The original PDF does not specify inlet and outlet pressures. If they impose an additional [pressure gradient](../../../../pressure-gradient.md), the general result with $K$ above applies; gravity alone does not determine that extra contribution.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
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
