<h1 id="section-b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expand the axisymmetric [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid-split.md) about the rotating equilibrium, retaining only terms linear in $u_r,u_\phi,u_z$ and in the [pressure](../../../../../pressure-split.md) perturbation. The symbol in this question is the [kinematic pressure](../../../../../kinematic-pressure.md) perturbation,

$$
\boxed{\pi(r,z,t)=\frac{p(r,z,t)-p_0(r)}\rho,\qquad[\pi]=\mathrm{m^2\,s^{-2}}.}
$$

The linearized centripetal term in the radial equation is $-2\Omega u_\phi$, after subtracting the equilibrium term $-r\Omega^2$. Radial advection of the background azimuthal [velocity](../../../../../velocity.md), together with the cylindrical-coordinate term $u_rv_\phi/r$, gives

$$
\left[\frac d{dr}(r\Omega)+\Omega\right]u_r
=(2\Omega+r\Omega')u_r
=\frac1r\frac d{dr}(r^2\Omega)u_r.
$$

This is the azimuthal coupling in the second equation; it also expresses conservation of [specific angular momentum](../../../../../specific-angular-momentum.md) $j=r^2\Omega$ for a radially displaced element. The axial equation is acceleration balanced by $-\partial_z\pi$. Finally, the axisymmetric [incompressible flow](../../../../../incompressible-flow.md) condition in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) is

$$
\frac1r\partial_r(ru_r)+\partial_zu_z=0,
$$

which expands to the last supplied equation. Background azimuthal advection contributes no $\Omega\partial_\phi$ term because the perturbations are axisymmetric.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [6](../../6.md)
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
