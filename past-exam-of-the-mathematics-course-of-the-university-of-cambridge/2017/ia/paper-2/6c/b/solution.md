<h1 id="6c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $r>0$, differentiate $r^2=x^2+y^2$ and use the angular derivative $(x\dot y-y\dot x)/r^2$. The [polar coordinates](../../../../../../polar-coordinates.md) satisfy

$$
\boxed{\dot r=r(1-r^2),\qquad\dot\theta=-1.}
$$

Hence the rotation is clockwise. The origin is an [unstable equilibrium](../../../../../../unstable-equilibrium.md), while $r=1$ is a [limit cycle](../../../../../../limit-cycle.md) of period $2\pi$. Writing $u=r^2$ gives the [logistic differential equation](../../../../../../logistic-differential-equation.md) $\dot u=2u(1-u)$. For $r(t_0)=r_0>0$,

$$
\boxed{r(t)^2=\frac1{1+(r_0^{-2}-1)e^{-2(t-t_0)}},\qquad
\theta(t)=\theta_0-(t-t_0).}
$$

All nonzero solutions tend to the [unit-circle attracting limit cycle](../../../../../../unit-circle-attracting-limit-cycle.md) as $t\to\infty$, spiralling outward for $r_0<1$ and inward for $r_0>1$. For $0<r_0<1$ the solution exists for every real time and approaches the origin as $t\to-\infty$; for $r_0=1$ it remains periodic in both time directions. For $r_0>1$, the denominator first vanishes at

$$
\boxed{t_*=t_0+\frac12\log(1-r_0^{-2}),\qquad r(t)\to\infty\text{ as }t\downarrow t_*.}
$$

This [finite-time blow-up of an ordinary differential equation](../../../../../../finite-time-blow-up-of-an-ordinary-differential-equation.md) occurs backward in time. Such exterior solutions have no $t\to-\infty$ behavior: their maximal time interval is $(t_*,\infty)$. The zero solution exists for all time and has no defined polar angle.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6C](../../6c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
