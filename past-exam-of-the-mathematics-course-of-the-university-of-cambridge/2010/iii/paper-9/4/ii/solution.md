<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n\geq1$, let $C_n=\{Z\in X:n\notin Z\}$. The presence or absence of $n$ is determined by a sufficiently long finite [initial segment](../../../../../../initial-segment.md), so $C_n$ and its complement are [open sets](../../../../../../open-set.md) in the [ordinary topology on infinite subsets](../../../../../../ordinary-topology-on-infinite-subsets.md). The [Ellentuck topology](../../../../../../ellentuck-topology.md) is finer, hence each $C_n$ is star-[clopen](../../../../../../clopen-set.md) and in particular star-[closed](../../../../../../closed-set.md). Their union is

$$
\bigcup_{n\geq1}C_n=X\setminus\{\mathbb N\}.
$$

Every basic star-neighborhood $[s,A]$ of $\mathbb N$ has $s=\{1,\ldots,k\}$ for some $k\geq0$, and its reservoir $A$ contains every integer greater than $k$. Choosing $n>k$ gives $\mathbb N\setminus\{n\}\in[s,A]\cap C_n$. Thus $\mathbb N$ is in the star-[closure](../../../../../../closure-topology.md) of the union, but not in the union itself. Therefore

$$
\boxed{\bigcup_{n\geq1}C_n\text{ is not star-closed, although every }C_n\text{ is star-closed}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
