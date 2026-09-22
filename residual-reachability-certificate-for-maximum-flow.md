# Residual reachability certificate for maximum flow

↑ **Parent:** [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)

In a finite [flow network](flow-network.md), a [maximum flow](maximum-flow-problem.md) exists because the [feasible flow](feasible-flow.md) set contains the zero [flow](flow.md) and is a [compact set](compact-space.md): the [capacity constraints](capacity-constraint.md) bound every coordinate, and they and [flow conservation](flow-conservation.md) define a [closed set](closed-set.md). The [strength of a flow](strength-of-a-flow.md) is a [continuous function](continuous-function.md), so the [extreme value theorem](extreme-value-theorem.md) gives an attained maximum. An [augmenting path](augmenting-path.md) in the [residual network](residual-network.md) would permit positive augmentation, contradicting maximality. The source-reachable [vertices](vertex-graph-theory.md) in the [residual network](residual-network.md) therefore define a [cut of a flow network](cut-of-a-flow-network.md) whose outgoing original [edges](edge-of-a-graph.md) are saturated and incoming original [edges](edge-of-a-graph.md) carry zero [flow](flow.md). [Flow conservation](flow-conservation.md) makes the [strength of a flow](strength-of-a-flow.md) equal to this [cut capacity](cut-capacity.md), proving the [max-flow min-cut theorem](max-flow-min-cut-theorem.md).

Existence and [strong duality](strong-duality.md) for finite real [flow network edge capacities](flow-network-edge-capacity.md) do not imply finite termination for every choice of [augmenting paths](augmenting-path.md) in the [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md). With irrational capacities, some choices can continue forever. With integer capacities, [Integrality of the Ford-Fulkerson algorithm](integrality-of-the-ford-fulkerson-algorithm.md) instead forces finite termination; rational capacities reduce to that case by a common denominator. Choosing shortest [augmenting paths](augmenting-path.md) as in the [Edmonds–Karp algorithm](edmonds-karp-algorithm.md) avoids dependence on capacity magnitudes.[Karger, MIT 6.854 Notes 6, section 2.1, rational and real capacities](https://courses.csail.mit.edu/6.854/21/Notes/n06-flow.html)

## ↑ Ancestors (7)

1. [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
