<h1 id="38b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $x$ point down the plane and $z$ normal to it, with velocity $(u,w)$. The two-dimensional incompressible [Navier-Stokes equation](../../../../../../navier-stokes-equation.md) is

$$
u_x+w_z=0,
$$



$$
u_t+uu_x+wu_z
=-\frac1\rho p_x+\nu(u_{xx}+u_{zz})+g\sin\alpha,
$$



$$
w_t+uw_x+ww_z
=-\frac1\rho p_z+\nu(w_{xx}+w_{zz})-g\cos\alpha.
$$

The [lubrication theory](../../../../../../lubrication-theory.md) limit has film thickness much smaller than its streamwise length. Transverse viscous derivatives dominate, inertia is negligible at late times, and the leading equations are

$$
0=-\frac1\rho p_x+\nu u_{zz}+g\sin\alpha,
\qquad
0=-\frac1\rho p_z-g\cos\alpha.
$$

At the wall, $u=w=0$ by the [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md). At the free surface $z=h(x,t)$, take $p=p_{\rm atm}$ and $u_z=0$, neglecting surface tension. The normal balance gives the [hydrostatic pressure](../../../../../../hydrostatic-pressure.md)

$$
p=p_{\rm atm}+\rho g\cos\alpha\,(h-z),
\qquad
\frac{p_x}{\rho}=g\cos\alpha\,h_x.
$$

If the current has thickness scale $H$ and length scale $L$, then

$$
\frac{|p_x|/\rho}{g\sin\alpha}
\sim\frac HL\cot\alpha\ll1.
$$

Thus the streamwise pressure gradient is asymptotically smaller than the downslope body force for a fixed nonzero inclination. The streamwise equation becomes

$$
\nu u_{zz}=-g\sin\alpha.
$$

Using $u(0)=0$ and $u_z(h)=0$ gives

$$
u(z)=\frac{g\sin\alpha}{\nu}
\left(hz-\frac{z^2}{2}\right).
$$

The [volume flux](../../../../../../volumetric-flow-rate.md) is

$$
q=\int_0^hu\,dz
=\frac{g\sin\alpha}{3\nu}h^3.
$$

Integrating incompressibility across the film and using the [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) gives $h_t+q_x=0$, hence

$$
\boxed{
h_t+\frac{\partial}{\partial x}
\left(\frac{gh^3\sin\alpha}{3\nu}\right)=0
}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [38B](../../38b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
