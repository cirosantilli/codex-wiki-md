<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Write $q=|\dot{\mathbf r}|=\sqrt{\dot r^2+r^2\dot\theta^2}$. Differentiating the [angular momentum](../../../../../../angular-momentum.md) and applying [Newton's second law](../../../../../../newton-s-second-law.md) gives

$$
\begin{aligned}
\dot{\mathbf L}
&=m\dot{\mathbf r}\times\dot{\mathbf r}+m\mathbf r\times\ddot{\mathbf r}
=\mathbf r\times\mathbf F\\
&=\mathbf r\times(-\alpha q\dot{\mathbf r})
=-\frac\alpha m q\mathbf L.
\end{aligned}
$$

The [central force](../../../../../../central-force.md) contributes no [torque](../../../../../../torque.md), because it is parallel to $\mathbf r$. The [angular momentum](../../../../../../angular-momentum.md) direction is fixed whenever it is nonzero; the motion is consequently planar. In the [plane](../../../../../../plane.md)'s [polar coordinates](../../../../../../polar-coordinates.md), $\mathbf L=mh\mathbf e_z$, so

$$
\boxed{\dot h=-\frac\alpha m\sqrt{\dot r^2+r^2\dot\theta^2}\,r^2\dot\theta.}
$$

For the [mechanical energy](../../../../../../mechanical-energy.md), use the [chain rule](../../../../../../chain-rule.md), [Newton's second law](../../../../../../newton-s-second-law.md), and $V'(r)=-F_c(r)$:

$$
\begin{aligned}
\dot E
&=m\dot{\mathbf r}\cdot\ddot{\mathbf r}+V'(r)\dot r\\
&=F_c(r)\dot r-\alpha q|\dot{\mathbf r}|^2+V'(r)\dot r
=-\alpha q^3.
\end{aligned}
$$

Thus

$$
\boxed{\dot E=-\alpha(\dot r^2+r^2\dot\theta^2)^{3/2}.}
$$

For a trajectory on a time interval, both $h$ and $E$ are each a [constant of motion](../../../../../../conserved-quantity.md) precisely when $\alpha=0$ or the [velocity](../../../../../../velocity.md) vanishes throughout that interval. Under the stated strictly attractive [central force](../../../../../../central-force.md) at a regular [point](../../../../../../point-geometry.md) $r>0$, a permanently stationary trajectory is impossible by [Newton's second law](../../../../../../newton-s-second-law.md). **For the stated attractive motion, both are conserved if and only if $\alpha=0$.** An isolated instant of zero [speed](../../../../../../speed.md) only makes the [derivatives](../../../../../../derivative.md) vanish at that instant. A radial trajectory has $h=0$ even with [quadratic drag](../../../../../../quadratic-drag.md), but its [mechanical energy](../../../../../../mechanical-energy.md) still decreases whenever it moves.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [4](../../4.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
