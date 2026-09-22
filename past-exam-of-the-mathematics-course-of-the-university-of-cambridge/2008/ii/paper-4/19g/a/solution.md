<h1 id="19g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work over the complex numbers. By [Maschke's theorem](../../../../../../maschke-s-theorem.md), restriction to the normal subgroup $A$ is a direct sum of its [isotypic components](../../../../../../isotypic-component.md). For an irreducible $A$-type $W$, denote its isotypic component in $V$ by $V_W$. Normality makes $G$ permute these components, by conjugating the $A$-types. Any union of orbits spans a $G$-invariant subspace, so irreducibility of $V$ means that all occurring components form a single orbit.

If there is only one component, restriction is isotypic, as claimed. Otherwise take one component $V_W$ and its stabilizer $H=\{g:gV_W=V_W\}$, a proper subgroup. This is an [irreducible representation](../../../../../../irreducible-representation.md) of $H$: if $0\ne U\subsetneq V_W$ were $H$-invariant, the direct sum of its translates over coset representatives for $G/H$ would be a nonzero proper $G$-invariant subspace of $V$. It is direct because the translates lie in distinct isotypic components, and proper because $\dim U<\dim V_W$.

The natural map from the [induced representation](../../../../../../induced-representation.md) sends $g\otimes v$ to $gv$. It identifies the direct-sum coset decomposition with all isotypic components of $V$, so is bijective and $G$-equivariant. Consequently

$$
\boxed{V\cong\operatorname{Ind}_H^G V_W.}
$$

This proves the dichotomy directly, including the irreducibility of the representation being induced.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19G](../../19g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
