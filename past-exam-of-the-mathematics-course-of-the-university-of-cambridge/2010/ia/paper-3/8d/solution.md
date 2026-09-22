<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

For each $g\in G$, conjugation sends a subgroup $H$ to $gHg^{-1}$, a subgroup of the same order and hence still proper. Identity conjugation fixes every subgroup, and

$$
g_1(g_2Hg_2^{-1})g_1^{-1}=(g_1g_2)H(g_1g_2)^{-1}.
$$

These verify the [group action](../../../../../group-action.md) laws.

The [stabilizer subgroup](../../../../../stabilizer-subgroup.md) of $B$ for this [conjugation action](../../../../../conjugation-action.md) is its [normalizer](../../../../../normalizer.md) $N_G(B)$. Since $B\leq N_G(B)$, the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) gives the number of distinct conjugates as

$$
\boxed{m=[G:N_G(B)]\leq[G:B].}
$$

All these conjugate subgroups contain the identity, so counting that element only once gives

$$
\left|\bigcup_{g\in G}gBg^{-1}\right|\leq1+m(|B|-1)\leq1+[G:B](|B|-1)=|G|-[G:B]+1<|G|.
$$

The last inequality uses the properness of $B$, so $[G:B]>1$. There is therefore an element outside this union, which is **not conjugate to any element of $B$**. This proves that [conjugates of a proper subgroup do not cover a finite group](../../../../../conjugates-of-a-proper-subgroup-do-not-cover-a-finite-group.md), including the case $B=\{1\}$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
