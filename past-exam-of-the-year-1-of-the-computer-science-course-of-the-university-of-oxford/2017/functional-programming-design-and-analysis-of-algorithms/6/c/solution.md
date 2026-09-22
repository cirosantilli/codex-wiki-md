<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the [vertex set](../../../../../vertex-set.md) is finite, at least one vertex occurs infinitely often, so $\operatorname{Inf}(\rho)$ is nonempty. Let $u,v$ belong to this set. After any chosen visit to $u$, a later visit to $v$ exists; the intervening edges give a directed walk from $u$ to $v$. After that visit to $v$, a later visit to $u$ also exists, giving a walk in the other direction. Removing repeated portions gives [directed paths](../../../../../directed-path.md) if desired.

Thus every pair in $\operatorname{Inf}(\rho)$ is mutually reachable and belongs to the same [strongly connected component](../../../../../strongly-connected-component.md). This proves the claimed inclusion, which need not be equality: an infinite walk can repeatedly follow one cycle while omitting other vertices in its component. This is the recurrence-set part of the [infinite walk criterion in a finite directed graph](../../../../../infinite-walk-criterion-in-a-finite-directed-graph.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
