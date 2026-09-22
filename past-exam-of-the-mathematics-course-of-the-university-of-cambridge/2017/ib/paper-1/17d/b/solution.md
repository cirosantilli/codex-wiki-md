<h1 id="17d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an [inclined viscous film with opposing surface shear](../../../../../../inclined-viscous-film-with-opposing-surface-shear.md), the steady parallel velocity automatically satisfies the [continuity equation](../../../../../../continuity-equation.md) and the advective acceleration vanishes. The two components of the [Navier-Stokes equations](../../../../../../navier-stokes-equation.md) reduce to

$$
0=-p_x+\mu u''+\rho g\sin\alpha,\qquad0=-p_z-\rho g\cos\alpha.
$$

The uniform thickness and constant atmospheric pressure make $p_x=0$. The boundary conditions are

$$
u(0)=0,\qquad\mu u'(h)=-S,\qquad p(h)=p_{\rm atm}.
$$

These are respectively [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md), imposed tangential [traction](../../../../../../traction.md) on the surface with outward normal $+\mathbf e_z$, and the normal stress condition on the flat free surface. The normal viscous stress is zero because the normal velocity vanishes. Integrating gives

$$
\boxed{u(z)=\frac{\rho g\sin\alpha}{\mu}\left(hz-\frac{z^2}{2}\right)-\frac S\mu z,\qquad p(z)=p_{\rm atm}+\rho g\cos\alpha(h-z)}.
$$

In particular $\mu u'(0)=\rho gh\sin\alpha-S$ is the downslope tangential [traction](../../../../../../traction.md) exerted by the fluid on the wall. The wall's tangential [traction](../../../../../../traction.md) on the fluid has the opposite sign, because the outward normal of the fluid at its bottom is $-\mathbf e_z$. This fixes the potentially confusing wall sign convention.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17D](../../17d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
