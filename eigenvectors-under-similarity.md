# Eigenvectors under similarity

↑ **Parent:** [Matrix similarity](matrix-similarity.md)

Under $B=S^{-1}AS$, an [eigenvector](eigenvector.md) in old [coordinates](coordinate-linear-algebra.md) becomes $S^{-1}v$ in new [coordinates](coordinate-linear-algebra.md). Indeed,

$$
B(S^{-1}v)=S^{-1}Av=\lambda S^{-1}v.
$$

Since $S^{-1}$ is an [invertible matrix](invertible-matrix.md), the new [coordinate vector](coordinate-vector.md) is nonzero. The inverse conversion $S$ proves that the two [eigenspaces](eigenspace.md) have the same [dimension](dimension-vector-space.md), hence the same [geometric multiplicity](geometric-multiplicity.md).

For $A=\operatorname{diag}(2,5)$, the [eigenvector](eigenvector.md) $e_2=(0,1)^T$ has [eigenvalue](eigenvalue.md) $5$. In the oblique [basis](basis.md) of the opening example, its [coordinate vector](coordinate-vector.md) is

$$
S^{-1}e_2=\begin{pmatrix}-1\\1\end{pmatrix},\qquad
B\begin{pmatrix}-1\\1\end{pmatrix}=\begin{pmatrix}-5\\5\end{pmatrix}.
$$

The [tuple](finite-tuple.md) changes from $(0,1)$ to $(-1,1)$, but reconstruction gives $-b_1+b_2=e_2$: the physical vertical direction is unchanged. Calling the [eigenvectors](eigenvector.md) unchanged is accurate only for the underlying [vectors](vector.md), not for their [coordinate vectors](coordinate-vector.md).

## ↑ Ancestors (6)

1. [Matrix similarity](matrix-similarity.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Same eigenvalues do not imply similarity](same-eigenvalues-do-not-imply-similarity.md)
