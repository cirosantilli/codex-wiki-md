<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The [Lie group](../../../../../lie-group.md) $PSL(2,\mathbb C)$ is a [second-countable space](../../../../../second-countable-space.md). For every point of its discrete [subgroup](../../../../../subgroup.md), choose the first basic neighbourhood isolating that point; different elements require different such neighbourhoods. This injects $G$ into a countable set, proving countability.

A discrete [subgroup](../../../../../subgroup.md) is closed and meets compact sets in finitely many points. Indeed, distinct [subgroup](../../../../../subgroup.md) elements accumulating anywhere would give quotients converging to identity, contradicting an identity neighbourhood containing no other [subgroup](../../../../../subgroup.md) element. To apply this, use the positive Hermitian determinant-one model of [hyperbolic space](../../../../../hyperbolic-space.md). At the base point $I$, the image under a determinant-one representative $g$ is $gg^*$ and

$$
2\cosh d(I,gg^*)=\operatorname{tr}(gg^*)=\sum_{i,j}|g_{ij}|^2.
$$

This distance formula follows by unitary diagonalization: [eigenvalues](../../../../../eigenvalue.md) are $e^t,e^{-t}$ and the axial hyperbolic displacement is $|t|$. Thus bounded displacement bounds all matrix entries. The determinant-one condition is closed, so the resulting set is compact; the quotient by $\{I,-I\}$ is compact too. Conjugation gives the same conclusion at any base point. These are the [bounded displacement sets of hyperbolic isometries are compact](../../../../../bounded-displacement-sets-of-hyperbolic-isometries-are-compact.md) facts.

Hence, for each $R$, only finitely many $g\in G$ satisfy $d(p,gp)\le R$. Any enumeration of an infinite group without repetitions therefore has **$d(p,g_np)\to\infty$**. A finite discrete group is a harmless exception to the wording: it has no infinite enumeration of distinct elements, and proper discontinuity is immediate.

For a [compact set](../../../../../compact-space.md) $C$, put $R=\max_{x\in C}d(p,x)$. If $gC\cap C\ne\varnothing$, choose $x,gx\in C$. The triangle inequality gives $d(p,gp)\le d(p,gx)+d(x,p)\le2R$. Only finitely many such $g$ exist, proving [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md). Conversely, if the [subgroup](../../../../../subgroup.md) is not discrete, there are distinct $g_n\to e$. A closed ball about $p$ then meets its images under infinitely many $g_n$, violating this compact-set definition. Thus **discreteness is equivalent to proper discontinuity**. Here proper discontinuity allows finite point stabilizers; a stronger convention requiring freeness would exclude discrete elliptic subgroups and is not the equivalence intended.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
