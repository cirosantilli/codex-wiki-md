<h1 id="1f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Move the first $n-k$ columns of

$$
A=\begin{pmatrix}0&M\\N&0\end{pmatrix}
$$

past its last $k$ columns. This requires $k(n-k)$ column interchanges and produces the [block diagonal matrix](../../../../../../block-diagonal-matrix.md)

$$
\begin{pmatrix}M&0\\0&N\end{pmatrix}.
$$

Each interchange reverses the determinant's sign, so part (a) gives

$$
\boxed{\det A=(-1)^{k(n-k)}(\det M)(\det N)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1F](../../1f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
