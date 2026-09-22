<h1 id="boruvka-s-algorithm">Borůvka's algorithm</h1>

↑ **Parent:** [Minimum spanning tree](minimum-spanning-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borůvka's_algorithm)

Start with isolated [vertices](vertex-graph-theory.md). In each round, determine the current [connected components of a graph](component-graph-theory.md), choose a least-weight outgoing [edge](edge-of-a-graph.md) for each component, add their union, and recompute the components. With distinct weights, each chosen edge is the unique lightest edge across that component's [graph cut](graph-cut.md). The [minimum spanning tree cut property](minimum-spanning-tree-cut-property.md) puts every such edge in every [minimum spanning tree](minimum-spanning-tree.md), so the selected edges remain acyclic. Every nonfinal component has an outgoing edge in a connected input, and merging makes progress until a [spanning tree](spanning-tree.md) remains. Duplicate choices of the same edge are one set insertion.

Each new component contains at least two old components, so there are $O(\log |V|)$ rounds. Scanning all edges per round gives $O(|E|\log |V|)$ time. Equal edge weights require a consistent secondary order to avoid choosing a cycle of tied edges.

[Otakar Borůvka](otakar-boruvka.md) formulated the distinct-cost minimum-connection problem in 1926.[pp. 37–38, opening formulation with positive distinct connection costs](o-jistem-problemu-minimalnim-by-otakar-boruvka.md)

## ↑ Ancestors (7)

1. [Minimum spanning tree](minimum-spanning-tree.md)
2. [Spanning tree](spanning-tree.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Otakar Borůvka](otakar-boruvka.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/7/e/solution.md)
