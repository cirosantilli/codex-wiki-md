# Infinite walk criterion in a finite directed graph

↑ **Parent:** [Strongly connected component](strongly-connected-component.md)

A finite [directed graph](directed-graph.md) admits an infinite edge-following walk from $s$ exactly when a [directed cycle](directed-cycle.md) is reachable from $s$. An infinite walk repeats a [vertex](vertex-graph-theory.md) and therefore contains a reachable cycle; conversely, reach a cycle and repeat it. In a [strongly connected component](strongly-connected-component.md), a cycle exists precisely when the component has at least two vertices or is a singleton with a self-loop. Reachability followed by the [two-pass strongly connected component algorithm](two-pass-strongly-connected-component-algorithm.md) decides the criterion in $O(|V|+|E|)$ time.

The nonempty set of vertices visited infinitely often by a single infinite walk lies within one [strongly connected component](strongly-connected-component.md). For two such vertices, arbitrarily late visits supply directed walks in both directions. This set need not be the whole component: the walk can keep choosing one cycle and omit other vertices.

## ↑ Ancestors (7)

1. [Strongly connected component](strongly-connected-component.md)
2. [Directed graph](directed-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/6/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/6/d/solution.md)
