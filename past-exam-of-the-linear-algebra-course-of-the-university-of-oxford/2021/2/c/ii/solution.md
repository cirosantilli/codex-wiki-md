<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Take the [Nilpotent Jordan block](../../../../../nilpotent-jordan-block.md)

$$
\boxed{A=J_3(0)=\begin{pmatrix}0&1&0\\0&0&1\\0&0&0\end{pmatrix}.}
$$

Then

$$
A^2=\begin{pmatrix}0&0&1\\0&0&0\\0&0&0\end{pmatrix}\ne0,\qquad A^3=0.
$$

Suppose that a complex [matrix](../../../../../matrix.md) $B$ of size three satisfied $B^3=A$. We would have $B^9=A^3=0$, so $B$ would be a [nilpotent matrix](../../../../../nilpotent-matrix.md). Every [eigenvalue](../../../../../eigenvalue.md) of $B$ must then be zero: if $Bv=\theta v$ with $v\ne0$, applying $B^9$ gives $\theta^9v=0$. Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is therefore $t^3$, and the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem-split.md) gives $B^3=0$. This contradicts $B^3=A\ne0$. Hence

$$
\boxed{A^2\ne0\quad\text{but }A\text{ has no complex matrix cube root}.}
$$

The obstruction is that a [nilpotent matrix](../../../../../nilpotent-matrix.md) of size three cannot have [nilpotency index](../../../../../nilpotency-index.md) greater than three.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [c](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
