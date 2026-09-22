# Cycle-cover patching half-approximation for Max-TSP

↑ **Parent:** [Max-TSP](max-tsp.md)

Solve the maximum-weight [assignment problem](assignment-problem.md) forbidding fixed points, obtaining a [cycle cover of a directed graph](cycle-cover-of-a-directed-graph.md) whose weight bounds every [Hamiltonian cycle](hamilton-cycle.md) above. Remove a lightest [edge](edge-of-a-graph.md) from each [graph cycle](cycle-in-a-graph.md). Each [graph cycle](cycle-in-a-graph.md) has at least two [edges](edge-of-a-graph.md), so at least half its nonnegative weight survives. Connect the resulting disjoint [graph paths](path-in-a-graph.md) cyclically; completeness supplies the connectors and their nonnegative weights cannot reduce the retained sum. The [Hungarian algorithm](hungarian-algorithm.md) and linear-time patching give a [polynomial time](polynomial-time.md) [approximation algorithm](approximation-algorithm.md). Negative weights invalidate a universal multiplicative half guarantee: when every weight is $-1$, every tour has weight $-n<(-n)/2$.

## ↑ Ancestors (6)

1. [Max-TSP](max-tsp.md)
2. [Travelling salesman problem](travelling-salesman-problem.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Max-TSP](max-tsp.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/5/solution.md)
