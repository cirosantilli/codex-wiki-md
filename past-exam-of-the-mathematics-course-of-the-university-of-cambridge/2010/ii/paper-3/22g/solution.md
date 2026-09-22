<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

A meromorphic function on the [Riemann sphere](../../../../../riemann-sphere.md) is rational: it has finitely many poles; subtract their principal parts, including a [polynomial](../../../../../polynomial-split.md) for a possible pole at infinity, and the remaining entire function is bounded at infinity, hence constant by [Liouville theorem](../../../../../liouville-theorem.md). A [rational map](../../../../../rational-map-complex-analysis.md) of degree $d$ has $d$ preimages of a regular value, counted with multiplicity. An analytic isomorphism is bijective, so $d=1$, giving precisely

$$
\boxed{z\longmapsto\frac{az+b}{cz+d},\qquad ad-bc\ne0.}
$$

Conversely these [Möbius transformations](../../../../../mobius-transformation.md) have a Möbius inverse and extend holomorphically at their pole and infinity, so are analytic isomorphisms.

For a nonconstant [analytic map](../../../../../biholomorphism.md) $f:X\to Y$ between compact connected [Riemann surfaces](../../../../../riemann-surfaces.md), the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) is

$$
\boxed{2g_X-2=d(2g_Y-2)+\sum_{p\in X}(e_p-1).}
$$

Here $g_X,g_Y$ are genera, $d$ is the degree (the sum of local multiplicities over any fiber), and $e_p$ is the local degree in coordinates where the map has the form $z\mapsto z^{e_p}$. Only finitely many terms are nonzero; these are the ramification points.

For a degree-two [sphere](../../../../../sphere.md) map the formula gives total ramification two. Each local degree is at most two, so there are exactly two distinct ramification points, each of local degree two. Their branch values are distinct, because one fiber cannot have multiplicity four. Choose $T$ sending $0,\infty$ to the two ramification points, and $S$ sending their values to $0,\infty$. Then $SfT$ has its only zero at zero, of order two, and its only pole at infinity, of order two; it is $cz^2$ with $c\ne0$. Rescale $S$ by $1/c$. Therefore **$SfT(z)=z^2$**, as required.

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
