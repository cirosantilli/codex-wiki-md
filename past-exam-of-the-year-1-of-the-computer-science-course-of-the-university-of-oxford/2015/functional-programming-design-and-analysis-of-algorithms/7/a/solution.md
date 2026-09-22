<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Depth-first search](../../../../../depth-first-search.md) marks a vertex when first reached, then recursively explores each still-unvisited neighbour before returning. To cover the whole graph, restart from every vertex not reached by earlier searches:
```
visit(v):
    visited[v] = true
    for w in adjacency[v]:
        if not visited[w]:
            visit(w)

for v in V:
    if not visited[v]:
        visit(v)
```
For a [directed graph](../../../../../directed-graph.md), use outgoing neighbours; for an [undirected graph](../../../../../undirected-graph.md), use both incidences of each edge. Each vertex is discovered once and each stored incidence is inspected once. Thus with [adjacency lists](../../../../../adjacency-list.md) the [running time](../../../../../running-time.md) is **$O(|V|+|E|)$** and the visited information and recursion stack use $O(|V|)$ space. An [adjacency matrix](../../../../../adjacency-matrix.md) representation instead requires scanning $|V|$ possible neighbours per visited vertex, giving $O(|V|^2)$ time.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
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
