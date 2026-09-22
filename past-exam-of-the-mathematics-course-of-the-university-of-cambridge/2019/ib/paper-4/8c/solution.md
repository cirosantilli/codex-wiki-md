<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

[Gaussian elimination](../../../../../gaussian-elimination.md) without row exchanges gives the [LU decomposition](../../../../../lu-decomposition.md)

$$
A=LU,
\qquad
L=\begin{pmatrix}
1&0&0&0\\
2&1&0&0\\
1&1&1&0\\
-2&-1&-1&1
\end{pmatrix},
\qquad
U=\begin{pmatrix}
3&2&-3&-3\\
0&-1&-1&-2\\
0&0&-2&1\\
0&0&0&-1
\end{pmatrix}.
$$

Because $L$ has unit diagonal and $U$ is [upper triangular](../../../../../upper-triangular-matrix.md),

$$
\boxed{\det A=\det L\det U=3(-1)(-2)(-1)=-6}.
$$

Solving the two triangular systems gives

$$
Ly=b
\quad\Longrightarrow\quad
y=(3,-3,-1,-1)^T,
$$

and

$$
Ux=y
\quad\Longrightarrow\quad
\boxed{x=(3,0,1,1)^T}.
$$

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
