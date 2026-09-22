<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

For the first assertion, use the standard nonempty finite-graph convention. Choose a longest simple path in an [acyclic graph](../../../../../forest.md). Its endpoint can have no neighbour outside the path, or the path could be extended; it can have no neighbour farther back than the adjacent path vertex, or there would be a cycle. Its degree is therefore at most one. The qualification matters for infinite graphs: a two-sided infinite path is acyclic and every vertex has degree two.

A finite tree with $n>1$ has a leaf by this argument and connectedness. Removing it and its one edge leaves a tree with $n-1$ vertices. Induction from the one-vertex tree proves **a tree of order $n$ has $n-1$ edges**. Conversely, a finite connected graph has a spanning tree: begin with one vertex and repeatedly add an edge to a new vertex until every vertex is reached. This creates no cycle and uses $n-1$ edges. If the original graph has exactly that many edges, it equals its spanning tree and is itself a tree.

To embed a tree $T$ of order $t$, root it and list its vertices so every nonroot vertex follows its parent. Embed the root at any vertex of $G$. When embedding a new vertex, at most $t-2$ neighbours of its parent's image are already used, while that image has degree at least $t-1$. An unused neighbour exists and can be chosen. This constructs an injective edge-preserving copy of $T$, so

$$
\boxed{\delta(G)\ge t-1\ \Longrightarrow\ T\subseteq G.}
$$

For $t\ge2$, the complete graph $K_{t-1}$ has minimum degree $t-2$ but too few vertices to contain $T$. Thus **the degree bound cannot be lowered in general**. A subgraph copy need not be induced; extra edges in $G$ do not obstruct the construction.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
