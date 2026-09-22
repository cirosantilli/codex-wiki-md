<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**[Depth-first tree search](../../../../../depth-first-tree-search.md) is complete under the stated initial [reachability](../../../../../reachability-in-a-graph.md) assumption, but is not bonus-optimal.**

Let $d_t$ be the [graph distance](../../../../../distance-graph-theory.md) between fox and rabbit after round $t$, with $d_0$ their initial [graph distance](../../../../../distance-graph-theory.md). Initial [reachability](../../../../../reachability-in-a-graph.md) makes $d_0$ finite, and ordinary moves preserve membership in their common [connected component of a graph](../../../../../component-graph-theory.md). After the rabbit's next move, the [triangle inequality](../../../../../triangle-inequality.md) gives intermediate separation at most $d_t+1$. If that separation is at most two, the fox catches the rabbit that round. Otherwise the fox takes two steps along a [shortest path](../../../../../shortest-path.md), leaving

$$
1\le d_{t+1}\le d_t-1.
$$

Thus a successful surviving history has at most $d_0-1$ rounds; if it does not escape by then, the next round captures it. The [shortest-path pursuit distance bound](../../../../../shortest-path-pursuit-distance-bound.md) excludes infinite live branches, even when the rabbit stays. Together with the finite [branching factor](../../../../../branching-factor.md), it makes the whole relevant [search tree](../../../../../search-tree.md) finite, so [depth-first tree search](../../../../../depth-first-tree-search.md) eventually finds an escape whenever one exists.

For nonoptimality, take the corridor of part (g) and let [depth-first tree search](../../../../../depth-first-tree-search.md) try left first. It immediately returns the one-round escape with bonus $1$, whereas trying right twice earns $2$. The decreasing separation proves termination, **not optimality of the first returned escape**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
