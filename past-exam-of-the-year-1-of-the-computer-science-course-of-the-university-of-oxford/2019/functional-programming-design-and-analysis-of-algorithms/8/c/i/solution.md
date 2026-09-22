<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Find a [topological sorting](../../../../../../topological-sorting.md) of the [Directed acyclic graph](../../../../../../directed-acyclic-graph.md). Initialize $L[s]=0$ and $L[v]=-\infty$ for $v\ne s$. Process [vertices](../../../../../../vertex-graph-theory.md) in that order. At a reachable [vertex](../../../../../../vertex-graph-theory.md) $u$, update each outgoing [edge](../../../../../../edge-of-a-graph.md) by $L[v]\gets\max\{L[v],L[u]+w(u,v)\}$, and retain a predecessor whenever an improvement is made.

Every path to a [vertex](../../../../../../vertex-graph-theory.md) ends at an earlier [vertex](../../../../../../vertex-graph-theory.md) in the [topological sorting](../../../../../../topological-sorting.md). Thus, when $v$ is processed, all possible final-edge candidates for $v$ have already been considered. [Induction](../../../../../../mathematical-induction.md) along the order proves that **$L[v]$ is the [longest path](../../../../../../longest-path.md) length from $s$**, with $-\infty$ exactly for unreachable [vertices](../../../../../../vertex-graph-theory.md). Signed weights cause no problem because the [graph](../../../../../../graph-split.md) has no directed cycle. The [running time](../../../../../../running-time.md) is **$O(|V|+|E|)$**, and predecessor pointers recover a maximizing path.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
