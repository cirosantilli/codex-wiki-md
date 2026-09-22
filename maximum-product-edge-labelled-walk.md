# Maximum-product edge-labelled walk

↑ **Parent:** [Edge-labelled walk matching](edge-labelled-walk-matching.md)

Attach nonnegative [edge](edge-of-a-graph.md) scores to [edge-labelled walk matching](edge-labelled-walk-matching.md). For each layer and endpoint, keep the greatest product over matching prefixes. Only [edges](edge-of-a-graph.md) with the required current label enter the maximum. Multiplication by a nonnegative score preserves order, proving the [dynamic programming](dynamic-programming.md) recurrence. Store a predecessor for each reachable layer entry to recover a maximizing walk. A reachable score of zero must be distinguished from no matching walk: keep reachability separately or use an impossible negative sentinel and skip it before multiplication. The score is the defined product; interpreting it as a physical event [probability](probability.md) can require extra independence assumptions.

## ↑ Ancestors (6)

1. [Edge-labelled walk matching](edge-labelled-walk-matching.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/7/c/ii/solution.md)
