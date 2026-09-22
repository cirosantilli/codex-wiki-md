# Circulation with vertex demands

↑ **Parent:** [Circulation in a flow network](circulation-in-a-flow-network.md)

A [flow](flow.md) on a [directed graph](directed-graph.md) satisfying [capacity constraints](capacity-constraint.md) and a specified net inflow $d_v$ at each [vertex](vertex-graph-theory.md). Positive $d_v$ denotes consumption and negative $d_v$ supply. Summing all balances cancels each [edge](edge-of-a-graph.md) once as inflow and once as outflow, so $\sum_vd_v=0$ is necessary. With balanced demands and no lower bounds, add a source [edge](edge-of-a-graph.md) of [flow network edge capacity](flow-network-edge-capacity.md) $-d_v$ into every supply [vertex](vertex-graph-theory.md) and an [edge](edge-of-a-graph.md) of [flow network edge capacity](flow-network-edge-capacity.md) $d_v$ from each demand [vertex](vertex-graph-theory.md) to a new sink. A [maximum flow](maximum-flow-problem.md) saturating all auxiliary [edges](edge-of-a-graph.md) exists exactly when the demands are feasible.

## ↑ Ancestors (7)

1. [Circulation in a flow network](circulation-in-a-flow-network.md)
2. [Flow network](flow-network-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Lower bounds on network flow](lower-bounds-on-network-flow.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/2/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/2/c/solution.md)
