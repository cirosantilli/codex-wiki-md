<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose disjoint [subsets](../../../../../../subset.md) $K_1,K_2\subseteq[n]$ of size $k$ and let $R=[n]\setminus(K_1\cup K_2)$. The [two-block extremisers for the cross-Sperner inequality](../../../../../../two-block-extremisers-for-the-cross-sperner-inequality.md) are

$$
\mathcal A=\{S\subseteq[n]:K_1\subseteq S,\ S\cap K_2=\varnothing\},\qquad \mathcal B=\{S\subseteq[n]:K_1\nsubseteq S,\ S\cap K_2\ne\varnothing\}.
$$

For $A\in\mathcal A$ and $B\in\mathcal B$, some point of $K_1$ belongs to $A$ but not $B$, so $A\nsubseteq B$. Some point of $K_2$ belongs to $B$ but not $A$, so $B\nsubseteq A$. Thus these form a [cross-Sperner family](../../../../../../cross-sperner-family.md) pair.

An element of $\mathcal A$ fixes its intersections with both blocks and freely chooses its [subset](../../../../../../subset.md) of $R$. An element of $\mathcal B$ chooses any proper [subset](../../../../../../subset.md) of $K_1$, any nonempty [subset](../../../../../../subset.md) of $K_2$, and any [subset](../../../../../../subset.md) of $R$. Hence

$$
\boxed{|\mathcal A|=2^{n-2k}=2^{-2k}2^n,\qquad |\mathcal B|=(2^k-1)^2\,2^{n-2k}=(1-2^{-k})^2\,2^n.}
$$

The hypotheses ensure that the blocks exist and both [set families](../../../../../../set-family.md) are nonempty, including when $n=2k$. Moreover,

$$
\sqrt{|\mathcal A|}+\sqrt{|\mathcal B|}=\bigl(1+(2^k-1)\bigr)2^{(n-2k)/2}=2^{n/2},
$$

so this construction attains equality in the [Cross-Sperner inequality](../../../../../../cross-sperner-inequality.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
