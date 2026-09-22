<h1 id="kruskal-s-algorithm">Kruskal's algorithm</h1>

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kruskal's_algorithm)

[Kruskal's algorithm](kruskal-s-algorithm.md) constructs a [minimum spanning tree](minimum-spanning-tree.md) of a finite [connected graph](connected-graph.md) with undirected [edges](edge-of-a-graph.md) and real [edge](edge-of-a-graph.md) weights. Start with all [vertices](vertex-graph-theory.md) and no [edges](edge-of-a-graph.md), a [forest](forest.md) of isolated [vertices](vertex-graph-theory.md). Sort the [edges](edge-of-a-graph.md) by nondecreasing weight, then accept an [edge](edge-of-a-graph.md) exactly when its endpoints belong to different current [connected components of a graph](component-graph-theory.md). Otherwise reject it: the existing [graph path](path-in-a-graph.md) between its endpoints would close a [graph cycle](cycle-in-a-graph.md). Each acceptance merges two [connected components of a graph](component-graph-theory.md). Stop after $|V|-1$ acceptances, when the [forest](forest.md) has become one [spanning tree](spanning-tree.md).

This is a [greedy algorithm](greedy-algorithm.md) for economical network connection: only the next affordable connection and the current [connected components of a graph](component-graph-theory.md) matter. Unlike [Prim's algorithm](prim-s-algorithm.md), which grows one reached [tree](tree-graph-theory-split.md), [Kruskal's algorithm](kruskal-s-algorithm.md) can grow several separate [trees](tree-graph-theory-split.md) before joining them. The essential safeguard is avoiding a [graph cycle](cycle-in-a-graph.md), rather than simply buying the cheapest fixed number of [edges](edge-of-a-graph.md).

[Joseph Bernard Kruskal](joseph-bernard-kruskal.md) described this rule as Construction A on page 49 of his February 1956 paper, [On the shortest spanning subtree of a graph and the traveling salesman problem](https://www.ams.org/journals/proc/1956-007-01/S0002-9939-1956-0078686-7/S0002-9939-1956-0078686-7.pdf); page 50 gives an exchange argument for distinct weights.[Joseph B. Kruskal, Jr., Proceedings of the American Mathematical Society 7(1), February 1956, pp. 48–50; inspected scan, Construction A and final exchange argument](https://langevin.univ-tln.fr/cours/graphe/bonus/Krukskal.pdf)

**Table of contents**

- [Kruskal's algorithm worked example](kruskal-s-algorithm-worked-example.md)
- [Kruskal safe edge](kruskal-safe-edge.md)
- [Kruskal component merging](kruskal-component-merging.md)

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Disjoint-set data structure](disjoint-set-data-structure.md)
- [Kruskal's algorithm](kruskal-s-algorithm.md)
- [Minimum spanning forest](minimum-spanning-forest.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/3/solution.md)
