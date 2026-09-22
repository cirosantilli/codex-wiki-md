<h1 id="37e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Order the interior grid values into a vector. The coefficient matrix has diagonal $4+ch^2$ and off-diagonal entries $-1$ at horizontal and vertical neighbours, with boundary values already zero. Every row is strictly diagonally dominant because $c>0$. The standard convergence theorem for [strict diagonal dominance](../../../../../../strictly-diagonally-dominant-matrix.md) gives **convergence of both the [Jacobi method](../../../../../../jacobi-method.md) and the [Gauss-Seidel method](../../../../../../gauss-seidel-method.md)**. The matrix is also symmetric positive definite.

For $D=(4+ch^2)I$, the [weighted Jacobi method](../../../../../../weighted-jacobi-method.md) is $u^{(r+1)}=u^{(r)}+\omega D^{-1}(b-Au^{(r)})$, with iteration matrix $H_\omega=I-\omega D^{-1}A$. The sine-product grid [eigenvectors](../../../../../../eigenvector.md) give

$$
\boxed{\lambda_{k,l}=1-\omega\frac{4\{\sin^2(\pi kh/2)+\sin^2(\pi lh/2)\}+ch^2}{4+ch^2},\qquad1\leq k,l\leq m.}
$$

These [weighted Jacobi eigenvalues for a square Dirichlet grid](../../../../../../weighted-jacobi-eigenvalues-for-a-square-dirichlet-grid.md) determine convergence. All [eigenvalues](../../../../../../eigenvalue.md) of $A$ are positive. Thus for fixed $h$ convergence requires $0<\omega<2(4+ch^2)/a_{\max}$, where $a_{\max}=8\cos^2(\pi h/2)+ch^2$. As $h\downarrow0$, this upper bound tends to $1$ from above. Any fixed $\omega>1$ therefore fails on sufficiently fine grids; $\omega\leq0$ also fails. Consequently **$0<\omega\leq1$ is necessary for all mesh sizes**, and it is sufficient, since $a_{\max}<2(4+ch^2)$ for every finite grid.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [37E](../../37e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
