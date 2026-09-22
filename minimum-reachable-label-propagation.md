# Minimum reachable label propagation

↑ **Parent:** [Condensation graph](condensation-graph.md)

Assign each [vertex](vertex-graph-theory.md) of a finite [directed graph](directed-graph.md) a label in a [total order](total-order.md). To find the least label reachable from each vertex, first compress its [strongly connected components](strongly-connected-component.md). Give each component its own least label, then process the [condensation graph](condensation-graph.md) in reverse [topological order](topological-order.md), replacing each label by the minimum of itself and its successors' labels. Every reachable component is either the current one or reached through a first outgoing edge; [induction](mathematical-induction.md) over this order proves the recurrence. The graph-processing work is $O(|V|+|E|)$ with constant-cost label comparisons. Store a representative vertex as well when a witness is required.

## ↑ Ancestors (8)

1. [Condensation graph](condensation-graph.md)
2. [Strongly connected component](strongly-connected-component.md)
3. [Directed graph](directed-graph.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/7/c/i/solution.md)
