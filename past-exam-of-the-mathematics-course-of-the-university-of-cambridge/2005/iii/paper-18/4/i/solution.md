<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $p:E\to S^r$ be the [Serre fibration](../../../../../../serre-fibration.md). For $r\geq1$, cover the base by $U=S^r\setminus\{s\}$ and a small open ball $V$ about $s$. Write $A=p^{-1}U$ and $B=p^{-1}V$. The contractible-base assumption gives $A\simeq F$ and identifies the pair $(B,A\cap B)$, up to fiberwise [homotopy](../../../../../../homotopy.md), with $(F\times V,F\times(V\setminus\{s\}))$.

[Excision](../../../../../../excision-theorem.md) for the open cover $E=A\cup B$ gives $H_i(E,A)\cong H_i(B,A\cap B)$. The relative base pair has

$$
H_j(V,V\setminus\{s\};\mathbb Z)=\begin{cases}\mathbb Z,&j=r,\\0,&j\ne r,\end{cases}
$$

by the deformation retraction of the punctured ball onto $S^{r-1}$ and its [relative homology](../../../../../../relative-homology.md) sequence. The relative [Künneth theorem](../../../../../../kunneth-theorem.md) therefore gives

$$
H_i(E,A;\mathbb Z)\cong H_{i-r}(F;\mathbb Z).
$$

There is no Tor term because the only nonzero base group is free. The [long exact sequence of a pair](../../../../../../long-exact-sequence-in-relative-homology.md), replacing $A$ by its homotopy-equivalent fiber, now becomes

$$
\boxed{\cdots\longrightarrow H_i(F;\mathbb Z)\longrightarrow H_i(E;\mathbb Z)
\longrightarrow H_{i-r}(F;\mathbb Z)\longrightarrow H_{i-1}(F;\mathbb Z)\longrightarrow\cdots.}
$$

The last arrow is the relative boundary transported through these identifications; it can encode twisting, so it has not been set to zero. This proves the [relative homology of a fibration over a sphere](../../../../../../relative-homology-of-a-fibration-over-a-sphere.md) sequence. In the dimension-zero case, the total space is the disjoint union of the two fibers and the same formula is the split sequence for that union.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
