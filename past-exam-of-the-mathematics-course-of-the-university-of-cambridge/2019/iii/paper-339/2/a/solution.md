<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $J=\mathbf1\mathbf1^T$ be the [all-ones matrix](../../../../../../all-ones-matrix.md). Every feasible block [matrix](../../../../../../matrix.md) in the first formulation has $t\geq1$, because its principal $2\times2$ [submatrix](../../../../../../submatrix.md) on indices $0,i$ is $\begin{pmatrix}t&1\\1&1\end{pmatrix}$ and is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md). In particular, $t>0$.

By the [Schur complement](../../../../../../schur-complement.md),

$$
\begin{pmatrix}t&\mathbf1^T\\\mathbf1&Z\end{pmatrix}\succeq0
\quad\Longleftrightarrow\quad
Z-\frac1tJ\succeq0.
$$

Set $U=tZ-J$. Then $U\succeq0$, $U_{ii}=t-1$, and $U_{ij}=-1$ on every [edge](../../../../../../edge-of-a-graph.md). Conversely, for a feasible $(t,U)$ in the second formulation, its nonnegative diagonal gives $t\geq1$, and $Z=(U+J)/t$ has $Z_{ii}=1$, $Z_{ij}=0$ on [edges](../../../../../../edge-of-a-graph.md), and $Z-J/t=U/t\succeq0$.

Both transformations preserve the objective $t$. Hence the two [semidefinite programs](../../../../../../semidefinite-programming.md) defining the [complement theta number](../../../../../../complement-theta-number.md) have the same feasible objective values and the same minimum.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
