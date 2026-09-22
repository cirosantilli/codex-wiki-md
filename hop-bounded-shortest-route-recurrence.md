# Hop-bounded shortest-route recurrence

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

Let $D_r(v)$ be the minimum weight of a route from a fixed source to $v$ using at most $r$ [edges](edge-of-a-graph.md); repeated [vertices](vertex-graph-theory.md) are permitted. Initialise $D_0$ to zero at the source and infinity elsewhere. Every feasible route either already uses at most $r-1$ [edges](edge-of-a-graph.md) or appends one [edge](edge-of-a-graph.md) to such a route, proving the displayed [dynamic programming](dynamic-programming.md) recurrence. Reading exclusively from the previous row enforces the [edge](edge-of-a-graph.md) budget. Negative cycles cause no unbounded objective because the budget is finite. Each round scans all [edges](edge-of-a-graph.md), costing $O(m)$ when only edge-incident [vertices](vertex-graph-theory.md) and the specified endpoints are processed. With nonnegative weights, cycle removal gives an equally good or better simple path within the budget.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/7/d/solution.md)
