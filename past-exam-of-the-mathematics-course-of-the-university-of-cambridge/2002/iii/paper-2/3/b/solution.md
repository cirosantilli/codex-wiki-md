<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K$ be the intersection under consideration. The family is nonempty since it contains $G$, and is invariant under conjugation: conjugating an irreducible inducing pair $(H,\varphi)$ gives another such pair. Hence $K$ is a [normal subgroup](../../../../../../normal-subgroup.md) of $G$.

For any $\chi\in\operatorname{Irr}(G)$, monomiality gives $\chi=\lambda^G$ with $\lambda$ a [linear character](../../../../../../linear-character.md) of some $H$. This $H$ belongs to the family, so $K\leq H$. Because $K$ is normal, $K\leq tHt^{-1}$ for every $t\in G$. In the [induced representation](../../../../../../induced-representation.md) on

$$
\mathbb C[G]\otimes_{\mathbb C[H]}\mathbb C_\lambda,
$$

each coset line $t\otimes\mathbb C_\lambda$ is therefore invariant under $K$: for $k\in K$,

$$
k(t\otimes v)=t\otimes\lambda(t^{-1}kt)v.
$$

Thus the restriction to $K$ is a direct sum of one-dimensional [group representations](../../../../../../group-representation.md). All representing matrices of $K$ commute, and the [derived subgroup](../../../../../../commutator-subgroup.md) $K'$ acts as the identity. Equivalently,

$$
K'\leq\ker\chi\qquad\text{for every }\chi\in\operatorname{Irr}(G).
$$

The intersection of the [character kernels](../../../../../../kernel-of-a-character.md) is trivial: the [regular representation](../../../../../../regular-representation.md) is faithful and is a direct sum of [irreducible representations](../../../../../../irreducible-representation.md). It follows that $K'=1$.

$$
\boxed{K\text{ is abelian}.}
$$

This proves the [abelian intersection of irreducible inducing subgroups](../../../../../../abelian-intersection-of-irreducible-inducing-subgroups.md) without assuming that every [subgroup](../../../../../../subgroup.md) of an M-group is itself monomial.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
