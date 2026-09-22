<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [symmetric positive-definite matrix](../../../../symmetric-positive-definite-matrix.md), the [conjugate gradient method](../../../../conjugate-gradient-method.md) chooses the unique point in $x_0+K_k(A,r_0)$ minimizing the [energy norm](../../../../energy-norm.md) of the error. Equivalently it minimizes $\tfrac12y^TAy-b^Ty$ on that affine space. Here $x_0=0$ and $r_0=b$.

Choose the eigenbasis orthonormally, as the [spectral theorem](../../../../spectral-theorem.md) permits, and write $x=\sum_i\alpha_iv_i$. By part (a), every admissible error is $p(A)x=\sum_i\alpha_ip(\lambda_i)v_i$, $\deg p\leq k$, $p(0)=1$. Orthogonality then gives

$$
\boxed{\|p(A)x\|_A^2=\sum_i\alpha_i^2\lambda_i[p(\lambda_i)]^2.}
$$

Thus the implicit CG polynomial minimizes exactly the displayed weighted sum. Strictly, the printed hypothesis that the eigenvectors are individually normalized must be supplemented by mutual orthogonality when eigenvalues repeat. Otherwise cross terms within a repeated-eigenvalue eigenspace need not vanish. An orthonormal eigenbasis always supplies the intended formulation.

If at most $\ell$ eigenvectors contribute to $x$, a polynomial with one factor $1-t/\lambda$ for each distinct contributing [eigenvalue](../../../../eigenvalue.md) is admissible by step $\ell$ and makes that error zero. CG minimizes a nonnegative quantity, so $\boxed{\text{exact termination occurs in at most }\ell\text{ steps}}$.

For the last question, write $x=\alpha v_1+\beta v_2$ with eigenvalues $1,L$, $L=10^6$. The first polynomial has the form $p_1(t)=1-\eta t$. Differentiating its weighted objective gives

$$
\boxed{\eta=\frac{\alpha^2+\beta^2L^2}{\alpha^2+\beta^2L^3},\qquad p_1(1)=1-\eta.}
$$

If the high-eigenvalue component is not exceptionally small, the $L$-weighted terms dominate and $\eta\approx1/L$, so $p_1(1)\approx1-10^{-6}\approx1$: the first step mainly removes the high-eigenvalue error. This is the [spectral weighting of conjugate gradient error](../../../../spectral-weighting-of-conjugate-gradient-error.md). The expectation is conditional on the coefficients, not guaranteed by the two [eigenvalues](../../../../eigenvalue.md) alone; if $\beta=0$, the first step instead solves the low-eigenvalue component exactly.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the numerical linear algebra and approximation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and approximation course of the University of Oxford](../../../../numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
