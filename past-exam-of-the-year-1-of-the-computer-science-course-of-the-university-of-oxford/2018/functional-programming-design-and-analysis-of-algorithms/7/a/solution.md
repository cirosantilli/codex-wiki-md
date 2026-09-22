<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In [depth-first search](../../../../../depth-first-search.md), mark every [vertex](../../../../../vertex-graph-theory.md) white initially. At a white start vertex $u$, increment a global clock, record $d[u]$ and color it gray. Scan its outgoing [adjacency list](../../../../../adjacency-list.md); recursively visit each still-white neighbor, recording the discovery [edge](../../../../../edge-of-a-graph.md). After all neighbors have been processed, color $u$ black, increment the clock and record $f[u]$. Start again from every remaining white [vertex](../../../../../vertex-graph-theory.md) to obtain a [forest](../../../../../forest.md). Each [vertex](../../../../../vertex-graph-theory.md) is discovered once and each [edge](../../../../../edge-of-a-graph.md) scanned once, so the time is $O(|V|+|E|)$ with [adjacency lists](../../../../../adjacency-list.md).

The [DFS parenthesis property](../../../../../depth-first-search-parenthesis-property.md) says that for distinct [vertices](../../../../../vertex-graph-theory.md) $u,v$, their intervals $[d[u],f[u]]$ and $[d[v],f[v]]$ are disjoint or one lies strictly inside the other. Moreover $v$ is a proper [descendant in a rooted tree](../../../../../descendant-in-a-rooted-tree.md) of $u$ exactly when $d[u]<d[v]<f[v]<f[u]$. A recursive call finishes before its caller returns, while completed calls from separate branches have disjoint intervals; these two possibilities prove the property.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
