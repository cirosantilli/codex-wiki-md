<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the increasing family, define the [measurable sets](../../../../measurable-set.md)

$$
D_1=A_1,\qquad D_n=A_n\setminus A_{n-1}\quad(n\geq2).
$$

They are pairwise [disjoint](../../../../disjoint-sets.md), with $A_N=\bigcup_{n=1}^ND_n$ and $\bigcup_nA_n=\bigcup_nD_n$. By [countable additivity](../../../../countable-additivity.md),

$$
\mu\left(\bigcup_{n=1}^{\infty}A_n\right)
=\sum_{n=1}^{\infty}\mu(D_n)
=\lim_{N\to\infty}\sum_{n=1}^N\mu(D_n)
=\lim_{N\to\infty}\mu(A_N).
$$

The nonnegative [series](../../../../series-mathematics.md) is defined by its increasing partial-sum [limit](../../../../limit-of-a-function.md), so this proof also covers an infinite value. This is [continuity from below of a measure](../../../../continuity-from-below-of-a-measure.md).

For the decreasing family, put $C_n=B_1\setminus B_n$. These [measurable sets](../../../../measurable-set.md) increase, and

$$
\bigcup_nC_n=B_1\setminus\bigcap_nB_n.
$$

Since $\mu(B_1)<\infty$, [finite additivity](../../../../finite-additivity-of-a-set-function.md) gives legitimate finite subtractions:

$$
\mu(C_n)=\mu(B_1)-\mu(B_n),\qquad
\mu\left(B_1\setminus\bigcap_nB_n\right)=\mu(B_1)-\mu\left(\bigcap_nB_n\right).
$$

Apply the first result to $C_n$ and subtract from $\mu(B_1)$ to obtain

$$
\boxed{\mu\left(\bigcap_{n=1}^{\infty}B_n\right)=\lim_{n\to\infty}\mu(B_n).}
$$

This is [continuity from above of a measure](../../../../continuity-from-above-of-a-measure.md). Its finiteness hypothesis matters: for [Lebesgue measure](../../../../lebesgue-measure.md) and $B_n=[n,\infty)$, every $B_n$ has infinite [measure](../../../../measure-split.md) but their [intersection](../../../../set-intersection.md) is empty. The proof must not subtract $\infty-\infty$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
