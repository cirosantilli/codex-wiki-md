<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

In [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md), $\theta=\omega t$ and $z=r^2/(2a)$. Thus

$$
\dot z=\frac ra\dot r,\qquad \ddot z=\frac{r\ddot r+\dot r^2}{a}.
$$

The [acceleration](../../../../../../acceleration.md) is

$$
\mathbf A=(\ddot r-r\omega^2)\mathbf e_r+2\omega\dot r\mathbf e_\theta+\frac{r\ddot r+\dot r^2}{a}\mathbf e_z.
$$

A [tangent vector](../../../../../../tangent-vector-split.md) along the wire is $\mathbf t=\mathbf e_r+(r/a)\mathbf e_z$. Because the wire is smooth, its [constraint force](../../../../../../constraint-force.md) is [orthogonal](../../../../../../orthogonal-vectors.md) to $\mathbf t$. Taking the [dot product](../../../../../../dot-product.md) of [Newton's second law](../../../../../../newton-s-second-law.md) with $\mathbf t$ eliminates that [force](../../../../../../force-split.md); [gravitational weight](../../../../../../weight-physics.md) contributes $-mgr/a$. Hence

$$
m\left[\ddot r-r\omega^2+\frac r{a^2}(r\ddot r+\dot r^2)\right]=-\frac{mgr}{a}.
$$

Multiplying by $a^2/m$ gives

$$
\boxed{(a^2+r^2)\ddot r+r\dot r^2-a^2\omega^2r=-agr.}
$$

## ↑ Ancestors (12)

1. [a](../a.md)
2. [6](../../6.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
