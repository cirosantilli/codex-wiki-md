# Matrix rounding with fixed margins

↑ **Parent:** [Integrality of the transportation problem](integrality-of-the-transportation-problem.md)

A [matrix](matrix.md) of nonnegative [rational numbers](rational-number.md) with [integer](integer-split.md) row and column [sums](sum.md) can be rounded entrywise up or down while preserving all those [sums](sum.md). Let $p_{ij}=\lfloor a_{ij}\rfloor$ and $f_{ij}=a_{ij}-p_{ij}$ be its [floor](floor-function.md) and [fractional part](fractional-part.md). The residual row and column [sums](sum.md) $r_i=\sum_jf_{ij}$ and $c_j=\sum_if_{ij}$ are [nonnegative integers](natural-number.md). Build a [flow network](flow-network-split.md) with source-to-row [flow network edge capacities](flow-network-edge-capacity.md) $r_i$, row-to-column [flow network edge capacities](flow-network-edge-capacity.md) one where $f_{ij}>0$, and column-to-sink [flow network edge capacities](flow-network-edge-capacity.md) $c_j$. The [fractional parts](fractional-part.md) supply a [feasible flow](feasible-flow.md) saturating all source arcs. The [integral max-flow theorem](integral-max-flow-theorem.md) supplies an integral one of the same total value. If its middle-arc [flows](flow.md) are $h_{ij}\in\{0,1\}$, with $h_{ij}=0$ where $f_{ij}=0$, then $b_{ij}=p_{ij}+h_{ij}$ is the required [matrix](matrix.md). This is a constructive [polynomial-time algorithm](polynomial-time-algorithm.md); no multiplication by a common denominator is required.

## ↑ Ancestors (8)

1. [Integrality of the transportation problem](integrality-of-the-transportation-problem.md)
2. [Transportation problem](transportation-problem.md)
3. [Linear programming duality](linear-programming-duality.md)
4. [Linear programming](linear-programming-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms/1/d/solution.md)
