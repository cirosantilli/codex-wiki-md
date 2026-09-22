<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $A^T=A$. For [eigenvectors](../../../../../../eigenvector.md) $v_i,v_j$ with distinct real [eigenvalues](../../../../../../eigenvalue.md), symmetry gives

$$
\lambda_i v_i^Tv_j=(Av_i)^Tv_j=v_i^TA^Tv_j=v_i^TAv_j
=\lambda_jv_i^Tv_j.
$$

Thus $(\lambda_i-\lambda_j)v_i^Tv_j=0$, and the [eigenvectors](../../../../../../eigenvector.md) are [orthogonal](../../../../../../orthogonal-vectors.md). Divide each by its nonzero [Euclidean norm](../../../../../../euclidean-norm.md) to obtain an [orthonormal basis](../../../../../../orthonormal-basis.md). The [matrix](../../../../../../matrix.md) $P$ having these normalized columns satisfies $P^TP=I$, so it is an [orthogonal matrix](../../../../../../orthogonal-matrix.md) and $P^{-1}=P^T$. As in part (a),

$$
\boxed{P^TAP=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).}
$$

This proves the needed [orthogonal diagonalization](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) from symmetry and distinct [eigenvalues](../../../../../../eigenvalue.md), without invoking an unproved [spectral theorem](../../../../../../spectral-theorem.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
