<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [maximum flow](../../../../../../maximum-flow-problem.md) problem specifies a finite directed [flow network](../../../../../../flow-network.md), a source $s$, a sink $t$, and nonnegative arc capacities. A feasible flow assigns $0\leq f_e\leq c_e$ to each arc, with incoming flow equal to outgoing flow at each vertex other than $s,t$. The objective is to maximize the net flow leaving $s$, equivalently entering $t$.

The [Ford-Fulkerson algorithm](../../../../../../ford-fulkerson-algorithm.md) starts with zero flow. Its [residual network](../../../../../../residual-network.md) has a forward arc of capacity $c_e-f_e$ and a reverse arc of capacity $f_e$ for each original arc. If an $s$–$t$ path has positive residual capacities, augment by their minimum: increase flow along forward arcs and decrease it along reverse arcs. This preserves capacity bounds and conservation, and increases the flow value by that positive bottleneck. Repeat until there is no augmenting path.

For rational capacities, choose a positive integer $D$ clearing every denominator. Initially all flows and residual capacities are integer multiples of $1/D$, and augmentation preserves that property. Every augmentation therefore increases the flow value by at least $1/D$. The flow value is bounded above by the sum of capacities of arcs leaving $s$. Thus only finitely many augmentations can occur, independently of how the augmenting paths are chosen.

To see why termination supplies a maximum, let $S$ consist of vertices reachable from $s$ in the final residual network. The sink is not in $S$. Each original arc from $S$ to its complement is saturated; each original arc entering $S$ has zero flow, since otherwise its reverse residual arc would leave $S$. The resulting flow value equals the capacity of this cut. No feasible flow exceeds a cut capacity. Hence **the algorithm terminates at a maximum flow for rational capacities**, proving the relevant [max-flow min-cut theorem](../../../../../../max-flow-min-cut-theorem.md) conclusion as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
