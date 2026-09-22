<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The horizontal velocities $u$ and $v$ point east and north, $\eta$ is the displacement of the free surface from its mean level, $H_0$ is the undisturbed depth, $g$ is gravitational acceleration, and $f$ is the constant [Coriolis parameter](../../../../../../coriolis-parameter.md) on an [f-plane](../../../../../../f-plane.md). The three [linearized shallow water equations](../../../../../../linearized-shallow-water-equations.md) are horizontal momentum balance and [mass conservation](../../../../../../mass-conservation.md):

$$
u_t-fv=-g\eta_x,\qquad
v_t+fu=-g\eta_y,\qquad
\eta_t+H_0(u_x+v_y)=0.
$$

They follow from the rotating [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) by assuming an inviscid homogeneous layer, [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), horizontal scales much larger than $H_0$, depth-independent horizontal velocity, a flat impermeable bottom, constant $f$, and small surface displacement and velocity so that nonlinear products are neglected.

In a steady state, [geostrophic balance](../../../../../../geostrophic-balance.md) gives

$$
\boxed{u_g=-\frac gf\eta_y},
\qquad
\boxed{v_g=\frac gf\eta_x}.
$$

The relative vorticity is $\zeta=v_x-u_y$. Expanding the [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md) $(f+\zeta)/(H_0+\eta)$ to first order gives

$$
\frac f{H_0}+\frac1{H_0}
\left(\zeta-\frac f{H_0}\eta\right).
$$

Thus one convenient normalization of its disturbance is

$$
\boxed{q=\zeta-\frac f{H_0}\eta}.
$$

Taking the curl of momentum and using continuity shows $q_t=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
