<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Erdős-Stone theorem](../../../../../../erdos-stone-theorem.md) states precisely that, for every fixed graph $H$ with [chromatic number](../../../../../../chromatic-number.md) $\chi(H)\geq2$,

$$
\lim_{n\to\infty}
\frac{\operatorname{ex}(n,H)}{\binom n2}
=1-\frac1{\chi(H)-1}.
$$

If the bipartite graph $G$ has an edge, then $\chi(G)=2$. Substitution into the theorem gives

$$
\boxed{
\frac{\operatorname{ex}(n,G)}{\binom n2}\longrightarrow
1-\frac1{2-1}=0.}
$$

If $G$ has no edges, then every graph of sufficiently large order contains $G$ as a [subgraph](../../../../../../subgraph.md), so the conclusion is immediate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
