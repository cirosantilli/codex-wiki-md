<h1 id="8d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

When $[G:H]=2$, there are exactly two left [cosets](../../../../../../coset.md) and two right [cosets](../../../../../../coset.md). For $g\notin H$, both $gH$ and $Hg$ are the complement $G\setminus H$; for $g\in H$, both equal $H$. This is the [index-two subgroup is normal](../../../../../../index-two-subgroup-is-normal.md) argument: $gH=Hg$ for every $g$, which is equivalent to $gHg^{-1}=H$. Therefore **every [subgroup](../../../../../../subgroup.md) of index two is normal**.

In the [dihedral group](../../../../../../dihedral-group.md) $D_{2n}=\langle r,s\rangle$, the rotation [cyclic subgroup](../../../../../../cyclic-subgroup.md) $\langle r\rangle$ has order $n$ and index two, so it is a [normal subgroup](../../../../../../normal-subgroup.md). It is nontrivial and proper for the usual dihedral convention $n\geq2$ (polygon symmetries have $n\geq3$). If the degenerate convention $D_2=C_2$ were allowed, the claimed nontrivial proper [subgroup](../../../../../../subgroup.md) would not exist; the rotation argument uses $n>1$.

For any $k\geq3$, let $G=S_k$ and take the [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) $H$ of the letter $1$. Its elements freely permute the other $k-1$ letters, so

$$
|G|=k!,\qquad |H|=(k-1)!,\qquad [G:H]=k.
$$

Conjugation by $(1\ 2)$ sends $H$ to the stabilizer of $2$, which is different: for instance $(2\ 3)$ belongs to $H$ but does not fix $2$. Thus

$$
\boxed{G=S_k,\quad H=\{\sigma:\sigma(1)=1\}}
$$

gives a nonnormal [subgroup](../../../../../../subgroup.md) of every prescribed index $k\geq3$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
