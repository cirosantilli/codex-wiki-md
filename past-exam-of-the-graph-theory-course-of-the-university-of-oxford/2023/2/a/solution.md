<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite [graph](../../../../graph-split.md) $G$, its [chromatic polynomial](../../../../chromatic-polynomial.md) $p_G(x)$ is the [polynomial](../../../../polynomial-split.md) whose value at each positive [integer](../../../../integer-split.md) $q$ counts [proper vertex colourings](../../../../proper-vertex-coloring.md) of $G$ from a fixed palette of $q$ labelled colours. Adjacent [vertices](../../../../vertex-graph-theory.md) must receive different colours, and unused colours are allowed.

For an [edge](../../../../edge-of-a-graph.md) $e=uv$, the [deletion-contraction recurrence for the chromatic polynomial](../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) is

$$
\boxed{p_G(x)=p_{G-e}(x)-p_{G/e}(x).}
$$

Here $G-e$ deletes only the [edge](../../../../edge-of-a-graph.md) $e$, while $G/e$ performs [edge contraction](../../../../edge-contraction.md), identifying $u,v$ and removing $e$. Any parallel [edges](../../../../edge-of-a-graph.md) produced by [edge contraction](../../../../edge-contraction.md) can be replaced by a single [edge](../../../../edge-of-a-graph.md), since their constraints on [proper vertex colourings](../../../../proper-vertex-coloring.md) are identical.

Indeed, the [proper vertex colourings](../../../../proper-vertex-coloring.md) of $G-e$ in which $u,v$ differ are precisely those of $G$, while those in which $u,v$ agree correspond bijectively to [proper vertex colourings](../../../../proper-vertex-coloring.md) of $G/e$. This proves the equality for every positive [integer](../../../../integer-split.md) $q$, hence as a [polynomial identity](../../../../polynomial-identity.md). Together with $p_G(x)=x^{|V(G)|}$ for a [graph](../../../../graph-split.md) without [edges](../../../../edge-of-a-graph.md), the recurrence also proves by [mathematical induction](../../../../mathematical-induction.md) that the counting function is a [polynomial](../../../../polynomial-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
