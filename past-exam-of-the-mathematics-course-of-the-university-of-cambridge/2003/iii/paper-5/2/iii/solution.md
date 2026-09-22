<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose representatives $T$ of the right cosets $Hg$, including $1$, and let $M=\max_{t\in T}|t|_A$. This is finite because the index is finite. For $t\in T$ and $a\in A^{\pm1}$, let $\overline{ta}\in T$ represent $Hta$. The elements

$$
s(t,a)=ta\overline{ta}^{-1}\in H
$$

form a finite generating set $S$ for $H$, after adjoining inverses and discarding identities. To see generation rather than merely quote [Schreier's lemma](../../../../../../schreier-s-lemma.md), write $h=a_1\cdots a_n$ and let $t_i$ represent $Ha_1\cdots a_i$. Then $t_0=t_n=1$ and

$$
h=(t_0a_1t_1^{-1})(t_1a_2t_2^{-1})\cdots(t_{n-1}a_nt_n^{-1}).
$$

Each factor is a Schreier generator. For a shortest $A$-word this gives $|h|_S\le|h|_A$. Conversely every Schreier generator has $A$-length at most $2M+1$, so $|h|_A\le(2M+1)|h|_S$. Hence the inclusion $H\hookrightarrow G$ obeys

$$
\boxed{d_S(h,h')\le d_A(h,h')\le(2M+1)d_S(h,h')}.
$$

Every $g\in G$ can be written $g=ht$, and $d_A(g,h)=|t|_A\le M$. Thus the inclusion is coarsely onto and is a [finite-index subgroup quasi-isometry](../../../../../../finite-index-subgroup-quasi-isometry.md).

Only finite generation of $G$ was needed for the metric argument. Under the given finite-presentation hypothesis, $H$ is also finitely presented: the corresponding finite-sheeted cover of a finite [presentation complex](../../../../../../presentation-complex.md) has finitely many cells, and a spanning-tree reduction of its one-skeleton gives a [finite group presentation](../../../../../../finite-group-presentation.md). Therefore it belongs to the class of groups used in part (ii).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
