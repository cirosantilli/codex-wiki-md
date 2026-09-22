<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [minimum spanning tree cut property](../../../../../../minimum-spanning-tree-cut-property.md), in its safe-edge form, says: if an edge set $A$ is contained in some [minimum spanning tree](../../../../../../minimum-spanning-tree.md), a [cut of a graph](../../../../../../cut-graph-theory.md) respects $A$, and $e$ is a [light edge crossing a cut](../../../../../../light-edge-crossing-a-cut.md), then $A\cup\{e\}$ is contained in some [minimum spanning tree](../../../../../../minimum-spanning-tree.md).

Choose an [MST](../../../../../../minimum-spanning-tree.md) $T$ containing $A$. If $e\in T$, nothing changes. Otherwise adding $e$ creates its unique [fundamental cycle](../../../../../../fundamental-cycle.md). The path in $T$ between the endpoints of $e$ must cross the chosen cut; take such an edge $f$. Since the cut respects $A$, $f\notin A$. Since $e$ is light, $w(e)\leq w(f)$. The exchange $T-f+e$ is a [spanning tree](../../../../../../spanning-tree.md) containing $A\cup\{e\}$, with total weight no greater than that of $T$. Minimality of $T$ forces equal optimum weight, proving the claim. Equal edge weights cause no difficulty: “safe” means belonging to some compatible optimum, not to every optimum.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
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
