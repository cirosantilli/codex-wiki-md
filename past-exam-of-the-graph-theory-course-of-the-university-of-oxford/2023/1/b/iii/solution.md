<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [mathematical induction](../../../../../mathematical-induction.md) on the [maximum degree](../../../../../maximum-degree.md) $\Delta$, including $\Delta=0$ as the base case. A [graph](../../../../../graph-split.md) of [maximum degree](../../../../../maximum-degree.md) zero has no [edges](../../../../../edge-of-a-graph.md), so zero colours suffice.

For $\Delta>0$, part (ii) supplies a [matching in a graph](../../../../../matching-graph-theory-split.md) $M$ meeting every [vertex](../../../../../vertex-graph-theory.md) of [vertex degree](../../../../../degree-graph-theory.md) $\Delta$. Delete its [edges](../../../../../edge-of-a-graph.md), retaining all [vertices](../../../../../vertex-graph-theory.md). Each [vertex](../../../../../vertex-graph-theory.md) formerly of [maximum degree](../../../../../maximum-degree.md) loses one incident [edge](../../../../../edge-of-a-graph.md); every other [vertex](../../../../../vertex-graph-theory.md) already had [vertex degree](../../../../../degree-graph-theory.md) at most $\Delta-1$. Hence

$$
\Delta(G-M)\leq\Delta-1.
$$

The resulting [graph](../../../../../graph-split.md) is still a [bipartite graph](../../../../../bipartite-graph-split.md). By [mathematical induction](../../../../../mathematical-induction.md), it has a [proper edge colouring](../../../../../proper-edge-coloring.md) using at most $\Delta-1$ colours. Give every [edge](../../../../../edge-of-a-graph.md) of $M$ one new colour. Since $M$ is a [matching in a graph](../../../../../matching-graph-theory-split.md), this produces a [proper edge colouring](../../../../../proper-edge-coloring.md) of $G$ with at most $\Delta$ colours. The [edges](../../../../../edge-of-a-graph.md) at a [vertex](../../../../../vertex-graph-theory.md) of [maximum degree](../../../../../maximum-degree.md) require at least $\Delta$ colours, so

$$
\boxed{\chi'(G)=\Delta.}
$$

This is [Kőnig's line colouring theorem](../../../../../konig-s-line-colouring-theorem.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the graph theory course of the University of Oxford](../../../../split.md)
6. [Graph theory course of the University of Oxford](../../../../../graph-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
