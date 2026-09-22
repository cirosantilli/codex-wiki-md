<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [flow network](../../../../../flow-network-split.md) is a finite [directed graph](../../../../../directed-graph.md) $G=(V,E)$ with nonnegative [flow network edge capacities](../../../../../flow-network-edge-capacity.md) $c_e$, together with distinct source and sink [vertices](../../../../../vertex-graph-theory.md) $s,t$. A [feasible flow](../../../../../feasible-flow.md) in the nonnegative directed-[edge](../../../../../edge-of-a-graph.md) convention is a [function](../../../../../function-split.md) $f:E\to\mathbb R_{\geq0}$ satisfying the [capacity constraints](../../../../../capacity-constraint.md) and [flow conservation](../../../../../flow-conservation.md):

$$
0\leq f_{uv}\leq c_{uv}\quad(uv\in E),\qquad
\sum_{u:uv\in E}f_{uv}=\sum_{w:vw\in E}f_{vw}\quad(v\notin\{s,t\}).
$$

Its [flow value](../../../../../strength-of-a-flow.md) is the net outflow at the source,

$$
|f|=\sum_{w:sw\in E}f_{sw}-\sum_{u:us\in E}f_{us},
$$

which equals the net inflow at the sink by [flow conservation](../../../../../flow-conservation.md).

A [cut of a flow network](../../../../../cut-of-a-flow-network.md) is a [partition of a set](../../../../../partition-of-a-set.md) $(S,V\setminus S)$ with $s\in S$ and $t\notin S$. Its [cut capacity](../../../../../cut-capacity.md) counts only directed [edges](../../../../../edge-of-a-graph.md) leaving $S$:

$$
c(S,V\setminus S)=\sum_{u\in S,\ v\notin S:\,uv\in E}c_{uv}.
$$

The net [flow](../../../../../flow.md) across the [cut of a flow network](../../../../../cut-of-a-flow-network.md) subtracts [flow](../../../../../flow.md) on [edges](../../../../../edge-of-a-graph.md) returning into $S$, and equals $|f|$.

For the following parts, a [circulation with vertex demands](../../../../../circulation-with-vertex-demands.md) has no exceptional source or sink in the original [directed graph](../../../../../directed-graph.md). Instead it satisfies net inflow minus net outflow equal to $d_v$ at every [vertex](../../../../../vertex-graph-theory.md). Thus positive demands consume [flow](../../../../../flow.md), and negative demands supply [flow](../../../../../flow.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Advanced data structures and algorithms](../../../advanced-data-structures-and-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
