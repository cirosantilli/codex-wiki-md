<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For a finite directed [flow network](../../../../../flow-network.md) with nonnegative finite edge capacities, a source $s$ and a distinct sink $t$, the [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md) states that the largest feasible flow value equals the smallest capacity of a cut separating $s$ from $t$. A feasible flow has $0\leq f_e\leq c_e$ on each directed edge and [flow conservation](../../../../../flow-conservation.md) at all other vertices. Its value is the net outflow at $s$.

For any cut $S$ containing $s$ but not $t$, sum conservation over vertices of $S$. Internal edges cancel, giving

$$
|f|=\sum_{e:S\to S^c}f_e-\sum_{e:S^c\to S}f_e
\leq\sum_{e:S\to S^c}c_e=\operatorname{cap}(S).
$$

Thus every flow value is bounded by every cut capacity.

A maximum flow exists: the feasible set is nonempty, closed and bounded in a finite-dimensional edge-coordinate space, hence compact, and the flow value is [continuous](../../../../../continuous-function.md). For such a flow, form its [residual network](../../../../../residual-network.md): each original edge has forward residual capacity $c_e-f_e$ and backward residual capacity $f_e$. Keep these as edge-labelled arcs if the original network already has edges in both directions. If a directed positive-residual path joined $s$ to $t$, increasing the flow along its forward arcs and decreasing it along its backward arcs by the path's positive bottleneck capacity would preserve feasibility and increase the value. That contradicts maximality.

Let $S$ be the vertices reachable from $s$ by positive residual arcs. Then $t\notin S$. Every original edge from $S$ to $S^c$ is saturated, otherwise its forward residual arc would extend reachability. Every original edge from $S^c$ to $S$ has zero flow, otherwise its backward residual arc would extend reachability. Therefore

$$
|f|=\sum_{e:S\to S^c}c_e=\operatorname{cap}(S).
$$

Together with the bound for every flow and cut, this proves

$$
\boxed{\max_f|f|=\min_{S:s\in S,\,t\notin S}\operatorname{cap}(S).}
$$

The compactness step makes the proof valid for arbitrary real capacities; it does not assume that a particular augmenting-path algorithm terminates after finitely many augmentations.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
