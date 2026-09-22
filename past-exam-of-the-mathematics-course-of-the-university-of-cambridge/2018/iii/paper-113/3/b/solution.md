<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\mathcal Q=\mathcal K_X^*/\mathcal O_X^*$, the quotient in [sheaves of abelian groups](../../../../../../sheaf-of-abelian-groups.md), where $\mathcal K_X^*$ is the [sheaf of nonzero rational functions on an irreducible variety](../../../../../../sheaf-of-nonzero-rational-functions-on-an-irreducible-variety.md) and $\mathcal O_X^*$ is the [sheaf of units of the structure sheaf](../../../../../../sheaf-of-units-of-the-structure-sheaf.md). At a closed point, the [discrete valuation](../../../../../../discrete-valuation.md) induces an isomorphism

$$
\mathcal Q_P=K^*/\mathcal O_{X,P}^*\xrightarrow{\ \sim\ }\mathbb Z,\qquad[f]\longmapsto\nu_P(f).
$$

The kernel consists precisely of the units of the [discrete valuation ring](../../../../../../discrete-valuation-ring.md), and surjectivity follows by taking powers of a [uniformizer](../../../../../../uniformizer.md).

A global section of $\mathcal Q$ is locally represented by nonzero [rational functions](../../../../../../rational-function.md). Since $X$ has a finite affine cover and is Noetherian, it is [quasi-compact](../../../../../../compact-space.md), so finitely many such representatives suffice. Each has only finitely many zeros and poles; consequently the valuations of the section define a finite [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md). A section with zero valuation at every closed point is zero in every stalk and therefore zero. This gives an injective map

$$
\Gamma(X,\mathcal Q)\longrightarrow\operatorname{Div}(X).
$$

It is surjective as well. For $D=\sum_P n_PP$, take a rational [uniformizer](../../../../../../uniformizer.md) $t_P$ at each point of its finite support. On a sufficiently small neighborhood of $P$, the function $t_P^{n_P}$ has the prescribed divisor there: remove the other points in its zero and pole set and the other support points of $D$. On the complement of the support use the rational function $1$. On overlaps these representatives have the same valuations at every point, so their ratios are units everywhere on the overlap, and their classes in $\mathcal Q$ agree. The [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md) now supplies a global section. Thus

$$
\Gamma(X,\mathcal Q)\cong\operatorname{Div}(X).
$$

Since $X$ is irreducible, $\Gamma(X,\mathcal K_X^*)=K^*$. Under this identification the map to $\Gamma(X,\mathcal Q)$ is $f\mapsto\operatorname{div}(f)$. Its image is exactly the group of [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) elements, and hence

$$
\boxed{\operatorname{coker}\bigl(H^0(X,\mathcal K_X^*)\to H^0(X,\mathcal Q)\bigr)\cong\operatorname{Cl}(X).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
