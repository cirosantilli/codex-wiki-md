<h1 id="39a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $L=\operatorname{tridiag}(1,-2,1)$. The zero Dirichlet boundary values introduce no forcing terms, so the scheme is

$$
\boxed{Bu^{n+1}=Cu^n,\quad B=I-\frac\mu2L=\operatorname{tridiag}(-\mu/2,1+\mu,-\mu/2),\quad
C=I+\frac\mu2L=\operatorname{tridiag}(\mu/2,1-\mu,\mu/2).}
$$

The common orthogonal sine [eigenvectors](../../../../../../eigenvector.md) have $L$-eigenvalues $-4\sin^2[\pi j/(2(M+1))]$. Thus $B$ is invertible for every $\mu>0$, and each amplification [eigenvalue](../../../../../../eigenvalue.md) is

$$
\boxed{g_j=\frac{1-2\mu\sin^2[\pi j/(2(M+1))]}{1+2\mu\sin^2[\pi j/(2(M+1))]},\qquad |g_j|\leq1.}
$$

The matrix $B^{-1}C$ is orthogonally diagonalizable, so its powers have [Euclidean norm](../../../../../../euclidean-norm.md) at most one, uniformly in the mesh and time step. Therefore **[Crank-Nicolson diffusion scheme](../../../../../../crank-nicolson-diffusion-scheme.md) is stable for every $\mu>0$**. Negative amplification factors at large $\mu$ can create temporal sign oscillations, which do not contradict this [norm](../../../../../../norm.md) stability.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
