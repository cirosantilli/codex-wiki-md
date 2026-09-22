<h1 id="5h/solution">Solution</h1>

↑ **Parent:** [5H](../5h.md)

Consider a finite directed [flow network](../../../../../flow-network.md) with source $s$, sink $t$, and nonnegative finite [flow network edge capacities](../../../../../flow-network-edge-capacity.md) $c_e$. A feasible [flow](../../../../../flow.md) assigns $0\le f_e\le c_e$ to each arc and satisfies [flow conservation](../../../../../flow-conservation.md) at every vertex except $s,t$. Its value $|f|$ is net outflow from $s$, equivalently net inflow to $t$. A maximal flow here means a flow of greatest value, also called a [maximum flow](../../../../../maximum-flow-problem.md). A source–sink [cut of a flow network](../../../../../cut-of-a-flow-network.md) is a partition $(S,S^c)$ with $s\in S$, $t\notin S$; its [cut capacity](../../../../../cut-capacity.md) is $c(S,S^c)=\sum_{u\in S,v\notin S}c_{uv}$, summing directed arcs from $S$ to its complement.

The [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) states

$$
\boxed{\max_f|f|=\min_{S:s\in S,\ t\notin S}c(S,S^c).}
$$

For any feasible flow and cut, summing [flow conservation](../../../../../flow-conservation.md) over vertices in $S$ cancels internal arcs and gives $|f|=\sum_{S\to S^c}f_e-\sum_{S^c\to S}f_e\le c(S,S^c)$. This proves the upper bound by every cut.

For the reverse bound, a maximum exists: the feasible set is a nonempty closed subset of the bounded product $\prod_e[0,c_e]$, hence compact, and $|f|$ is continuous. Choose a maximizing flow $f$. Its [residual network](../../../../../residual-network.md) has a forward arc for unused capacity $c_e-f_e$ and a reverse arc for cancellable flow $f_e$, retaining original-arc identities if necessary. If a residual path joined $s$ to $t$, the minimum of its positive residual capacities would be positive. Increasing forward flows and cancelling reverse flows by this amount would preserve all constraints while increasing $|f|$, a contradiction.

Let $S$ consist of vertices reachable from $s$ through positive residual arcs. Then $t\notin S$. An original arc from $S$ to $S^c$ must be saturated, since otherwise its forward residual arc would make its endpoint reachable. An original arc from $S^c$ to $S$ must carry zero flow, since a positive reverse residual arc would again extend reachability. Thus

$$
|f|=\sum_{S\to S^c}c_e-0=c(S,S^c).
$$

The upper bound and this equality prove the theorem and exhibit a [residual reachability certificate for maximum flow](../../../../../residual-reachability-certificate-for-maximum-flow.md). The argument works for real capacities and does not assume that an arbitrary augmenting-path algorithm terminates in finitely many steps.

## ↑ Ancestors (10)

1. [5H](../5h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
