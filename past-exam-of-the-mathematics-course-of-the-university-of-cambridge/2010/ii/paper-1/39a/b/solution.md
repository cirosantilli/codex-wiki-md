<h1 id="39a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A=D+L+U$, with $D$ diagonal and $L,U$ the strict triangular parts. The [Jacobi method](../../../../../../jacobi-method.md) updates all coordinates using the preceding iterate:

$$
\boxed{x^{(k+1)}=D^{-1}(b-(L+U)x^{(k)}).}
$$

For a symmetric positive definite [matrix](../../../../../../matrix.md), $D$ has positive diagonal entries. In its splitting take $M=D$, $N=D-A$. The theorem requires $M^*+N=2D-A$ to be positive definite, which need not hold for every positive definite [matrix](../../../../../../matrix.md).

For this tridiagonal [matrix](../../../../../../matrix.md), let $S=\operatorname{diag}((-1)^1,\ldots,(-1)^n)$. Neighboring indices have opposite signs, so $SAS=2D-A$: the diagonal stays fixed and every nonzero off-diagonal entry changes sign. Thus

$$
x^T(2D-A)x=(Sx)^TA(Sx)>0\quad(x\ne0).
$$

The [Householder-John theorem](../../../../../../householder-john-theorem.md) now applies and proves **Jacobi convergence for every initial vector**. This is precisely why the tridiagonal structure matters.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [39A](../../39a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
