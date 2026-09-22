<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a constant-[mass density](../../../../../density.md) [incompressible flow](../../../../../incompressible-flow.md) with no imposed [body force](../../../../../body-force.md), the two-dimensional [Navier-Stokes equation](../../../../../navier-stokes-equation.md) is

$$
\boxed{\begin{aligned}
u_x+v_y&=0,\\
\rho(u_t+uu_x+vu_y)&=-p_x+\mu(u_{xx}+u_{yy}),\\
\rho(v_t+uv_x+vv_y)&=-p_y+\mu(v_{xx}+v_{yy}).
\end{aligned}}
$$

A conservative [body force](../../../../../body-force.md), if retained, may be incorporated into a modified [pressure](../../../../../pressure-split.md). Using scales $L,U_0,L/U_0$ and $\rho U_0^2$ gives

$$
\boxed{\mathrm{Re}=\frac{\rho U_0L}{\mu}=\frac{U_0L}{\nu},\qquad
\mathbf u_t+\mathbf u\cdot\nabla\mathbf u=-\nabla p+\mathrm{Re}^{-1}\nabla^2\mathbf u.}
$$

Here $\nu=\mu/\rho$ is the molecular [kinematic viscosity](../../../../../kinematic-viscosity.md). At high [Reynolds number](../../../../../reynolds-number.md), inertia and the [pressure gradient](../../../../../pressure-gradient.md) dominate on the outer length scale, while molecular viscous diffusion is small there. Thin [boundary layers](../../../../../boundary-layer.md), narrow [shear flows](../../../../../shear-flow.md) and fine turbulent scales can still have sufficiently large [velocity](../../../../../velocity.md) gradients for viscous effects to matter. High [Reynolds number](../../../../../reynolds-number.md) permits instability and [turbulence](../../../../../turbulence-split.md), but does not alone prove that every flow is turbulent. Molecular [viscous dissipation](../../../../../viscous-dissipation.md) remains essential at the small end of the turbulent cascade.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
