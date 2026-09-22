<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Gaussian elimination uses first-column multipliers $-2,2,-3$, second-column multiplier $2$ in the last row, and third-column multiplier $1$ there. Recording these in a unit lower-triangular matrix gives the [LU decomposition](../../../../../lu-decomposition.md)

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\-2&1&0&0\\2&0&1&0\\-3&2&1&1\end{pmatrix},\qquad
U=\begin{pmatrix}2&-1&3&2\\0&1&2&2\\0&0&-3&2\\0&0&0&1\end{pmatrix},\qquad A=LU.}
$$

Forward substitution in $Ly=b$ gives $y=(-2,-2,8,1)^T$. Back substitution gives $x_4=1$, $-3x_3+2x_4=8$, $x_2+2x_3+2x_4=-2$, and $2x_1-x_2+3x_3+2x_4=-2$. Hence **the solution is**

$$
\boxed{x=(1,0,-2,1)^T.}
$$

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
