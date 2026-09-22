# Symmetry of divided differences

↑ **Parent:** [Divided difference](divided-difference.md)

A [divided difference](divided-difference.md) depends on the chosen [interpolation nodes](interpolation-node.md) and their data, but is unchanged by any [permutation](permutation.md) $\sigma$ of those same [interpolation nodes](interpolation-node.md). The explicit [sum](sum.md) in [divided difference](divided-difference.md) makes this visible: a [permutation](permutation.md) merely rearranges its summands.[NIST Digital Library of Mathematical Functions; §3.3(iii), equation 3.3.35: symmetric explicit expression](nist-digital-library-of-mathematical-functions/3-3-interpolation.md)

There is also a short explanation using [Lagrange cardinal polynomials](lagrange-cardinal-polynomial.md). The [coefficient](coefficient.md) of $x^k$ in the $j$th [Lagrange cardinal polynomial](lagrange-cardinal-polynomial.md) is $1/\prod_{i\ne j}(x_j-x_i)$. Taking that [coefficient](coefficient.md) in their weighted [sum](sum.md) gives exactly the explicit [divided difference](divided-difference.md) formula. Since [polynomial interpolation](polynomial-interpolation.md) has a unique answer for a fixed set of distinct [interpolation nodes](interpolation-node.md), this [coefficient](coefficient.md) cannot depend on their ordering. If the [interpolation polynomial](interpolation-polynomial.md) has [polynomial degree](degree-of-a-polynomial.md) below $k$, the [coefficient](coefficient.md) is zero.

For the four-point example in [divided difference table](divided-difference-table.md), every ordering gives third [divided difference](divided-difference.md) $1$. This does not make every [Newton polynomial](newton-polynomial.md) coefficient invariant: $f[-1,0]=-1$ whereas $f[3,2]=17$, because these use different pairs of [interpolation nodes](interpolation-node.md). Even at second order, $f[-1,0,2]=1$ and $f[3,2,0]=5$ use different triples. The [node order in Newton interpolation](node-order-in-newton-interpolation.md) determines which subsets occur along the top row.

## ↑ Ancestors (8)

1. [Divided difference](divided-difference.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Node order in Newton interpolation](node-order-in-newton-interpolation.md)
