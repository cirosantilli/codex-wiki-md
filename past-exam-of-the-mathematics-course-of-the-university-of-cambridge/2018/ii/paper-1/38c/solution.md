<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

At the rigid surface, the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and no penetration give

$$
\boxed{u=v=0\qquad(y=0).}
$$

At the horizontal [free surface](../../../../../free-surface.md), the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) and the [stress boundary condition](../../../../../stress-boundary-condition.md) are

$$
\boxed{v=\dot h,
\qquad \sigma_{xy}=0,
\qquad \sigma_{yy}=-p_{
m air}
=-p_0+\frac12\rho_aE^2x^2
\qquad(y=h).}
$$

Here surface tension is absent and the inviscid air exerts no tangential traction.

The incompressible [Stokes equation](../../../../../stokes-equation.md) is

$$
-\nabla p+\mu\nabla^2\mathbf u=0,
\qquad \nabla\mathbin\cdot\mathbf u=0.
$$

Use the [Cartesian streamfunction](../../../../../cartesian-streamfunction.md) convention $u=\psi_y$, $v=-\psi_x$ and set

$$
\psi=xf(y).
$$

Then

$$
u=xf'(y),
\qquad v=-f(y),
$$

and the wall and zero-shear conditions become

$$
f(0)=f'(0)=0,
\qquad f''(h)=0.
$$

The two momentum equations read

$$
p_x=\mu x f'''(y),
\qquad p_y=-\mu f''(y).
$$

Equality of mixed derivatives gives $f^{(4)}=0$, so the boundary conditions imply

$$
f(y)=C\left(y^3-3hy^2\right).
$$

Integrating for the pressure and imposing the normal-stress condition at $y=h$ determines

$$
C=-\frac{\rho_aE^2}{6\mu}.
$$

The complete instantaneous velocity and pressure fields are therefore

$$
\boxed{u=\frac{\rho_aE^2}{2\mu}xy(2h-y),
\qquad
v=-\frac{\rho_aE^2}{6\mu}y^2(3h-y),}
$$



$$
\boxed{p=p_0-\frac{\rho_aE^2}{2}
\left(x^2+2hy-y^2+h^2\right).}
$$

Indeed, with the [viscous stress tensor](../../../../../viscous-stress-tensor.md) $\sigma=-pI+\mu(\nabla\mathbf u+\nabla\mathbf u^T)$, these expressions satisfy both traction conditions. Evaluating the vertical velocity at the material surface gives the [pressure-driven thinning of a uniform Stokes layer](../../../../../pressure-driven-thinning-of-a-uniform-stokes-layer.md):

$$
\dot h=v(h)=-\frac{\rho_aE^2}{3\mu}h^3.
$$

Thus

$$
\boxed{V=-\frac{dh}{dt}=\frac13\frac{\rho_a}{\mu}E^2h^3.}
$$

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
