# Two-pass strongly connected component algorithm

↑ **Parent:** [Strongly connected component](strongly-connected-component.md)

Run [depth-first search](depth-first-search.md) on a finite [directed graph](directed-graph.md), then search its [graph transpose](graph-transpose.md) in decreasing first-pass finish order, marking [vertices](vertex-graph-theory.md) permanently during the second pass. Each second-pass search tree is one [strongly connected component](strongly-connected-component.md). The component finish-order property ensures that the next search cannot enter another still-unassigned component in the [graph transpose](graph-transpose.md); mutual reachability ensures that it reaches every [vertex](vertex-graph-theory.md) in its own component. Two traversals and transposition take $O(|V|+|E|)$ time.

## ↑ Ancestors (7)

1. [Strongly connected component](strongly-connected-component.md)
2. [Directed graph](directed-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Infinite walk criterion in a finite directed graph](infinite-walk-criterion-in-a-finite-directed-graph.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms/8/e/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/6/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit/7/b/solution.md)
