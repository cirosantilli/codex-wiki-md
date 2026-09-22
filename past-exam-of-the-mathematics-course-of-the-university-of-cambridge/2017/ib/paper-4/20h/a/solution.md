<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A finite [flow network](../../../../../../flow-network.md) is a [directed graph](../../../../../../directed-graph.md) with distinguished source $s$, sink $t$, and nonnegative finite [flow network edge capacities](../../../../../../flow-network-edge-capacity.md) $c_{ij}$ on its directed edges. A feasible [flow](../../../../../../flow.md) consists of numbers $f_{ij}$ satisfying

$$
0\leq f_{ij}\leq c_{ij},\qquad
\sum_j f_{ij}=\sum_j f_{ji}\quad(i\ne s,t).
$$

The second condition is [flow conservation](../../../../../../flow-conservation.md); absent edges contribute zero. The [strength of a flow](../../../../../../strength-of-a-flow.md) is its net outflow from the source,

$$
|f|=\sum_j f_{sj}-\sum_j f_{js},
$$

which equals net inflow to the sink by summing [flow conservation](../../../../../../flow-conservation.md) over the other vertices. The [maximum flow problem](../../../../../../maximum-flow-problem.md) is

$$
\boxed{\text{maximise }|f|\text{ over all feasible flows}}.
$$

No assumption that a capacity-saturating flow at the source is feasible downstream is made. On a finite network a maximum exists, because the constraints define a nonempty [compact](../../../../../../compact-space.md) set of edge flows and the objective is [continuous](../../../../../../continuous-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
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
