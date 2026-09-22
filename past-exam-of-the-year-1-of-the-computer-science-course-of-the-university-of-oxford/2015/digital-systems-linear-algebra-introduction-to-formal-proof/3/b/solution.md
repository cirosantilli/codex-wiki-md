<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose an [invertible matrix](../../../../../invertible-matrix.md) has two [LU factorizations](../../../../../lu-decomposition.md), $A=L_1U_1=L_2U_2$, with $L_1,L_2$ [unit lower triangular matrices](../../../../../unit-lower-triangular-matrix.md) and $U_1,U_2$ [upper triangular matrices](../../../../../upper-triangular-matrix.md). All four factors are [invertible matrices](../../../../../invertible-matrix.md), since their square products are invertible. Multiplication by the appropriate [inverse matrices](../../../../../matrix-inverse-split.md) gives

$$
L_2^{-1}L_1=U_2U_1^{-1}.
$$

By the supplied closure properties, the left side is a [unit lower triangular matrix](../../../../../unit-lower-triangular-matrix.md) and the right side is an [upper triangular matrix](../../../../../upper-triangular-matrix.md). A [matrix](../../../../../matrix.md) of both types is diagonal; its diagonal entries are all one. Thus both sides are the [identity matrix](../../../../../identity-matrix.md), whence

$$
\boxed{L_1=L_2,\qquad U_1=U_2.}
$$

**Qualification of the printed wording:** this establishes uniqueness **if the specified [LU factorization](../../../../../lu-decomposition.md) exists**. Invertibility alone does not guarantee an unpivoted [LU factorization](../../../../../lu-decomposition.md). For example $\begin{pmatrix}0&1\\1&0\end{pmatrix}$ is invertible, but in a product $\begin{pmatrix}1&0\\\ell&1\end{pmatrix}\begin{pmatrix}u_{11}&u_{12}\\0&u_{22}\end{pmatrix}$, the zero top-left entry forces $u_{11}=0$, making the bottom-left entry $\ell u_{11}=0$ as well, contrary to the required value one. A [permutation matrix](../../../../../permutation-matrix.md) is needed in general, as in [PLU factorization](../../../../../plu-factorization.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
