<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Prim's algorithm](../../../../../prim-s-algorithm.md) grows a tree from any root $r$. For each vertex outside the current tree, its [priority queue](../../../../../priority-queue.md) key is the cheapest single edge connecting it to the tree, not the total length of a root-to-vertex path:
```
for v in V:
    key[v] = infinity
    parent[v] = NONE
key[r] = 0
Q = indexed_min_priority_queue(V, key)
while Q is not empty:
    u = Q.extract_min()
    for (v,weight) in adjacency[u]:
        if Q.contains(v) and weight < key[v]:
            parent[v] = u
            key[v] = weight
            Q.decrease_key(v, weight)
return {(parent[v],v) : v != r}
```
The [indexed priority queue](../../../../../indexed-priority-queue.md) supports membership and locating a vertex's heap entry. After the first extraction, the chosen parent edge is a least-weight edge crossing the cut between the current tree and its complement. The [minimum spanning tree cut property](../../../../../minimum-spanning-tree-cut-property.md) makes that edge safe: exchanging it for a crossing edge of a suitable minimum tree preserves minimality. Repeating this establishes a minimum tree. Connectivity ensures every nonroot vertex eventually has a parent; edge weights may be negative.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
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
