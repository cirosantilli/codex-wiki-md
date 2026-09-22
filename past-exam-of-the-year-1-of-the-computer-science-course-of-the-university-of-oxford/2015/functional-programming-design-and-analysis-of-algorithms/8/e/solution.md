<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Process outgoing edges in [topological order](../../../../../topological-order.md):
```
order = topological_sort(G)
for v in V:
    distance[v] = infinity
    predecessor[v] = none
distance[s] = 0

for u in order:
    if distance[u] != infinity:
        for edge (u,v) of weight w:
            if distance[u] + w < distance[v]:
                distance[v] = distance[u] + w
                predecessor[v] = u
```
For correctness, argue by induction through the [topological sort](../../../../../topological-sorting.md). Every path ending at a vertex $v\ne s$ reaches it through some incoming edge $uv$. All such predecessors $u$ occur earlier, so their finalized shortest-path distances have already been considered when $v$ is processed. Taking the minimum of $\operatorname{distance}(u)+w(u,v)$ over these edges therefore gives exactly the shortest-path distance to $v$. Unreachable vertices retain infinity. Negative edge weights cause no difficulty because a later vertex cannot lead back to an earlier one.

This is the [DAG shortest-path algorithm](../../../../../dag-shortest-path-algorithm.md). [Topological sorting](../../../../../topological-sorting.md) and the single pass of [edge relaxation](../../../../../edge-relaxation.md) each take **$O(|V|+|E|)$ time** with [adjacency lists](../../../../../adjacency-list.md); distances, predecessors and the order use $O(|V|)$ auxiliary space. Following predecessors reconstructs a shortest path to any reachable target.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
