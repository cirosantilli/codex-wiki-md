# Left preconditioning

↑ **Parent:** [Matrix preconditioning](matrix-preconditioning.md)

[Left preconditioning](left-preconditioning.md) multiplies both sides of the [linear system](system-of-linear-equations.md) $Ax=b$ by the same [invertible matrix](invertible-matrix.md) $M^{-1}$. It leaves the unknown [vector](vector.md) $x$ unchanged. The original [linear-system residual](linear-system-residual.md) is $r=b-Ax$; the transformed [linear-system residual](linear-system-residual.md) is $M^{-1}r$. Applying the transformed [linear map](linear-map.md) to $v$ first computes $Av$, then solves $Mz=Av$.

For [symmetric positive-definite matrices](symmetric-positive-definite-matrix.md) $A$ and $M$, $M^{-1}A$ is generally not a [symmetric matrix](symmetric-matrix.md) in the [Euclidean inner product](dot-product.md). Its positive [eigenvalues](eigenvalue.md) alone do not justify ordinary Euclidean [Conjugate gradient method](conjugate-gradient-method.md) recurrences. The remedy is [symmetric positive-definite preconditioning](symmetric-positive-definite-preconditioning.md), implemented through the [Preconditioned conjugate gradient method](preconditioned-conjugate-gradient-method.md).

## ↑ Ancestors (7)

1. [Matrix preconditioning](matrix-preconditioning.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Diagonal scaling for a two-dimensional linear system](diagonal-scaling-for-a-two-dimensional-linear-system.md)
- [Left preconditioning](left-preconditioning.md)
- [Right preconditioning](right-preconditioning.md)
