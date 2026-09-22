<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Augment [depth-first search](../../../../../depth-first-search.md) with a two-valued colour:
```
paint(v, c):
    colour[v] = c
    for w in adjacency[v]:
        if colour[w] is unset:
            if not paint(w, 1-c):
                return false
        else if colour[w] == c:
            return false
    return true

for v in V:
    if colour[v] is unset:
        if not paint(v, 0):
            return false
return true
```
Each tree edge receives opposite endpoint colours. If an inspected edge has equal colours, the preceding parity argument produces an [odd cycle](../../../../../odd-cycle.md), so the graph is not [bipartite](../../../../../bipartite-graph-split.md). If the procedure succeeds, every edge has differently coloured endpoints, and the two colour classes are a [bipartition](../../../../../bipartition-of-a-graph.md). The outer loop handles disconnected graphs and isolated vertices.

Each vertex is coloured once and each edge incidence is checked once, giving **$O(|V|+|E|)$ time** and $O(|V|)$ extra space with [adjacency lists](../../../../../adjacency-list.md). No separate cycle enumeration is required.

## ↑ Ancestors (12)

1. [C](../c.md)
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
