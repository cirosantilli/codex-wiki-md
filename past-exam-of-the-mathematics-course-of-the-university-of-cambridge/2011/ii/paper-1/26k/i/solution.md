<h1 id="26k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Lp space](../../../../../../lp-space.md) is the vector space of equivalence classes, modulo equality almost everywhere, of measurable functions $f$ with $\int|f|^p\,d\mu<\infty$, equipped with $\|f\|_p=(\int|f|^p\,d\mu)^{1/p}$. To prove it is a [Banach space](../../../../../../banach-space-split.md), let $(f_n)$ be Cauchy in this norm. Choose a subsequence $(f_{n_j})$ such that

$$
\|f_{n_{j+1}}-f_{n_j}\|_p\leq2^{-j}.
$$

Take measurable representatives and put $g_j=|f_{n_{j+1}}-f_{n_j}|$, $G_M=\sum_{j=1}^Mg_j$. The [Minkowski inequality](../../../../../../minkowski-inequality.md) gives $\|G_M\|_p\leq\sum_j2^{-j}\leq1$. By the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md), $G=\sum_{j\geq1}g_j$ satisfies $\int G^p\,d\mu\leq1$. Consequently $G$ is finite almost everywhere, and the telescoping series

$$
f=f_{n_1}+\sum_{j\geq1}(f_{n_{j+1}}-f_{n_j})
$$

converges absolutely almost everywhere. Define it arbitrarily on the null exceptional set. The bound $|f|\leq|f_{n_1}|+G$ puts $f$ in $L^p$.

For the tails, monotone convergence and Minkowski again give

$$
\|f-f_{n_J}\|_p\leq\left\|\sum_{j\geq J}g_j\right\|_p\leq\sum_{j\geq J}2^{-j}\longrightarrow0.
$$

Since the original sequence is Cauchy, the [triangle inequality](../../../../../../triangle-inequality.md) then gives $f_n\to f$ in norm, not merely along the subsequence. Hence

$$
\boxed{L^p(E,\mathcal E,\mu)\text{ is complete for every }1\leq p<\infty.}
$$

This proof needs no finiteness or sigma-finiteness assumption on the measure space.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [26K](../../26k.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
