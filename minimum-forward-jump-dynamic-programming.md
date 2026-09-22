# Minimum forward-jump dynamic programming

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

For nonnegative maximum jump lengths in an [array](array-data-structure.md), let $D[0]=0$ and let unreachable positions have value $\infty$. Classifying a route to $j$ by its penultimate position proves this [dynamic programming recurrence](dynamic-programming-recurrence.md). Increasing $j$ is a valid dependency order because every jump advances. Scanning all previous positions uses $\Theta(n^2)$ [time complexity](time-complexity.md) and $\Theta(n)$ [space complexity](space-complexity.md). Store a minimizing predecessor to reconstruct a shortest route.

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms/6/d/solution.md)
