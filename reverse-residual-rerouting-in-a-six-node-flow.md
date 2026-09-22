# Reverse residual rerouting in a six-node flow

↑ **Parent:** [Residual network](residual-network.md)

For arc capacities $(c_{12},c_{13},c_{24},c_{34},c_{35},c_{46},c_{56})=(3,3,2,2,3,3,2)$, the feasible flow $(1,3,1,2,1,3,1)$ has value four. The displayed residual path has bottleneck one and traverses $4\to3$ opposite to the original arc $3\to4$. Augmentation cancels one unit there and gives $(2,3,2,1,2,3,2)$ of value five. The sink cut has capacity five, proving optimality. Reverse residual arcs are what permit rerouting instead of only adding flow along unused forward arcs.

## ↑ Ancestors (8)

1. [Residual network](residual-network.md)
2. [Max-flow min-cut theorem](max-flow-min-cut-theorem.md)
3. [Flow network](flow-network-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
