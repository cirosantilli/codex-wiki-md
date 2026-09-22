<h1 id="r/r2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $k=\chi(G)$. For $k\leq1$ the bound is immediate. Otherwise choose a [vertex](../../../../../vertex-graph-theory.md)-minimal subgraph $H$ with [chromatic number](../../../../../chromatic-number.md) $k$. Each [vertex](../../../../../vertex-graph-theory.md) has degree at least $k-1$ in $H$: if one had degree at most $k-2$, a $(k-1)$-colouring of the smaller [graph](../../../../../graph-split.md) obtained by deleting it could be extended to it using an absent neighbour colour, contradicting $\chi(H)=k$.

The [graph](../../../../../graph-split.md) $H$ has at least $k$ vertices. By the degree-sum identity,

$$
2m\geq2|E(H)|=\sum_{v\in H}\deg_Hv\geq(k-1)|V(H)|\geq k(k-1).
$$

Solving the quadratic inequality gives

$$
\boxed{\chi(G)=k\leq\frac12+\sqrt{2m+\frac14}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [R2](../../r2.md)
3. [R](../../../r.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
