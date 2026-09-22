# Matrix decomposition

↑ **Parent:** [Matrix](matrix.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matrix_decomposition)

A [matrix decomposition](matrix-decomposition.md) expresses a [matrix](matrix.md) as a [matrix product](matrix-product.md) of factors with simpler structure. An [LU decomposition](lu-decomposition.md) uses triangular factors, a [QR decomposition](qr-decomposition.md) uses an [orthogonal matrix](orthogonal-matrix.md) and a triangular factor, and a [singular value decomposition](singular-value-decomposition.md) separates input directions, stretching factors and output directions. The factorization is an identity; the chosen structure determines what it helps compute.

For an original two-by-two example,

$$
M=\begin{pmatrix}2&1\\1&3\end{pmatrix}
=\begin{pmatrix}1&0\\1/2&1\end{pmatrix}
\begin{pmatrix}2&0\\0&5/2\end{pmatrix}
\begin{pmatrix}1&1/2\\0&1\end{pmatrix}.
$$

The outer factors are a [lower triangular matrix](lower-triangular-matrix.md) and an [upper triangular matrix](upper-triangular-matrix.md), each with unit diagonal as in a [unit triangular matrix](unit-triangular-matrix.md); the middle factor is a [diagonal matrix](diagonal-matrix.md). Their [matrix product](matrix-product.md) is $M$, and the final diagonal entry $5/2$ is the [Schur complement](schur-complement.md) of the first entry $2$. This is the scalar version of the factorization under [block elimination](block-elimination.md).

To solve $Mz=(3,4)^T$, solve with the three factors in their displayed order from left to right: first the lower triangular factor, then the diagonal factor, then the upper triangular factor. The intermediate [vectors](vector.md) are $(3,5/2)^T$ and $(3/2,1)^T$, giving the concise answer $z=(1,1)^T$. A new right-hand side uses the same factors. This is why [Reusing LU factors for multiple right-hand sides](reusing-lu-factors-for-multiple-right-hand-sides.md) is useful: factorization records work that otherwise would be repeated, while [forward substitution](forward-substitution.md) and [back substitution](back-substitution.md) apply it cheaply.[§C.4.1, printed pp. 673–674: block factor-solve interpretation](convex-optimization-by-stephen-boyd-and-lieven-vandenberghe.md)

Different decompositions reveal different features. A [Cholesky decomposition](cholesky-decomposition.md) uses [positive definiteness](positive-definiteness.md) of a [symmetric matrix](symmetric-matrix.md), while a [singular value decomposition](singular-value-decomposition.md) also applies to rectangular [matrices](matrix.md) and exposes [matrix rank](matrix-rank.md). The existence and numerical behaviour of the factors depend on their own hypotheses; for example, an unpivoted [LU decomposition](lu-decomposition.md) can fail when a chosen [pivot element](pivot-element.md) is zero even though the [matrix](matrix.md) is an [invertible matrix](invertible-matrix.md).

## ↑ Ancestors (8)

1. [Matrix](matrix.md)
2. [Linear map](linear-map.md)
3. [Vector space](vector-space-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Matrix decomposition](matrix-decomposition.md)
