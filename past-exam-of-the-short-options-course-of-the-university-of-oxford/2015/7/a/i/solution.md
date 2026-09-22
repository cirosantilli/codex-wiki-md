<h1 id="7/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [tree](../../../../../tree-graph-theory-split.md) is a nonempty [connected graph](../../../../../connected-graph.md) with no [graph cycle](../../../../../cycle-in-a-graph.md). A [leaf of a tree](../../../../../leaf-of-a-tree.md) is a [vertex](../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../degree-graph-theory.md) one. As usual in this finite [graph theory](../../../../../graph-theory-split.md) problem, [trees](../../../../../tree-graph-theory-split.md) are finite; the assertion would fail for a doubly infinite [graph path](../../../../../path-in-a-graph.md).

Take a [longest path](../../../../../longest-path.md) $v_0,v_1,\ldots,v_m$ in a [tree](../../../../../tree-graph-theory-split.md) with at least two [vertices](../../../../../vertex-graph-theory.md). Connectedness gives $m\ge1$. If $v_0$ had a neighbour outside this [graph path](../../../../../path-in-a-graph.md), the path could be extended, contradicting maximal length. If it had a neighbour $v_j$ with $j\ge2$, that [edge](../../../../../edge-of-a-graph.md) together with the segment $v_0,v_1,\ldots,v_j$ would make a [graph cycle](../../../../../cycle-in-a-graph.md). Thus its only neighbour is $v_1$, and it is a [leaf of a tree](../../../../../leaf-of-a-tree.md). The same argument at the other end makes $v_m$ a second, distinct [leaf of a tree](../../../../../leaf-of-a-tree.md). Hence

$$
\boxed{\text{Every finite tree with at least two vertices has at least two leaves.}}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
