<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Partition the vertex set into disjoint sets $A$ and $B$ of sizes $\lfloor n/2\rfloor$ and $\lceil n/2\rceil$. The [induced subgraph](../../../../../../induced-subgraph.md) on $A$ has distribution

$$
G(\lfloor n/2\rfloor,p).
$$

For $p=n^{-0.9}$,

$$
p|A|\sim\frac12n^{0.1}\longrightarrow\infty,
$$

so part (b) shows that $A$ contains a triangle with probability tending to one.

On that event, choose a triangle using only the edges internal to $A$. The edges from its three vertices to $B$ remain independent of this choice. The probability that all $3|B|$ such edges are absent is

$$
(1-p)^{3|B|}
\leq e^{-3p|B|}
\longrightarrow0,
$$

because $p|B|\sim n^{0.1}/2$. Thus, with probability tending to one, some vertex of $B$ is adjacent to a vertex of the triangle. Those four vertices and the four required edges form the given graph $H$, a [triangle with an attached leaf in a binomial random graph](../../../../../../triangle-with-an-attached-leaf-in-a-binomial-random-graph.md). Therefore

$$
\boxed{\mathbb P(F)\longrightarrow1}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
