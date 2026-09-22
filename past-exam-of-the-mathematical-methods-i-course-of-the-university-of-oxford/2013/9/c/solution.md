<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The coefficient matrix and right-hand side are

$$
A=\begin{pmatrix}2&4&3\\2&-2&-3\\-4&-2&2\end{pmatrix},\qquad
\mathbf b=\begin{pmatrix}4\\0\\-6\end{pmatrix}.
$$

For an [LU decomposition](../../../../lu-decomposition.md) with unit diagonal in the lower factor, subtract row 1 from row 2, add twice row 1 to row 3, and then add the new row 2 to row 3. The elimination multipliers are $l_{21}=1$, $l_{31}=-2$, and $l_{32}=-1$. Thus

$$
\boxed{L=\begin{pmatrix}1&0&0\\1&1&0\\-2&-1&1\end{pmatrix},\qquad
U=\begin{pmatrix}2&4&3\\0&-6&-6\\0&0&2\end{pmatrix}.}
$$

Multiplication verifies $LU=A$. Forward substitution in $L\mathbf y=\mathbf b$ gives $y_1=4$, $y_2=-4$, and $y_3=-2$. Back substitution then gives $x_3=-1$, $x_2=5/3$, and $x_1=1/6$:

$$
\boxed{\mathbf y=(4,-4,-2)^T,\qquad
\mathbf x=(1/6,5/3,-1)^T.}
$$

Every pivot is nonzero, so no row permutation is needed and the [linear system](../../../../system-of-linear-equations.md) has a unique solution.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
