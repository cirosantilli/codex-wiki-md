<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) proof gives the coefficients directly. For an [edge](../../../../../edge-of-a-graph.md) set $F\subseteq E(G)$, let $c(F)$ be the number of connected components of the spanning [graph](../../../../../graph-split.md) $(V(G),F)$, including isolated vertices. Requiring the two endpoints of every [edge](../../../../../edge-of-a-graph.md) of $F$ to have the same colour leaves exactly $x^{c(F)}$ colourings. Thus the [chromatic polynomial inclusion-exclusion formula](../../../../../chromatic-polynomial-inclusion-exclusion-formula.md) is

$$
p_G(x)=\sum_{F\subseteq E(G)}(-1)^{|F|}x^{c(F)}.
$$

Consider a term with $n-c(F)=i\leq k-2$. If $(V(G),F)$ contained a [cycle](../../../../../permutation-cycle.md), that [cycle](../../../../../permutation-cycle.md) would have length at least $k$. The component containing it would have at least $k$ vertices and hence contribute at least $k-1$ to $n-c(F)$, a contradiction. Therefore $F$ is a [forest](../../../../../forest.md). For a [forest](../../../../../forest.md), $n-c(F)=|F|$, so necessarily $|F|=i$.

Conversely, every $i$-element [edge](../../../../../edge-of-a-graph.md) set with $i\leq k-2$ is a [forest](../../../../../forest.md), since a [cycle](../../../../../permutation-cycle.md) would require at least $k$ edges. Thus exactly $\binom mi$ [edge](../../../../../edge-of-a-graph.md) sets contribute to the coefficient of $x^{n-i}$, and they all have sign $(-1)^i$. Consequently

$$
\boxed{a_i=\binom mi\qquad(0\leq i\leq\min(k-2,n-1)).}
$$

This proves [girth determines initial chromatic coefficients](../../../../../girth-determines-initial-chromatic-coefficients.md) without requiring the suggested double [induction](../../../../../mathematical-induction.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
