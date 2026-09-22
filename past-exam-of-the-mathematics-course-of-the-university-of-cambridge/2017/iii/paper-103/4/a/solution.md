<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The inclusion here is inclusion of [Young diagrams](../../../../../../young-diagram.md), not the [dominance order on partitions](../../../../../../dominance-order-on-partitions.md). The [skew Young diagram](../../../../../../skew-young-diagram.md) $\lambda/\mu$ is the set difference of their cells. Two cells are adjacent when they share an edge. It is connected when any two cells can be joined by such steps, and is a [rim hook](../../../../../../rim-hook.md) when it is connected and contains no $2\times2$ square. Under the usual edge-adjacency convention a [totally disconnected skew Young diagram](../../../../../../totally-disconnected-skew-young-diagram.md) has only singleton components, equivalently no two cells share an edge. A [horizontal strip](../../../../../../horizontal-strip.md) instead means at most one cell per column; this distinction matters for the last part of this question.

A [standard skew Young tableau](../../../../../../standard-skew-young-tableau.md) is a [linear extension of a partially ordered set](../../../../../../linear-extension.md): the cells are ordered by the row and column inequalities, and the tableau lists them in increasing label order. Write the current list as $x_1,\ldots,x_k$ and let $r_j$ be the desired label of $x_j$ in $R$. Then $(r_1,\ldots,r_k)$ is the one-line notation of the unique permutation $\pi$ with $\pi T=R$.

Whenever this list of desired labels is not increasing, there is an adjacent descent $r_j>r_{j+1}$. The cells $x_j,x_{j+1}$ are incomparable in the cell [partial order](../../../../../../partially-ordered-set.md): if they were comparable, both $T$ and $R$ would have to put them in the same order. Interchanging their consecutive current labels is therefore admissible. It removes exactly one [inversion of a permutation](../../../../../../inversion-of-a-permutation.md) from the list of desired labels. Repeating ends at $R$ after exactly the original inversion count, which is the [Coxeter length](../../../../../../coxeter-length.md) $\ell(\pi)$. Thus

$$
\boxed{T\longrightarrow R\text{ by exactly }\ell(\pi)\text{ admissible adjacent swaps}.}
$$

This proves the [reduced adjacent-swap path between linear extensions](../../../../../../reduced-adjacent-swap-path-between-linear-extensions.md) and applies equally to ordinary tableaux.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
