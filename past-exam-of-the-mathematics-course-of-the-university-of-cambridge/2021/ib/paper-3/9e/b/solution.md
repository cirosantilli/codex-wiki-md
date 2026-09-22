<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand $\det(A+tB)$ by [multilinearity of the determinant](../../../../../../multilinearity-of-the-determinant.md) in its columns. The coefficient of $t^j$ is a sum of determinants obtained by choosing $j$ columns from $B$ and the remaining columns from $A$. Since the columns of $B$ span a space of dimension $k$, every choice of more than $k$ columns from $B$ is [linearly dependent](../../../../../../linear-dependence.md). All coefficients of $t^j$ for $j>k$ therefore vanish, so

$$
\deg\det(A+tB)\leq k.
$$

If $k=n$, then $B$ is invertible and the coefficient of $t^n$ is $\det B\ne0$. Hence the degree is exactly $n$.

For a zero-polynomial example with $k=1$, take

$$
A=\begin{pmatrix}0&0\\0&0\end{pmatrix},
\qquad
B=\begin{pmatrix}1&0\\0&0\end{pmatrix}.
$$

Then $\operatorname{rank}B=1$, while $\det(A+tB)=0$ for every $t$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
