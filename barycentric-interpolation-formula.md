# Barycentric interpolation formula

↑ **Parent:** [Lagrange polynomial](lagrange-polynomial.md)

The [barycentric interpolation formula](barycentric-interpolation-formula.md) evaluates the same [Lagrange polynomial](lagrange-polynomial.md) using weights that depend only on the distinct [interpolation nodes](interpolation-node.md):

$$
w_i=\frac1{\prod_{j\ne i}(x_i-x_j)},\qquad
p_n(x)=\frac{\displaystyle\sum_{i=0}^n\frac{w_i y_i}{x-x_i}}
{\displaystyle\sum_{i=0}^n\frac{w_i}{x-x_i}},\qquad x\ne x_i.
$$

At $x=x_i$, return $y_i$ directly, before dividing; the formula has [removable singularities](removable-singularity.md) at the [interpolation nodes](interpolation-node.md). Multiplying every $w_i$ by the same nonzero constant leaves the answer unchanged. Driscoll and Braun derive this formula as a more efficient, numerically stable way to evaluate [polynomial interpolation](polynomial-interpolation.md).[Driscoll and Braun, Fundamentals of Numerical Computation, §9.2, Theorem 9.2.1 and Algorithm 9.2.1](https://fncbook.com/barycentric/)

For the [interpolation nodes](interpolation-node.md) $0,1,2$, the weights are $(1/2,-1,1/2)$, or equivalently $(1,-2,1)$. With data $(1,2,5)$, at $x=1/2$ the denominator using the latter weights is $2+4-2/3=16/3$ and the numerator is $2+8-10/3=20/3$, giving $p_2(1/2)=5/4$ again. For eleven [interpolation nodes](interpolation-node.md) in the [Runge phenomenon](runge-s-phenomenon.md) figure, the generator computes the weights by the direct products above and returns stored values exactly at every [interpolation node](interpolation-node.md).

The direct products require $O(n^2)$ [arithmetic operations](arithmetic-operation.md) once; each subsequent value uses $O(n)$ [arithmetic operations](arithmetic-operation.md). Here $O$ denotes [Big O notation](big-o-notation.md). At large [polynomial degree](degree-of-a-polynomial.md) or on poorly scaled intervals, forming these products can exceed the range of [floating-point arithmetic](floating-point-arithmetic-split.md); normalization or specialized weight formulas may be needed. Stable evaluation also cannot cure sensitivity intrinsic to the chosen [interpolation nodes](interpolation-node.md), measured by the [Lebesgue constant of interpolation](lebesgue-constant-of-interpolation.md), or the approximation failure in the [Runge phenomenon](runge-s-phenomenon.md).

## ↑ Ancestors (8)

1. [Lagrange polynomial](lagrange-polynomial.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Barycentric interpolation formula](barycentric-interpolation-formula.md)
- [Lagrange polynomial](lagrange-polynomial.md)
- [Runge's phenomenon](runge-s-phenomenon.md)
