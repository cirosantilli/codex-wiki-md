# Right preconditioning

↑ **Parent:** [Matrix preconditioning](matrix-preconditioning.md)

[Right preconditioning](right-preconditioning.md) substitutes $x=M^{-1}u$ into the [linear system](system-of-linear-equations.md) $Ax=b$. Applying its transformed [linear map](linear-map.md) first solves $Mz=v$, then computes $Az$. Recover the solution by solving $Mx=u$. Its [linear-system residual](linear-system-residual.md) $b-AM^{-1}u$ is exactly the original [linear-system residual](linear-system-residual.md) $b-Ax$, which is useful when monitoring the imbalance in the original equations.

The [left preconditioning](left-preconditioning.md) and [right preconditioning](right-preconditioning.md) transformed [matrices](matrix.md) are [similar matrices](matrix-similarity.md):

$$
AM^{-1}=M(M^{-1}A)M^{-1}.
$$

They therefore have the same [eigenvalues](eigenvalue.md), although their [Euclidean norm](euclidean-norm.md) [condition numbers](condition-number.md) and residual histories need not agree. A [similarity transformation](similarity-transformation.md) preserves [eigenvalues](eigenvalue.md); a nonorthogonal change of coordinates need not preserve lengths.

## ↑ Ancestors (7)

1. [Matrix preconditioning](matrix-preconditioning.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Right preconditioning](right-preconditioning.md)
