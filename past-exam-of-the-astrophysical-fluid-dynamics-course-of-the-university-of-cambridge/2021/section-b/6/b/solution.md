<h1 id="section-b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a homogeneous [Newtonian fluid](../../../../../newtonian-fluid.md) with constant [kinematic viscosity](../../../../../kinematic-viscosity.md) $\nu>0$, assume the same steady purely azimuthal flow. In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), the azimuthal [Navier-Stokes equation](../../../../../navier-stokes-equation.md) has no pressure forcing or convective term in this state, and becomes

$$
0=\nu\left[\frac{d^2v_\phi}{dr^2}+\frac1r\frac{dv_\phi}{dr}-\frac{v_\phi}{r^2}\right],\qquad v_\phi=r\Omega.
$$

Equivalently, $\Omega''+3\Omega'/r=0$, or $(r^3\Omega')'=0$. Two integrations give the [steady circular Couette profile](../../../../../steady-circular-couette-profile.md),

$$
\boxed{\Omega(r)=A+\frac B{r^2},\qquad v_\phi(r)=Ar+\frac Br.}
$$

This is the basic [Taylor-Couette flow](../../../../../taylor-couette-flow.md) between rotating cylinders. The constants depend on boundary [angular velocities](../../../../../angular-velocity.md); for radii $R_<,R_>$ and prescribed [angular velocities](../../../../../angular-velocity.md) $\Omega_<,\Omega_>$,

$$
A=\frac{\Omega_>R_>^2-\Omega_<R_<^2}{R_>^2-R_<^2},\qquad
B=\frac{R_<^2R_>^2(\Omega_<-\Omega_>)}{R_>^2-R_<^2}.
$$

If the domain includes $r=0$, regularity requires $B=0$, leaving [solid-body rotation](../../../../../solid-body-rotation.md). On an annulus a nonzero $B$ is allowed and wall torques maintain the shear.

The restriction concerns a steady profile. An arbitrary initial [angular velocity](../../../../../angular-velocity.md) does not cease to exist when [viscosity](../../../../../dynamic-viscosity-split.md) is introduced; within the purely azimuthal ansatz it evolves according to $\partial_t\Omega=\nu(\Omega''+3\Omega'/r)$ until compatible boundary conditions and angular-momentum constraints determine its long-time state.

## ↑ Ancestors (14)

1. [B](../b.md)
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
