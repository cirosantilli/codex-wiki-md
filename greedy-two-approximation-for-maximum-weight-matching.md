# Greedy two-approximation for maximum-weight matching

↑ **Parent:** [Maximum-weight matching](maximum-weight-matching.md)

For nonnegative weights on a finite [graph](graph-split.md), scan [edges](edge-of-a-graph.md) in nonincreasing weight order, selecting each when it shares no endpoint with an already selected [edge](edge-of-a-graph.md). This [greedy matching](greedy-matching.md) is a factor-two [approximation algorithm](approximation-algorithm.md) for [maximum-weight matching](maximum-weight-matching.md).

**Proof.** Charge each optimal [edge](edge-of-a-graph.md) to itself if selected, and otherwise to an earlier selected [edge](edge-of-a-graph.md) that blocked it. The receiving [edge](edge-of-a-graph.md) weighs at least as much. Each selected [edge](edge-of-a-graph.md) receives at most two charges, since its two endpoints each meet at most one optimal [edge](edge-of-a-graph.md). Summing proves the bound. Sorting takes $O(|E|\log|E|)$ time, followed by a scan that records which [vertices](vertex-graph-theory.md) are used.

The factor is sharp even for strictly positive weights. On a four-[vertex](vertex-graph-theory.md) [path graph](path-graph.md) with consecutive weights $1,1+\varepsilon,1$, where $0<\varepsilon<1$, the [greedy matching](greedy-matching.md) weighs $1+\varepsilon$ and the optimal [matching in a graph](matching-graph-theory-split.md) weighs two. Their ratio tends to two as $\varepsilon\downarrow0$. For infinitely many sizes, use $k$ disjoint copies with $\varepsilon=1/k$, $k\geq2$. This example isolates the obstruction: a locally attractive [edge](edge-of-a-graph.md) can block two compatible [edges](edge-of-a-graph.md).

## ↑ Ancestors (7)

1. [Maximum-weight matching](maximum-weight-matching.md)
2. [Matching (graph theory)](matching-graph-theory-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/3/c/ii/solution.md)
