<h1 id="2b/solution">Solution</h1>

↑ **Parent:** [2B](../2b.md)

Let $H,K$ be the [normal subgroups](../../../../../normal-subgroup.md) of orders $3,5$. Their intersection is a [subgroup](../../../../../subgroup.md) of both, so [Lagrange's theorem](../../../../../lagrange-s-theorem.md) makes its order divide both $3$ and $5$; hence $H\cap K=\{1\}$. For $h\in H$ and $k\in K$, normality shows that $hkh^{-1}k^{-1}$ belongs to both $H$ and $K$. It must be the identity, so $hk=kh$. This proves the needed instance of [normal subgroups of coprime order commute](../../../../../normal-subgroups-of-coprime-order-commute.md).

Choose nonidentity $h\in H$ and $k\in K$. Their orders are $3$ and $5$, since these orders divide the respective prime subgroup orders. If $(hk)^m=1$, commutativity gives $h^m=k^{-m}\in H\cap K$, so $3\mid m$ and $5\mid m$. Conversely $(hk)^{15}=1$. Thus the [product of commuting elements of coprime order](../../../../../product-of-commuting-elements-of-coprime-order.md) gives **an element $hk$ of order $15$**.

For the counterexample, take the [dihedral group](../../../../../dihedral-group.md) of symmetries of a regular pentagon:

$$
\boxed{D_5=\langle r,s\mid r^5=s^2=1,\ srs=r^{-1}\rangle}.
$$

Its ten elements are $r^j$ and $sr^j$, $0\le j<5$. Nonidentity rotations have order $5$, and $(sr^j)^2=r^{-j}r^j=1$, so all [reflections](../../../../../reflection-mathematics.md) have order $2$. **There is no element of order $10$.**

## ↑ Ancestors (10)

1. [2B](../2b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
