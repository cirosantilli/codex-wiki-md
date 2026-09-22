<h1 id="40c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Householder-John theorem](../../../../../../householder-john-theorem.md) states: if $A=M-N$ is [Hermitian](../../../../../../hermitian-operator.md) positive definite and $M^*+N$ is also Hermitian positive definite, then $M$ is invertible and

$$
\rho(M^{-1}N)<1.
$$

Now let $A=D+L+L^T$ be real symmetric positive definite and tridiagonal. For the Jacobi splitting, $M=D$ and $N=-(L+L^T)$. Positive definiteness of $A$ implies every diagonal entry is positive, so $D$ is positive definite. Introduce the alternating-sign [diagonal matrix](../../../../../../diagonal-matrix.md)

$$
S=\operatorname{diag}(1,-1,1,-1,\ldots).
$$

Tridiagonality gives

$$
SAS=D-L-L^T=M^*+N.
$$

Since $S$ is orthogonal, $SAS$ is positive definite whenever $A$ is. Both hypotheses of the Householder-John theorem hold, and hence the Jacobi iteration matrix satisfies $\rho(M^{-1}N)<1$. Therefore the [Jacobi convergence for a symmetric positive-definite tridiagonal matrix](../../../../../../jacobi-convergence-for-a-symmetric-positive-definite-tridiagonal-matrix.md) follows.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40C](../../40c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
