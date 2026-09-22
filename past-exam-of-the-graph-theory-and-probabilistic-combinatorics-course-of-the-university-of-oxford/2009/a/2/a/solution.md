<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite simple loopless [graph](../../../../../graph-split.md), $p_G(q)$ counts [proper vertex colorings](../../../../../proper-vertex-coloring.md) with $q$ labelled available colors, initially for nonnegative integer $q$. For an edge $e=uv$, proper colorings of $G-e$ split into those with different endpoint colors, counted by $p_G(q)$, and those with equal endpoint colors, counted by the contracted [graph](../../../../../graph-split.md). Hence the [deletion-contraction recurrence for the chromatic polynomial](../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) is

$$
p_G(q)=p_{G-e}(q)-p_{G/e}(q).
$$

Parallel edges created by contraction can be suppressed since they impose the same coloring constraint. A [graph](../../../../../graph-split.md) with no edges has $p_G(q)=q^{|V(G)|}$. [Induction](../../../../../mathematical-induction.md) by this recurrence therefore gives a [polynomial](../../../../../polynomial-split.md) agreeing with the counting function on all nonnegative integers. That [polynomial](../../../../../polynomial-split.md) is unique because two distinct polynomials cannot agree at infinitely many points.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
