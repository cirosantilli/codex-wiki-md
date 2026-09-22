<h1 id="12a/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**False.** Tests against [symmetric second-rank tensors](../../../../../../../symmetric-second-rank-tensor.md) see only the symmetric part $A_s=(A+A^T)/2$, because the [Frobenius inner product](../../../../../../../frobenius-inner-product.md) of a symmetric matrix and an antisymmetric matrix is zero:

$$
\sum_{ij}K_{ij}B_{ij}=-\sum_{ij}K_{ji}B_{ij}=-\sum_{ij}K_{ij}B_{ij}=0.
$$

An arbitrary basis-dependent antisymmetric part is invisible to these tests. For example, prescribe

$$
A=\begin{pmatrix}0&1&0\\-1&0&0\\0&0&0\end{pmatrix}
$$

in one basis, and $A'=0$ in another rotated basis, choosing antisymmetric arrays in every remaining basis. Every contraction with any [symmetric second-rank tensor](../../../../../../../symmetric-second-rank-tensor.md) is the invariant scalar zero. But an invertible rotation cannot transform this nonzero matrix to zero, so the array is not a [Cartesian second-rank tensor](../../../../../../../cartesian-second-rank-tensor.md). This is the [blindness of symmetric contraction tests to antisymmetric arrays](../../../../../../../blindness-of-symmetric-contraction-tests-to-antisymmetric-arrays.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [12A](../../../12a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
