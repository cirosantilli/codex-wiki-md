<h1 id="3g/solution">Solution</h1>

↑ **Parent:** [3G](../3g.md)

On the unit three-ball $B^3$, the distance in the [Poincare ball model](../../../../../poincare-ball-model.md) is the infimum of the lengths

$$
L(\gamma)=\int\frac{2|\gamma'(t)|}{1-|\gamma(t)|^2}\,dt
$$

over piecewise smooth paths joining the two points. Equivalently the [hyperbolic metric](../../../../../hyperbolic-metric.md) as a metric-space distance is

$$
\boxed{d(x,y)=\operatorname{arcosh}\left(1+\frac{2|x-y|^2}{(1-|x|^2)(1-|y|^2)}\right).}
$$

It has curvature-minus-one normalization; in particular $d(0,x)=2\operatorname{artanh}|x|$.

For a nonempty finite set $p_1,\ldots,p_m$, define $R(x)=\max_jd(x,p_j)$. The triangle inequality gives $|R(x)-R(y)|\leq d(x,y)$, so $R$ is continuous. Take $R_0=R(p_1)$. Any improving center satisfies $d(x,p_1)\leq R(x)\leq R_0$, and thus lies in the closed hyperbolic ball $K=\overline B(p_1,R_0)$.

This ball is compact: an [isometry](../../../../../isometry.md) sending $p_1$ to the origin identifies it with the Euclidean closed ball of radius $\tanh(R_0/2)<1$, and the Euclidean and hyperbolic topologies agree inside $B^3$. The continuous function $R$ attains a minimum on $K$. Centers outside $K$ have $R>R_0$, so this is also the global minimum. Its associated closed ball proves **a minimum enclosing ball in [hyperbolic space](../../../../../hyperbolic-space.md) exists**. For the empty finite set, any center and radius zero suffice.

## ↑ Ancestors (10)

1. [3G](../3g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
