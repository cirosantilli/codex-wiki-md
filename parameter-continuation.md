# Parameter continuation

↑ **Parent:** [Continuation method](continuation-method.md)

[Parameter continuation](parameter-continuation.md) changes $\lambda$ by a small amount and solves again for $u$, using the previous solution as the initial guess for [Newton method](newton-s-method-in-optimization.md). If $F_u$ is an [invertible matrix](invertible-matrix.md), the [implicit function theorem](implicit-function-theorem.md) gives a local [solution branch](solution-branch.md) $u(\lambda)$, with

$$
\frac{du}{d\lambda}=-F_u^{-1}F_\lambda.
$$

Local convergence of [Newton method](newton-s-method-in-optimization.md) also needs regularity and a sufficiently small step: the cited result assumes a [Lipschitz continuous](lipschitz-continuity.md) [derivative](derivative.md) and an invertible $F_u$ at the seed.[§2.1, Corollary 2.1, printed pp. 264–265: Lipschitz continuously differentiable map, nonsingular state Jacobian, and a sufficiently small parameter increment](condition-estimates-for-pseudo-arclength-continuation-by-k-i-dickson-and-others.md)

For the cubic [polynomial](polynomial-split.md),

$$
F_x=3x^2-1,\qquad F_\lambda=1,\qquad \frac{dx}{d\lambda}=\frac1{1-3x^2}.
$$

The [derivative](derivative.md) becomes unbounded at either [continuation fold](fold-of-a-solution-branch.md), and the scalar [Newton method](newton-s-method-in-optimization.md) divides by $F_x=0$ there. Just beyond the upper [continuation fold](fold-of-a-solution-branch.md), no nearby real solution exists at the increased $\lambda$, although a distant negative-$x$ solution still exists. Converging to that solution would jump away from the local [solution branch](solution-branch.md). Decreasing the parameter step cannot make $x(\lambda)$ a valid smooth local description at the bend.

## ↑ Ancestors (6)

1. [Continuation method](continuation-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Parameter continuation](parameter-continuation.md)
