<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md),

$$
\mathbf e_r=(\cos\theta,\sin\theta,0),\quad
\mathbf e_\theta=(-\sin\theta,\cos\theta,0),\quad
\dot{\mathbf e}_r=\dot\theta\mathbf e_\theta,\quad
\dot{\mathbf e}_\theta=-\dot\theta\mathbf e_r.
$$

Differentiating the [position vector](../../../../../../position-vector.md) $\mathbf r=r\mathbf e_r+z\mathbf e_z$ twice gives the [velocity](../../../../../../velocity.md) and [acceleration](../../../../../../acceleration.md)

$$
\begin{aligned}
\dot{\mathbf r}&=\dot r\mathbf e_r+r\dot\theta\mathbf e_\theta+\dot z\mathbf e_z,\\
\ddot{\mathbf r}&=(\ddot r-r\dot\theta^2)\mathbf e_r
+(r\ddot\theta+2\dot r\dot\theta)\mathbf e_\theta+\ddot z\mathbf e_z.
\end{aligned}
$$

This derives [acceleration in cylindrical coordinates](../../../../../../acceleration-in-cylindrical-coordinates.md) rather than assuming it.

At a fixed time, the wire has [parametrization](../../../../../../parametric-equation.md) $r\mapsto r\mathbf e_r+f(r)\mathbf e_z$. Its [derivative](../../../../../../derivative.md) is the nonzero [tangent vector](../../../../../../tangent-vector-split.md)

$$
\mathbf t=\mathbf e_r+f'(r)\mathbf e_z.
$$

A smooth wire exerts a [constraint force](../../../../../../constraint-force.md) $\mathbf R$ with $\mathbf R\cdot\mathbf t=0$. Because $g$ is the [gravitational acceleration](../../../../../../gravitational-acceleration.md), the gravitational [force](../../../../../../force-split.md) is $-mg\mathbf e_z$; the printed $-g\mathbf e_z$ is interpreted per unit mass. Projecting [Newton's second law](../../../../../../newton-s-second-law.md), $m\ddot{\mathbf r}=\mathbf R-mg\mathbf e_z$, along $\mathbf t$ eliminates $\mathbf R$:

$$
\ddot r-r\omega^2+f'(r)\ddot z=-gf'(r).
$$

The [chain rule](../../../../../../chain-rule.md) gives $\ddot z=f'(r)\ddot r+f''(r)\dot r^2$. Rearrangement yields

$$
\boxed{\left(1+f'(r)^2\right)\ddot r
=r\omega^2-f'(r)\left(g+f''(r)\dot r^2\right).}
$$

This is the governing equation for a [bead on a uniformly rotating wire](../../../../../../bead-on-a-uniformly-rotating-wire.md). Its azimuthal [acceleration](../../../../../../acceleration.md) contributes nothing to the projection because $\mathbf e_\theta\cdot\mathbf t=0$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
