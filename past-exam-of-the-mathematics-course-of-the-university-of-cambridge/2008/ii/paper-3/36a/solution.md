<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

For two-dimensional [incompressible flow](../../../../../incompressible-flow.md), introduce the [stream function](../../../../../stream-function.md) by $u_r=r^{-1}\psi_\varphi$, $u_\varphi=-\psi_r$. The scalar [vorticity](../../../../../vorticity.md) is $\omega=-\nabla^2\psi$. Taking the curl of the [Stokes equations](../../../../../stokes-equation.md) $-\nabla p+\mu\nabla^2u=0$ gives $\nabla^2\omega=0$, and taking their divergence gives $\nabla^2p=0$. Thus the [biharmonic stream function for planar Stokes flow](../../../../../biharmonic-stream-function-for-planar-stokes-flow.md) satisfies $\nabla^4\psi=0$.

The far-field shear has stream function $\Gamma y^2/2=(\Gamma r^2/4)(1-\cos2\varphi)$. For a [cylinder in a simple shear Stokes flow](../../../../../cylinder-in-a-simple-shear-stokes-flow.md), the axisymmetric biharmonic terms $r^2,\log r,1$ and the angular terms $r^2,1,r^{-2}$ suffice to impose $\psi=\psi_r=0$ at $r=a$ without changing the leading far field. They give

$$
\boxed{\psi=\frac\Gamma4\left[r^2-2a^2\log(r/a)-a^2-\left(r^2-2a^2+\frac{a^4}{r^2}\right)\cos2\varphi\right].}
$$

Differentiation supplies the flow everywhere outside the cylinder:

$$
\boxed{\begin{aligned}u_r&=\frac\Gamma2\left(r-\frac{2a^2}r+\frac{a^4}{r^3}\right)\sin2\varphi,\\
u_\varphi&=\frac\Gamma2\left[-r+\frac{a^2}r+\left(r-\frac{a^4}{r^3}\right)\cos2\varphi\right],\\
p&=p_\infty-\frac{2\mu\Gamma a^2}{r^2}\sin2\varphi.
\end{aligned}}
$$

Both velocity components vanish at $r=a$, and their far-field values are precisely the cylindrical components of $(\Gamma y,0)$. The pressure follows by substitution into the [Stokes equations](../../../../../stokes-equation.md).

The tangential surface [traction](../../../../../traction.md) is $2\mu e_{r\varphi}=\mu\Gamma(2\cos2\varphi-1)$. Integrating its moment about the axis gives

$$
\boxed{\mathcal T_z=a^2\int_0^{2\pi}2\mu e_{r\varphi}\,d\varphi=-2\pi\mu\Gamma a^2.}
$$

This is the fluid's torque on the stationary cylinder, clockwise for $\Gamma>0$; the external holding torque has the opposite sign.

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
