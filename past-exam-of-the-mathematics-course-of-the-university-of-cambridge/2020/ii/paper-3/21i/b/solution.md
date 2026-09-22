<h1 id="21i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compactness gives a stronger statement than the one requested. Since $T(B_H)$ has compact closure, finitely many open balls of radius $\delta$ cover it. Choose their centres from $T(B_H)$ and let $E$ be their finite-dimensional linear span. Then

$$
\sup_{\|x\|\leq1}\operatorname{dist}(Tx,E)<\delta.
$$

For the [orthogonal projection](../../../../../../orthogonal-projection.md) $P_E$, best approximation in a Hilbert space gives

$$
\|(I-P_E)Tx\|<\delta
\qquad(\|x\|\leq1).
$$

In particular this holds for every vector $e_n$ in the given [orthonormal basis](../../../../../../orthonormal-basis.md).

The operator $P_ET$ has image in $E$ and hence has [finite rank](../../../../../../finite-rank-operator.md), while

$$
\|T-P_ET\|
=\sup_{\|x\|\leq1}\|(I-P_E)Tx\|<\delta.
$$

**Thus every compact operator is an [operator norm](../../../../../../operator-norm.md) limit of finite-rank operators. This is the [finite-rank approximation theorem for compact operators on a Hilbert space](../../../../../../finite-rank-approximation-theorem-for-compact-operators-on-a-hilbert-space.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21I](../../21i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
