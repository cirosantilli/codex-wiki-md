<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\theta_k=k\pi h=k\pi/(m+1)$ and define $q^{(k)}_j=\sin(j\theta_k)$. The artificial boundary values are $q^{(k)}_0=q^{(k)}_{m+1}=0$. For the [symmetric tridiagonal Toeplitz matrix](../../../../../../symmetric-tridiagonal-toeplitz-matrix.md) $H=[\beta,\alpha,\beta]$, the [sine addition formula](../../../../../../sine-addition-formula.md) gives

$$
(Hq^{(k)})_j
=\alpha\sin(j\theta_k)
+\beta\bigl[\sin((j-1)\theta_k)+\sin((j+1)\theta_k)\bigr]
=\bigl(\alpha+2\beta\cos\theta_k\bigr)q^{(k)}_j.
$$

Thus all such matrices have the same [discrete sine transform](../../../../../../discrete-sine-transform.md) eigenvectors, with eigenvalues

$$
\boxed{\lambda_k=\alpha+2\beta\cos(k\pi h),
\qquad k=1,\ldots,m.}
$$

The sine vectors are mutually [orthogonal vectors](../../../../../../orthogonal-vectors.md) and nonzero, so the matrix $Q=(\sin(ij\pi h))_{i,j=1}^m$ is invertible. If $D=\operatorname{diag}(\lambda_1,\ldots,\lambda_m)$, then $HQ=QD$ and therefore

$$
\boxed{H=QDQ^{-1}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
