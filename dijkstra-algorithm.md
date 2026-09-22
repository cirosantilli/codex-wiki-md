# Dijkstra algorithm

↑ **Parent:** [Shortest path problem](shortest-path-problem.md)

Starting with distance zero at the source and infinity elsewhere, repeatedly finalize the unfinalized vertex with least tentative distance and relax its outgoing edges. Nonnegative lengths ensure that no later path can improve a finalized distance: any alternative path first reaches an unfinalized vertex whose tentative distance is at least the finalized one. A binary heap gives $O((|V|+|E|)\log |V|)$ arithmetic operations, and storing predecessors recovers a minimizing path.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Label-setting shortest-path algorithm](label-setting-shortest-path-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-35/2/solution.md)
- [Shortest path problem](shortest-path-problem.md)
