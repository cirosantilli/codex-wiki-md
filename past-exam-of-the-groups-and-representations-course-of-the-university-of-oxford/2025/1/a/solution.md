<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [group representation](../../../../group-representation.md) on a [vector space](../../../../vector-space-split.md) $V$ is a [group homomorphism](../../../../group-homomorphism.md) $R:G\to\operatorname{GL}(V)$, so $R(gh)=R(g)R(h)$ and $R(e)=I$. A nonzero [group representation](../../../../group-representation.md) is an [irreducible representation](../../../../irreducible-representation.md) if its only [invariant subspaces](../../../../invariant-subspace.md) are $0$ and $V$. Here the [representations](../../../../group-representation.md) and [characters](../../../../character-of-a-representation.md) are finite-dimensional over the [complex numbers](../../../../complex-number.md).

The [character of a representation](../../../../character-of-a-representation.md) is $\chi_R(g)=\operatorname{tr}R(g)$. Three useful properties are:

- It is a [class function](../../../../class-function.md): $\chi_R(hgh^{-1})=\chi_R(g)$, by the cyclic property of the [trace](../../../../matrix-trace.md).
- It is additive on a [direct sum](../../../../direct-sum.md) and multiplicative on a [tensor product of group representations](../../../../tensor-product-of-group-representations.md): $\chi_{R\oplus S}=\chi_R+\chi_S$ and $\chi_{R\otimes S}=\chi_R\chi_S$.
- The [irreducible characters](../../../../irreducible-character.md) obey [character orthogonality](../../../../character-orthogonality.md):$$
  \langle\chi_r,\chi_s\rangle=\frac1{|G|}\sum_{g\in G}\chi_r(g)^*\chi_s(g)=\delta_{rs}.
  $$

In particular, $\chi_R(e)=\dim V$ and $\chi_R(g^{-1})=\chi_R(g)^*$, the latter following from [unitarization of a finite-group representation](../../../../unitarization-of-a-finite-group-representation.md). The [character inner product](../../../../character-inner-product.md) $\langle\chi_r,\chi_R\rangle$ counts the multiplicity of an [irreducible representation](../../../../irreducible-representation.md) $r$ in $R$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
