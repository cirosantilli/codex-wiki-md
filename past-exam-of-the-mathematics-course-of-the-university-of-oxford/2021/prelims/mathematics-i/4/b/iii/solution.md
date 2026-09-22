<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

By the [spectral theorem for real symmetric matrices](../../../../../../../spectral-theorem-for-real-symmetric-matrices.md), there is an [orthogonal matrix](../../../../../../../orthogonal-matrix.md) $Q$ such that

$$
Q^TAQ=\operatorname{diag}(\lambda_1,\ldots,\lambda_n).
$$

For clarity, the diagonalization can also be justified recursively. The [characteristic polynomial](../../../../../../../characteristic-polynomial.md) has a complex [root of a polynomial](../../../../../../../root-of-a-polynomial.md) by the [fundamental theorem of algebra](../../../../../../../fundamental-theorem-of-algebra.md). By [ii](../ii.md) its [eigenvalue](../../../../../../../eigenvalue.md) is real; taking a nonzero real or imaginary part of an associated [eigenvector](../../../../../../../eigenvector.md) in $\mathbb C^n$ gives a real [eigenvector](../../../../../../../eigenvector.md), which can be normalized. Its [orthogonal complement](../../../../../../../orthogonal-complement.md) is invariant, because $\langle Ax,z\rangle=\langle x,Az\rangle=\lambda\langle x,z\rangle=0$. Restriction to this [linear subspace](../../../../../../../vector-subspace.md) is again symmetric, and induction on [dimension](../../../../../../../dimension-vector-space.md) gives an [orthonormal basis](../../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../../eigenvector.md).

All $\lambda_i\geq0$ by [ii](../ii.md). The permitted invariance of [determinant](../../../../../../../determinant.md) and [matrix trace](../../../../../../../matrix-trace.md) under [change of basis](../../../../../../../change-of-basis.md), applied to the [diagonal matrix](../../../../../../../diagonal-matrix.md), yields

$$
\boxed{\det A=\prod_{i=1}^n\lambda_i,\qquad
\operatorname{tr}A=\sum_{i=1}^n\lambda_i,\qquad\lambda_i\geq0.}
$$

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [b](../../b.md)
3. [4](../../../4.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
