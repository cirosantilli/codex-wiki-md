<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A finite [tree](../../../../../tree-graph-theory-split.md) is a nonempty [connected graph](../../../../../connected-graph.md) with no [graph cycles](../../../../../cycle-in-a-graph.md). We show by [mathematical induction](../../../../../mathematical-induction.md) on its number $v$ of [vertices](../../../../../vertex-graph-theory.md) that it has $v-1$ [edges](../../../../../edge-of-a-graph.md). For $v=1$ there are no [edges](../../../../../edge-of-a-graph.md), so the assertion holds.

If $v>1$, take a [path in a graph](../../../../../path-in-a-graph.md) of maximal length among those without repeated [vertices](../../../../../vertex-graph-theory.md). Each endpoint is a [leaf of a tree](../../../../../leaf-of-a-tree.md): an additional incident [edge](../../../../../edge-of-a-graph.md) would either extend the [path in a graph](../../../../../path-in-a-graph.md) or create a [graph cycle](../../../../../cycle-in-a-graph.md). Delete one such [leaf of a tree](../../../../../leaf-of-a-tree.md) and its unique incident [edge](../../../../../edge-of-a-graph.md). The remaining [graph](../../../../../graph-split.md) stays [connected](../../../../../connected-space.md), since a [path in a graph](../../../../../path-in-a-graph.md) between remaining [vertices](../../../../../vertex-graph-theory.md) never needs that terminal [edge](../../../../../edge-of-a-graph.md), and it has no [graph cycles](../../../../../cycle-in-a-graph.md). It is therefore a [tree](../../../../../tree-graph-theory-split.md) with $v-1$ [vertices](../../../../../vertex-graph-theory.md) and, by [mathematical induction](../../../../../mathematical-induction.md), $v-2$ [edges](../../../../../edge-of-a-graph.md). Restoring the deleted [edge](../../../../../edge-of-a-graph.md) gives $e=v-1$.

Thus its [Euler characteristic](../../../../../euler-characteristic.md) is

$$
\boxed{\chi(X)=v-e=v-(v-1)=1.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology and groups course of the University of Oxford](../../../../split.md)
6. [Topology and groups course of the University of Oxford](../../../../../topology-and-groups-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
