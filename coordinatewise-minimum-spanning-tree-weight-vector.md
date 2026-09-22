# Coordinatewise minimum spanning-tree weight vector

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)

Sort the [edge weights](edge-weight.md) of a [minimum spanning tree](minimum-spanning-tree.md) $T$ and of any [spanning tree](spanning-tree.md) $S$ in nondecreasing order. Then $w_i(T)\leq w_i(S)$ for every position. To prove it, fix a threshold $t$ and retain the graph's edges of weight at most $t$. If this graph has $c$ [connected components](connected-component.md), $T$ contains a [spanning forest](spanning-forest.md) of each component using those edges: otherwise a light edge joining two of its pieces could replace an edge heavier than $t$ on its tree path, decreasing total weight. Hence exactly $|V|-c$ edges of $T$ have weight at most $t$. No other [spanning tree](spanning-tree.md) can have more, since its retained edges form a [forest](forest.md) inside those components. These threshold counts imply the coordinatewise inequality for sorted weights.

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/8/c/ii/solution.md)
