<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

For a smooth surface the [friction](../../../../../../friction.md) force vanishes. The $\mathbf e_\theta$ component of [Newton's second law](../../../../../../newton-s-second-law.md) then gives $r^2\dot\theta=h$, constant. Along the [constraint](../../../../../../constraint-mechanics.md) $z=H(r)$, the [chain rule](../../../../../../chain-rule.md) gives

$$
\dot z=H'\dot r,\qquad\ddot z=H'\ddot r+H''\dot r^2.
$$

The [acceleration in cylindrical coordinates](../../../../../../acceleration-in-cylindrical-coordinates.md) is

$$
\ddot{\mathbf r}=(\ddot r-r\dot\theta^2)\mathbf e_r+(r\ddot\theta+2\dot r\dot\theta)\mathbf e_\theta+\ddot z\mathbf e_z.
$$

Take the [dot product](../../../../../../dot-product.md) of [Newton's second law](../../../../../../newton-s-second-law.md) with the [tangent vector](../../../../../../tangent-vector-split.md) $\mathbf e_r+H'\mathbf e_z$. The [normal force](../../../../../../normal-force.md) disappears, while the [gravity](../../../../../../gravity.md) term is $-mgH'$. Dividing by $m$ gives

$$
\ddot r-r\dot\theta^2+H'(H'\ddot r+H''\dot r^2)=-gH'.
$$

Using $\dot\theta=h/r^2$ yields

$$
\boxed{[1+(H')^2]\ddot r+H'H''\dot r^2-\frac{h^2}{r^3}=-gH'.}
$$

## ↑ Ancestors (12)

1. [b](../b.md)
2. [5](../../5.md)
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
