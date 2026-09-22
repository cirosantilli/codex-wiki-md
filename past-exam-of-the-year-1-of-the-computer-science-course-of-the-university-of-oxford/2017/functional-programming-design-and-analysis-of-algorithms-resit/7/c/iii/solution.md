<h1 id="7/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**True for a directed cycle.** Suppose there were no back edges. On examining an edge $u\to v$, its target would either be white, in which case its recursive call finishes before $u$; or black, in which case it has already finished. A gray target would be an active ancestor and hence give a back edge, contrary to the supposition. Therefore every edge would satisfy $f(v)<f(u)$.

Applying those strict inequalities around a directed cycle would imply $f(u)<f(u)$, a contradiction. Thus some [back edge in depth-first search](../../../../../../back-edge-in-depth-first-search.md) must exist in the search's edge classification. Such an edge is classified relative to the DFS forest; it is not one of the forest's tree edges.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Functional programming, design and analysis of algorithms (resit)](../../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
