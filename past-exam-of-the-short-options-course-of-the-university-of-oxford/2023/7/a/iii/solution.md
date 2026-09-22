<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [Dijkstra's algorithm](../../../../../dijkstra-algorithm.md), initialize $d(x)=0$ and $d(v)=\infty$ for other [vertices](../../../../../vertex-graph-theory.md), with no predecessor initially. Repeatedly select an unfinalized vertex $u$ of least tentative distance, finalize it, and relax each [edge](../../../../../edge-of-a-graph.md) $uv$: if $d(u)+\ell(uv)<d(v)$, replace $d(v)$ by that value and set the predecessor of $v$ to $u$. Continue until all vertices are finalized. The predecessor edges form the [shortest-path tree](../../../../../shortest-path-tree.md).

To justify finalization, consider a supposedly shorter route to the next selected vertex. Its first unfinalized vertex is preceded by a finalized one, whose relaxation would already have offered a tentative distance no greater than the length of that route's prefix. Nonnegative remaining lengths would contradict the selected vertex's minimal tentative label. Thus final labels are the true shortest distances. Strictly positive lengths also make predecessors have smaller distances, ruling out predecessor [cycles in a graph](../../../../../cycle-in-a-graph.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
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
