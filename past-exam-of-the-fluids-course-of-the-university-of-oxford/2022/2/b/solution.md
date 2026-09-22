<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [stream function](../../../../stream-function.md) convention $u=-\psi_y$, $v=\psi_x$, so that this is an incoming [stagnation point](../../../../stagnation-point.md) flow rather than the reversed flow. The [velocity field](../../../../velocity-field.md) is

$$
u=Ax,\qquad v=-Ay.
$$

At the plate $v(x,0)=0$, satisfying the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md). The nonzero tangential [velocity](../../../../velocity.md) $u(x,0)=Ax$ is permitted for an [inviscid flow](../../../../inviscid-flow.md); the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) is not imposed on the [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md).

The steady [convective acceleration](../../../../convective-acceleration.md) is $(A^2x,A^2y)$. Thus the [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md) require

$$
p_x=-\rho A^2x,\qquad p_y=-\rho A^2y-\rho g.
$$

Integrating gives

$$
\boxed{p_\infty(x,y)=p_0-\frac{\rho A^2}{2}(x^2+y^2)-\rho gy.}
$$

**The printed formula omits $\rho$ from its quadratic term.** The source uses physical [pressure](../../../../pressure-split.md), not [pressure](../../../../pressure-split.md) divided by [mass density](../../../../density.md), as is clear from its $\rho gy$ term and its [Navier-Stokes equation](../../../../navier-stokes-equation.md). The omitted factor is also required by [dimensional analysis](../../../../dimensional-analysis.md). For a concrete substitution check, the printed expression gives $-p_x/\rho=A^2x/\rho$ rather than the required $A^2x$ when $\rho\ne1$ in the chosen numerical units.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
