<h1 id="17f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Turán graph](../../../../../../turan-graph.md) $T_r(n)$ is the complete $r$-partite [graph](../../../../../../graph-split.md) with part sizes differing by at most one. [Turan theorem](../../../../../../turan-s-theorem.md) states that a [graph](../../../../../../graph-split.md) on $n$ vertices containing no $K_r$ has at most $e(T_{r-1}(n))$ edges, with equality precisely for that balanced [complete multipartite graph](../../../../../../complete-multipartite-graph.md).

Here is a symmetrization proof, including equality. Choose a $K_r$-free [graph](../../../../../../graph-split.md) with the maximum number of edges. Replacing a vertex $u$ by a nonadjacent twin of a nonadjacent vertex $v$ preserves $K_r$-freeness: a [clique](../../../../../../clique-graph-theory.md) using the replacement would give the same [clique](../../../../../../clique-graph-theory.md) using $v$. Thus nonadjacent vertices must have equal degrees, or cloning the higher-degree vertex increases the edge count. In fact their neighborhoods are identical. Otherwise choose $w$ adjacent to $u$ but not $v$. Cloning $u$ to $v$ preserves the total number of edges but lowers $w$'s degree by one, leaving $v$'s degree unchanged. The still nonadjacent pair $w,v$ now has unequal degrees, allowing an edge-increasing clone and contradicting maximality.

Nonadjacency is consequently an equivalence relation, and the extremal [graph](../../../../../../graph-split.md) is complete multipartite. It has at most $r-1$ parts because choosing one vertex from each part forms a [clique](../../../../../../clique-graph-theory.md). For $n\geq r-1$, using fewer parts cannot be extremal if a part can be split. Finally its number of edges is $\frac12(n^2-\sum n_i^2)$, maximized uniquely by balanced sizes: moving a vertex from a part at least two larger than another decreases the sum of squares. This proves the theorem and its equality characterization. The cases with fewer vertices than the forbidden [clique](../../../../../../clique-graph-theory.md) are immediate.

## ↑ Ancestors (11)

1. [I](../i.md)
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
