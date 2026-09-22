<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Kruskal's algorithm](../../../../../kruskal-s-algorithm.md) sorts the edges and accepts an edge precisely when it joins two currently different [connected components of a graph](../../../../../component-graph-theory.md). A [disjoint-set data structure](../../../../../disjoint-set-data-structure.md) maintains those components:

```
Kruskal(V, E, w):
    A = empty set
    make one disjoint set for each vertex in V
    for (u,v) in E sorted by nondecreasing w:
        if find(u) != find(v):
            add (u,v) to A
            union(u,v)
            if size(A) == size(V) - 1:
                break
    return A
```

An accepted edge merges two trees of the current [forest](../../../../../forest.md). An edge within one component would complete a [graph cycle](../../../../../cycle-in-a-graph.md) and is skipped. On connected input, after $|V|-1$ acceptances the forest is a spanning tree. For a one-vertex graph the empty set is already the answer.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
