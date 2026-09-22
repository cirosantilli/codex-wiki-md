<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first equation expresses horizontal [incompressibility](../../../../incompressible-flow.md). The other two express steady balance of the [Coriolis force](../../../../coriolis-force.md), a [geopotential](../../../../geopotential.md) gradient, [linear drag](../../../../linear-drag.md) and a prescribed zonal acceleration $F_u(y)$; nonlinear [advection](../../../../advection.md) has been neglected. The parameter $r>0$ is an inverse drag time, so the frictional acceleration is $-r(u,v)$. On the equatorial [beta plane](../../../../beta-plane.md), $f=\beta y$.

Use the [streamfunction](../../../../stream-function.md) convention

$$
u=-\psi_y,\qquad v=\psi_x,\qquad \zeta=v_x-u_y=\nabla_h^2\psi.
$$

Take $\partial_x$ of the meridional momentum equation minus $\partial_y$ of the zonal one. The mixed [geopotential](../../../../geopotential.md) [derivatives](../../../../derivative.md) cancel, and

$$
f(u_x+v_y)+\beta v=-r(v_x-u_y)-\frac{dF_u}{dy}.
$$

Horizontal [incompressibility](../../../../incompressible-flow.md) removes the first term, leaving

$$
\boxed{\beta\psi_x+r\nabla_h^2\psi=F_\zeta(y),\qquad F_\zeta=-\frac{dF_u}{dy}.}
$$

The right side is the vertical [curl](../../../../curl.md) of the imposed acceleration, with units $\mathrm{s^{-2}}$. The left side balances [planetary vorticity](../../../../planetary-vorticity.md) [advection](../../../../advection.md) and frictional removal of [relative vorticity](../../../../relative-vorticity.md). The [streamfunction](../../../../stream-function.md) has units $\mathrm{m^2\,s^{-1}}$, since it describes horizontal [velocity](../../../../velocity.md), rather than depth-integrated [volume flux](../../../../volumetric-flow-rate.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
