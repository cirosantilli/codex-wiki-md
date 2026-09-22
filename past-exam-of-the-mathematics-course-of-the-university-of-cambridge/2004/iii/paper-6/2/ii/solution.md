<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This proof uses neither the [axiom of choice](../../../../../../axiom-of-choice.md) nor a preliminary choice of points in all the given sets. For each nonempty $A_j$, form a disjoint union $X_j=A_j\sqcup\{\infty_j\}$ with a distinguished added point, and give it the [topology](../../../../../../topology-split.md)

$$
\tau_j=\{\varnothing,A_j,\{\infty_j\},X_j\}.
$$

The original set $A_j$ has the indiscrete subspace topology, and is [clopen](../../../../../../clopen-set.md). Any open cover of $X_j$ either contains $X_j$, or contains both $A_j$ and $\{\infty_j\}$, so it has a subcover of at most two members. Thus $X_j$ is compact by a proof requiring no choices. No [Hausdorff](../../../../../../hausdorff-space.md) restriction is imposed in this question, and these generally non-Hausdorff spaces are allowed.

The product $X=\prod_{j\geq1}X_j$ has the explicitly given all-infinity point, so it is nonempty without choice. By the assumed countable-product [compactness](../../../../../../compact-space.md) it is compact. For each $j$ let

$$
F_j=\{x\in X:x_j\in A_j\}.
$$

The coordinate projection is continuous and $A_j$ is closed in $X_j$, so $F_j$ is closed. Any finite intersection of the $F_j$ is nonempty: pick an element of each of those finitely many nonempty sets and put $\infty_k$ in every other coordinate. Finite choice follows by induction in ordinary set theory without assuming the [axiom of choice](../../../../../../axiom-of-choice.md).

[Compactness](../../../../../../compact-space.md) and the [finite intersection property](../../../../../../finite-intersection-property.md) now give $\bigcap_{j\geq1}F_j\ne\varnothing$. Choose one point $x$ from this single nonempty set. The function $f(j)=x_j$ satisfies $f(j)\in A_j$ for every $j$, proving the [axiom of countable choice](../../../../../../axiom-of-countable-choice.md).

**The implication holds in choice-free set theory:** [countable product compactness implies countable choice](../../../../../../countable-product-compactness-implies-countable-choice.md). The printed lower index zero is inconsistent with the stated positive-integer index set; indexing from one merely relabels this argument and changes no conclusion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
