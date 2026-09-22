<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The only possibilities are $f[2]\in\{10,11\}$.** Vertex $2$ reaches all of $1,3,5,6$. In [depth-first search](../../../../../../depth-first-search.md), all vertices reachable from an active vertex must have been discovered and finished before its own finishing event, except for active ancestors. None of these four can be an ancestor of $2$, because none can reach $2$. Thus all four are finished before $2$ finishes.

Vertex $4$ cannot already be finished at that point: its outgoing edge to $2$ would have caused $2$ to be visited before it could finish. It also cannot be a descendant of $2$, since $2$ cannot reach $4$. Therefore $4$ is either still undiscovered or an active ancestor. In the first case the only remaining events are discovery and finishing of $4$, giving $f[2]=10$. In the second case the only remaining event is finishing of $4$, giving $f[2]=11$.

Both occur. Starting the outer traversal with $2$ leaves $4$ undiscovered and gives time $10$. Starting with $4$ and taking its edge to $2$ first makes $4$ an ancestor and gives time $11$. The argument does not assume any particular order on the other edges.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
