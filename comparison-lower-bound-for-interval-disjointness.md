# Comparison lower bound for interval disjointness

↑ **Parent:** [Algorithm](algorithm-split.md)

Deciding whether $n$ open real intervals are pairwise disjoint has comparison complexity $\Theta(n\log n)$. Sort by left endpoint and scan the maximum previous right endpoint for the upper bound. For the lower bound, map integer keys $z_i$ to $(2z_i,2z_i+1)$. Such intervals intersect exactly when the original integers agree. Each comparison between endpoints $2z_i+a$ and $2z_j+b$, with $a,b\in\{0,1\}$, is determined by a comparison of $z_i,z_j$ and their fixed offsets, so the reduction preserves the [comparison model](comparison-model.md). Apply the [element distinctness problem](element-distinctness-problem.md) lower bound.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
