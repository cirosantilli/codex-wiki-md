<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $V=V(G)$ and $E=E(G)$. For $F\subseteq E$, let $c(F)$ denote the number of [connected components of a graph](../../../../component-graph-theory.md) of the spanning [subgraph](../../../../subgraph.md) $(V,F)$, including isolated [vertices](../../../../vertex-graph-theory.md). The [inclusion-exclusion principle](../../../../inclusion-exclusion-principle.md), applied to the unwanted events that the two endpoints of an [edge](../../../../edge-of-a-graph.md) receive the same colour, gives the [chromatic polynomial inclusion-exclusion formula](../../../../chromatic-polynomial-inclusion-exclusion-formula.md)

$$
p_G(x)=\sum_{F\subseteq E}(-1)^{|F|}x^{c(F)}.
$$

To justify the exponent, imposing equal colours across all [edges](../../../../edge-of-a-graph.md) in $F$ forces a single colour on each [connected component of a graph](../../../../component-graph-theory.md) of $(V,F)$, with independent choices between its [connected components of a graph](../../../../component-graph-theory.md). Thus the corresponding count at $q$ colours is $q^{c(F)}$. Equality for all positive [integers](../../../../integer-split.md) proves the [polynomial identity](../../../../polynomial-identity.md).

Fix an index $i$ in the stated range. A [subset](../../../../subset.md) $F$ contributes to the coefficient of $x^{n-i}$ exactly when $n-c(F)=i$. If $(V,F)$ contains a [graph cycle](../../../../cycle-in-a-graph.md) of length $s$, the hypothesis gives $s\geq\ell$. All its $s$ [vertices](../../../../vertex-graph-theory.md) lie in one [connected component of a graph](../../../../component-graph-theory.md). For any [connected component of a graph](../../../../component-graph-theory.md) $D$, its contribution to $n-c(F)$ is $|V(D)|-1$, so

$$
n-c(F)=\sum_D(|V(D)|-1)\geq s-1\geq\ell-1.
$$

This contradicts $i\leq\ell-2$. Therefore every contributing $(V,F)$ is a [forest](../../../../forest.md). The [forest](../../../../forest.md) identity $|F|=n-c(F)$ then gives $|F|=i$.

Conversely, every $i$-[edge](../../../../edge-of-a-graph.md) [subset](../../../../subset.md) is a [forest](../../../../forest.md), since a [graph cycle](../../../../cycle-in-a-graph.md) in it would have at most $i<\ell$ [edges](../../../../edge-of-a-graph.md). It therefore has $c(F)=n-i$ and contributes exactly $(-1)^i$. There are $\binom mi$ such [subsets](../../../../subset.md), by the definition of a [binomial coefficient](../../../../binomial-coefficient-split.md). Consequently

$$
[x^{n-i}]p_G(x)=(-1)^i\binom mi,\qquad
\boxed{a_i=\binom mi\quad(0\leq i\leq\ell-2).}
$$

Here the coefficient notation is understood within the defined indices $0\leq i\leq n$; if the displayed range is extended past $n$, the coefficients beyond the constant term can be set to zero. For a [forest](../../../../forest.md), $m\leq n-1$, so the [binomial coefficients](../../../../binomial-coefficient-split.md) there are also zero. The key reason [girth determines initial chromatic coefficients](../../../../girth-determines-initial-chromatic-coefficients.md) is that a [graph cycle](../../../../cycle-in-a-graph.md) can affect only exponents whose loss of [connected components of a graph](../../../../component-graph-theory.md) is at least $\ell-1$.

## ↑ Ancestors (12)

1. [C](../c.md)
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
