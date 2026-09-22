# Cholesky decomposition

↑ **Parent:** [Positive-definite matrix](positive-definite-matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cholesky_decomposition)

Every real [symmetric matrix](symmetric-matrix.md) that is a [positive-definite matrix](positive-definite-matrix.md) has a unique [Cholesky decomposition](cholesky-decomposition.md) $A=LL^T$, where $L$ is a [lower triangular matrix](lower-triangular-matrix.md) with positive [diagonal entries](diagonal-matrix-entry.md).[DPOTRF, LAPACK 3.12.1: Purpose, lower-triangular factorization; UPLO and INFO argument documentation](dpotrf-lapack-3-12-1-by-lapack-project.md) For a complex [Hermitian positive-definite matrix](hermitian-positive-definite-matrix.md), the corresponding factorization is $A=LL^*$, with $L^*$ the [conjugate transpose](conjugate-transpose.md) and the diagonal of $L$ positive and real.[ZPOTRF, LAPACK 3.12.1: Purpose, Hermitian factorization with conjugate transpose](zpotrf-lapack-3-12-1-by-lapack-project.md) The factorization turns a [linear system](system-of-linear-equations.md) into two [triangular systems](triangular-system.md).

For example, matching entries in $A=LL^T$ gives

$$
A=\begin{pmatrix}4&2\\2&5\end{pmatrix},\qquad
L=\begin{pmatrix}\ell_{11}&0\\\ell_{21}&\ell_{22}\end{pmatrix},
\qquad
\ell_{11}^2=4,\quad\ell_{11}\ell_{21}=2,\quad
\ell_{21}^2+\ell_{22}^2=5.
$$

Choose the positive [square roots](square-root.md) in order: $\ell_{11}=2$, $\ell_{21}=1$ and $\ell_{22}=2$. Therefore

$$
\boxed{A=\begin{pmatrix}2&0\\1&2\end{pmatrix}
\begin{pmatrix}2&1\\0&2\end{pmatrix}.}
$$

The second radicand, $5-1^2=4$, is the scalar [Schur complement](schur-complement.md) remaining after eliminating the first variable. A positive diagonal of $A$ alone would not guarantee that this quantity is positive; [Sylvester's criterion](sylvester-s-criterion.md) explains the relevant [leading principal minors](leading-principal-minor.md).

<a id="image-cholesky-decomposition-replaces-one-coupled-linear-system-by-two-triangular-systems"></a>
![](cholesky-two-triangular-solves.png)

**[Figure 1](#image-cholesky-decomposition-replaces-one-coupled-linear-system-by-two-triangular-systems). Cholesky decomposition replaces one coupled linear system by two triangular systems**. Original exact two-by-two example. Multiplying the displayed [lower triangular matrix](lower-triangular-matrix.md) by its [transpose](transpose.md) recovers $A$; [forward substitution](forward-substitution.md) and [backward substitution in a triangular system](backward-substitution-in-a-triangular-system.md) give $x=(1,2)^T$ for $b=(8,12)^T$.

For that right-hand side, first use [forward substitution](forward-substitution.md) to solve $Ly=b$: $2y_1=8$ and $y_1+2y_2=12$, so $y=(4,4)^T$. Then use [backward substitution in a triangular system](backward-substitution-in-a-triangular-system.md) to solve $L^Tx=y$: $2x_2=4$ and $2x_1+x_2=4$, giving **$x=(1,2)^T$**. No [matrix inverse](matrix-inverse-split.md) is required. For several right-hand sides with the same $A$, keep the same factor $L$ and repeat only these [triangular solves](triangular-solve.md).

**Table of contents**

- [Cholesky decomposition as a sum of squares](cholesky-decomposition-as-a-sum-of-squares.md)
- [Cholesky decomposition and geodetic adjustment](cholesky-decomposition-and-geodetic-adjustment.md)
- [Rank-one Cholesky update](rank-one-cholesky-update.md)

## ↑ Ancestors (8)

1. [Positive-definite matrix](positive-definite-matrix.md)
2. [Definite matrix](definite-matrix.md)
3. [Quadratic form](quadratic-form-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (31)

- [Block elimination](block-elimination.md)
- [Cholesky decomposition](cholesky-decomposition.md)
- [Cholesky decomposition and geodetic adjustment](cholesky-decomposition-and-geodetic-adjustment.md)
- [Cholesky decomposition as a sum of squares](cholesky-decomposition-as-a-sum-of-squares.md)
- [Ellipsoid level sets of a positive-definite quadratic form](ellipsoid-level-sets-of-a-positive-definite-quadratic-form.md)
- [Fill-in](fill-in.md)
- [Gaussian sampling from a precision Cholesky factor](gaussian-sampling-from-a-precision-cholesky-factor.md)
- [Matrix bandwidth](matrix-bandwidth.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/14e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/14e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-1/6f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/5/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/1/e/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Rank-one Cholesky update](rank-one-cholesky-update.md)
- [Schur complement as a minimized quadratic form](schur-complement-as-a-minimized-quadratic-form.md)
- [Sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Sylvester's criterion](sylvester-s-criterion.md)
- [Thin QR factorization from Cholesky decomposition](thin-qr-factorization-from-cholesky-decomposition.md)
