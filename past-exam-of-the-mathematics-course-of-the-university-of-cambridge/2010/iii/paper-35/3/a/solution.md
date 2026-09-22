<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite directed [flow network](../../../../../../flow-network.md) with source $s$, sink $t$ and nonnegative finite [flow network edge capacities](../../../../../../flow-network-edge-capacity.md) $c_e$, the [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) states

$$
\boxed{\max_{f\text{ feasible}}|f|=\min_{S:s\in S,\ t\notin S}c(S,S^c).}
$$

Here feasible arc flows satisfy $0\leq f_e\leq c_e$ and [flow conservation](../../../../../../flow-conservation.md) at every vertex except $s,t$. Their [strength of a flow](../../../../../../strength-of-a-flow.md) is the net outflow at $s$. A [cut of a flow network](../../../../../../cut-of-a-flow-network.md) has [cut capacity](../../../../../../cut-capacity.md) equal to the sum of capacities on arcs directed from $S$ to $S^c$.

For any feasible [flow](../../../../../../flow.md) and any such [cut of a flow network](../../../../../../cut-of-a-flow-network.md), summing [flow conservation](../../../../../../flow-conservation.md) over $S$ cancels internal arcs and gives

$$
|f|=\sum_{u\in S,v\notin S}f_{uv}-\sum_{u\notin S,v\in S}f_{uv}\leq\sum_{u\in S,v\notin S}c_{uv}=c(S,S^c).
$$

Thus every flow value is bounded by every cut capacity.

A maximum [flow](../../../../../../flow.md) exists: the feasible arc-flow vectors form a nonempty closed subset of the finite-dimensional compact box $\prod_e[0,c_e]$, and flow value is continuous. Choose one, $f^*$. Its [residual network](../../../../../../residual-network.md) has a forward arc of capacity $c_e-f_e^*$ and a reverse arc of capacity $f_e^*$ for each original arc. If a residual $s$–$t$ [augmenting path](../../../../../../augmenting-path.md) existed, its smallest positive residual capacity would permit increasing forward flows and decreasing reverse flows along the path. This preserves all capacity bounds and internal [flow conservation](../../../../../../flow-conservation.md) while strictly increasing $|f^*|$, a contradiction.

Let $S$ be the vertices reachable from $s$ through positive residual arcs. Then $t\notin S$. Every original arc leaving $S$ is saturated, since otherwise its endpoint would also be reachable. Every original arc entering $S$ carries zero flow, since a positive flow would create a residual reverse arc leaving $S$. Therefore

$$
|f^*|=\sum_{u\in S,v\notin S}c_{uv}=c(S,S^c).
$$

Together with the universal upper bound, this proves both optimality claims and the theorem. This existence argument works for real capacities; it does not assume that arbitrary choices in the [Ford-Fulkerson algorithm](../../../../../../ford-fulkerson-algorithm.md) terminate. For integer capacities, positive augmentations are integral and increase the flow value by at least one, so the algorithm does terminate.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
