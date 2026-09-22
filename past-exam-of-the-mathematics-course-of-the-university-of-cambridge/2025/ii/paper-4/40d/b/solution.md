<h1 id="40d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write

$$
A=D+L+U,
$$

where $D=\operatorname{diag}(a_1,\ldots,a_n)$ and $L,U$ are the strict lower and upper triangular parts. The [Jacobi method](../../../../../../jacobi-method.md) is

$$
x^{(k+1)}=D^{-1}\left(b-(L+U)x^{(k)}\right),
$$

with iteration matrix

$$
H=-D^{-1}(L+U).
$$

Here $A$ is symmetric, so $U=L^T$. Regard the iteration as the splitting

$$
A=M-N,
\qquad
M=D,
\qquad
N=-(L+L^T).
$$

Let

$$
S=\operatorname{diag}(1,-1,1,-1,\ldots).
$$

Because $A$ is tridiagonal, changing alternating signs reverses the sign of every off-diagonal entry while preserving every diagonal entry. Therefore

$$
M^T+N=D-L-L^T=SAS.
$$

Since $S^T=S=S^{-1}$ and $A$ is positive definite, $SAS$ is positive definite. The [Householder-John theorem](../../../../../../householder-john-theorem.md) now gives

$$
\rho(H)<1.
$$

The Jacobi iterates therefore converge to the unique solution $A^{-1}b$ for every starting vector, which is the [jacobi convergence for a symmetric positive-definite tridiagonal matrix](../../../../../../jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40D](../../40d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
