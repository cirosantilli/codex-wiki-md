<h1 id="36e/solution">Solution</h1>

↑ **Parent:** [36E](../36e.md)

The incompressible [Navier-Stokes equations](../../../../../navier-stokes-equation.md) are $u_t+(u\cdot\nabla)u=-\nabla p/\rho+\nu\Delta u$ and $\nabla\cdot u=0$, with no penetration and no slip at a stationary rigid wall. The [Euler limit](../../../../../euler-limit.md) takes $\nu\to0$ at fixed distance from the wall, leaving the inviscid [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) and a no-penetration condition; imposing tangential no slip on that outer problem generally overdetermines it. The [Prandtl limit](../../../../../prandtl-limit.md) resolves a shrinking wall layer in which transverse viscous diffusion remains comparable to convection and restores no slip.

For the steady flat-plate [boundary layer](../../../../../boundary-layer.md), $\delta/x\ll1$, continuity makes $v/U=O(\delta/x)$, and $u_{xx}$ is small compared with $u_{yy}$. Normal momentum makes pressure independent of $y$ to leading order. The constant outer speed makes the outer pressure gradient, and hence $p_x$ throughout the layer, zero. The leading equations are $uu_x+vu_y=\nu u_{yy}$ and $u_x+v_y=0$. With the [stream function](../../../../../stream-function.md) convention $u=\psi_y$, $v=-\psi_x$, these give

$$
\psi_y\psi_{xy}-\psi_x\psi_{yy}=\nu\psi_{yyy}.
$$

Balancing $U^2/x$ against $\nu U/\delta^2$ gives $\delta=\sqrt{\nu x/U}$. There is no independent streamwise scale for the semi-infinite plate, motivating the similarity solution

$$
\boxed{\eta=y\sqrt{\frac U{\nu x}},\qquad \psi=\sqrt{\nu Ux}\,f(\eta).}
$$

It gives $u=Uf'$ and $v=\tfrac12\sqrt{\nu U/x}(\eta f'-f)$. Substitution yields $uu_x+vu_y=-U^2ff''/(2x)$ and $\nu u_{yy}=U^2f'''/x$, so the [Blasius equation](../../../../../blasius-equation.md) and conditions are

$$
\boxed{f'''+\tfrac12ff''=0,\qquad f(0)=f'(0)=0,\qquad f'(\infty)=1.}
$$

The first two conditions impose no penetration and no slip; the last matches the outer stream.

The wall shear on one face is $\tau(x)=\rho\nu u_y(x,0)=\rho U\sqrt{\nu U/x}\,f''(0)$. Integration from zero to $L$ gives $2\rho U^2Lf''(0)/\sqrt{UL/\nu}$ on one face. With the same flow on both faces, the total [drag force](../../../../../drag-physics.md) per unit width is

$$
\boxed{F=\frac{4\rho U^2L}{\sqrt{UL/\nu}}\frac{f''(0)}{[f'(\infty)]^2}.}
$$

Our normalization has $f'(\infty)=1$, so the displayed denominator is one. The factor four refers to both faces; for a plate wetted on only one face the drag is half this value.

## ↑ Ancestors (10)

1. [36E](../36e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
