<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a connected, weighted, undirected graph, grow a tree from any root $r$. For every vertex outside the tree, store the cheapest edge currently connecting it to the tree, not its source-path distance:

```
for v in V: key[v] = infinity; parent[v] = none
key[r] = 0
Q = indexed min-priority-queue containing all vertices
while Q is not empty:
    u = extract-min(Q)
    if parent[u] != none: output edge (parent[u],u)
    for each edge {u,v} of weight w with v still in Q:
        if w < key[v]:
            key[v] = w
            parent[v] = u
            decrease-key(Q,v,w)
```

The maintained key chooses the minimum-weight edge crossing the cut between the tree and remaining vertices. The [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md) makes that edge safe; induction therefore preserves the existence of a minimum spanning tree containing all selected edges. This proves why [Prim's algorithm](../../../../../prim-s-algorithm.md) is greedy and correct. With adjacency lists and a binary heap its time is $O((|V|+|E|)\log |V|)$. For a disconnected graph, starting another component when the minimum key is infinity produces a [minimum spanning forest](../../../../../minimum-spanning-forest.md) instead of claiming that a spanning tree exists.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
