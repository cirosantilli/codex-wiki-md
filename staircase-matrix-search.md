# Staircase matrix search

↑ **Parent:** [Search algorithm](search-algorithm.md)

Search a matrix whose rows and columns are both nondecreasing by inspecting the top-right corner of the remaining rectangle. If that value is below the target, discard its row; if above, discard its column; if equal, return its coordinates. The [loop invariant](loop-invariant.md) retains every possible match inside the rectangle. Each failure decreases its remaining height plus width by one, proving at most $n+m-1$ inspections for positive dimensions and constant [auxiliary space](auxiliary-space.md). Row monotonicity alone is insufficient for the column exclusion.

## ↑ Ancestors (4)

1. [Search algorithm](search-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Monotone matrix](monotone-matrix.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/imperative-programming-resit/2/d/solution.md)
