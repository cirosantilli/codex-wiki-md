# Christofides algorithm

↑ **Parent:** [Metric travelling salesman problem](metric-travelling-salesman-problem.md)

Compute a [minimum spanning tree](minimum-spanning-tree.md), then a [minimum-weight perfect matching](minimum-weight-perfect-matching.md) on its odd-degree vertices. Their multiset union is connected with even degrees, so it has an [Euler circuit](euler-circuit.md). Shortcut repeated vertices to obtain a metric tour. The tree costs at most the optimal tour, and shortcutting the optimal tour to its odd-degree subset gives a cyclic order whose alternating matchings show that the added matching costs at most half the optimum. The result is a polynomial-time $3/2$-[approximation algorithm](approximation-algorithm.md) for symmetric metric instances.

## ↑ Ancestors (6)

1. [Metric travelling salesman problem](metric-travelling-salesman-problem.md)
2. [Travelling salesman problem](travelling-salesman-problem.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Minimum-weight perfect matching](minimum-weight-perfect-matching.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-42/3/c/solution.md)
