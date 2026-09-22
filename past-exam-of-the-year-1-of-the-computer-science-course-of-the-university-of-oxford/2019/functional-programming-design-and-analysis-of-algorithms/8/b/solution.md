<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

All [edge](../../../../../edge-of-a-graph.md) lengths are positive, so run the [Dijkstra algorithm](../../../../../dijkstra-algorithm.md) from every source $s$, retaining distances $d_s$ and a [shortest-path tree](../../../../../shortest-path-tree.md) of its reachable component. Each run takes $O((|V|+|E|)\log(|V|+1))$ with a [binary heap](../../../../../binary-heap.md). The following scans after each run use only $O(|E|)$ additional work.

For a [directed graph](../../../../../directed-graph.md), inspect every closing [edge](../../../../../edge-of-a-graph.md) $(u,s)$ and consider $d_s(u)+w(u,s)$ when $u$ is reachable. The [tree](../../../../../tree-graph-theory-split.md) route from $s$ to $u$ followed by this [edge](../../../../../edge-of-a-graph.md) is a closed walk. Every directed cycle supplies one such upper bound by choosing any of its [vertices](../../../../../vertex-graph-theory.md) as $s$; the shortest route to its predecessor is no longer than the corresponding cycle segment. Positivity lets any repeated portion be removed, so the smallest candidate is **the shortest directed-cycle length**.

For an [undirected graph](../../../../../undirected-graph.md), do _not_ combine an [edge](../../../../../edge-of-a-graph.md) with the distance between its endpoints indiscriminately: that can count traversal of one bridge out and back as a false cycle. Instead inspect only [edges](../../../../../edge-of-a-graph.md) $\{u,v\}$ absent from the current [shortest-path tree](../../../../../shortest-path-tree.md), with both endpoints reachable, and consider

$$
d_s(u)+w(u,v)+d_s(v).
$$

The two [tree](../../../../../tree-graph-theory-split.md) routes and this non-tree [edge](../../../../../edge-of-a-graph.md) contain a genuine cycle. If they share a prefix, its cost is counted twice, so that cycle is no longer than the candidate. Every candidate is consequently at least the global shortest-cycle length.

To prove equality is attained, take a shortest cycle $C$ and a source $s$ on it. If either cycle [edge](../../../../../edge-of-a-graph.md) incident to $s$ is absent from the [tree](../../../../../tree-graph-theory-split.md), its candidate uses a shortest route no longer than the rest of $C$, so it is at most the length of $C$. Otherwise both incident [edges](../../../../../edge-of-a-graph.md) are in the [tree](../../../../../tree-graph-theory-split.md), and their other endpoints lie in different branches below $s$. Along the remaining segment of $C$, some [edge](../../../../../edge-of-a-graph.md) crosses between different branches. Such an [edge](../../../../../edge-of-a-graph.md) is not a [tree](../../../../../tree-graph-theory-split.md) [edge](../../../../../edge-of-a-graph.md). The two distances to its endpoints are bounded by the two corresponding, disjoint segments of $C$ from $s$; their sum plus the crossing [edge](../../../../../edge-of-a-graph.md) is at most the length of $C$. Thus some candidate is no greater than the optimum, completing the proof.

Return the smallest finite candidate, or report acyclicity if none exists. The total [running time](../../../../../running-time.md) is **$O((|V|^2+|V||E|)\log(|V|+1))$**, as required. The ordinary convention is a simple [graph](../../../../../graph-split.md); if parallel [edges](../../../../../edge-of-a-graph.md) are allowed, track actual [edge](../../../../../edge-of-a-graph.md) identities when excluding [tree](../../../../../tree-graph-theory-split.md) [edges](../../../../../edge-of-a-graph.md), and treat a self-loop as its own cycle rather than discarding it. This is [shortest cycle by repeated shortest-path trees](../../../../../shortest-cycle-by-repeated-shortest-path-trees.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
