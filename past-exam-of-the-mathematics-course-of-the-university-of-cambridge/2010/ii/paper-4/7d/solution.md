<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

A useful version of the [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) says that a forward orbit of a continuously differentiable planar autonomous vector field which stays in a compact set has a nonempty compact omega-limit set; if that omega-limit set contains no equilibrium, it is a [periodic orbit](../../../../../periodic-orbit.md).

Let $r^2=x^2+y^2$. Direct calculation gives

$$
r\dot r=\frac14x^2(1-2r^2)+\frac12y^2(1-r^2),\qquad
\dot\theta=-1+\frac{xy}{4r^2}.
$$

For $r>0$, $|xy|\le r^2/2$, so $-9/8\le\dot\theta\le-7/8$. In particular **there is no equilibrium away from the origin**.

On $r=1/2$, both coefficients in the radial expression are strictly positive, so the flow crosses outward. On $r=2$, both are strictly negative, so the flow crosses inward. Consequently the compact annulus

$$
\boxed{D=\{(x,y):1/4\le x^2+y^2\le4\}}
$$

is forward invariant. Any orbit starting there stays there, and its omega-limit set avoids the only equilibrium, the origin. The [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) therefore supplies **at least one [periodic orbit](../../../../../periodic-orbit.md) in this annulus**.

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
