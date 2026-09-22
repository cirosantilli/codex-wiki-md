<h1 id="8b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using the monic convention for the [characteristic polynomial](../../../../../../characteristic-polynomial.md), expand the [determinant](../../../../../../determinant.md) along the last column:

$$
\boxed{\chi_A(t)=\det(tI-A)=(t-2)\det\begin{pmatrix}t&-1\\1&t-2\end{pmatrix}=(t-2)(t-1)^2}.
$$

For the [eigenvalue](../../../../../../eigenvalue.md) $1$, the equations $(A-I)v=0$ give $v_2=v_1$ and $v_3=0$. Thus every corresponding nonzero [eigenvector](../../../../../../eigenvector.md) is a nonzero multiple of $(1,1,0)^T$. For the [eigenvalue](../../../../../../eigenvalue.md) $2$, the first two equations give $v_2=2v_1$ and $v_1=0$, so every corresponding nonzero [eigenvector](../../../../../../eigenvector.md) is a nonzero multiple of $(0,0,1)^T$. Therefore

$$
\boxed{E_1=\operatorname{span}\{(1,1,0)^T\},\qquad E_2=\operatorname{span}\{(0,0,1)^T\}}.
$$

These [eigenspaces](../../../../../../eigenspace.md) together have dimension $2$, so they cannot provide an [eigenvector](../../../../../../eigenvector.md) [basis](../../../../../../basis.md) of $\mathbb R^3$. **The [matrix](../../../../../../matrix.md) is not diagonalizable**; the [eigenvalue](../../../../../../eigenvalue.md) $1$ has algebraic multiplicity $2$ but geometric multiplicity $1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8B](../../8b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
