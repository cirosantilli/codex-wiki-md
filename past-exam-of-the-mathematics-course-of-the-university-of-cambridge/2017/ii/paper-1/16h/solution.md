<h1 id="16h/solution">Solution</h1>

↑ **Parent:** [16H](../16h.md)

Let $v_1\cdots v_r$ be a longest path in the finite simple [graph](../../../../../graph-split.md). Every neighbour of either endpoint lies on it. Among indices $1\le i<r$, consider those with edges $v_1v_{i+1}$ and those with edges $v_iv_r$. Their cardinalities are the endpoint degrees, whose sum is at least $n\ge r$, exceeding the $r-1$ available indices. They intersect, producing the cycle

$$
v_1v_2\cdots v_i v_r v_{r-1}\cdots v_{i+1}v_1.
$$

Every connected component has at least $\delta(G)+1>n/2$ vertices, so the graph is connected. If $r<n$, an edge joins a vertex outside this cycle to it, and breaking the cycle there gives a longer path, a contradiction. Hence $r=n$ and this is a [Hamilton cycle](../../../../../hamilton-cycle.md), proving [Dirac theorem](../../../../../dirac-s-theorem.md).

The complete graph $K_4$ is planar, has [chromatic number](../../../../../chromatic-number.md) four and a Hamilton cycle. Adding one leaf attached to one of its vertices preserves planarity and [chromatic number](../../../../../chromatic-number.md) four but prevents a Hamilton cycle, since a leaf has degree one.

For the last claim, the given plane embedding has all vertices on the outer cycle. Add noncrossing diagonals until its polygonal interior is triangulated. A triangulated polygon has a vertex incident with only its two boundary neighbours: for example the dual graph of its triangles is a tree and a leaf triangle supplies an ear. Remove this vertex. Inductively three-colour the smaller triangulated polygon, starting with a triangle. The removed vertex's neighbours are adjacent and have different colours, so it can receive the third. Restriction to the original graph gives

$$
\boxed{\chi(G)\le3}.
$$

This uses the specified embedding, not the false assertion that every planar [Hamiltonian](../../../../../hamiltonian.md) graph is three-colourable; $K_4$ is already a counterexample to that broader assertion.

## ↑ Ancestors (10)

1. [16H](../16h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
