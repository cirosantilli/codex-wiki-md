<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A complex square matrix $A$ is a [normal matrix](../../../../../../normal-matrix.md) if it commutes with its [conjugate transpose](../../../../../../conjugate-transpose.md):

$$
AA^*=A^*A.
$$

By [unitary diagonalization of a normal matrix](../../../../../../unitary-diagonalization-of-a-normal-matrix.md), there are a [unitary matrix](../../../../../../unitary-matrix.md) $U$ and a diagonal matrix $\Lambda=\operatorname{diag}(\lambda_1,\ldots,\lambda_N)$ such that

$$
A=U\Lambda U^*.
$$

The [matrix 2-norm](../../../../../../matrix-2-norm.md) is invariant under multiplication by unitary matrices, so

$$
\lVert A\rVert_2=\lVert\Lambda\rVert_2.
$$

For a diagonal matrix,

$$
\lVert\Lambda x\rVert_2^2
=\sum_j|\lambda_j|^2|x_j|^2
\leq\left(\max_j|\lambda_j|^2\right)\lVert x\rVert_2^2,
$$

with equality on a coordinate vector belonging to an eigenvalue of greatest modulus. Hence

$$
\boxed{\lVert A\rVert_2=\max_j|\lambda_j|=\rho(A)},
$$

the [matrix 2-norm of a normal matrix](../../../../../../matrix-2-norm-of-a-normal-matrix.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
