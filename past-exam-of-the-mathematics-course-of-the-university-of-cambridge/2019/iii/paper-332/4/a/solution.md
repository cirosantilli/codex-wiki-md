<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\ell=(H_m-H_0)/\sin\alpha$ be the along-slope distance to the [snowline](../../../../../../snowline.md), so $H(x)=H_m-x\sin\alpha$ and $a(x)=A(1-x/\ell)$. Define $D=g\sin\alpha/(3\nu)$.

Treat ice as an incompressible [Newtonian fluid](../../../../../../newtonian-fluid.md), neglect inertia, and use [lubrication theory](../../../../../../lubrication-theory.md) with thickness measured normal to the slope. The bed has a [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md), the [free surface](../../../../../../free-surface.md) has zero tangential stress, and normal pressure is hydrostatic. The small thickness slope allows its pressure-gradient contribution to be neglected against gravity along the mountain. With normal coordinate $y$, the tangential equation and boundary conditions are

$$
\nu u_{yy}=-g\sin\alpha,\qquad u(0)=0,\qquad u_y(h)=0.
$$

Integration gives

$$
u=\frac{g\sin\alpha}{\nu}\left(hy-\frac{y^2}{2}\right),\qquad q=\int_0^h u\,dy=Dh^3.
$$

The horizontal radius of a ring is $x\cos\alpha$, so [mass conservation](../../../../../../mass-conservation.md) gives the [gravity-driven ice flow on a conical slope](../../../../../../gravity-driven-ice-flow-on-a-conical-slope.md) equation

$$
\boxed{h_t+\frac1x\partial_x(xDh^3)=A\left(1-\frac x\ell\right).}
$$

Negative accumulation is [ice ablation](../../../../../../ice-ablation.md) and applies only where ice exists; the ice-free region has $h=0$.

In a steady state, regularity and zero total flux at the apex require $xDh^3\to0$ as $x\to0$. Integrating gives

$$
Dx h_s^3=A\left(\frac{x^2}{2}-\frac{x^3}{3\ell}\right).
$$

Requiring a continuous zero-thickness steady terminus yields the [steady conical ice cap with a linear accumulation gradient](../../../../../../steady-conical-ice-cap-with-a-linear-accumulation-gradient.md):

$$
\boxed{h_s(x)=\left[\frac AD\left(\frac x2-\frac{x^2}{3\ell}\right)\right]^{1/3},\qquad x_N=\frac32\ell.}
$$

The terminus lies below the [snowline](../../../../../../snowline.md), allowing the ablation region to balance snowfall. The maximum thickness occurs at $x=3\ell/4$.

The volume follows from integrating the ring areas. With $s=x/\ell$,

$$
V_0=2\pi\cos\alpha\left(\frac AD\right)^{1/3}\ell^{7/3}\int_0^{3/2}s\left(\frac s2-\frac{s^2}{3}\right)^{1/3}ds.
$$

Substituting $D$ and $\ell=\Delta H/\sin\alpha$ gives

$$
\boxed{V_0=\lambda\left(\frac{\nu A\Delta H^7}{g\sin^8\alpha}\right)^{1/3}\cos\alpha,\qquad \lambda=2\pi3^{1/3}\int_0^{3/2}s\left(\frac s2-\frac{s^2}{3}\right)^{1/3}ds.}
$$

The ideal outer profile has steep slopes very close to the apex and terminus. Those small regions require local corrections to the assumed slope balance, while the bulk profile and leading volume follow from the stated approximation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
