<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take a [minimum spanning tree](../../../../../minimum-spanning-tree.md) $T$, for example one constructed by [Kruskal's algorithm](../../../../../kruskal-s-algorithm.md). Fix $v$ and let $e$ be a longest edge of the tree's unique $xv$ path. Deleting $e$ partitions $T$ into two components separating $x$ and $v$. Any alternative $xv$ path crosses this [graph cut](../../../../../graph-cut.md). If all of its edges were shorter than $e$, a crossing edge $f$ would let us replace $e$ by $f$, producing a [spanning tree](../../../../../spanning-tree.md) of smaller total length. This contradicts minimality of $T$.

Therefore every competing path has an edge at least as long as $e$, and the tree path solves the [bottleneck shortest path problem](../../../../../bottleneck-shortest-path-problem.md). The same [minimum spanning tree](../../../../../minimum-spanning-tree.md) works simultaneously for every $v$; this is the [minimax path property of a minimum spanning tree](../../../../../minimax-path-property-of-a-minimum-spanning-tree.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
