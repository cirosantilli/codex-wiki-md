# Preimage

↑ **Parent:** [Image and preimage of a function](image-and-preimage-of-a-function.md)

For a [function](function-split.md) $f:X\to Y$ and a [subset](subset.md) $U\subseteq Y$, its [preimage](preimage.md) is

$$
f^{-1}(U)=\{x\in X:f(x)\in U\}.
$$

It is a [subset](subset.md) of the original [domain of a function](domain-of-a-function.md). The notation does not require an [inverse function](inverse-function.md): the [preimage](preimage.md) of a [singleton set](singleton-mathematics.md) can have no members, one member, or many members. In the finite example, $f^{-1}(\{0\})=\{a,b\}$, $f^{-1}(\{1\})=\{c\}$ and $f^{-1}(\{3\})=\varnothing$. The [preimage](preimage.md) of a [singleton set](singleton-mathematics.md) is also its [fiber of a function](fiber-of-a-function.md).

For [subsets](subset.md) $U,V\subseteq Y$, [preimages](preimage.md) preserve both [unions](set-union.md) and [intersections](set-intersection.md):

$$
f^{-1}(U\cup V)=f^{-1}(U)\cup f^{-1}(V),\qquad
f^{-1}(U\cap V)=f^{-1}(U)\cap f^{-1}(V).
$$

For the [intersection](set-intersection.md), the same input $x$ belongs precisely when its single output $f(x)$ belongs to both $U$ and $V$. There is no opportunity to choose different witnesses, which is what made the image counterexample fail. The identities also hold for arbitrary families of output [subsets](subset.md).

In the finite example, choose $U=\{0,1\}$ and $V=\{0,2\}$. Then

$$
f^{-1}(U)=\{a,b,c\},\qquad f^{-1}(V)=\{a,b,d\},\qquad
f^{-1}(U\cap V)=f^{-1}(\{0\})=\{a,b\}.
$$

The [intersection](set-intersection.md) of the two preimages is exactly the same [set](set-split.md) $\{a,b\}$. Complements are preserved with respect to the appropriate source and target [sets](set-split.md):

$$
f^{-1}(Y\setminus U)=X\setminus f^{-1}(U).
$$

For example, the unused output three contributes no extra input: with $U=\{0,2\}$, both sides of the complement identity are $\{c\}$. See [Lebl, Proposition 0.3.15: preimages of unions, intersections and complements](https://www.jirka.org/ra/html/sec_basicset.html).

This makes [preimages](preimage.md) useful for transporting conditions. The [solution set](solution-set.md) of $g(x)=0$ is $g^{-1}(\{0\})$, and a [zero set](zero-set.md) is a preimage of zero. Requiring two output conditions takes the [intersection](set-intersection.md) of their preimages. In [topology](topology-split.md), a [continuous function](continuous-function.md) pulls every [open set](open-set.md) back to an [open set](open-set.md); a [measurable function](measurable-function.md) pulls the specified [measurable sets](measurable-set.md) in its [codomain](codomain.md) back to [measurable sets](measurable-set.md) in its [domain of a function](domain-of-a-function.md). These definitions use [preimages](preimage.md) because their set operations remain consistent even when the [function](function-split.md) is noninjective.

## ↑ Ancestors (6)

1. [Image and preimage of a function](image-and-preimage-of-a-function.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Canonical projection of a quotient set](canonical-projection-of-a-quotient-set.md)
- [Continuity into a product space](continuity-into-a-product-space.md)
- [Entire function](entire-function.md)
- [Essential range](essential-range.md)
- [Fiber of a function](fiber-of-a-function.md)
- [Finite-coordinate basis for the product topology](finite-coordinate-basis-for-the-product-topology.md)
- [Great Picard theorem](great-picard-theorem.md)
- [Hash collision](hash-collision.md)
- [Image and preimage of a function](image-and-preimage-of-a-function.md)
- [Image of a function](image-of-a-function.md)
- [Inverse function](inverse-function.md)
- [Kernel (algebra)](kernel-algebra.md)
- [Little Picard theorem](little-picard-theorem.md)
- [Open map](open-map.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/14a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/1d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/1/solution.md)
- [Preimage](preimage.md)
- [Pushforward filter](pushforward-filter.md)
- [Quotient topological space](quotient-topological-space.md)
- [Quotient topology](quotient-topology.md)
- [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
- [Strictly increasing function](strictly-increasing-function.md)
- [Total variation distance under a measurable map](total-variation-distance-under-a-measurable-map.md)
- [Zero set](zero-set.md)
