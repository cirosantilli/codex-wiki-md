<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use induction on the order of the finite [p-group](../../../../../../p-group.md). The trivial group is nilpotent. For $G\ne1$, the permitted center theorem gives $Z=Z(G)\ne1$, so the [quotient group](../../../../../../quotient-group.md) $G/Z$ is a smaller [p-group](../../../../../../p-group.md). By induction it has a [central series](../../../../../../central-series.md)

$$
1=\overline H_0\le\overline H_1\le\cdots\le\overline H_s=G/Z.
$$

Let $H_i$ be the inverse image of $\overline H_i$ under the quotient map, so $H_0=Z$ and $H_s=G$. Centrality in the quotient gives $[H_i,G]\le H_{i-1}$ for $i\ge1$: the image of every such [group commutator](../../../../../../group-commutator.md) lies in $\overline H_{i-1}$. Also $[Z,G]=1$. Therefore

$$
\boxed{1\le Z=H_0\le H_1\le\cdots\le H_s=G}
$$

is a [central series](../../../../../../central-series.md) of $G$. This proves **every finite p-group is nilpotent**, including the case $Z=G$, when the quotient is trivial and the series is simply $1\le G$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
