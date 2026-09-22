<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**False.** Use only the directed [edge](../../../../../../edge-of-a-graph.md) $u\to v$, but choose $v$ first in the outer loop of [depth-first search](../../../../../../depth-first-search.md). It finishes before a second discovery tree starts at $u$: $d[v]=1$, $f[v]=2$, $d[u]=3$, $f[u]=4$. The edge supplies the required [directed path](../../../../../../directed-path.md) and $f[u]>f[v]$, yet $d[u]>d[v]$. A path to an already black [vertex](../../../../../../vertex-graph-theory.md) need not put the two [vertices](../../../../../../vertex-graph-theory.md) into one discovery [tree](../../../../../../tree-graph-theory-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
