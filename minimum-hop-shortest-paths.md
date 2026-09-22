# Minimum-hop shortest paths

↑ **Parent:** [Dijkstra algorithm](dijkstra-algorithm.md)

Among paths of minimum total weight, choose the fewest edges. Store a [lexicographic order](lexicographic-order.md) pair $(d,h)$ and extend it across weight $w$ as $(d+w,h+1)$. For positive edge weights, every extension strictly increases its first component, so [Dijkstra's algorithm](dijkstra-algorithm.md) settles these pairs correctly when its [priority queue](priority-queue.md) and relaxation both compare the full pair. Equal total weight then selects the smaller hop count; arbitrary vertex-name tie-breaking does not express this objective.

## ↑ Ancestors (7)

1. [Dijkstra algorithm](dijkstra-algorithm.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms-resit/5/d/solution.md)
