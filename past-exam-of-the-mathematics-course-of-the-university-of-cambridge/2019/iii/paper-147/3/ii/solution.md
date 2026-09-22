<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Give $X\times Y$ the uniform [probability measure](../../../../../../probability-measure.md) and let $f$ be the [indicator function](../../../../../../indicator-function.md) of the edge set. For partitions $\mathcal P=\{X_i\}$ and $\mathcal Q=\{Y_j\}$, define the energy

$$
\mathcal E(\mathcal P,\mathcal Q)
=\left\|\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2
=\sum_{i,j}\frac{|X_i||Y_j|}{|X||Y|}d(X_i,Y_j)^2.
$$

Because [conditional expectation](../../../../../../conditional-expectation.md) is an [orthogonal projection](../../../../../../orthogonal-projection.md) in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md), $0\leq\mathcal E\leq\|f\|_2^2\leq1$.

Suppose the pair of partitions is not $\varepsilon$-regular. For each irregular $(X_i,Y_j)$ choose witnesses $A_{ij}\subseteq X_i$ and $B_{ij}\subseteq Y_j$ with

$$
|A_{ij}|\geq\varepsilon|X_i|,qquad
|B_{ij}|\geq\varepsilon|Y_j|,qquad
|d(A_{ij},B_{ij})-d(X_i,Y_j)|>\varepsilon.
$$

Refine each $X_i$ by all sets $A_{ij}$ and each $Y_j$ by all sets $B_{ij}$. If the old partitions have $r,s$ cells, the refined ones have at most $r2^s,s2^r$ cells.

The [Pythagorean theorem](../../../../../../pythagorean-theorem.md) for the two nested conditional-expectation projections gives

$$
\mathcal E(\mathcal P',\mathcal Q')-\mathcal E(\mathcal P,\mathcal Q)
=\left\|\mathbb E(f\mid\mathcal P'\otimes\mathcal Q')-
\mathbb E(f\mid\mathcal P\otimes\mathcal Q)\right\|_2^2.
$$

Inside an irregular $X_i\times Y_j$, the witness rectangle occupies at least an $\varepsilon^2$ proportion and the mean of the displayed difference over it has magnitude greater than $\varepsilon$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) therefore gives an energy gain greater than

$$
\varepsilon^4\frac{|X_i||Y_j|}{|X||Y|}
$$

from that pair. Since irregular pairs have total weight greater than $\varepsilon$, the complete refinement raises the energy by more than $\varepsilon^5$.

Energy is at most one, so after at most $\lceil\varepsilon^{-5}\rceil$ refinements the process stops at an $\varepsilon$-regular pair of partitions. Iterating the cell-count bounds $r\mapsto r2^s$ and $s\mapsto s2^r$ from $r=s=1$ a bounded number of times produces a finite $K(\varepsilon)$ independent of $G$. This proves the [Bipartite Szemerédi regularity lemma](../../../../../../bipartite-szemeredi-regularity-lemma.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 147](../../../paper-147-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
