<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First justify the finite bound used in the hint. Fix $k$. If no finite $T$ forced a [monochromatic](../../../../../../monochromatic-set.md) positive solution of $\sum_i a_i x_i=0$, consider the rooted [tree](../../../../../../tree-graph-theory.md) whose level $t$ consists of the solution-free [finite colorings](../../../../../../finite-coloring.md) of $[t]$, with restriction as the predecessor map. Every level is nonempty and every vertex has at most $k$ children. The [König infinity lemma](../../../../../../konig-s-lemma.md) gives an infinite branch, hence a [finite coloring](../../../../../../finite-coloring.md) of all [positive integers](../../../../../../positive-integer.md) with no such solution, contradicting the [partition regular matrix](../../../../../../partition-regular-matrix.md) hypothesis. This is the [compactness bound for partition regularity](../../../../../../compactness-bound-for-partition-regularity.md).

Choose such a $T$ and let $S=\operatorname{lcm}(1,\ldots,T)$, the [least common multiple](../../../../../../least-common-multiple.md). For a given [finite coloring](../../../../../../finite-coloring.md) $\chi$ of the [positive integers](../../../../../../positive-integer.md), pull it back to $[T]$ by

$$
\widetilde\chi(t)=\chi(S/t).
$$

Each $S/t$ is a [positive integer](../../../../../../positive-integer.md) in $[S]$. The defining property of $T$ gives $x_1,\ldots,x_n\in[T]$ of one color under $\widetilde\chi$, with $\sum_i a_i x_i=0$. Set $y_i=S/x_i$. Their colors under $\chi$ agree, and

$$
\boxed{\sum_{i=1}^n\frac{a_i}{y_i}
=\frac1S\sum_{i=1}^n a_i x_i=0.}
$$

Thus [reciprocal partition regularity](../../../../../../reciprocal-partition-regularity.md) follows. This construction is an involution on the divisors of $S$; it permits repeated coordinates and never requires a reciprocal of a [positive integer](../../../../../../positive-integer.md) to itself be integral without the common scaling factor $S$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
