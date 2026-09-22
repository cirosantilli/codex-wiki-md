# Floyd-Warshall algorithm

↑ **Parent:** [Shortest path problem](shortest-path-problem-split.md)

The Floyd-Warshall algorithm computes all-pairs shortest [graph path](path-in-a-graph.md) lengths in a finite weighted [directed graph](directed-graph.md) with no negative-length [cycles in a graph](cycle-in-a-graph.md). Initialize $d_{ii}=0$, use the arc cost for each existing directed [edge](edge-of-a-graph.md), and use $+\infty$ when no arc exists. For $k=1,\ldots,n$, update every ordered pair $(i,j)$ by the displayed rule. The storage is $n^2$ lengths and the running time is $O(n^3)$.

For correctness, let $d_{ij}^{(k)}$ be the shortest simple [graph path](path-in-a-graph.md) length whose intermediate [vertices](vertex-graph-theory.md) lie among the first $k$. A shortest allowed [graph path](path-in-a-graph.md) either avoids $k$ or splits at its unique occurrence of $k$, giving the recurrence. Conversely, concatenate shortest paths through $k$ and remove any repeated-vertex sections; each such closed [walk](walk-in-a-graph.md) has nonnegative length, so removal cannot increase the length. This proves equality. The update can be performed in place because $d_{kk}=0$ and the $k$th row and column remain unchanged during stage $k$.

If negative-length [cycles in a graph](cycle-in-a-graph.md) are present, a shortest [walk](walk-in-a-graph.md) may not exist and the recurrence need not compute shortest simple [graph paths](path-in-a-graph.md). Two optimal subpaths can concatenate into a repeated-vertex [walk](walk-in-a-graph.md) with a negative cycle; deleting that cycle increases its length. A negative diagonal entry in the algorithm's final array detects this obstruction to finite shortest-walk distances.

## ↑ Ancestors (6)

1. [Shortest path problem](shortest-path-problem-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2007/s/3/c/solution.md)
