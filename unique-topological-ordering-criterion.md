# Unique topological ordering criterion

↑ **Parent:** [Topological sorting](topological-sorting.md)

A finite nonempty [Directed acyclic graph](directed-acyclic-graph.md) has a unique [topological sort](topological-sorting.md) exactly when it has a [Hamiltonian path](hamiltonian-path.md). A [Hamiltonian path](hamiltonian-path.md) forces the relative order of every consecutive pair and therefore of all [vertices](vertex-graph-theory.md). Conversely, in a unique [topological sort](topological-sorting.md), every consecutive pair must have a forward edge: if such an edge were absent, swapping that adjacent pair would preserve all edge constraints and produce a second [topological sort](topological-sorting.md). The consecutive edges give a [Hamiltonian path](hamiltonian-path.md). Consequently one may compute any [topological sort](topological-sorting.md) and test its consecutive edges, taking $O(n^2)$ time on an [adjacency matrix](adjacency-matrix.md) representation.

## ↑ Ancestors (6)

1. [Topological sorting](topological-sorting.md)
2. [Directed acyclic graph](directed-acyclic-graph.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/functional-programming-design-and-analysis-of-algorithms/6/d/solution.md)
