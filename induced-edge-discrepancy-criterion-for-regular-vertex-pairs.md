# Induced-edge discrepancy criterion for regular vertex pairs

↑ **Parent:** [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)

Let $0<\epsilon<1$ and suppose an $N$-vertex [graph](graph-split.md) has induced-edge discrepancies $|e(G[W])-p\binom{|W|}{2}|<\epsilon^5N^2/9$ whenever $|W|\ge\epsilon^2N$. Any two disjoint vertex sets of size at least $\epsilon N$ then form an [epsilon-regular pair](regular-pair-of-vertex-sets.md). Indeed, inclusion-exclusion of the induced edge counts gives

$$
|e(U,W)-p|U||W||<\epsilon^5N^2/3
$$

whenever both sets have size at least $\epsilon^2N$. The original pair has density within $\epsilon^3/3$ of $p$, while each pair of allowed relative subsets has density within $\epsilon/3$ of $p$. Their densities differ by less than $(\epsilon+\epsilon^3)/3<\epsilon$.

Thus induced subgraph counts control bipartite regularity, even when the two original sets have different sizes. Equal partitions with a small exceptional remainder follow for each fixed $k<1/\epsilon$ once $N$ is sufficiently large to absorb integer rounding. That size condition cannot be discarded if all $k$ nonexceptional classes must be nonempty.

## ↑ Ancestors (8)

1. [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)
2. [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)
3. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
