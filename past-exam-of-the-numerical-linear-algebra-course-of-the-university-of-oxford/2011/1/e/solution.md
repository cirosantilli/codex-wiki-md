<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The two columns are [orthogonal](../../../../orthogonal-vectors.md), with lengths one and two; equivalently $A^TA=\operatorname{diag}(1,4)$. Ordering the [singular values](../../../../singular-value.md) decreasingly requires swapping the right coordinate directions. One full [singular value decomposition](../../../../singular-value-decomposition.md) is

$$
\boxed{U=\begin{pmatrix}1&0&0\\0&0&1\\0&-1&0\end{pmatrix},\quad
\Sigma=\begin{pmatrix}2&0\\0&1\\0&0\end{pmatrix},\quad
V=\begin{pmatrix}0&1\\1&0\end{pmatrix}.}
$$

Both $U$ and $V$ are [orthogonal matrices](../../../../orthogonal-matrix.md), and direct [matrix multiplication](../../../../matrix-multiplication.md) gives $U\Sigma V^T=A$. Hence

$$
\boxed{\|A\|_2=2,\qquad\|A\|_F=\sqrt5.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
