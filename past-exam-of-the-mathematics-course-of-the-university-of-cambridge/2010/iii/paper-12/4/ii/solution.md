<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $q=m/s$, an integer under the stated divisibility assumption. The degree relation gives $n=rm/s=qr$. Take the [disjoint union of graphs](../../../../../../disjoint-union-of-graphs.md) of $q$ copies of the [complete bipartite graph](../../../../../../complete-bipartite-graph.md) $K_{s,r}$, placing its $s$-vertex part in $U$ and its $r$-vertex part in $W$. The total part sizes are then $qs=m$ and $qr=n$. Each left [vertex](../../../../../../vertex-graph-theory.md) has [vertex degree](../../../../../../degree-graph-theory.md) $r$, and each right [vertex](../../../../../../vertex-graph-theory.md) has [vertex degree](../../../../../../degree-graph-theory.md) $s$, so the graph has exactly the required [biregular graph](../../../../../../biregular-graph.md) parameters.

An [independent set](../../../../../../independent-set-graph-theory.md) in one component can be any subset of its left part or any subset of its right part. It cannot contain a vertex from both parts, because all cross-pairs are [edges](../../../../../../edge-of-a-graph.md). The two families share only the empty set, so the component has $2^s+2^r-1$ [independent sets](../../../../../../independent-set-graph-theory.md). Choices in different [connected components of a graph](../../../../../../component-graph-theory.md) are independent combinatorial choices, and their counts multiply. Hence

$$
\boxed{i(G)=(2^s+2^r-1)^q=(2^r+2^s-1)^{m/s}.}
$$

This attains equality in part (i). It also explains the entropy weight $2^r$ there: the empty selected left neighbourhood permits all $2^r$ subsets of the opposite part.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
