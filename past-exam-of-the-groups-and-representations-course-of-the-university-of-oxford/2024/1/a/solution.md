<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [group representation](../../../../group-representation.md) on a [vector space](../../../../vector-space-split.md) $V$ is a [group homomorphism](../../../../group-homomorphism.md) $R:G\to\operatorname{GL}(V)$: $R(gh)=R(g)R(h)$ and $R(e)=I$. A [reducible representation](../../../../reducible-representation.md) has a nonzero proper [invariant subspace](../../../../invariant-subspace.md) $W\subset V$, meaning $R(g)W\subseteq W$ for every $g$. Over the [complex numbers](../../../../complex-number.md), a finite-dimensional [representation](../../../../group-representation.md) of a [finite group](../../../../finite-group.md) is a [direct sum](../../../../direct-sum.md) of [irreducible representations](../../../../irreducible-representation.md), by [Maschke's theorem](../../../../maschke-s-theorem.md).

The [character of a representation](../../../../character-of-a-representation.md) is $\chi_R(g)=\operatorname{tr}R(g)$. The cyclic property of the [trace](../../../../matrix-trace.md) makes it a [class function](../../../../class-function.md):

$$
\chi_R(hgh^{-1})=\operatorname{tr}\bigl(R(h)R(g)R(h)^{-1}\bigr)=\chi_R(g).
$$

Thus a [character](../../../../character-of-a-representation.md) is specified by one number per [conjugacy class](../../../../conjugacy-class.md), much less information than all the [representation](../../../../group-representation.md) [matrices](../../../../matrix.md). Moreover,

$$
\chi_{R\oplus S}=\chi_R+\chi_S,\qquad
\chi_{R\otimes S}=\chi_R\chi_S,\qquad
\boxed{m_r=\frac1{|G|}\sum_{g\in G}\overline{\chi_r(g)}\chi_R(g).}
$$

Here [character orthogonality](../../../../character-orthogonality.md) says that $m_r$ is the multiplicity of the [irreducible representation](../../../../irreducible-representation.md) $r$. Consequently [characters](../../../../character-of-a-representation.md) determine finite-dimensional complex [representations](../../../../group-representation.md) up to [equivalence of group representations](../../../../equivalence-of-group-representations.md) and compute [tensor product of group representations](../../../../tensor-product-of-group-representations.md) decompositions without constructing a new [basis](../../../../basis.md) explicitly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
