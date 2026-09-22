<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [minimum-hop shortest paths](../../../../../minimum-hop-shortest-paths.md) by minimizing the [lexicographic order](../../../../../lexicographic-order.md) pair $(d,h)$: total weight first, number of edges second. Extend a pair across an edge of weight $w$ by adding $(w,1)$, and compare the full pair in both the [priority queue](../../../../../priority-queue.md) and relaxation:

```
for v in V: key[v] = (infinity,infinity)
key[s] = (0,0)
Q = indexed min-priority-queue containing all vertices, keyed by key
while Q is not empty:
    u = extract-min(Q)
    if key[u].distance == infinity: break
    for each edge (u,v) of weight w with v still in Q:
        candidate = (key[u].distance + w, key[u].hops + 1)
        if candidate <lex key[v]:
            key[v] = candidate
            decrease-key(Q,v,candidate)
for v in V: best[v] = key[v].hops
```

All weights are positive, so extending a path strictly increases its first component. The usual [Dijkstra's algorithm](../../../../../dijkstra-algorithm.md) settled-label proof therefore applies to these ordered pairs: no path through a not-yet-settled vertex can later improve an extracted minimum. Among equal minimum weights, the secondary component selects the fewest edges. Merely breaking extraction ties by vertex name would not implement this objective.

With a [binary heap](../../../../../binary-heap.md) and [adjacency lists](../../../../../adjacency-list.md), the bound is **$O((|V|+|E|)\log |V|)$**, with $O(|V|)$ extra storage. Unreachable vertices have `best = infinity`. In the paper's example, the resulting pairs in order $s,a,b,c,d,e,f$ are $(0,0),(2,1),(2,1),(4,1),(5,2),(5,2),(6,3)$, so the requested edge counts are **$0,1,1,1,2,2,3$**.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
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
