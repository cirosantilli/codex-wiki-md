<h1 id="18d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The first column already has zeros below the top entry. In the last three rows of the second column, reflect $w=(4,2,4)^T$ to $(-6,0,0)^T$ using $u=w+6e_1=(10,2,4)^T$. Since $u^Tu=120$, the [Householder reflection](../../../../../../householder-transformation.md) is

$$
H=I-\frac{uu^T}{60}
=\begin{pmatrix}-2/3&-1/3&-2/3\\-1/3&14/15&-2/15\\-2/3&-2/15&11/15\end{pmatrix}.
$$

With $Q=\operatorname{diag}(1,H)$, direct multiplication gives

$$
QA=\begin{pmatrix}1&2\\0&-6\\0&0\\0&0\end{pmatrix},\qquad
Qb=\begin{pmatrix}1\\-2/3\\5/3\\-5/3\end{pmatrix}.
$$

The transformed least-squares objective is $(x_1+2x_2-1)^2+(-6x_2+2/3)^2+50/9$. Its first two squares can both vanish, so the unique answer is

$$
\boxed{x_2=\frac19,\qquad x_1=\frac79,\qquad\min\|Ax-b\|^2=\frac{50}{9}.}
$$

Uniqueness follows because the triangular leading block is invertible; this calculation implements [Householder QR decomposition](../../../../../../householder-qr-decomposition.md) without squaring the condition number through normal equations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
