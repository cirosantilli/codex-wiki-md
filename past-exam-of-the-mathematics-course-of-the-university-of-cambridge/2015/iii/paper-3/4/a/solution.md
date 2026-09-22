<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [dimension of a topological space by irreducible chains](../../../../../../dimension-of-a-topological-space-by-irreducible-chains.md) is the supremum of the integers $d$ for which there is a chain $Z_0\subsetneq Z_1\subsetneq\cdots\subsetneq Z_d$ of nonempty irreducible closed subsets of the space. Closedness here is relative to the given locally closed space. For varieties this is their [Krull dimension](../../../../../../krull-dimension.md).

An [algebraic group](../../../../../../algebraic-group.md) is a group whose underlying space is an [algebraic variety](../../../../../../algebraic-variety.md) and whose multiplication $G\times G\to G$ and inversion $G\to G$ are morphisms. An [algebraic group action](../../../../../../algebraic-group-action.md) on a variety $V$ is a morphism $G\times V\to V$ satisfying the identity and associativity axioms of a [group action](../../../../../../group-action.md).

For the homomorphism $\varphi$, the kernel is $\varphi^{-1}(1_H)$, so **the kernel is closed**. To prove closedness of the image, use the [Chevalley constructibility theorem](../../../../../../chevalley-constructibility-theorem.md): the image of a morphism of varieties is constructible. Thus $S=\varphi(G)$ is a [constructible subset of a variety](../../../../../../constructible-subset-of-a-variety.md) and an abstract subgroup. Its closure $C$ is also a subgroup: translation by elements of $S$ preserves $C$, and continuity then extends multiplication and inversion to $C$.

A dense constructible subset contains a dense open subset $U$ of its closure. For $c\in C$, both $U$ and $cU$ are dense open subsets of $C$, so their intersection is nonempty. If $u=cv$ with $u,v\in U\subseteq S$, then $c=uv^{-1}\in S$. Hence $S=C$, proving that **the image is closed**. This is the principle that a [constructible subgroup is closed](../../../../../../constructible-subgroup-is-closed.md).

Every nonempty fiber of $G\to S$ is a translate of $\ker\varphi$ and has that same dimension. The [fiber dimension theorem](../../../../../../fiber-dimension-theorem.md) therefore gives

$$
\boxed{\dim G=\dim\ker\varphi+\dim\operatorname{im}\varphi.}
$$

This [dimension formula for an algebraic group homomorphism](../../../../../../dimension-formula-for-an-algebraic-group-homomorphism.md) is a dimension statement, so it does not require separability of $\varphi$.

For a [dimension vector of a quiver representation](../../../../../../dimension-vector-of-a-quiver-representation.md) $\mathbf n$, set

$$
\operatorname{Rep}_Q(\mathbf n)=\prod_{\rho:i\to j}\operatorname{Hom}_k(k^{n_i},k^{n_j}),\qquad\operatorname{GL}(\mathbf n)=\prod_i\operatorname{GL}_{n_i}(k).
$$

The [base change action on quiver representations](../../../../../../base-change-action-on-quiver-representations.md) is

$$
\boxed{(g\cdot f)_\rho=g_{t(\rho)}f_\rho g_{s(\rho)}^{-1}.}
$$

The entries are regular functions on the product of the [general linear groups](../../../../../../general-linear-group.md) and the [quiver representation space](../../../../../../quiver-representation-space.md), because inverse entries are cofactors divided by the invertible determinant. Thus this is an [algebraic group action](../../../../../../algebraic-group-action.md).

For nonzero $\mathbf n$, let $\Delta k^\times$ be the common scalar subgroup $(\lambda I_{n_i})_i$ and define $\operatorname{PGL}(\mathbf n)=\operatorname{GL}(\mathbf n)/\Delta k^\times$. Common scalars act trivially, so the formula descends to an [algebraic group action](../../../../../../algebraic-group-action.md) of this [projective base change group of a quiver](../../../../../../projective-base-change-group-of-a-quiver.md). This is a quotient by one common scalar, not a product of the individual projective groups. If every $n_i=0$, the representation space is a point and both actions are taken to be trivial.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
