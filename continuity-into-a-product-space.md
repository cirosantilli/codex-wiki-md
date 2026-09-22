# Continuity into a product space

↑ **Parent:** [Product topology](product-topology.md)

For a [topological space](topological-space.md) $Y$ and [topological spaces](topological-space.md) $X_i$, a [function](function-split.md) $f:Y\to\prod_iX_i$ is [continuous](continuous-function.md) into the [product topology](product-topology.md) exactly when every coordinate [function](function-split.md) $f_i=\pi_i\circ f$ is [continuous](continuous-function.md).[Lecture 5, Proposition 5.3.2, printed page 21: continuity into a product is equivalent to continuity of all component functions](18-901-fall-2024-lecture-notes.md)

Proof outline: one direction uses [function composition](function-composition.md) with the [continuous](continuous-function.md) [projection maps](projection-map.md). For the other, the [preimage](preimage.md) of a basic [cylinder set](cylinder-set.md) is

$$
f^{-1}(B(F,U))=\bigcap_{i\in F}f_i^{-1}(U_i),
$$

a finite [set intersection](set-intersection.md) of [open sets](open-set.md) in $Y$. This gives [continuity](continuous-function.md) on every basic test. It explains, for example, why $t\mapsto(t,t^2,t^3,\ldots)$ from the [real line](real-line.md) to $\mathbb R^{\mathbb N}$ is [continuous](continuous-function.md) in the [product topology](product-topology.md): each coordinate is a [polynomial](polynomial-split.md) [function](function-split.md). The general coordinate criterion fails for the [box topology](box-topology.md), where infinitely many [preimages](preimage.md) can be required at once. For example, $g(t)=(t,t,\ldots)$ has [continuous](continuous-function.md) coordinate [functions](function-split.md), but the [preimage](preimage.md) of the box $\prod_{j\geq1}(-1/j,1/j)$ is $\{0\}$, which is not an [open set](open-set.md) in the [real line](real-line.md).

## ↑ Ancestors (5)

1. [Product topology](product-topology.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Product topology](product-topology.md)
