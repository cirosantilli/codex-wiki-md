<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $z$ measure distance normal to the plane, with the wall at $z=0$ and the [free surface](../../../../../../free-surface.md) at $z=h$. Take density $\rho$, dynamic viscosity $\mu$, and gravitational acceleration $g$. In [lubrication theory](../../../../../../lubrication-theory.md), normal momentum balance gives [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) while inertia and streamwise viscous derivatives are smaller. With negligible [surface tension](../../../../../../surface-tension.md) and negligible air shear,

$$
p=p_{\mathrm{atm}}+\rho g\cos\alpha\,(h-z),\qquad
\mu u_{zz}=\rho g(\cos\alpha\,h_x-\sin\alpha),\qquad
\mu v_{zz}=\rho g\cos\alpha\,h_y.
$$

Apply the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) $u=v=0$ at $z=0$, and zero leading tangential stress $u_z=v_z=0$ at $z=h$. The velocity profiles are

$$
u=\frac{\rho g}{\mu}(\sin\alpha-\cos\alpha\,h_x)(hz-z^2/2),\qquad
v=-\frac{\rho g}{\mu}\cos\alpha\,h_y(hz-z^2/2).
$$

Depth integration gives the [volume flux](../../../../../../volumetric-flow-rate.md), with $K=\rho g/(3\mu)$:

$$
q_x=Kh^3(\sin\alpha-\cos\alpha\,h_x),\qquad
q_y=-Kh^3\cos\alpha\,h_y.
$$

Combining [incompressibility](../../../../../../incompressible-flow.md) with the wall and surface kinematic conditions gives [conservation of mass](../../../../../../mass-conservation.md), $h_t+\partial_xq_x+\partial_yq_y=0$. Therefore the two-dimensional version of the [gravity-driven thin film on an incline](../../../../../../gravity-driven-thin-film-on-an-incline.md) satisfies

$$
\boxed{h_t+K\sin\alpha\,\partial_x(h^3)
=K\cos\alpha\left[\partial_x(h^3h_x)+\partial_y(h^3h_y)\right].}
$$

Direct downslope gravity supplies the advective term, while gradients of the [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) spread the film along the surface. At $\alpha=0$ this reduces to nonlinear gravitational spreading in a horizontal film.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
