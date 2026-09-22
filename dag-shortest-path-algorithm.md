# DAG shortest-path algorithm

↑ **Parent:** [Single-source shortest-path problem](single-source-shortest-path-problem.md)

Initialize source distance to zero and other distances to infinity, then process vertices in [topological order](topological-order.md), relaxing their outgoing edges once. Every predecessor on a path to a vertex appears earlier, so induction through that ordering proves that its distance is final when processed. Negative weights are allowed because there are no directed cycles. With [adjacency lists](adjacency-list.md), [topological sorting](topological-sorting.md) and all [edge relaxations](edge-relaxation.md) take $O(|V|+|E|)$ time; predecessor pointers reconstruct paths.

## ↑ Ancestors (7)

1. [Single-source shortest-path problem](single-source-shortest-path-problem.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/5/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/functional-programming-design-and-analysis-of-algorithms/8/e/solution.md)
