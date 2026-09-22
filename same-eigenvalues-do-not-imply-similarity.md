# Same eigenvalues do not imply similarity

↑ **Parent:** [Matrix similarity](matrix-similarity.md)

Consider the [diagonal matrix](diagonal-matrix.md) $D=2I_2$ and a [Jordan block](jordan-block.md)

$$
J=\begin{pmatrix}2&1\\0&2\end{pmatrix}.
$$

Both have [characteristic polynomial](characteristic-polynomial.md) $(t-2)^2$, [trace](matrix-trace.md) $4$, [determinant](determinant.md) $4$, and [eigenvalue](eigenvalue.md) $2$ with [algebraic multiplicity](algebraic-multiplicity.md) two. But $\ker(D-2I)$ is the whole plane, whereas $(J-2I)(a,b)^T=(b,0)^T$ vanishes only when $b=0$. Their [eigenspaces](eigenspace.md) have different [dimensions](dimension-vector-space.md), so [eigenvectors under similarity](eigenvectors-under-similarity.md) rules out [matrix similarity](matrix-similarity.md). There is an even shorter proof: $S^{-1}(2I)S=2I$ for every [invertible matrix](invertible-matrix.md) $S$.

The missing information is how the [linear operator](linear-operator.md) acts beyond its [eigenvectors](eigenvector.md). Here $D-2I=0$, while $J-2I\ne0$ but $(J-2I)^2=0$. Their [minimal polynomials](minimal-polynomial.md) are respectively $t-2$ and $(t-2)^2$. Over a [field](field.md) where the [characteristic polynomial](characteristic-polynomial.md) splits, the full sizes of the [Jordan blocks](jordan-block.md), encoded by the [Jordan normal form](jordan-normal-form.md), determine the [matrix similarity](matrix-similarity.md) class.

## ↑ Ancestors (6)

1. [Matrix similarity](matrix-similarity.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Matrix similarity invariants](matrix-similarity-invariants.md)
