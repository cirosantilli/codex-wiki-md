<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

The [system of linear equations](../../../../../system-of-linear-equations.md) is consistent precisely when $\mathbf b$ belongs to the [column space](../../../../../column-space.md) of $A$. If $\mathbf x_0$ is one solution, all solutions form the [affine subspace](../../../../../affine-subspace.md)

$$
\mathbf x_0+\ker A,
$$

because subtracting two solutions produces a vector in the [kernel](../../../../../kernel-of-a-linear-map.md), and adding any [kernel](../../../../../kernel-of-a-linear-map.md) vector preserves the equation. Therefore the necessary and sufficient cases are:

- **No solution:** $\operatorname{rank}[A\mid\mathbf b]>\operatorname{rank}A$, equivalently $\mathbf b$ is outside the [column space](../../../../../column-space.md).
- **Exactly one solution:** $\operatorname{rank}A=3$, equivalently $\det A\ne0$; then $\mathbf x=A^{-1}\mathbf b$ for every $\mathbf b$.
- **Infinitely many solutions:** $\operatorname{rank}[A\mid\mathbf b]=\operatorname{rank}A<3$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives a nonzero [kernel](../../../../../kernel-of-a-linear-map.md) vector $\mathbf v$, and $\mathbf x_0+t\mathbf v$ gives distinct solutions for all real $t$.

For the matrix equation, each column of $X$ solves the same [system of linear equations](../../../../../system-of-linear-equations.md) with the corresponding column of $B$. Thus **a unique $X$ exists if and only if $A$ is invertible**, and then $X=A^{-1}B$. Necessity does not depend on $B$: if $A$ is singular and one $X$ exists, put any nonzero [kernel](../../../../../kernel-of-a-linear-map.md) vector in one column of a matrix $Y$ and zeros in its other columns. Then $AY=0$ and every $X+tY$ is another solution.

For the specified data, $\det A=3$. If $\mathbf x_j$ denotes row $j$ of $X$ and $\mathbf b_j$ row $j$ of $B$, row elimination yields $\mathbf x_3=(2\mathbf b_1-\mathbf b_2-\mathbf b_3)/3$, $\mathbf x_1=\mathbf b_2-\mathbf x_3$, and $\mathbf x_2=\mathbf b_1-\mathbf b_2-\mathbf x_3$. Hence

$$
\boxed{X=\begin{pmatrix}1&1&-1\\1&-1&0\\1&0&1\end{pmatrix}.}
$$

Multiplying $AX$ gives the prescribed $B$, which both checks the arithmetic and confirms the unique answer.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
