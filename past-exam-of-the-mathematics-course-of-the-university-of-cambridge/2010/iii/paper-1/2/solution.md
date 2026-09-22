<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Equip $E$ with the [inner product](../../../../../inner-product.md) defining the [root system](../../../../../root-system.md), so the [Weyl group](../../../../../weyl-group.md) acts by [orthogonal transformations](../../../../../orthogonal-transformation.md). As usual, the [root system](../../../../../root-system.md) spans its ambient space $E$. Let $U\subseteq E$ be an [invariant subspace](../../../../../invariant-subspace.md) for the [reflection representation of a Weyl group](../../../../../reflection-representation-of-a-weyl-group.md). Its [orthogonal complement](../../../../../orthogonal-complement.md) is also invariant.

For a [root](../../../../../root-of-a-root-system.md) $\alpha$, the [Weyl reflection](../../../../../weyl-reflection.md) satisfies

$$
s_\alpha(u)=u-\frac{2(u,\alpha)}{(\alpha,\alpha)}\alpha.
$$

If $(u,\alpha)=0$ for every $u\in U$, then $\alpha\in U^\perp$. Otherwise choose $u\in U$ with $(u,\alpha)\ne0$. Both $u$ and $s_\alpha(u)$ belong to $U$, and their difference is a nonzero multiple of $\alpha$, so $\alpha\in U$. Hence

$$
R=(R\cap U)\sqcup(R\cap U^\perp).
$$

The two sets are mutually [orthogonal](../../../../../orthogonal-vectors.md) and individually closed under their root reflections. If both were nonempty, this would decompose $R$ into two [orthogonal](../../../../../orthogonal-vectors.md) [root systems](../../../../../root-system.md), contradicting that it is an [irreducible root system](../../../../../irreducible-root-system.md). All roots therefore lie in one of the two subspaces. Because they span $E$, either $U=E$ or $U^\perp=E$, the latter giving $U=0$. Thus the reflection representation is an [irreducible representation](../../../../../irreducible-representation.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
