<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

An [cut of a flow network](../../../../../cut-of-a-flow-network.md) partitions a [flow network](../../../../../flow-network.md) into $S,S^c$, with source $A\in S$ and sink $B\notin S$. Its [cut capacity](../../../../../cut-capacity.md) is the sum of capacities of arcs directed from $S$ to $S^c$; a [minimum cut](../../../../../minimum-cut.md) minimizes this sum.

Use the suggested nodes. Give $A\to a_e$ capacity $1$, each $a_e\to b_v$ capacity $M=m+kn+1$, and each $b_v\to B$ capacity $k$. By the [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md), a flow of value $kn$ exists once every [cut capacity](../../../../../cut-capacity.md) is at least $kn$.

Consider a [cut of a flow network](../../../../../cut-of-a-flow-network.md) containing no crossing arc of capacity $M$, and let $U$ be the intersections on the sink side. Every street incident to $U$ must also be on that side, or its arc to an endpoint in $U$ would cross the [cut of a flow network](../../../../../cut-of-a-flow-network.md). Hence at least $d(U)$ source-to-street arcs cross, as do the $n-|U|$ intersection-to-sink arcs from the other intersections. Therefore its [cut capacity](../../../../../cut-capacity.md) is at least

$$
d(U)+k(n-|U|)\geq kn.
$$

A [cut of a flow network](../../../../../cut-of-a-flow-network.md) crossing a capacity-$M$ arc has still larger capacity. The [cut of a flow network](../../../../../cut-of-a-flow-network.md) just before the sink has capacity $kn$, proving the maximum flow value is exactly $kn$.

The [integral max-flow theorem](../../../../../integral-max-flow-theorem.md) supplies an integral maximum flow. Every intersection sends $k$ units to the sink; each street can supply at most one unit, assigned to one endpoint. Orient each assigned street **away from its assigned endpoint**. Orient unassigned streets arbitrarily. Then each vertex has at least $k$ outgoing streets. An [Ford-Fulkerson algorithm](../../../../../ford-fulkerson-algorithm.md) with integer capacities constructs this [flow](../../../../../flow.md) and therefore the street directions. Notice that the condition also is necessary: outgoing streets from vertices in $U$ are distinct edges incident to $U$, so $d(U)\geq k|U|$. This is an [outdegree orientation criterion](../../../../../outdegree-orientation-criterion.md).

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
