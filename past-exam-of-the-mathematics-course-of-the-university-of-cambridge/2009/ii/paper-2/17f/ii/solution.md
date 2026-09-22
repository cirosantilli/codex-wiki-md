<h1 id="17f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $r\geq3$, join a [clique](../../../../../../clique-graph-theory.md) on $r-2$ vertices to an independent set on $n-r+2$ vertices. The resulting complete $(r-1)$-partite [graph](../../../../../../graph-split.md) has

$$
\boxed{e=(r-2)n-\binom{r-1}{2}.}
$$

Its largest [clique](../../../../../../clique-graph-theory.md) has size $r-1$. Every missing edge joins two vertices of the independent set; adding it produces a $K_r$ with the original $(r-2)$-clique. It is therefore maximal $K_r$-free. For $n>r$ its part sizes are unbalanced, so its edge count is strictly less than that of $T_{r-1}(n)$.

For $r=3$ the construction is a star with $n-1$ edges. Every maximal triangle-free [graph](../../../../../../graph-split.md) on $n>3$ vertices is connected: an edge between distinct components would create no triangle. A [connected graph](../../../../../../connected-graph.md) has at least $n-1$ edges, so **the minimum is $n-1$**, attained by the star. Literally the requested construction is impossible for $r=2$, since $T_1(n)$ has zero edges. The nontrivial assertion thus requires the customary $r\geq3$ hypothesis.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
