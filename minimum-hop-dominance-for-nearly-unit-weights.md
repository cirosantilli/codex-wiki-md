# Minimum-hop dominance for nearly unit weights

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

For a graph on $n$ vertices with all edge weights in $[1,1+1/n]$, every minimum-weight [shortest path](shortest-path.md) has the smallest possible number of edges. Indeed, positivity permits a simple optimum, and a simple $r$-edge path weighs at most $r+r/n<r+1$ for $r\leq n-1$, while any path with more edges weighs at least $r+1$. A [breadth-first search](breadth-first-search.md) followed by weighted [dynamic programming](dynamic-programming.md) along increasing-hop edges therefore solves the single-source problem in $O(|V|+|E|)$ time. Choosing an arbitrary breadth-first tree alone is insufficient: equal-hop routes may still have different weights.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/5/c/solution.md)
