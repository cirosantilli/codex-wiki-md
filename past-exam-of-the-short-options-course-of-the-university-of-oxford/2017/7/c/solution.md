<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the usual [walk](../../../../walk-in-a-graph.md) convention allowing repeated edges, **the stated hypothesis is insufficient**. Take the connected graph consisting of one zero-weight edge $xy$. It has no simple cycles, so the cycle condition holds. Nevertheless $Q=x,y,x,y$ is a minimum-weight $xy$-walk of weight zero and is not a path.

If the course uses “walk” to mean an edge-nonrepeating [trail](../../../../trail-in-a-graph.md), the intended argument is valid. If such a minimum trail repeats a vertex, take its first repeated-vertex segment. Its interior vertices are distinct and no edge repeats, so this segment is a simple cycle $C$. Removing it leaves an $xy$-trail of weight $w(Q)-w(C)<w(Q)$, a contradiction. Hence $Q$ is a path. Since every $xy$-path is a competing trail, it is a shortest path.

For unrestricted walks, the same proof works if every nontrivial closed subwalk has positive weight, in particular if every edge has positive weight. This is [cycle erasure in minimum-weight walks](../../../../cycle-erasure-in-minimum-weight-walks.md). The exact 2017 course convention was not available to check; the counterexample and the trail interpretation distinguish the two meanings explicitly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
