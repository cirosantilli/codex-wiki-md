<h1 id="25k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D_n=B_n\setminus B_{n+1}$. These sets are pairwise disjoint and

$$
B_1=B\ \dot\cup\ \bigsqcup_{n\geq1}D_n,\qquad B_m=B\ \dot\cup\ \bigsqcup_{n\geq m}D_n.
$$

By [countable additivity](../../../../../../countable-additivity.md), $\sum_n\mu(D_n)=\mu(B_1)-\mu(B)<\infty$. The tails of this convergent nonnegative series tend to zero, so

$$
\boxed{\mu(B_m)=\mu(B)+\sum_{n\geq m}\mu(D_n)\longrightarrow\mu(B).}
$$

This proves [continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md) and explains the finite-measure assumption.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
