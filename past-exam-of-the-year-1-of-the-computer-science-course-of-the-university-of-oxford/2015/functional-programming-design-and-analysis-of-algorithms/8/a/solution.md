<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dijkstra's algorithm](../../../../../dijkstra-algorithm.md) solves the [single-source shortest-path problem](../../../../../single-source-shortest-path-problem.md) with nonnegative edge weights: it finds minimum path lengths from the source to all reachable vertices and can store predecessor edges. With [adjacency lists](../../../../../adjacency-list.md) and a binary-heap [priority queue](../../../../../priority-queue.md), it takes **$O((|V|+|E|)\log|V|)$ time**; a direct array implementation takes $O(|V|^2)$.

The [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) allows negative edge weights. If no negative-weight cycle is reachable from the source, it computes the finite shortest-path distances to reachable vertices and identifies unreachable ones. Otherwise it can report a reachable [negative cycle](../../../../../negative-cycle.md), whose repeated traversal makes distances to some reachable vertices unbounded below. It performs at most $|V|-1$ full relaxation rounds and one further detection round, taking **$O(|V||E|+|V|)$ time**, conventionally written $O(|V||E|)$ for nontrivial edge sets. A negative cycle unreachable from the source does not affect its distance problem.

## ↑ Ancestors (12)

1. [A](../a.md)
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
