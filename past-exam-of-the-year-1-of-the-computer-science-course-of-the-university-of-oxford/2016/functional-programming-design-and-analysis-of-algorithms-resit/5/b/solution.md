<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Start a [depth-first search](../../../../../depth-first-search.md) from each as-yet unlabelled [vertex](../../../../../vertex-graph-theory.md), propagating a fresh component number:
```
component = 0
for u in V:
    cc[u] = UNLABELLED
for u in V:
    if cc[u] == UNLABELLED:
        visit(u, component)
        component = component + 1

visit(u, label):
    cc[u] = label
    for v in adjacency[u]:
        if cc[v] == UNLABELLED:
            visit(v, label)
```
A search follows only [edges](../../../../../edge-of-a-graph.md), so every vertex it labels is reachable from its root. Conversely, if a reachable vertex remained unlabelled, a path to it would contain a first edge from a visited vertex to an unvisited one; scanning that edge would visit the latter, a contradiction. Thus each search labels exactly one [connected component](../../../../../connected-component.md), proving both directions of the required equivalence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
