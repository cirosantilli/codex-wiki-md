<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here a directed cycle has at least one edge. If zero-length paths were treated as cycles, an edgeless one-vertex [graph](../../../../../../graph-split.md) would already satisfy the predicate; that convention would give the trivial nonempty-graph predicate instead of the intended [directed cycle detection](../../../../../../directed-cycle-detection.md) problem.

For [NL](../../../../../../nl-complexity.md) membership, guess a starting vertex $v$, follow a guessed directed walk for between one and $N=|V|$ edges, and accept if it returns to $v$. Store only the start, current vertex and step counter. A [graph](../../../../../../graph-split.md) with a nonempty closed walk contains a simple directed cycle of at most $N$ edges, including a self-loop if present. Thus the algorithm uses [logarithmic space](../../../../../../logarithmic-space.md) and is complete for the predicate.

For hardness, reduce the [directed graph reachability problem](../../../../../../st-connectivity.md) to cycle detection. Form $G^{(N+1)}$ and add the single backward arc

$$
(t,N+1)\longrightarrow(s,1).
$$

All layering arcs advance exactly one layer, including the waiting arcs $(v,i)\to(v,i+1)$, so the layered [graph](../../../../../../graph-split.md) alone is a [Directed acyclic graph](../../../../../../directed-acyclic-graph.md). Any cycle in the augmented [graph](../../../../../../graph-split.md) must contain the backward arc and therefore contains a path from $(s,1)$ to $(t,N+1)$.

If $t$ is reachable from $s$ in $G$, use a simple path of length at most $N-1$ and pad it with waits to exactly $N$ steps. It becomes the required layered path and closes to a cycle. Conversely, projecting such a layered path and deleting waits gives a walk from $s$ to $t$ in $G$. This includes the case $s=t$, where reachability has a zero-length witness but the augmented [graph](../../../../../../graph-split.md) has a genuinely positive-length cycle.

There are $N(N+1)$ vertices and polynomially many arcs. A transducer enumerates pairs/layers and checks old adjacency by scanning its input, using only $O(\log N)$ bits. Hence this is a [logspace many-one reduction](../../../../../../logspace-many-one-reduction.md), proving

$$
\boxed{\mathrm{CYCLE}\text{ is NL-complete}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
