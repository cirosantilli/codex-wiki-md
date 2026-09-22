# Bellman-Ford algorithm

↑ **Parent:** [Shortest path problem](shortest-path-problem.md)

For an all-to-one [shortest path problem](shortest-path-problem.md) with root $r$, initialize $d_r^{(0)}=0$ and all other labels to infinity. Set $d_i^{(k)}=\min(d_i^{(k-1)},\min_{(i,j)\in A}\{c_{ij}+d_j^{(k-1)}\})$, keeping the root at zero. Induction identifies the labels with the shortest [directed paths](directed-path.md) using at most $k$ [directed edges](directed-edge.md). Without a reachable negative [directed cycle](directed-cycle.md), $|V|-1$ rounds suffice after removing [directed cycles](directed-cycle.md) from a shortest walk. In-place or queue variants repeatedly relax incoming [directed edges](directed-edge.md) to an improved label. Labels may decrease multiple times, so this is a [label-correcting shortest-path algorithm](label-correcting-shortest-path-algorithm.md).

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Label-correcting shortest-path algorithm](label-correcting-shortest-path-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-31/4/solution.md)
