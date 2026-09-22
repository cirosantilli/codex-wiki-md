<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The associated [matroid](../../../../matroid.md) is

$$
\boxed{M=(E,\mathcal I),\qquad\mathcal I=\{A\subseteq E:r(A)=|A|\}.}
$$

Thus the [graph](../../../../graph-split.md)'s [edges](../../../../edge-of-a-graph.md) are the [ground set](../../../../ground-set.md), and the members of $\mathcal I$ are its [matroid independent sets](../../../../independent-set-of-a-matroid.md).

For the specified rank, if $(V,A)$ is a [forest](../../../../forest.md), $A$ itself is an allowed choice in the rank maximum, so $r(A)=|A|$. Conversely, if $r(A)=|A|$, some [forest](../../../../forest.md) $F\subseteq A$ has $|F|=|A|$. Finiteness forces $F=A$, so $(V,A)$ is a [forest](../../../../forest.md). Hence **the independent sets are exactly all [forests](../../../../forest.md) in $G$**, including the empty [forest](../../../../forest.md) and [forests](../../../../forest.md) with isolated vertices.

The [matroid independence axioms](../../../../matroid-independence-axioms.md) can also be checked directly. The empty set is a [forest](../../../../forest.md), and deleting [edges](../../../../edge-of-a-graph.md) cannot create a cycle. For exchange, let [forests](../../../../forest.md) $I,J$ have $|I|<|J|$. If every [edge](../../../../edge-of-a-graph.md) of $J$ joined vertices within one component of $(V,I)$, its restriction to each component $S$ would have at most $|S|-1$ [edges](../../../../edge-of-a-graph.md). Summing would give $|J|\leq|I|$, a contradiction. Thus some [edge](../../../../edge-of-a-graph.md) of $J\setminus I$ joins two components of $I$ and can be added without creating a cycle. This proves augmentation and identifies $M$ as the **[graphic matroid](../../../../graphic-matroid.md)**.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
