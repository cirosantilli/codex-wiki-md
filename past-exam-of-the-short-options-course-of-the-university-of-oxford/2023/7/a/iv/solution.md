<h1 id="7/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Starting from $3$, the initial tentative distances to $0,1,2,4$ are $5,7,9,13$. Finalize $0$ next. Its edges improve these to $d(1)=5+1=6$, $d(2)=5+3=8$, and $d(4)=5+7=12$. No subsequent relaxation improves them. Hence one [shortest-path tree](../../../../../shortest-path-tree.md) is

$$
\boxed{E(T)=\{\{3,0\},\{0,1\},\{0,2\},\{0,4\}\}},\qquad
\boxed{(d(0),d(1),d(2),d(3),d(4))=(5,6,8,0,12)}.
$$

These values follow either by completing [Dijkstra's algorithm](../../../../../dijkstra-algorithm.md) in the order $3,0,1,2,4$, or by observing that any internal vertex $w$ on a simple route adds $4w-1$ to the direct-edge cost: only the internal vertex $0$ can reduce it.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
