<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Deleting a [vertex](../../../../../vertex-graph-theory.md) and its incident [edge](../../../../../edge-of-a-graph.md) cannot create a [graph cycle](../../../../../cycle-in-a-graph.md), so $T\setminus v$ is acyclic. It remains to establish connectedness and nonemptiness.

Since the [leaf of a tree](../../../../../leaf-of-a-tree.md) $v$ has one neighbour, $T$ has at least two [vertices](../../../../../vertex-graph-theory.md), so $T\setminus v$ is nonempty. For any two remaining [vertices](../../../../../vertex-graph-theory.md) $a,b$, take their unique simple [graph path](../../../../../path-in-a-graph.md) in $T$. It cannot pass through $v$: an internal [vertex](../../../../../vertex-graph-theory.md) on such a [graph path](../../../../../path-in-a-graph.md) has two incident [edges](../../../../../edge-of-a-graph.md), whereas $v$ has [vertex degree](../../../../../degree-graph-theory.md) one. Neither endpoint is $v$, so the entire [graph path](../../../../../path-in-a-graph.md) remains after deletion. The remaining [graph](../../../../../graph-split.md) is connected and acyclic, giving

$$
\boxed{T\setminus v\text{ is a tree}.}
$$

This includes the two-[vertex](../../../../../vertex-graph-theory.md) case, where deletion leaves the one-[vertex](../../../../../vertex-graph-theory.md) [tree](../../../../../tree-graph-theory-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
