# Triangularization using dual spaces

↑ **Parent:** [Triangularization over an algebraically closed field](triangularization-over-an-algebraically-closed-field.md)

A [linear map](linear-map.md) on a [finite-dimensional vector space](finite-dimensional-vector-space.md) over an [algebraically closed field](algebraically-closed-field.md) has both an [upper triangular matrix](upper-triangular-matrix.md) and a [lower triangular matrix](lower-triangular-matrix.md) in suitable [bases](basis.md). One proof uses [invariant subspaces and annihilators](invariant-subspaces-and-annihilators.md) to make the induction step entirely in the [dual space](dual-space-split.md).

Choose an [eigenvector](eigenvector.md) $v$ and let $U=\operatorname{span}\{v\}$. The [dual map](transpose-of-a-linear-map.md) preserves the [annihilator of a vector subspace](annihilator-of-a-vector-subspace.md) $U^0$, of [dimension](dimension-vector-space.md) one less. By induction, choose a [basis](basis.md) of $U^0$ making the [restriction](restriction-mathematics.md) upper triangular. Extend this to a [basis](basis.md) of the whole [dual space](dual-space-split.md); its [matrix](matrix.md) $C$ remains upper triangular because $U^0$ is an [invariant subspace](invariant-subspace.md). In the corresponding primal [basis](basis.md), the [matrix](matrix.md) is $C^T$, which is lower triangular. Reversing the primal [basis](basis.md) makes it upper triangular. Dimension zero and one start the induction. This also allows the original [eigenvector](eigenvector.md) to be the first vector of the resulting upper triangular [basis](basis.md).

## ↑ Ancestors (8)

1. [Triangularization over an algebraically closed field](triangularization-over-an-algebraically-closed-field.md)
2. [Characteristic polynomial](characteristic-polynomial.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/1/b/iv/solution.md)
