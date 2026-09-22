# Cycle erasure in minimum-weight walks

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

If every nontrivial closed subwalk has strictly positive weight, removing any repeated-vertex segment strictly decreases a [walk](walk-in-a-graph.md)'s weight. Hence a minimum-weight walk must be a [graph path](path-in-a-graph.md), and it is a [shortest path](shortest-path.md). Strictly positive edge weights are sufficient in an undirected graph. For a [trail](trail-in-a-graph.md), positivity of every simple [cycle](permutation-cycle.md) is already sufficient: its first repeated-vertex segment is a cycle because no edge is repeated.

Under the usual unrestricted [walk](walk-in-a-graph.md) convention, positivity of simple cycles alone is insufficient. A graph consisting of one zero-weight edge $xy$ has no cycles, but the walk $x,y,x,y$ is a minimum-weight walk and is not a path. A zero-weight backtrack cannot be removed with a strict improvement. For nonnegative edge weights, one may erase such backtracks without increasing weight and obtain a shortest path, but cannot conclude that every minimum walk was already a path.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2017/7/c/solution.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2017/7/d/i/solution.md)
