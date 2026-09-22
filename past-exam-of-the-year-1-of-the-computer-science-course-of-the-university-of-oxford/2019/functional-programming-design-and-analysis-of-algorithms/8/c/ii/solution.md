<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Permit every [vertex](../../../../../../vertex-graph-theory.md) to start a path: initialize $L[v]=0$ for all $v$, then perform the same maximum-relaxation pass in [topological sorting](../../../../../../topological-sorting.md) order. Equivalently, the recurrence is

$$
L[v]=\max\left(0,\ \max_{(u,v)\in E}\{L[u]+w(u,v)\}\right).
$$

The zero option starts a fresh, zero-edge path; the other options extend an optimal path ending at a predecessor. The largest final entry is therefore **the longest path length in the [graph](../../../../../../graph-split.md)**, allowing a zero-edge path. This takes $O(|V|+|E|)$, which is **$O(|V|^2)$** for the ordinary simple-graph representation.

If at least one [edge](../../../../../../edge-of-a-graph.md) is required, keep the same prefix values but return $\max_{(u,v)\in E}(L[u]+w(u,v))$ instead of $\max_vL[v]$. That variant correctly returns a negative optimum when all nonempty paths have negative weight, and reports no nonempty path if the [edge](../../../../../../edge-of-a-graph.md) set is empty. No all-pairs repetition is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
