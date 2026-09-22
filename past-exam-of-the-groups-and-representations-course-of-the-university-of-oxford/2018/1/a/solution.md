<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [group](../../../../group-split.md) is a nonempty set $G$ with an operation $G\times G\to G$, $(g,h)\mapsto gh$, satisfying [associativity](../../../../associative-property.md), an [identity element](../../../../identity-element.md) $e$ with $eg=ge=g$, and an [inverse element](../../../../inverse-element.md) $g^{-1}$ with $gg^{-1}=g^{-1}g=e$ for every $g$. These are the [group axioms](../../../../group-axioms.md). An [Abelian group](../../../../abelian-group.md) additionally satisfies $gh=hg$ for every pair. A [subgroup](../../../../subgroup.md) is a subset that is itself a [group](../../../../group-split.md) under the restricted operation; equivalently, it is nonempty and closed under $hk^{-1}$.

Let $R:G\to\operatorname{GL}(V)$ be a nonzero, finite-dimensional complex [irreducible representation](../../../../irreducible-representation.md) of an [Abelian group](../../../../abelian-group.md). For each fixed $g$, commutativity gives

$$
R(g)R(h)=R(h)R(g)\qquad(h\in G).
$$

Thus $R(g)$ is an [intertwining operator](../../../../intertwining-operator.md) from $R$ to itself. By [Schur's lemma](../../../../schur-s-lemma.md) over the [complex numbers](../../../../complex-number.md), $R(g)=\lambda_g I_V$. Every line in $V$ is therefore an [invariant subspace](../../../../invariant-subspace.md). Since $R$ is [irreducible](../../../../irreducible-representation.md), this forces

$$
\boxed{\dim_{\mathbb C}V=1.}
$$

This is the finite-dimensional convention used throughout the paper. Without it, the literal assertion for arbitrary [Abelian groups](../../../../abelian-group.md) needs qualification. A concrete counterexample is $G=\mathbb C(t)^\times$ acting by multiplication on the complex [vector space](../../../../vector-space-split.md) $V=\mathbb C(t)$ of [rational functions](../../../../rational-function.md). Any nonzero invariant complex [vector subspace](../../../../vector-subspace.md) containing $f$ contains $gf$ for every nonzero rational $g$, hence contains every rational function. This is an infinite-dimensional [irreducible representation](../../../../irreducible-representation.md). The scalar conclusion of [Schur's lemma](../../../../schur-s-lemma.md) used above depends on finite dimensionality.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
