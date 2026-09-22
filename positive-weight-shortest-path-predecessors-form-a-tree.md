# Positive-weight shortest-path predecessors form a tree

↑ **Parent:** [Shortest-path tree](shortest-path-tree.md)

In a finite connected graph with strictly positive edge weights, choose any [shortest path](shortest-path.md) from a root $v$ to every other vertex $u$, and let $p(u)$ be its penultimate vertex. Every prefix is shortest: a better prefix followed by the final edge would give a cheaper walk, whose positive-weight cycles can be erased to give a cheaper path. Thus the displayed distance identity holds.

Following predecessors strictly decreases the shortest-path distance, so no predecessor cycle is possible. Since every nonroot vertex has a predecessor, every chain reaches the root. Opposite predecessor choices cannot select the same undirected edge, again by strict distance decrease. The selected graph is connected and has exactly one edge per nonroot vertex, so is a [spanning tree](spanning-tree.md). Along its root paths the distance differences telescope, proving that it is a [shortest-path tree](shortest-path-tree.md) even if the original shortest paths were chosen independently.

## ↑ Ancestors (7)

1. [Shortest-path tree](shortest-path-tree.md)
2. [Shortest path problem](shortest-path-problem-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2017/7/d/i/solution.md)
