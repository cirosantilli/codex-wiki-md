<h1 id="7/a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At weight $x+1/2$, column $x$ is considered just after horizontal row $x$. At this point its first $x$ [graph vertices](../../../../../vertex-graph-theory.md) already lie in the component built so far, while [graph vertices](../../../../../vertex-graph-theory.md) above them in that column are isolated. Consequently vertical [edges](../../../../../edge-of-a-graph.md) with $y<x$ create a [graph cycle](../../../../../cycle-in-a-graph.md), while those with $y\ge x$ attach the isolated [graph vertices](../../../../../vertex-graph-theory.md) in a chain:

$$
\boxed{(x,y)(x,y+1)\text{ is accepted exactly when }y\ge x.}
$$

Together with the horizontal rule this gives an [induction](../../../../../mathematical-induction.md) on the alternating row and column stages and justifies the component description used in both numbered answers. The vertical contribution to the [minimum spanning tree](../../../../../minimum-spanning-tree.md) cost is

$$
\sum_{x=1}^{n-1}\left(x+\frac12\right)(n-x)=\frac{n(n-1)(2n+5)}{12}.
$$

## ↑ Ancestors (13)

1. [2](../2.md)
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
