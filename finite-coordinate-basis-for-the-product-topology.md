# Finite-coordinate basis for the product topology

↑ **Parent:** [Product topology](product-topology.md)

For a [finite set](finite-set.md) $F\subseteq I$ and [open sets](open-set.md) $U_i\subseteq X_i$ for $i\in F$, the sets

$$
B(F,U)=\bigcap_{i\in F}\pi_i^{-1}(U_i)
=\prod_{i\in I}V_i,\qquad
V_i=\begin{cases}U_i&i\in F,\\X_i&i\notin F\end{cases}
$$

form a [basis of a topology](basis-of-a-topology.md) for the [product topology](product-topology.md). The empty [set intersection](set-intersection.md) is $X$. Each basic [open set](open-set.md) is a [cylinder set](cylinder-set.md); all coordinates outside $F$ are free. Arbitrary [open sets](open-set.md) are unions of these basic tests and need not themselves depend on one fixed finite collection of coordinates.[Proposition 2.2.1, Definition 2.2.2 and Remark 2.2.8: finite-coordinate basis and general open subsets](point-set-topology-by-romyar-sharifi/point-set-topology-chapter-2-continuous-functions.md)

Why finitely many? Any [topology](topology-split.md) making the [projection maps](projection-map.md) [continuous](continuous-function.md) must contain their [preimages](preimage.md) of [open sets](open-set.md), and hence finite [set intersections](set-intersection.md) of those [preimages](preimage.md). Taking arbitrary unions supplies exactly the [product topology](product-topology.md). Intersecting two basic [cylinder sets](cylinder-set.md) still restricts only the finite union of their coordinate sets.

**Table of contents**

- [Open rectangles in a finite product](open-rectangles-in-a-finite-product.md)

## ↑ Ancestors (5)

1. [Product topology](product-topology.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Product topology](product-topology.md)
