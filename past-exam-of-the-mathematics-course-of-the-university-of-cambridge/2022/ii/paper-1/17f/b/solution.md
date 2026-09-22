<h1 id="17f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A graph is $k$-connected when it has more than $k$ vertices and remains connected after deletion of fewer than $k$ vertices. In a noncomplete 3-connected graph, choose a vertex $v$ with two nonadjacent neighbors $a,b$. Since $G-\{a,b\}$ is connected, take a spanning tree rooted at $v$ and order its vertices so every vertex other than $v$ has a later tree neighbor. Color $a$ and $b$ first with the same color, then greedily color the other vertices in reverse tree order, leaving $v$ last. Every nonfinal vertex has one uncolored neighbor and therefore sees at most $\Delta-1$ colors. At $v$, the two neighbors $a,b$ share a color, so again at most $\Delta-1$ colors occur. Hence

$$
\boxed{\chi(G)\leq\Delta(G)}.
$$

This is the relevant 3-connected case of [Brooks' theorem](../../../../../../brooks-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17F](../../17f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
