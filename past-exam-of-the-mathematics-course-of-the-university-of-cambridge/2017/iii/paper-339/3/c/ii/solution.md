<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $z$ on the [unit circle](../../../../../../../complex-unit-circle.md), use the conjugated monomial [vector](../../../../../../../vector.md)

$$
w(z)=(1,z^{-1},\ldots,z^{-d})^T
=(1,\overline z,\ldots,\overline z^{\,d})^T.
$$

Then the prescribed diagonal sums give

$$
w(z)^*Mw(z)=\sum_{i,j=0}^dM_{ij}z^{i-j}
=\sum_{k=-d}^d p_kz^k=p(z).
$$

[Positive semidefiniteness](../../../../../../../positive-semidefinite-matrix.md) proves

$$
\boxed{p(z)=w(z)^*Mw(z)\geq0\quad(|z|=1)}.
$$

This is the [Gram matrix representation of a trigonometric polynomial](../../../../../../../gram-matrix-representation-of-a-trigonometric-polynomial.md). The Hermitian condition also implies $p_{-k}=\overline{p_k}$, so its values on the [unit circle](../../../../../../../complex-unit-circle.md) are real. The conjugated monomial [vector](../../../../../../../vector.md) is required by the source's $i-j=k$ convention; the unconjugated [vector](../../../../../../../vector.md) would represent $p(z^{-1})$ instead.

In particular $p_0=\operatorname{tr}M\geq0$. If this [matrix trace](../../../../../../../matrix-trace.md) is zero, all nonnegative [eigenvalues](../../../../../../../eigenvalue.md) vanish and $M=0$, so $p=0$. A general feasible [Gram matrix](../../../../../../../gram-matrix.md) need not have [matrix rank](../../../../../../../matrix-rank.md) one; the [Fejér–Riesz theorem](../../../../../../../fejer-riesz-theorem.md) ensures a rank-one representative exists whenever the nonnegative [trigonometric polynomial](../../../../../../../trigonometric-polynomial.md) is nonzero.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 339](../../../../paper-339-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
