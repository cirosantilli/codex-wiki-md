<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Build a [maximum spanning tree](../../../../../maximum-spanning-tree.md) $T$ by the decreasing-weight version of [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md). For the specified distinct endpoints $s,t$, find their unique [graph path](../../../../../path-in-a-graph.md) $P_T$ in $T$ by [depth-first search](../../../../../depth-first-search.md), retaining predecessors to reconstruct it. Return that path and its minimum [edge weight](../../../../../edge-weight.md) $b$.

For correctness, choose an [edge](../../../../../edge-of-a-graph.md) $e$ of weight $b$ on $P_T$. Deleting it splits $T$ into two [connected components](../../../../../connected-component.md), separating $s$ from $t$. No [edge](../../../../../edge-of-a-graph.md) $f$ across this [cut of a graph](../../../../../cut-graph-theory.md) can have $w(f)>b$: replacing $e$ by $f$ would give a [spanning tree](../../../../../spanning-tree.md) of greater total weight, contradicting maximality of $T$.

Every $s$–$t$ [graph path](../../../../../path-in-a-graph.md) $P$ must cross the same [cut of a graph](../../../../../cut-graph-theory.md), so it contains a crossing [edge](../../../../../edge-of-a-graph.md) $f$ with $w(f)\le b$. Therefore its minimum [edge weight](../../../../../edge-weight.md) is at most $b$. The tree route attains $b$, proving

$$
\boxed{\min_{e\in P_T}w(e)=\max_{P:s\leadsto t}\min_{e\in P}w(e).}
$$

This is precisely the [widest path problem](../../../../../widest-path-problem.md). The proof allows tied, zero and negative [edge weights](../../../../../edge-weight.md). It depends on maximizing the total tree weight, not on a shortest-distance [algorithm](../../../../../algorithm-split.md).

Let $v=|V|$ and $e=|E|$. Sorting and [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) take $O(e\log e+v)$ time; the tree search adds $O(v)$. Hence

$$
\boxed{\text{time }O(e\log e+v),\qquad\text{auxiliary space }O(e+v).}
$$

For a connected simple graph with at least two [vertices](../../../../../vertex-graph-theory.md), $v-1\le e\le v(v-1)/2$, so the time is also $O(e\log v)$. The $O(e\log e+v)$ expression remains valid when parallel [edges](../../../../../edge-of-a-graph.md) are permitted. If the two endpoints coincide, the empty path is returned, with bottleneck $+\infty$ under the usual empty-minimum convention; otherwise connectedness guarantees a nonempty route.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
