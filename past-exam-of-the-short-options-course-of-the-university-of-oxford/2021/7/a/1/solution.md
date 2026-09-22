<h1 id="7/a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

At weight $y$ the [edges](../../../../../edge-of-a-graph.md) considered are precisely the horizontal [edges](../../../../../edge-of-a-graph.md) in row $y$. For $y=1$ all $n$ [graph vertices](../../../../../vertex-graph-theory.md) in that row are isolated, so all $n-1$ [edges](../../../../../edge-of-a-graph.md) are accepted. For $y\ge2$, the first $y-1$ [graph vertices](../../../../../vertex-graph-theory.md) in that row already belong to the one component built by earlier stages, because vertical columns $1,\ldots,y-1$ have already been processed. The other [graph vertices](../../../../../vertex-graph-theory.md) are isolated. Thus the [edges](../../../../../edge-of-a-graph.md) with $x<y-1$ would create a [graph cycle](../../../../../cycle-in-a-graph.md), and all the [edges](../../../../../edge-of-a-graph.md) with $x\ge y-1$ are accepted, successively attaching the remaining [graph vertices](../../../../../vertex-graph-theory.md). The rule is

$$
\boxed{(x,y)(x+1,y)\text{ is accepted exactly when }x\ge y-1.}
$$

The selected [edges](../../../../../edge-of-a-graph.md) of equal weight have no cycles after the existing component is contracted, so tie ordering does not affect this conclusion. Their combined contribution to the [minimum spanning tree](../../../../../minimum-spanning-tree.md) cost is

$$
(n-1)+\sum_{y=2}^n y(n-y+1)=\frac{n(n+1)(n+2)}6-1.
$$

## ↑ Ancestors (13)

1. [1](../1.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
