<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Ford-Fulkerson algorithm](../../../../../../ford-fulkerson-algorithm.md) starts with zero [flow](../../../../../../flow.md). For each original edge $i\to j$, the [residual network](../../../../../../residual-network.md) has a forward edge with residual capacity $c_{ij}-f_{ij}$ and a reverse edge with residual capacity $f_{ij}$. Distinguish these labelled residual edges if the original graph has antiparallel edges. While there is a source-to-sink [augmenting path](../../../../../../augmenting-path.md) with positive residual capacities, increase the [flow](../../../../../../flow.md) by the minimum residual capacity along it, adding on forward edges and subtracting on reverse edges. This preserves capacity bounds and [flow conservation](../../../../../../flow-conservation.md) and increases the [strength of a flow](../../../../../../strength-of-a-flow.md) by that positive bottleneck.

A [cut of a flow network](../../../../../../cut-of-a-flow-network.md) is a partition $(S,V\setminus S)$ with $s\in S$, $t\notin S$, of capacity $c(S)=\sum_{i\in S,j\notin S}c_{ij}$. Summing [flow conservation](../../../../../../flow-conservation.md) gives $|f|=f(S,V\setminus S)-f(V\setminus S,S)\leq c(S)$. The [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) states

$$
\boxed{\max_f|f|=\min_{S:s\in S,\,t\notin S}c(S)}.
$$

When no [augmenting path](../../../../../../augmenting-path.md) remains, take $S$ to be the vertices reachable from $s$ in the [residual network](../../../../../../residual-network.md). Every original outgoing edge of this [cut of a flow network](../../../../../../cut-of-a-flow-network.md) is saturated and every incoming edge has zero [flow](../../../../../../flow.md); otherwise a positive residual edge would leave $S$. Thus $|f|=c(S)$, certifying optimality and the theorem. For general finite real capacities, one can also apply this argument to an existing maximum: it cannot admit an [augmenting path](../../../../../../augmenting-path.md).

With integer capacities, each augmentation increases the value by at least one, so the [Ford-Fulkerson algorithm](../../../../../../ford-fulkerson-algorithm.md) terminates. Rational capacities can be scaled to integers. Arbitrary path choices with irrational capacities need not terminate; the existence theorem does not justify claiming finite termination in that generality. The given network has integer capacities, so this caveat does not obstruct its computation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
