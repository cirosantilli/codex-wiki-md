<h1 id="ore-s-theorem">Ore's theorem</h1>

↑ **Parent:** [Hamiltonian graph](hamiltonian-graph.md)

[Ore's theorem](ore-s-theorem.md), named after [Øystein Ore](oystein-ore.md), says that a finite simple [graph](graph-split.md) with $n\geq3$ vertices is Hamiltonian if every nonadjacent pair has degree sum at least $n$.

For a proof, enlarge a hypothetical counterexample to an edge-maximal non-Hamiltonian graph. Adding a missing edge $uv$ creates a [Hamiltonian cycle](hamilton-cycle.md), hence the original graph has a Hamiltonian path $u=v_1,\ldots,v_n=v$. If both $uv_{i+1}$ and $vv_i$ are edges, the path closes to a cycle by reversing its final segment. Thus the index sets of these two kinds of edges are disjoint in $\{1,\ldots,n-1\}$, giving $d(u)+d(v)\leq n-1$, a contradiction. The degree condition is sufficient and need not follow from a lower bound of $n/2$ on every individual degree.

## ↑ Ancestors (10)

1. [Hamiltonian graph](hamiltonian-graph.md)
2. [Hamilton cycle](hamilton-cycle.md)
3. [Cycle graph](cycle-graph.md)
4. [Cycle in a graph](cycle-in-a-graph.md)
5. [Path in a graph](path-in-a-graph.md)
6. [Graph theory](graph-theory-split.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Ore's theorem](ore-s-theorem.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2011/r/r2/a/i/solution.md)
