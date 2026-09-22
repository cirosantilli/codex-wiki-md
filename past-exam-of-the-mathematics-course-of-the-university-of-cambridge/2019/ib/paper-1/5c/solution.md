<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Take $x$ down the plane and $y$ normally away from it, with the solid at $y=0$ and the [free surface](../../../../../free-surface.md) at $y=h$. A steady unidirectional [falling film flow](../../../../../falling-film-flow.md) has velocity $\mathbf u=u(y)\mathbf e_x$. The streamwise [Navier-Stokes equation](../../../../../navier-stokes-equation.md) reduces to

$$
\nu u''=-g\sin\alpha,
$$

where $\nu$ is the [kinematic viscosity](../../../../../kinematic-viscosity.md). The lower [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and upper [stress-free boundary condition](../../../../../stress-free-boundary-condition.md) are

$$
u(0)=0,
\qquad
u'(h)=0.
$$

Integrating gives the velocity profile

$$
\boxed{u(y)=\frac{g\sin\alpha}{\nu}\left(hy-\frac{y^2}{2}\right)}.
$$

The [volume flux](../../../../../volumetric-flow-rate.md) per unit width is

$$
\boxed{Q=\int_0^hu(y)\,dy=\frac{g h^3\sin\alpha}{3\nu}}.
$$

If the upper surface is replaced by a stationary solid plane, the second boundary condition becomes $u(h)=0$. The resulting plane-channel profile and flux are

$$
u(y)=\frac{g\sin\alpha}{2\nu}y(h-y),
\qquad
\boxed{Q_{\rm closed}=\frac{g h^3\sin\alpha}{12\nu}=\frac14Q}.
$$

The free surface exerts no tangential [shear stress](../../../../../shear-stress.md), whereas the stationary upper wall enforces no slip and exerts a retarding shear. This additional drag accounts for the reduced flux.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
