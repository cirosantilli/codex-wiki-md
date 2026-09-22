<h1 id="bipartite-szemeredi-regularity-lemma">Bipartite Szemerédi regularity lemma</h1>

↑ **Parent:** [Regular pair of bipartite partitions](regular-pair-of-bipartite-partitions.md)

For every $\varepsilon>0$ there is a positive [integer](integer.md) $K(\varepsilon)$ such that every finite [bipartite graph](bipartite-graph.md) has an $\varepsilon$-regular pair of partitions with at most $K(\varepsilon)$ cells on each side.

To prove this, give $X\times Y$ the uniform [probability measure](probability-measure.md), let $f$ be the [indicator function](indicator-function.md) of the edge set, and for partitions $\mathcal P,\mathcal Q$ define their energy by

$$
\mathcal E(\mathcal P,\mathcal Q)
=\left\|\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2
=\sum_{i,j}\frac{|X_i||Y_j|}{|X||Y|}d(X_i,Y_j)^2.
$$

This [conditional expectation](conditional-expectation.md) is an [orthogonal projection](orthogonal-projection.md), so $0\leq\mathcal E\leq\|f\|_2^2\leq1$. If the partitions are not $\varepsilon$-regular, choose witnesses $A_{ij}\subseteq X_i$ and $B_{ij}\subseteq Y_j$ in every irregular cell pair and refine each $X_i$ by all its $A_{ij}$ and each $Y_j$ by all its $B_{ij}$. The refined energy exceeds the old energy by

$$
\left\|\mathbb E(f\mid\mathcal P'\otimes\mathcal Q')-
\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2.
$$

On $A_{ij}\times B_{ij}$ the [absolute value function](absolute-value.md) of the mean of the difference is greater than $\varepsilon$, while this rectangle occupies at least an $\varepsilon^2$ fraction of $X_i\times Y_j$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) therefore contributes more than $\varepsilon^4|X_i||Y_j|/(|X||Y|)$ from that cell pair. Irregular pairs have total weight greater than $\varepsilon$, so every refinement raises the energy by more than $\varepsilon^5$. The process stops after at most $\lceil\varepsilon^{-5}\rceil$ refinements. If the current cell counts are $r,s$, the construction gives at most $r2^s,s2^r$ new cells, so a finite iterated bound depending only on $\varepsilon$ supplies $K(\varepsilon)$.

## ↑ Ancestors (9)

1. [Regular pair of bipartite partitions](regular-pair-of-bipartite-partitions.md)
2. [Regular pair of vertex sets](regular-pair-of-vertex-sets.md)
3. [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)
4. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-147/3/ii/solution.md)
