<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Initialize $d[s]=0$ and every other tentative distance to infinity. The [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) repeatedly relaxes every directed edge:

```
for v in V: d[v] = infinity; parent[v] = none
d[s] = 0
repeat |V|-1 times:
    changed = false
    for each edge (u,v) of weight w:
        if d[u] != infinity and d[u] + w < d[v]:
            d[v] = d[u] + w
            parent[v] = u
            changed = true
    if not changed: break
for each edge (u,v) of weight w:
    if d[u] != infinity and d[u] + w < d[v]:
        report a reachable negative-weight cycle
```

An unreachable vertex retains infinity. A reachable negative-weight cycle prevents finite shortest-walk distances for vertices reachable from that cycle, so the detection case must not be reported as an ordinary finite answer. With edge-list scans the worst-case work is **$O(|V||E|+|V|)$**, conventionally stated as $O(|V||E|)$, and the auxiliary storage is $O(|V|)$ beyond the graph.

## ↑ Ancestors (12)

1. [A](../a.md)
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
