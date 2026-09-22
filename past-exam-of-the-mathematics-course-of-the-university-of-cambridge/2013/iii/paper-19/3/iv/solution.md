<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**There is a [cofinal branch](../../../../../../cofinal-branch.md).** We give a proof that does not require distinct limit-level nodes to have different predecessor chains.

The set $S=\{\alpha<\lambda:\operatorname{cf}(\alpha)=\kappa\}$ is stationary. Indeed a strictly increasing continuous $\kappa$-sequence in any [club set](../../../../../../club-set.md) has supremum in that [club set](../../../../../../club-set.md), below $\lambda$, of [cofinality](../../../../../../cofinality.md) $\kappa$. At each $\alpha\in S$, there are fewer than $\kappa$ pairs of nodes on $T_\alpha$. For every pair whose predecessor chains below $\alpha$ differ, choose a height where they differ. Since $\operatorname{cf}(\alpha)=\kappa$, all these heights are bounded by some $\beta_\alpha<\alpha$. Consequently nodes in $T_\alpha$ having the same predecessor at $\beta_\alpha$ have identical predecessor chains below $\alpha$.

The [Fodor lemma](../../../../../../fodor-lemma.md) states that a regressive [function](../../../../../../function-split.md) on a stationary [subset](../../../../../../subset.md) of a regular uncountable [cardinal](../../../../../../cardinal-number.md) is constant on a stationary [subset](../../../../../../subset.md). Applying it here, $\beta_\alpha$ has a constant value $\beta$ on a stationary [subset](../../../../../../subset.md) $S'$. Choose $t_\alpha\in T_\alpha$ for each $\alpha\in S'$. The level $T_\beta$ has fewer than $\kappa<\lambda$ nodes. Partitioning $S'$ according to the predecessor of $t_\alpha$ at height $\beta$, one fiber $S''$ is stationary, since the union of fewer than $\lambda$ nonstationary sets is nonstationary. Let its common predecessor be $t$.

For $\alpha<\alpha'$ in $S''$, the predecessor of $t_{\alpha'}$ at level $\alpha$ and $t_\alpha$ have the same predecessor $t$ at level $\beta$. Their chains below $\alpha$ therefore agree. For each $\nu<\lambda$, choose $\alpha\in S''$ above $\nu$ and let $b_\nu$ be the predecessor of $t_\alpha$ at level $\nu$. The preceding comparison makes $b_\nu$ independent of that choice. The nodes $b_\nu$ form a chain through every level:

$$
\boxed{\{b_\nu:\nu<\lambda\}\text{ is a cofinal branch of }T.}
$$

This proves the [uniformly narrow regular-height tree branch theorem](../../../../../../uniformly-narrow-regular-height-tree-branch-theorem.md). The uniform bound below the smaller regular $\kappa$ is stronger than merely bounding each level below $\lambda$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
