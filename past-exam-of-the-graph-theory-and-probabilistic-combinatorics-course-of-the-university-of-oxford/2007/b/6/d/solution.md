<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Realize the random [graph](../../../../../graph-split.md) process by giving every edge an independent uniform arrival time. For a fixed four-set $S$, only its six internal edges and its $4(n-4)$ outgoing edges affect whether it is an isolated [clique](../../../../../clique-graph-theory.md). It is an isolated [clique](../../../../../clique-graph-theory.md) at some time exactly when all six internal edges arrive before every outgoing edge.

The relative ordering of these $4n-10$ edges is uniform. The chance that the first six are exactly the six internal edges is $\binom{4n-10}{6}^{-1}$. A [union bound](../../../../../boole-s-inequality.md) over the possible vertex sets gives

$$
\boxed{P(\text{an isolated four-clique ever appears})\le\frac{\binom n4}{\binom{4n-10}{6}}=O(n^{-2})\longrightarrow0}.
$$

Edges entirely outside $S$ are irrelevant. Counting the whole arrival-order event avoids an invalid union over continuously many times.

This is an example of [isolated clique appearance in a uniform random graph process](../../../../../isolated-clique-appearance-in-a-uniform-random-graph-process.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
