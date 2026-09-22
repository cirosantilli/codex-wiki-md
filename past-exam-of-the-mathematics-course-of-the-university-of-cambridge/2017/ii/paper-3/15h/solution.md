<h1 id="15h/solution">Solution</h1>

↑ **Parent:** [15H](../15h.md)

A [graph Ramsey number](../../../../../graph-ramsey-number.md) $R(s,t)$ is the least $N$ such that every red-blue edge colouring of the [complete graph](../../../../../complete-graph.md) $K_N$ has a red $K_s$ or a blue $K_t$. At a vertex in $K_{R(s-1,t)+R(s,t-1)}$, either at least $R(s-1,t)$ neighbours have red incident edges or at least $R(s,t-1)$ have blue incident edges. In the first case find a red $K_{s-1}$ and adjoin the vertex, or a blue $K_t$; the second case is symmetric. Thus

$$
 R(s,t)\leq R(s-1,t)+R(s,t-1).
$$

Starting with $R(2,t)=t$ and $R(s,2)=s$, induction gives the [binomial upper bound for a Ramsey number](../../../../../binomial-upper-bound-for-a-ramsey-number.md)

$$
\boxed{R(s,t)\leq\binom{s+t-2}{s-1},\qquad R(s,s)\leq\binom{2s-2}{s-1}\leq4^{s-1}<4^s.}
$$

For the lower construction, partition $2t-2$ vertices into two classes of size $t-1$, colour inside-class edges red and between-class edges blue. Red [cliques](../../../../../clique-graph-theory.md) have at most $t-1$ vertices, and the blue [graph](../../../../../graph-split.md) is [bipartite](../../../../../bipartite-graph.md), so has no [odd cycle](../../../../../odd-cycle.md).

Conversely, a [graph](../../../../../graph-split.md) without an [odd cycle](../../../../../odd-cycle.md) is [bipartite](../../../../../bipartite-graph.md): in each connected component colour vertices by the parity of the length of a path from a root; differing path parities would give an odd closed walk, hence an [odd cycle](../../../../../odd-cycle.md). On $2t-1$ vertices one of the two blue bipartition classes has at least $t$ vertices. Every edge within it is red, giving a red $K_t$. Thus **$2t-1$ is the exact threshold** for this alternative.

## ↑ Ancestors (10)

1. [15H](../15h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
