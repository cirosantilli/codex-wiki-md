<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [group representation](../../../../group-representation.md) on a [vector space](../../../../vector-space-split.md) $V$ over a [field](../../../../field.md) $K$ is a [group homomorphism](../../../../group-homomorphism.md) $R:G\to\operatorname{GL}(V)$. In particular, $R(gh)=R(g)R(h)$, $R(e)=I$ and $R(g^{-1})=R(g)^{-1}$. Choosing a [basis](../../../../basis.md) identifies it with a [matrix representation](../../../../matrix-representation.md).

Two [group representations](../../../../group-representation.md) $R$ on $V$ and $S$ on $W$ are [equivalent representations](../../../../equivalence-of-group-representations.md) when an invertible [linear map](../../../../linear-map.md) $T:V\to W$ satisfies $TR(g)=S(g)T$ for every $g$. Thus $S(g)=TR(g)T^{-1}$; they differ only by a choice of [basis](../../../../basis.md).

A nonzero [group representation](../../../../group-representation.md) is a [reducible representation](../../../../reducible-representation.md) if there is a [vector subspace](../../../../vector-subspace.md) $U$ with $0\ne U\ne V$ and $R(g)U\subseteq U$ for every $g$. It is an [irreducible representation](../../../../irreducible-representation.md) if it has no such [invariant subspace](../../../../invariant-subspace.md). Reducibility alone does not assert the existence of an invariant complementary [vector subspace](../../../../vector-subspace.md); that stronger conclusion says that the [representation](../../../../group-representation.md) is a [semisimple representation](../../../../semisimple-representation.md).

The [Schur lemma](../../../../schur-s-lemma.md) states that an [intertwiner](../../../../intertwiner.md) $T$ between [irreducible representations](../../../../irreducible-representation.md) is either zero or an [isomorphism](../../../../isomorphism.md). Consequently an [intertwiner](../../../../intertwiner.md) between inequivalent [irreducible representations](../../../../irreducible-representation.md) is zero. For a finite-dimensional [irreducible representation](../../../../irreducible-representation.md) over the [complex numbers](../../../../complex-number.md), every commuting [endomorphism](../../../../endomorphism.md) is scalar:

$$
\boxed{TR(g)=R(g)T\quad(\forall g)\quad\Longrightarrow\quad T=\lambda I.}
$$

For the first assertion, the [kernel](../../../../kernel-of-a-linear-map-split.md) and [image](../../../../image-of-a-function.md) of $T$ are [invariant subspaces](../../../../invariant-subspace.md), so a nonzero $T$ is injective and surjective. For the scalar conclusion, choose an [eigenvalue](../../../../eigenvalue.md) $\lambda$ of $T$. The [intertwiner](../../../../intertwiner.md) $T-\lambda I$ has a nonzero [kernel](../../../../kernel-of-a-linear-map-split.md), so it must vanish. The finite-dimensional complex hypothesis matters: the scalar conclusion need not hold over the [real numbers](../../../../real-number.md), as a real planar rotation through $\pi/2$ is an [irreducible representation](../../../../irreducible-representation.md) of the cyclic [group](../../../../group-split.md) of order four, while the rotation itself is a commuting nonscalar [endomorphism](../../../../endomorphism.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
