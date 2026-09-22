<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sphere $\{p\}\times S^2$ in $S^1\times S^2$ is nonseparating: its complement is $(S^1\setminus\{p\})\times S^2$, which is connected. A sphere bounding a ball separates, so this product is not an [irreducible three-manifold](../../../../../../irreducible-three-manifold.md).

To show it is prime, suppose a separating sphere cuts it into compact pieces $V,W$ with one spherical boundary each. The [Seifert-van Kampen theorem](../../../../../../seifert-van-kampen-theorem.md) gives

$$
\mathbb Z\cong\pi_1(S^1\times S^2)\cong\pi_1(V)*\pi_1(W).
$$

A [free product](../../../../../../free-product.md) of two nontrivial groups is nonabelian: choose nonidentity elements in the two factors; their products in the two orders are distinct reduced words. Hence one factor, say $\pi_1(V)$, is trivial. The inclusion of this simply connected compact piece lifts to the universal cover $\mathbb R\times S^2\cong\mathbb R^3\setminus\{0\}$. The lift is an embedding: equality of lifted points would imply equality of their projections in $V$. Its image $\widetilde V$ is compact with boundary the lifted sphere.

Use the [three-dimensional Schoenflies theorem](../../../../../../three-dimensional-schoenflies-theorem.md): a locally flat embedded sphere in $\mathbb R^3$ bounds a ball, and its compact side is that ball. The interior of $\widetilde V$ is both open and closed in the corresponding complement component, and [compactness](../../../../../../compact-space.md) rules out the unbounded component. Thus $\widetilde V$ is the bounded ball, and $V$ itself is a ball. Capping $V$ gives $S^3$, so every connected-sum decomposition is trivial. Therefore **$S^1\times S^2$ is prime but not irreducible**.

Now let a prime closed connected orientable $M$ fail irreducibility. A sphere not bounding a ball cannot separate: if it did, primeness would make one capped side $S^3$, and the [three-dimensional Schoenflies theorem](../../../../../../three-dimensional-schoenflies-theorem.md) would make its uncapped side a ball. Thus there is a nonseparating sphere $S$. Its two-sided neighborhood is $S^2\times[-1,1]$. Since the complement is connected, join its two boundary spheres by an embedded arc in that complement and thicken the arc. The union is a punctured $S^2\times S^1$: the thickened arc joins the two ends of the sphere-cylinder, and the remaining boundary is one sphere. This is the [nonseparating sphere gives a sphere-circle summand](../../../../../../nonseparating-sphere-gives-a-sphere-circle-summand.md) construction and yields

$$
M\cong(S^1\times S^2)\mathbin\#N.
$$

The product is not $S^3$, since its [fundamental group](../../../../../../fundamental-group.md) is $\mathbb Z$. Primeness forces $N\cong S^3$, so

$$
\boxed{M\cong S^1\times S^2.}
$$

The background results used are van Kampen, the explicit universal cover of the product, and the locally flat three-dimensional Schoenflies theorem; no Poincaré-conjecture argument is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
