<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**No: equal-length shortest paths permit different trees.** Consider edges $s\to a,s\to b,a\to t,b\to t$, all of weight one. Both routes to $t$ have length two. A [shortest-path tree](../../../../../shortest-path-tree.md) may therefore choose either $a$ or $b$ as the predecessor of $t$.

The processing order and tie-breaking rules of [Dijkstra's algorithm](../../../../../dijkstra-algorithm.md) and the [Bellman-Ford algorithm](../../../../../bellman-ford-algorithm.md) need not agree, so either tree can result while all [shortest-path distances](../../../../../shortest-path-distance.md) agree. If every reachable vertex has a unique shortest path from $s$, then both correct algorithms must select those same paths.

## ↑ Ancestors (12)

1. [B](../b.md)
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
