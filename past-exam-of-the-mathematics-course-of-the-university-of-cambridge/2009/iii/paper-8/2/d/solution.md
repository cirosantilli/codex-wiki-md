<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Pass to $B=\overline A^{\|\cdot\|}$. Closed invariant subspaces and intertwining maps are unchanged by this closure, and $BH$ is still dense. Because $B$ is a star-algebra, every closed invariant subspace reduces it.

Every nonzero nondegenerate compact-operator representation contains an irreducible reducing subspace. Indeed choose a nonzero positive compact element $b$; an isolated nonzero [eigenvalue](../../../../../../eigenvalue.md) gives a nonzero finite-rank spectral projection $e\in B$ by [continuous functional calculus](../../../../../../continuous-functional-calculus.md), using a function vanishing at zero. The finite-dimensional corner $eBe$ has a minimal nonzero projection $p$, with $pBp=\mathbb Cp$. Choose a unit vector $v\in pH$ and set $K=\overline{Bv}$. Then $pK=\mathbb Cv$, since $pbv=pbpv$ is scalar times $v$. If $Q$ is the projection onto a reducing subspace of $K$, it commutes with $B$, and $Qv=pQv\in\mathbb Cv$. Its projection property makes $Qv$ either zero or $v$. Cyclicity then makes $Q=0$ or $I_K$. Thus $K$ is irreducible.

Take a maximal orthogonal family of such irreducible reducing subspaces, by the [axiom of choice](../../../../../../axiom-of-choice.md). If their orthogonal complement were nonzero, its restricted representation would be nondegenerate: a vector annihilated by all restricted $B$ would, by taking adjoints, be orthogonal to $BH$ and hence zero. The image of $B$ on this complement is a norm-closed [C-star algebra](../../../../../../c-star-algebra.md) of [compact operators](../../../../../../compact-operator-split.md), so the preceding construction gives another irreducible summand, contradicting maximality. The family therefore exhausts $H$.

Finally, suppose one irreducible equivalence class occurred infinitely often. Choose some $b\in B$ acting nontrivially on that class, and a unit vector $v$ with $\|bv\|>0$. Transport $v$ by unitary intertwiners into distinct equivalent summands. These vectors are orthonormal; their images under $b$ are orthogonal and all have the same nonzero norm. That contradicts compactness of $b$. **The decomposition has finite multiplicity for every irreducible type**, as claimed in [nondegenerate representations by compact operators](../../../../../../nondegenerate-representations-by-compact-operators.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
