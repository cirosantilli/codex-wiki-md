# Degree ordering in an orthonormal polynomial basis

↑ **Parent:** [Orthonormal polynomial](orthonormal-polynomial.md)

An [orthonormal basis](orthonormal-basis.md) of the [polynomial](polynomial-split.md) space $\Pi_n$ need not be indexed by [polynomial degree](degree-of-a-polynomial.md). Permuting the normalized [Legendre polynomials](legendre-polynomial.md), for example, preserves [orthonormality](orthonormal-set.md) but changes the degrees attached to the labels. Results about the number of [polynomial roots](root-of-a-polynomial.md) of $p_k$ require the extra condition $\deg p_k=k$, or that the [polynomials](polynomial-split.md) arise by applying the [Gram-Schmidt process](gram-schmidt-process.md) to $1,x,x^2,\ldots$ in that order. Under this [degree](degree-graph-theory.md) ordering, $p_k$ is [orthogonal](orthogonal-vectors.md) to every [polynomial](polynomial-split.md) of lower [polynomial degree](degree-of-a-polynomial.md) because those earlier [basis](basis.md) members span $\Pi_{k-1}$.

For a positive integration weight on a nondegenerate [interval](interval-mathematics.md), this implies that $p_k$ has $k$ distinct [polynomial roots](root-of-a-polynomial.md) in the [open interval](open-interval.md). If fewer than $k$ roots change sign there, multiply $p_k$ by the product of their linear factors. The product has constant nonzero sign except at its finitely many zeros, so its weighted integral cannot vanish, contradicting [orthogonality](orthogonal-vectors.md) to this lower-[degree](degree-graph-theory.md) [polynomial](polynomial-split.md). The usual [Gaussian quadrature](gaussian-quadrature.md) construction therefore uses the [degree](degree-graph-theory.md)-ordered family; arbitrary relabelling is not enough.

## ↑ Ancestors (7)

1. [Orthonormal polynomial](orthonormal-polynomial.md)
2. [Orthogonal polynomial](orthogonal-polynomial-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
