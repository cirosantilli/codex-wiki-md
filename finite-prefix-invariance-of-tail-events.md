# Finite-prefix invariance of tail events

↑ **Parent:** [Tail sigma-algebra](tail-sigma-algebra.md)

On the full [Cartesian product](cartesian-product.md) $\Omega=\mathbb R^{\mathbb N}$ with its [product sigma-algebra](product-sigma-algebra.md), take the coordinate [random variables](random-variable-split.md) $X_j(x)=x_j$. A product-measurable [set](set-split.md) $A$ is a [tail event](tail-event.md) if and only if membership is unchanged whenever two [sequences](sequence.md) differ in finitely many coordinates. The [measurability](measurability.md) condition is essential: invariance alone is not a license to assign a [probability](probability.md) to an arbitrary [subset](subset.md).

For the forward implication, fix $m$. An [event](event.md) in $\sigma(X_{m+1},X_{m+2},\ldots)$ cannot distinguish points with the same remaining coordinates. Since a [tail event](tail-event.md) belongs to this [sigma-algebra](sigma-algebra.md) for every $m$, every finite change preserves membership.

For the converse, freeze the first $m$ coordinates to zero. The insertion [map](function-class.md)

$$
i_m(y_{m+1},y_{m+2},\ldots)
=(\underbrace{0,\ldots,0}_{m\text{ entries}},y_{m+1},y_{m+2},\ldots)
$$

is a [measurable function](measurable-function.md) for the [product sigma-algebras](product-sigma-algebra.md). Thus $B_m=i_m^{-1}(A)$ is a [measurable set](measurable-set.md). Invariance gives $A=\pi_m^{-1}(B_m)$, where the coordinate projection $\pi_m$ discards the first $m$ entries. Hence $A\in\sigma(X_{m+1},X_{m+2},\ldots)$ for every $m$. The same argument works on $\{0,1\}^{\mathbb N}$. On a general [probability space](probability-space-split.md), coordinates need not admit arbitrary replacements, so the defining [intersection](set-intersection.md) of [sigma-algebras](sigma-algebra.md) remains the reliable formulation.

## ↑ Ancestors (7)

1. [Tail sigma-algebra](tail-sigma-algebra.md)
2. [Independent sigma-algebras](independent-sigma-algebras.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Tail event](tail-event.md)
