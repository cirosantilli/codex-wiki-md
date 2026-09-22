<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The bidual range condition implies both weak compactness and the stronger continuity of $T^*$.** First assume $T^{**}(X^{**})\subseteq J_YY$. The [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) makes $B_{X^{**}}$ weak-star compact, and $T^{**}$ is weak-star continuous. Hence its image is compact for the [weak-star topology](../../../../../../weak-star-topology.md) in $Y^{**}$. Because it lies in $J_YY$, it corresponds to a weakly compact subset $C\subseteq Y$ under $J_Y^{-1}$.

The identity $T^{**}J_X=J_YT$ gives $T(B_X)\subseteq C$. A [weakly compact set](../../../../../../weakly-compact-set.md) in a [Hausdorff space](../../../../../../hausdorff-space.md) is closed for the [weak topology](../../../../../../weak-topology-split.md), so $C$ is also norm-closed and contains the norm closure of $T(B_X)$. That closure is a [convex set](../../../../../../convex-set.md) closed in the [norm topology](../../../../../../norm-topology.md), hence weakly closed by the [Mazur theorem](../../../../../../mazur-theorem.md). It is therefore a weakly closed subset of the weakly compact $C$, and is a [weakly compact set](../../../../../../weakly-compact-set.md). This proves $(ii)\Longrightarrow(i)$.

For $(ii)\Longrightarrow(iii)$, fix $F\in X^{**}$. By the range assumption there is $y_F\in Y$ with $T^{**}F=J_Yy_F$. For every $y^*\in Y^*$,

$$
F(T^*y^*)=(T^{**}F)(y^*)=y^*(y_F).
$$

The right side is a defining weak-star continuous evaluation on $Y^*$. Since the [weak topology](../../../../../../weak-topology-split.md) on $X^*$ is determined by all $F\in X^{**}$, every scalar coordinate of $T^*$ for that topology is weak-star continuous. Therefore

$$
\boxed{T^*:(Y^*,w^*)\longrightarrow(X^*,w)\text{ is continuous}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
