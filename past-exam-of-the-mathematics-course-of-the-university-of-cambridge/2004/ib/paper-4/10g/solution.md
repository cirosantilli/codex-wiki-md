<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

Take a finite directed [flow network](../../../../../flow-network.md) with distinct source $s$, sink $t$ and finite nonnegative [flow network edge capacities](../../../../../flow-network-edge-capacity.md). A [flow](../../../../../flow.md) assigns $f_e$ to each edge with $0\leq f_e\leq c_e$ and obeys [flow conservation](../../../../../flow-conservation.md) at every vertex except $s,t$. Its value is net outflow from the source, $|f|=\sum_{s\to v}f_e-\sum_{v\to s}f_e$. A maximal flow here means a [maximum flow](../../../../../maximum-flow-problem.md): one with greatest value among feasible flows. A source-to-sink [cut of a flow network](../../../../../cut-of-a-flow-network.md) is a partition $(S,S^c)$ with $s\in S$, $t\notin S$; its [cut capacity](../../../../../cut-capacity.md) is $c(S)=\sum_{u\in S,v\notin S}c_{uv}$, counting directed edges leaving $S$.

The [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) states

$$
\boxed{\max_f|f|=\min_{S:s\in S,\ t\notin S}c(S).}
$$

Summing conservation over $S$ cancels internal edges and gives

$$
|f|=\sum_{S\to S^c}f_e-\sum_{S^c\to S}f_e\leq c(S).
$$

This is the upper bound for every flow and every cut. To prove equality, a maximum exists: the feasible edge vectors form a nonempty closed bounded subset of a finite-dimensional real space, and flow value is continuous.

For a maximum $f$, construct its [residual network](../../../../../residual-network.md). Each edge has a forward residual edge of capacity $c_e-f_e$ and a backward residual edge of capacity $f_e$; retain those of positive capacity. If a residual source-to-sink path existed, augment by the smallest residual capacity on that finite path. Increasing original forward flows and decreasing backward flows preserves all feasibility conditions and increases value, contradicting maximality. Thus no such [augmenting path](../../../../../augmenting-path.md) exists.

Let $S$ be the vertices reachable from $s$ in the residual network. Then $t\notin S$. Every original edge leaving $S$ is saturated, since otherwise its positive forward residual edge would make its endpoint reachable. Every original edge entering $S$ has zero flow, since otherwise its backward residual edge would give the same contradiction. Hence

$$
|f|=\sum_{S\to S^c}c_e=c(S).
$$

Together with the universal upper bound this proves equality and identifies a minimum cut. This proof covers real capacities without assuming that an augmenting-path algorithm terminates after finitely many steps. Merely being impossible to increase all edge flows coordinatewise is not the optimization meaning of “maximal” used in the theorem.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
