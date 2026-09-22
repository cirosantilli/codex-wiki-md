<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Eliminate the first entries of rows two, three and four using multipliers $a^3,a^2,a$. All remaining subdiagonal entries are then already zero. The unit-lower-triangular [LU decomposition](../../../../../lu-decomposition.md) is

$$
\boxed{L=\begin{pmatrix}1&0&0&0\\a^3&1&0&0\\a^2&0&1&0\\a&0&0&1\end{pmatrix},\quad
U=\begin{pmatrix}1&a&a^2&a^3\\0&\gamma&a\gamma&a^2\gamma\\0&0&\gamma&a\gamma\\0&0&0&\gamma\end{pmatrix}.}
$$

Multiplication verifies $LU=A$. Since $\gamma\ne0$, all pivots are nonzero. Forward substitution in $Ly=b$ gives

$$
y=(\gamma,-a^3\gamma,-a^2\gamma,0)^T.
$$

Backward substitution in $Ux=y$ gives $x_4=0$, $x_3=-a^2$, $x_2=0$, and $x_1=\gamma+a^4=1$. Thus

$$
\boxed{x=(1,0,-a^2,0)^T.}
$$

Direct substitution yields $Ax=(\gamma,0,0,a\gamma)^T$ as a check.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
