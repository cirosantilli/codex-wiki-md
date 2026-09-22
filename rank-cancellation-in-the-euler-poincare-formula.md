# Rank cancellation in the Euler-Poincare formula

↑ **Parent:** [Euler-Poincare formula](euler-poincare-formula.md)

Use the [cellular chain complex](cellular-chain-complex.md) or [simplicial chain complex](simplicial-chain-complex.md) over $\mathbb Q$, rather than the infinite [singular chain complex](singular-chain-complex.md). Put $r_i=\operatorname{rank}\partial_i$, with $r_0=r_{d+1}=0$. The [rank-nullity theorem](rank-nullity-theorem.md) gives $\dim\ker\partial_i=\dim C_i-r_i$; quotienting the [chain cycles](chain-cycle.md) by the [chain boundaries](chain-boundary.md) then gives $b_i=\dim C_i-r_i-r_{i+1}$. Each [boundary operator](boundary-operator.md)'s rank occurs in adjacent degrees with opposite signs, so

$$
\sum_{i=0}^{d}(-1)^i\dim C_i=\sum_{i=0}^{d}(-1)^ib_i.
$$

Finiteness makes this cancellation an ordinary finite sum. This is the algebra behind the [cell-count formula for Euler characteristic](cell-count-formula-for-euler-characteristic.md).

## ↑ Ancestors (9)

1. [Euler-Poincare formula](euler-poincare-formula.md)
2. [Euler characteristic](euler-characteristic.md)
3. [Simplicial homology](simplicial-homology.md)
4. [Homology (mathematics)](homology-split.md)
5. [Algebraic topology](algebraic-topology-split.md)
6. [Geometry and topology](geometry-and-topology-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
