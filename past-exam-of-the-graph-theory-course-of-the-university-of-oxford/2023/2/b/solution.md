<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the nonempty [connected components of a graph](../../../../component-graph-theory.md) of $G$ be $G_1,\ldots,G_t$. A [proper vertex colouring](../../../../proper-vertex-coloring.md) can be chosen separately on each [connected component of a graph](../../../../component-graph-theory.md), since no [edge](../../../../edge-of-a-graph.md) joins different [connected components of a graph](../../../../component-graph-theory.md). The [multiplication principle](../../../../rule-of-product.md) gives, first at positive [integers](../../../../integer-split.md) and then as a [polynomial identity](../../../../polynomial-identity.md),

$$
p_G(x)=\prod_{j=1}^t p_{G_j}(x).
$$

It remains to justify that every factor has zero constant term. More generally, for every nonempty [simple graph](../../../../simple-graph.md) $H$, prove $p_H(0)=0$ by [mathematical induction](../../../../mathematical-induction.md) on the number of [edges](../../../../edge-of-a-graph.md). If there are no [edges](../../../../edge-of-a-graph.md), then $p_H(x)=x^{|V(H)|}$ with $|V(H)|\geq1$. Otherwise choose an [edge](../../../../edge-of-a-graph.md) $e$. Both $H-e$ and the simplified [edge contraction](../../../../edge-contraction.md) $H/e$ are nonempty [graphs](../../../../graph-split.md) with fewer [edges](../../../../edge-of-a-graph.md). The [deletion-contraction recurrence for the chromatic polynomial](../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) and [mathematical induction](../../../../mathematical-induction.md) give

$$
p_H(0)=p_{H-e}(0)-p_{H/e}(0)=0.
$$

Thus $p_{G_j}(x)=xq_j(x)$ for a [polynomial](../../../../polynomial-split.md) $q_j$, and

$$
\boxed{p_G(x)=x^t\prod_{j=1}^t q_j(x),\qquad x^t\mid p_G(x).}
$$

For the empty [graph](../../../../graph-split.md), $t=0$ and $p_G(x)=1$, so the conclusion also holds. This is the [chromatic polynomial product over components](../../../../chromatic-polynomial-product-over-components.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
