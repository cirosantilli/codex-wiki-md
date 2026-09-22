<h1 id="p/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [invertible matrix](../../../../../invertible-matrix.md) $A=\left(\begin{smallmatrix}0&1\\1&0\end{smallmatrix}\right)$, whose determinant is $-1$. Suppose it had an [LU factorization](../../../../../lu-decomposition.md) with any lower triangular $L$ and upper triangular $U$:

$$
L=\begin{pmatrix}\ell_{11}&0\\\ell_{21}&\ell_{22}\end{pmatrix},\qquad U=\begin{pmatrix}u_{11}&u_{12}\\0&u_{22}\end{pmatrix}.
$$

The $(1,2)$ entry gives $\ell_{11}u_{12}=1$, so $\ell_{11}\ne0$. The $(1,1)$ entry gives $\ell_{11}u_{11}=0$, so $u_{11}=0$. But then the $(2,1)$ entry would be $\ell_{21}u_{11}=0$, contradicting $a_{21}=1$. Thus **this nonsingular matrix has no unpermuted LU factorization**, even without imposing a unit diagonal on $L$. A row permutation resolves the zero pivot, explaining the role of [partial pivoting](../../../../../columnwise-partial-pivoting.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [P](../../../p.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
