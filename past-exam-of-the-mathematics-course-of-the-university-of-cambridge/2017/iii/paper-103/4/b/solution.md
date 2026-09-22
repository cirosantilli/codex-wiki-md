<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $m=n-k$ and take the subgroup $S_m\times S_k$ permuting the first $m$ and last $k$ letters. Define the [skew representation of a symmetric group](../../../../../../skew-representation-of-a-symmetric-group.md) as the multiplicity space

$$
\boxed{V^{\lambda/\mu}=\operatorname{Hom}_{S_m}(V^\mu,\operatorname{Res}^{S_n}_{S_m}V^\lambda).}
$$

The last-letter copy of $S_k$ commutes with $S_m$, so it acts on a map $f$ by $g\cdot f=\rho_\lambda(g)\circ f$. This gives a genuine $\mathbb C S_k$-module, without claiming that the whole restricted module is itself the skew representation. Equivalently,

$$
\operatorname{Res}^{S_n}_{S_m\times S_k}V^\lambda\cong\bigoplus_{\nu\vdash m}V^\nu\otimes V^{\lambda/\nu}.
$$

Fix a prefix tableau of shape $\mu$ and complete it to shape $\lambda$. Iterated [restriction branching rule for a symmetric group](../../../../../../restriction-branching-rule-for-a-symmetric-group.md) identifies the multiplicity-space [orthonormal basis](../../../../../../orthonormal-basis.md) with [standard skew Young tableaux](../../../../../../standard-skew-young-tableau.md), using labels $1,\ldots,k$ for the last $k$ cells. The [Young orthogonal form](../../../../../../young-orthogonal-form.md) restricts to this basis. When $R=s_iT$ is standard and $d=c_T(i+1)-c_T(i)$,

$$
s_iw_T=d^{-1}w_T+\sqrt{1-d^{-2}}\,w_R.
$$

An admissible interchange has $|d|\geq2$, so its off-diagonal coefficient is nonzero. Consequently $w_R$ belongs to the [group algebra](../../../../../../group-algebra.md) span of $w_T$. The preceding reduced-path argument reaches every standard skew tableau, so this span is the whole module. **Every $w_T$ is a [cyclic vector for a group representation](../../../../../../cyclic-vector-for-a-group-representation.md).** The inherited invariant inner product makes this a [unitary representation](../../../../../../unitary-representation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
