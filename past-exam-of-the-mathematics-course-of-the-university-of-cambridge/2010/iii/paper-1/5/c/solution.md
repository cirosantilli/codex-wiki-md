<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a real [vector subspace](../../../../../../vector-subspace.md) $\mathfrak m$ complementary to $\mathfrak h$, so $\mathfrak g=\mathfrak m\oplus\mathfrak h$. The smooth map

$$
F:\mathfrak m\times\mathfrak h\longrightarrow G,\qquad F(U,V)=\exp U\exp V
$$

has differential $(U,V)\mapsto U+V$ at $(0,0)$, an [isomorphism](../../../../../../isomorphism.md). The [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $F$ a [diffeomorphism](../../../../../../diffeomorphism.md) from a sufficiently small product neighborhood onto an open neighborhood of the identity in $G$.

There is a neighborhood of zero in $\mathfrak m$ in which $\exp U\in H$ implies $U=0$. Otherwise choose nonzero $U_j\in\mathfrak m$ tending to zero with $\exp U_j\in H$. A normalized subsequence tends to a unit vector $U\in\mathfrak m$. The [limit directions of a closed subgroup](../../../../../../limit-directions-of-a-closed-subgroup.md) from part (a) give $U\in\mathfrak h$, contradicting $\mathfrak m\cap\mathfrak h=0$. Shrink the product neighborhood so that this exclusion holds throughout its first factor.

If $F(U,V)\in H$, then $\exp V\in H$ by the definition of $\mathfrak h$, and hence $\exp U=F(U,V)\exp(-V)\in H$. The exclusion forces $U=0$. Conversely, every $F(0,V)=\exp V$ belongs to $H$. Thus the [local product coordinates for a closed subgroup](../../../../../../local-product-coordinates-for-a-closed-subgroup.md) identify $H$ near the identity exactly with the smooth coordinate slice $U=0$.

Left translation by each element of $H$ gives the same description around that element, so $H$ is an [embedded submanifold](../../../../../../embedded-submanifold.md) of $G$ in its subspace topology. The multiplication and inversion maps of $G$ restrict to smooth maps on this [embedded submanifold](../../../../../../embedded-submanifold.md), making $H$ a [Lie group](../../../../../../lie-group.md) and an embedded [Lie subgroup](../../../../../../lie-subgroup.md). Its tangent space at the identity is $\mathfrak h$, because $d\exp_0$ is the identity on this coordinate slice. It remains closed by hypothesis. This proves the [closed-subgroup theorem](../../../../../../closed-subgroup-theorem.md), with no prior smoothness assumption on $H$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
