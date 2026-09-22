# Forest polytope

↑ **Parent:** [Matroid independence polytope](matroid-independence-polytope.md)

For an undirected finite [graph](graph-split.md), its [forest](forest.md) polytope is the [matroid independence polytope](matroid-independence-polytope.md) of its [graphic matroid](graphic-matroid.md). It has the exact inequality descriptions

$$
\{x\geq0:x(A)\leq |V|-\kappa(V,A)\text{ for all }A\subseteq E\}
=\{x\geq0:x(E(S))\leq|S|-1\text{ for all nonempty }S\subseteq V\}.
$$

Here $\kappa(V,A)$ counts all [connected components of a graph](component-graph-theory.md), including isolated vertices, and $E(S)$ denotes the [edges](edge-of-a-graph.md) internal to $S$. A maximal [forest](forest.md) has one fewer [edge](edge-of-a-graph.md) than vertices in each component, giving the rank $|V|-\kappa(V,A)$. The [matroid independence polytope](matroid-independence-polytope.md) theorem therefore proves the first description. It implies the second since the rank of $E(S)$ is at most $|S|-1$. Conversely, split any $A$ into its vertex components $S_j$; nonnegativity gives $x(A)\leq\sum_jx(E(S_j))\leq\sum_j(|S_j|-1)=|V|-\kappa(V,A)$. No spanning requirement is imposed, so an optimum with negative [edge](edge-of-a-graph.md) weights can leave vertices isolated.

## ↑ Ancestors (6)

1. [Matroid independence polytope](matroid-independence-polytope.md)
2. [Matroid](matroid.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/e/solution.md)
