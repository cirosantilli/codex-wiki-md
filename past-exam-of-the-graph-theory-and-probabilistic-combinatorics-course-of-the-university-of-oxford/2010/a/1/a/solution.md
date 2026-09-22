<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative integer $q$, the [chromatic polynomial](../../../../../chromatic-polynomial.md) $p_G(q)$ counts the proper [vertex](../../../../../vertex-graph-theory.md) colourings of $G$ using a fixed set of $q$ colours. In a proper colouring, the endpoints of every [edge](../../../../../edge-of-a-graph.md) have different colours. The counting function extends uniquely to a [polynomial](../../../../../polynomial-split.md), as follows either from the recurrence below with the edgeless base case $p_G(x)=x^{|V(G)|}$ or from [inclusion-exclusion](../../../../../chromatic-polynomial-inclusion-exclusion-formula.md).

Let $e=uv$. Every proper colouring of $G-e$ falls into exactly one of two classes. If $u$ and $v$ have different colours, it is a proper colouring of $G$. If they have the same colour, identifying $u$ and $v$ gives a proper colouring of the contracted [graph](../../../../../graph-split.md) $G/e$, and this correspondence is bijective. Parallel edges produced by contraction impose identical conditions and can be suppressed. Hence, at every nonnegative integer $q$,

$$
p_{G-e}(q)=p_G(q)+p_{G/e}(q).
$$

Since polynomials agreeing at infinitely many values agree identically, the [deletion-contraction recurrence for the chromatic polynomial](../../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) is

$$
\boxed{p_G(x)=p_{G-e}(x)-p_{G/e}(x).}
$$

Throughout, the graphs are finite and simple, as in the usual convention for these statements.

## ↑ Ancestors (13)

1. [A](../a.md)
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
