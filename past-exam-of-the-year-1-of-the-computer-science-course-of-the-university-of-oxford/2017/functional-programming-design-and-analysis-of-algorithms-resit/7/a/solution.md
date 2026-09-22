<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maintain white, gray and black colors for undiscovered, active and completed vertices. A single traversal clock records [DFS discovery and finishing times](../../../../../dfs-discovery-and-finishing-times.md):

```
for v in V: color[v] = white; parent[v] = none
time = 0
visit(u):
    time = time+1; d[u] = time; color[u] = gray
    for v in adjacency[u]:
        if color[v] == white:
            parent[v] = u
            visit(v)
    color[u] = black; time = time+1; f[u] = time
for u in V:
    if color[u] == white: visit(u)
```

The outer loop makes a [depth-first search](../../../../../depth-first-search.md) forest even when the directed graph is disconnected. Each vertex is entered once and each directed adjacency entry is inspected once. Thus an [adjacency list](../../../../../adjacency-list.md) representation gives **$O(|V|+|E|)$ time** and $O(|V|)$ auxiliary storage, including the worst-case recursive stack. Sorting neighbors to impose a particular visit order would be additional work.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
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
