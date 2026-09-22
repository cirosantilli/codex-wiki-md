<h1 id="38b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $x$ tangential to the solid boundary and locally along the outer inviscid streamlines, and let $y$ be the inward normal coordinate. Write $u$ and $v$ for the corresponding tangential and normal [velocity field](../../../../../../velocity-field.md) components, $U(x)$ for the outer tangential velocity, and $\nu$ for the [kinematic viscosity](../../../../../../kinematic-viscosity.md).

For a layer of streamwise scale $L$ and thickness $\delta\ll L$, [incompressible flow](../../../../../../incompressible-flow.md) gives

$$
u_x+v_y=0,
$$

so $u=O(U)$ and $v=O(U\delta/L)$. The normal [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) then gives $p_y=0$ to leading order, while the outer [Euler equations](../../../../../../euler-equations-for-an-inviscid-fluid.md) give

$$
-\frac1\rho p_x=U\frac{dU}{dx}.
$$

In the tangential Navier-Stokes equation, streamwise viscous diffusion is smaller than normal diffusion by $O((\delta/L)^2)$. Retaining the leading inertial and normal-diffusion terms produces the [Prandtl boundary-layer equation](../../../../../../prandtl-boundary-layer-equation.md)

$$
\boxed{u u_x+v u_y=U\frac{dU}{dx}+\nu u_{yy}}.
$$

It is supplemented by $u=v=0$ at a stationary wall and $u\to U(x)$ on matching to the outer flow.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38B](../../38b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
