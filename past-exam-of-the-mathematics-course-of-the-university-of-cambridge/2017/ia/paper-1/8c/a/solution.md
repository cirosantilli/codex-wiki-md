<h1 id="8c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $y=(y_1,y_2,y_3)^T$. From the coordinate formula for the [cross product](../../../../../../cross-product.md),

$$
\boxed{T=
\begin{pmatrix}
1&y_3&-y_2\\
-y_3&0&y_1\\
y_2&-y_1&0
\end{pmatrix}}.
$$

If $y=c_1e_1$, this becomes

$$
\begin{pmatrix}1&0&0\\0&0&c_1\\0&-c_1&0\end{pmatrix}.
$$

Thus $c_1\ne0$ gives rank three and a zero-dimensional kernel, while $c_1=0$ gives rank one and kernel dimension two.

If $y\mathbin{\cdot}e_1=0$, then $y_1=0$. When $y\ne0$, the equations $Tx=0$ force $x_1=0$ and $y_3x_2-y_2x_3=0$, so

$$
\ker T=\mathbb Ry,
\qquad \operatorname{rank}T=2.
$$

When $y=0$, again $\operatorname{rank}T=1$ and $\dim\ker T=2$. These dimensions also agree with the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8C](../../8c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
