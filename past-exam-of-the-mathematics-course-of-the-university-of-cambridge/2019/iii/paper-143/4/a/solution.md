<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [amenable group](../../../../../../amenable-group.md) is a group $G$ admitting a left-invariant [finitely additive probability measure](../../../../../../finitely-additive-probability-measure.md) $m:\mathcal P(G)\to[0,1]$. For a $G$-set $X$, subsets $A,B\subseteq X$ are [equidecomposable subsets under a group action](../../../../../../equidecomposable-subsets-under-a-group-action.md) if there are finite partitions $A=\bigsqcup_iA_i$, $B=\bigsqcup_iB_i$ and elements $g_i\in G$ such that $g_iA_i=B_i$. The action is a [paradoxical group action](../../../../../../paradoxical-group-action.md) if $X$ contains two disjoint subsets, each $G$-equidecomposable with $X$.

To prove the [nonamenability of a nonabelian free group](../../../../../../nonamenability-of-a-nonabelian-free-group.md), write $F_2=\langle a,b\rangle$ and let $W(s)$ be the set of nonempty reduced words beginning with $s\in\{a,a^{-1},b,b^{-1}\}$. Cancellation of the first letter gives the disjoint decompositions

$$
F_2=W(a)\sqcup aW(a^{-1}),
\qquad
F_2=W(b)\sqcup bW(b^{-1}).
$$

If an invariant measure $m$ existed, these would imply

$$
1=m(W(a))+m(W(a^{-1})),
\qquad
1=m(W(b))+m(W(b^{-1})).
$$

Every singleton has measure zero: invariance gives all singletons the same measure, and finite additivity over arbitrarily many distinct points forces that measure to vanish. The four sets $W(s)$ partition $F_2\setminus\{1\}$, so their measures sum to one. The two displayed equations say that the same sum is two, a contradiction. Hence

$$
\boxed{F_2\text{ is not amenable}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 143](../../../paper-143-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
