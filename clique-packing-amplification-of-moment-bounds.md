# Clique-packing amplification of moment bounds

↑ **Parent:** [Edge-disjoint clique packing](edge-disjoint-clique-packing.md)

Let $X$ count $k$-[cliques](clique-graph-theory.md) in a [binomial random graph](binomial-random-graph.md) on $m$ [vertices](vertex-graph-theory.md) and $Y$ count distinct ordered pairs sharing an [edge](edge-of-a-graph.md). The [clique conflict graph](clique-conflict-graph.md) gives $Z_k\ge X^2/(X+Y)$: order its [vertices](vertex-graph-theory.md) randomly and keep each one preceding all its neighbours, then apply the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Another application gives $\mathbb EZ_k\ge(\mathbb EX)^2/(\mathbb EX+\mathbb EY)$. If $\mathbb EY/(\mathbb EX)^2=O(k^4/m^2)$ and $1/\mathbb EX$ is no larger, then $\mathbb EZ_k=\Omega(m^2/k^4)$. Changing one [edge](edge-of-a-graph.md) changes $Z_k$ by at most one, so the [Azuma-Hoeffding inequality](azuma-s-inequality.md) for an [edge-exposure martingale](edge-exposure-martingale.md) yields the displayed exponential absence bound. This supports a [union bound](boole-s-inequality.md) over exponentially many adaptive candidate subsets.

## ↑ Ancestors (8)

1. [Edge-disjoint clique packing](edge-disjoint-clique-packing.md)
2. [Clique (graph theory)](clique-graph-theory.md)
3. [Complete graph](complete-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12/4/solution.md)
