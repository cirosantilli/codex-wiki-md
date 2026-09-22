<h1 id="7/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**False for directed distance.** Take four [vertices](../../../../../../vertex-graph-theory.md) $a,b,c,d$. Put both directed [edges](../../../../../../edge-of-a-graph.md) between every distinct pair in $\{a,b,c\}$, and add $d\to a$ and $d\to b$. Every [vertex](../../../../../../vertex-graph-theory.md) has [out-degree](../../../../../../outdegree.md) two, satisfying $|V|/2$, and there are no [self-loops](../../../../../../loop-graph-theory.md). Nevertheless no [directed path](../../../../../../directed-path.md) leads from any of $a,b,c$ to $d$, so the claimed finite upper bound on [graph distance](../../../../../../distance-graph-theory.md) fails.

If “connected” means weakly connected, that portion does follow: a weak component of size $m$ gives each of its vertices [out-degree](../../../../../../outdegree.md) at most $m-1$, so each component would have size at least $|V|/2+1$, making two components impossible. It does not imply a [strongly connected directed graph](../../../../../../strong-connectivity.md). Thus either the strong-connectivity interpretation fails outright or the weak interpretation leaves the distance assertion false; the complete claim is false in either case.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
