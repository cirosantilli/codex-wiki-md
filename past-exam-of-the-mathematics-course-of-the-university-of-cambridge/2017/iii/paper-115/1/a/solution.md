<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A smooth real [vector bundle](../../../../../../vector-bundle.md) of [vector bundle rank](../../../../../../rank-of-a-vector-bundle.md) $r$ consists of a [smooth manifold](../../../../../../smooth-manifold.md) $E$, a smooth projection $\pi:E\to M$, real [vector space](../../../../../../vector-space-split.md) structures on its fibers, and local [vector bundle trivializations](../../../../../../vector-bundle-trivialization.md)

$$
\Phi_U:\pi^{-1}(U)\longrightarrow U\times\mathbb R^r
$$

that commute with projection to $U$ and are [linear isomorphisms](../../../../../../linear-isomorphism.md) on each fiber. On overlaps the change of trivialization is $(p,v)\mapsto(p,g_{VU}(p)v)$, with $g_{VU}:U\cap V\to GL_r(\mathbb R)$ smooth into the [general linear group](../../../../../../general-linear-group.md). The usual [smooth manifold](../../../../../../smooth-manifold.md) convention is [Hausdorff](../../../../../../hausdorff-space.md) and [second countable](../../../../../../second-countable-space.md).

For an $n$-dimensional $M$, take the disjoint union of its [tangent spaces](../../../../../../tangent-space.md). A [manifold chart](../../../../../../manifold-chart.md) $x:U\to\mathbb R^n$ supplies

$$
\Phi_x(v_p)=(p,dx_p(v_p)),\qquad
\widetilde\Phi_x(v_p)=(x(p),dx_p(v_p)).
$$

If $y$ is another chart, the resulting change of coordinates on the total space is

$$
(a,v)\longmapsto\bigl(y\circ x^{-1}(a),D(y\circ x^{-1})_a v\bigr).
$$

This is smooth, its inverse is the same construction with $x,y$ exchanged, and the fiber map is invertible and linear. Thus these charts define a smooth structure with the required bundle trivializations.

For completeness, the topology so constructed is [Hausdorff](../../../../../../hausdorff-space.md): different base points can be separated downstairs, while vectors over one point can be separated inside one product chart. A countable base atlas for $M$ and countable bases for its products with $\mathbb R^n$ give [second countability](../../../../../../second-countable-space.md). Hence the total space is genuinely a [smooth manifold](../../../../../../smooth-manifold.md), not just a collection of fibers. We obtain

$$
\boxed{TM\longrightarrow M\text{ is a smooth vector bundle of rank }n.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
