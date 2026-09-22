<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $A$ has finite rank, the image of its unit ball is bounded in the finite-dimensional space $\operatorname{ran}A$. The closure of a bounded set in a finite-dimensional normed space is compact. Hence every bounded [finite-rank operator](../../../../../../finite-rank-operator.md) is a [compact operator](../../../../../../compact-operator-split.md).

Let $Q_n=P_n^*P_n$ be the orthogonal projection onto

$$
H_n=\operatorname{span}\{e_1,\ldots,e_n\}.
$$

Then $Q_n\to I$ strongly. Strong convergence is uniform on every compact subset: if $K$ is compact, cover it by finitely many small balls and use $\|I-Q_n\|\leq1$ at their centers. Since the closure of $A$ applied to the unit ball is compact,

$$
\|(I-Q_n)A\|\longrightarrow0.
$$

The adjoint of a compact operator is compact, so the same argument for $A^*$ gives

$$
\|A(I-Q_n)\|
=\|(I-Q_n)A^*\|\longrightarrow0.
$$

Since $A_n=Q_nAQ_n$,

$$
A-A_n=(I-Q_n)A+Q_nA(I-Q_n).
$$

Therefore

$$
\boxed{
\|A-A_n\|
\leq\|(I-Q_n)A\|+\|A(I-Q_n)\|
\longrightarrow0}.
$$

This is the [finite-section approximation of a compact operator](../../../../../../finite-section-approximation-of-a-compact-operator.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
