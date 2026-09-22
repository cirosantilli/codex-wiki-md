<h1 id="38a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u(r,z)$ and $w(r,z)$ be the radial and vertical velocity components. For steady incompressible [axisymmetric flow](../../../../../../axisymmetric-flow.md) without swirl, [mass conservation](../../../../../../mass-conservation.md) and the relevant cylindrical components of the [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) are

$$
\frac1r\frac{\partial(ru)}{\partial r}+\frac{\partial w}{\partial z}=0,
$$



$$
\rho\left(u\frac{\partial u}{\partial r}+w\frac{\partial u}{\partial z}\right)
=-\frac{\partial p}{\partial r}
+\mu\left(\frac{\partial^2u}{\partial r^2}+\frac1r\frac{\partial u}{\partial r}-\frac{u}{r^2}+\frac{\partial^2u}{\partial z^2}\right),
$$



$$
\rho\left(u\frac{\partial w}{\partial r}+w\frac{\partial w}{\partial z}\right)
=-\frac{\partial p}{\partial z}
+\mu\left(\frac{\partial^2w}{\partial r^2}+\frac1r\frac{\partial w}{\partial r}+\frac{\partial^2w}{\partial z^2}\right).
$$

The vertical scale is $w\sim V$. [Incompressibility](../../../../../../incompressible-flow.md) over radial scale $R$ and gap scale $h$ gives $u\sim VR/h=V/\varepsilon$. In the radial equation, inertia is smaller than transverse viscous stress by

$$
\frac{\rho Vh}{\mu}=\operatorname{Re}\ll1,
$$

while radial viscous derivatives are smaller than $u_{zz}$ by $\varepsilon^2$. The pressure scale is $\mu VR^2/h^3$. In the vertical equation, both viscous and inertial terms are smaller than the corresponding cross-gap pressure-gradient scale by at least $O(\varepsilon^2)$. Thus the leading [lubrication theory](../../../../../../lubrication-theory.md) equations are

$$
\boxed{\frac1r(ru)_r+w_z=0,
\qquad p_r=\mu u_{zz},
\qquad p_z=0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38A](../../38a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
