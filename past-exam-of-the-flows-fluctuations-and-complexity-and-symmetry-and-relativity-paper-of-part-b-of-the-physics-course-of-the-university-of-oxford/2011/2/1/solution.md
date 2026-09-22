<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\mu$ for [dynamic viscosity](../../../../dynamic-viscosity-split.md) and $\nu=\mu/\rho$ for [kinematic viscosity](../../../../kinematic-viscosity.md), consistently with the introductory [Navier-Stokes equation](../../../../navier-stokes-equation.md). The phrase “dynamic viscosity $\nu$” in this request mixes these conventions. A fully developed [plane Poiseuille flow](../../../../plane-poiseuille-flow.md), $\mathbf u=(u(z),0,0)$, has zero [convective acceleration](../../../../convective-acceleration.md). The [Navier-Stokes equation](../../../../navier-stokes-equation.md) gives $\mu u''=-f$ and $p_z=-\rho g$. Applying the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) at both stationary plates gives

$$
\boxed{u(z)=\frac{f}{2\mu}z(b-z)=\frac{f}{2\rho\nu}z(b-z).}
$$

The material coefficients must be effectively constant and positive. The profile is an exact parallel-flow solution for every $\mu>0$; experimental validity additionally requires that the realized flow remain in the [laminar flow](../../../../laminar-flow.md) regime. A sufficient conservative condition is

$$
\boxed{\mathrm{Re}=\frac{\bar u b}{\nu}=\frac{fb^3}{12\rho\nu^2}\ll1,
\qquad \bar u=\frac{fb^2}{12\mu}.}
$$

Equivalently $\nu\gg\sqrt{fb^3/(12\rho)}$, or $\mu\gg\sqrt{\rho fb^3/12}$. This sufficient bound is stronger than necessary; there is no need to discard [convective acceleration](../../../../convective-acceleration.md) by an approximation here because it vanishes identically for the assumed profile.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity and symmetry and relativity paper of Part B of the physics course of the University of Oxford](../../../../flows-fluctuations-and-complexity-and-symmetry-and-relativity-paper-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
