<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [divergence](../../../../divergence.md) in [polar coordinates](../../../../polar-coordinates.md) and the given [streamfunction](../../../../stream-function.md) convention yield

$$
\nabla\cdot\mathbf v
=\frac1r\partial_r(rv_r)+\frac1r\partial_\theta v_\theta
=\frac1r\left(\partial_r\partial_\theta\psi-\partial_\theta\partial_r\psi\right)=0.
$$

Thus the [incompressibility condition](../../../../incompressible-flow.md) holds wherever the mixed [partial derivatives](../../../../partial-derivative.md) commute. The vertical [vorticity](../../../../vorticity-split.md) is

$$
\zeta=\frac1r\left[\partial_r(rv_\theta)-\partial_\theta v_r\right]
=-\left(\partial_r^2+\frac1r\partial_r+\frac1{r^2}\partial_\theta^2\right)\psi
=-\nabla^2\psi.
$$

Neglecting both inertial terms in the [Navier-Stokes equation](../../../../navier-stokes-equation.md), for constant [dynamic viscosity](../../../../dynamic-viscosity-split.md) and [mass density](../../../../density.md), gives the [Stokes equation](../../../../stokes-equation.md):

$$
0=-\nabla p+\mu\nabla^2\mathbf v-\rho g\widehat{\mathbf z}.
$$

Its [curl](../../../../curl.md) eliminates the [pressure gradient](../../../../pressure-gradient.md) and the uniform gravitational [body force](../../../../body-force.md), so $\mu\nabla^2\zeta=0$. Hence the [biharmonic streamfunction](../../../../biharmonic-stream-function-for-planar-stokes-flow.md) satisfies

$$
\boxed{\nabla^4\psi\approx0.}
$$

This conclusion requires the [quasi-steady Stokes approximation](../../../../quasi-steady-stokes-approximation.md). If local [acceleration](../../../../acceleration.md) were retained, the corresponding planar [vorticity equation](../../../../vorticity-equation.md) would instead be $\partial_t\nabla^2\psi=\nu\nabla^4\psi$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
