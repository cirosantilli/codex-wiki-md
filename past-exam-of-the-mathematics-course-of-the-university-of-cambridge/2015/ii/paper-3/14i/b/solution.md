<h1 id="14i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $v_1\cdots v_k$ be a longest [path](../../../../../../continuous-path.md). Every neighbour of either endpoint lies on it. Among the $k-1$ indices $i=1,\ldots,k-1$, mark those with $v_1v_{i+1}$ an edge and those with $v_iv_k$ an edge. Their total number is

$$
\deg v_1+\deg v_k\geq n>k-1,
$$

so some index has both marks. The edges at that index close the path into the [cycle graph](../../../../../../cycle-graph.md)

$$
v_1v_2\cdots v_iv_kv_{k-1}\cdots v_{i+1}v_1.
$$

The minimum-degree hypothesis also forces the graph to be a [connected graph](../../../../../../connected-graph.md): each component would otherwise have at least $n/2+1$ vertices. If $k<n$, an edge from this cycle to an outside vertex would give a longer path by opening the cycle at its incident vertex. Hence $k=n$, proving the [Dirac theorem](../../../../../../dirac-s-theorem.md) and **Hamiltonicity**.

The bound is sharp. For $n=2m$, take two disjoint copies of $K_m$, with minimum degree $m-1$. For $n=2m+1$, take two copies of $K_{m+1}$ sharing exactly one vertex. The minimum degree is $m$, but the shared vertex is a [cut vertex](../../../../../../cut-vertex.md), which no Hamiltonian graph can have. Both constructions have

$$
\boxed{\delta=\lceil n/2\rceil-1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14I](../../14i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
