<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $z$ measure distance across the narrow gap and let $\theta$ be polar angle about the tube axis. In [lubrication theory](../../../../../../lubrication-theory.md), radial velocity and radial pressure variation are negligible. Axisymmetric [incompressible flow](../../../../../../incompressible-flow.md) is obtained from

$$
u_\theta(\theta,z)=\frac{\phi(z)}{\sin\theta},
$$

because $\partial_\theta(u_\theta\sin\theta)=0$. The tangential [Stokes equation](../../../../../../stokes-equation.md) then separates:

$$
\sin\theta\frac{\partial p}{\partial\theta}
=\mu R\frac{d^2\phi}{dz^2}=a,
$$

and hence, after choosing an irrelevant pressure constant,

$$
\boxed{p(\theta)=\frac a2
\log\frac{1-\cos\theta}{1+\cos\theta}}.
$$

In the sphere frame, $u_z=-u_\theta\sin\theta=-\phi$. The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) gives $\phi(0)=0$ on the sphere and $\phi(\delta)=U$ on the membrane translating backward relative to it. The sphere-frame volume flux inherited from the narrow remote tube is $-\pi r_0^2U$, so

$$
2\pi R\int_0^\delta\phi(z)\,dz=\pi r_0^2U.
$$

Under the asymptotic condition $r_0^2\ll R\delta$, the right-hand side is negligible at leading order. Solving the quadratic profile subject to the two wall values and zero leading-order integral gives

$$
\boxed{\phi(z)=U\left[3\left(\frac z\delta\right)^2
-2\frac z\delta\right]},
\qquad
\boxed{a=\frac{6\mu RU}{\delta^2}}.
$$

Changing the chosen positive tube direction reverses both signs but leaves the drag magnitude unchanged.

The pressure scale is $p\sim\mu UR/\delta^2$, whereas the viscous shear scale is $\tau\sim\mu U/\delta$. After multiplication by comparable areas, pressure drag exceeds shear drag by $R/\delta\gg1$, an instance of [lubrication pressure dominates shear stress](../../../../../../lubrication-pressure-dominates-shear-stress.md). Put $c=\cos\Delta\theta$. The axial pressure force is

$$
F_p=2\pi R^2\int_{\Delta\theta}^{\pi-\Delta\theta}
p(\theta)\sin\theta\cos\theta\,d\theta
$$



$$
=\pi aR^2\left[
-2c+(1-c^2)\log\frac{1+c}{1-c}
\right].
$$

As $\Delta\theta\to0$, the bracket tends to $-2$, and therefore

$$
F_p\sim-\frac{12\pi\mu R^3}{\delta^2}U.
$$

The resulting [confined-sphere drag coefficient](../../../../../../confined-sphere-drag-coefficient.md) is

$$
\boxed{\zeta_{\rm tube}=\frac{12\pi\mu R^3}{\delta^2}
=\left(6\pi\mu R\right)\frac{2R^2}{\delta^2}}.
$$

Thus it exceeds the free [Stokes drag law](../../../../../../stokes-s-law.md) coefficient by $2R^2/\delta^2$. The [Stokes–Einstein relation](../../../../../../stokes-einstein-relation.md) then gives

$$
\boxed{D_{\rm tube}=\frac{k_BT}{\zeta_{\rm tube}}
=D_0\frac{\delta^2}{2R^2}},
\qquad
D_0=\frac{k_BT}{6\pi\mu R}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
