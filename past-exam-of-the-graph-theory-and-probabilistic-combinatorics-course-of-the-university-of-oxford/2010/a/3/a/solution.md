<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Hall's marriage theorem](../../../../../hall-s-marriage-theorem.md) states that a finite [bipartite graph](../../../../../bipartite-graph-split.md) with [vertex](../../../../../vertex-graph-theory.md) classes $X,Y$ has a [matching](../../../../../matching-graph-theory-split.md) covering $X$ if and only if

$$
|N(S)|\geq|S|\quad\text{for every }S\subseteq X.
$$

Necessity follows because the matched neighbors of the vertices in $S$ are distinct members of $N(S)$.

For sufficiency, induct on $|X|$. The empty case is immediate. First suppose there is a nonempty proper subset $S\subset X$ with $|N(S)|=|S|$. The induced [graph](../../../../../graph-split.md) between $S$ and $N(S)$ satisfies Hall's condition, so [induction](../../../../../mathematical-induction.md) matches $S$. In the remaining [graph](../../../../../graph-split.md) between $X\setminus S$ and $Y\setminus N(S)$, every $T\subseteq X\setminus S$ satisfies

$$
|N(T)\setminus N(S)|=|N(T\cup S)|-|N(S)|\geq|T|.
$$

[Induction](../../../../../mathematical-induction.md) matches the rest, and the two matchings are disjoint.

Otherwise every nonempty proper $S\subset X$ has $|N(S)|\geq|S|+1$. Choose any [edge](../../../../../edge-of-a-graph.md) $xy$, which exists by Hall's condition if $X$ is nonempty. Delete $x$ and $y$. Every nonempty subset of $X\setminus\{x\}$ loses at most one neighbor and therefore still satisfies Hall's condition. [Induction](../../../../../mathematical-induction.md) provides a [matching](../../../../../matching-graph-theory-split.md) of this smaller [graph](../../../../../graph-split.md); append $xy$. If $|X|=1$, choosing its neighbor already completes the argument. This proves the theorem.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
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
