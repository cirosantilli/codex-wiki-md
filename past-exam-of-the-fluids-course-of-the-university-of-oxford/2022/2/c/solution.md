<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A stationary viscous wall imposes the [no-slip boundary condition](../../../../no-slip-boundary-condition.md), $u=v=0$, whereas the outer [inviscid flow](../../../../inviscid-flow.md) has $u=Ax$. At large [Reynolds number](../../../../reynolds-number.md), the transition is confined to a thin [viscous boundary layer](../../../../viscous-boundary-layer.md), where normal [velocity gradients](../../../../velocity-gradient.md) amplify the otherwise small viscous term.

Take a horizontal scale $L$, an outer speed $U=AL$, and a [boundary layer thickness](../../../../boundary-layer-thickness.md) $\delta\ll L$. The [continuity equation](../../../../continuity-equation.md) gives $v=O(U\delta/L)$. Write $\epsilon=\delta/L$ and $\mathrm{Re}_L=UL/\nu$. The tangential [Navier-Stokes equation](../../../../navier-stokes-equation.md) has scales

$$
u u_x+v u_y=O(U^2/L),\qquad
\nu u_{yy}=O(\nu U/\delta^2),\qquad
\frac{\nu u_{xx}}{\nu u_{yy}}=O(\epsilon^2).
$$

Balancing [convective acceleration](../../../../convective-acceleration.md) with normal viscous diffusion gives $\epsilon=O(\mathrm{Re}_L^{-1/2})$. The leading tangential equation and [incompressible flow](../../../../incompressible-flow.md) constraint are

$$
\boxed{u u_x+v u_y=-\frac1\rho\frac{\partial p_\infty}{\partial x}+\nu u_{yy},\qquad
u_x+v_y=0.}
$$

Here and below $\nu$ is the [kinematic viscosity](../../../../kinematic-viscosity.md), while $u$ is the horizontal [velocity](../../../../velocity.md).

For the normal equation, first remove the [hydrostatic pressure](../../../../hydrostatic-pressure.md) by writing $P=p+\rho gy$. Normal [inertia](../../../../inertia.md) and normal viscous terms are $O(\rho U^2\delta/L^2)$, so the change of $P$ across the layer is only $O(\rho U^2\epsilon^2)$. Matching to the outer [pressure](../../../../pressure-split.md) therefore makes the leading $O(\rho U^2)$ excess [pressure](../../../../pressure-split.md) independent of $y$:

$$
P(x,y)=P_e(x)+O(\rho U^2\epsilon^2),\qquad
p_y=-\rho g+O(\rho U^2\delta/L^2).
$$

The outer expression similarly has $(p_\infty)_y=-\rho g-\rho A^2y$. Thus the printed condition

$$
\boxed{p_y=(p_\infty)_y}
$$

is a **leading-order [boundary layer](../../../../boundary-layer.md) matching statement**, with the smaller normal dynamic terms discarded on both sides. It is not an exact identity at the next order. In particular, retaining the outer $-\rho A^2y$ while dropping normal [inertia](../../../../inertia.md) and normal viscous terms inconsistently mixes orders. The tangential driving term is unambiguous: $-(p_\infty)_x/\rho=A^2x$.

## ↑ Ancestors (12)

1. [C](../c.md)
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
