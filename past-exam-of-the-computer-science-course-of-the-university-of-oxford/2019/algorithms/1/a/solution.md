<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use nonnegative amounts on the original [directed edges](../../../../../directed-edge.md) of the [flow network](../../../../../flow-network-split.md). A [feasible flow](../../../../../feasible-flow.md) is a [function](../../../../../function-split.md) $f:E\to\mathbb R_{\geq0}$ satisfying the [capacity constraints](../../../../../capacity-constraint.md) $f(u,v)\leq c(u,v)$ and [flow conservation](../../../../../flow-conservation.md) at every internal [vertex](../../../../../vertex-graph-theory.md):

$$
\sum_{u:(u,v)\in E}f(u,v)=\sum_{w:(v,w)\in E}f(v,w)\qquad(v\notin\{s,t\}).
$$

Its [flow value](../../../../../strength-of-a-flow.md) is net outflow at the source,

$$
\boxed{|f|=\sum_{v:(s,v)\in E}f(s,v)-\sum_{u:(u,s)\in E}f(u,s).}
$$

Summing [flow conservation](../../../../../flow-conservation.md) shows that this is also net inflow at the sink. Subtracting incoming [flow](../../../../../flow.md) matters when the source has incoming [edges](../../../../../edge-of-a-graph.md).

An $s$–$t$ [cut of a flow network](../../../../../cut-of-a-flow-network.md) is a [partition of a set](../../../../../partition-of-a-set.md) $(S,V\setminus S)$ with $s\in S$ and $t\notin S$. Its [cut capacity](../../../../../cut-capacity.md) is **the total outward [flow network edge capacity](../../../../../flow-network-edge-capacity.md)**,

$$
c(S,V\setminus S)=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c(u,v).
$$

Incoming [edges](../../../../../edge-of-a-graph.md) do not contribute to this [sum](../../../../../sum.md). Equivalently, one may use the antisymmetric net-[flow](../../../../../flow.md) convention, but the nonnegative arc convention above will also be used in the subsequent reductions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
