# Forest

↑ **Parent:** [Tree (graph theory)](tree-graph-theory.md)

A [forest](forest.md) is an [undirected graph](undirected-graph.md) with no [graph cycle](cycle-in-a-graph.md); each of its [connected components of a graph](component-graph-theory.md) is a [tree](tree-graph-theory.md), including any isolated [vertex](vertex-graph-theory.md). A finite [forest](forest.md) with $n$ [vertices](vertex-graph-theory.md) and $c$ [connected components of a graph](component-graph-theory.md) has

$$
|E|=n-c.
$$

Indeed, a [connected component of a graph](component-graph-theory.md) with $n_i$ [vertices](vertex-graph-theory.md) contributes $n_i-1$ [edges](edge-of-a-graph.md); adding these counts gives $n-c$. Equivalently, start with $n$ isolated [vertices](vertex-graph-theory.md): every added [edge](edge-of-a-graph.md) must join different [connected components of a graph](component-graph-theory.md), reducing their number by one. Joining [vertices](vertex-graph-theory.md) already connected would create a [graph cycle](cycle-in-a-graph.md). [MIT, counting notes, p. 4: building forests by merging components](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec05-06.pdf)

Deleting $13$ in our example gives $n=7$, $c=2$, and five [edges](edge-of-a-graph.md): the two [trees](tree-graph-theory.md) contribute $3+2=5=7-2$. Deleting $67$ as well leaves $7$ isolated, so $c=3$ and four [edges](edge-of-a-graph.md). A [forest](forest.md) therefore describes separate hierarchies or the intermediate stages of building a [spanning tree](spanning-tree.md). The [acyclic graph](forest.md) condition accounts for missing connections without assuming that all locations are mutually reachable.

**Table of contents**

- [Two-component spanning forest](two-component-spanning-forest.md)

## ↑ Ancestors (5)

1. [Tree (graph theory)](tree-graph-theory.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Admissible crystallographic Coxeter graph](admissible-crystallographic-coxeter-graph.md)
- [Breadth-first search](breadth-first-search.md)
- [Depth-first search](depth-first-search.md)
- [DFS lowpoint](dfs-lowpoint.md)
- [Edge boundary of a finite forest in a regular tree](edge-boundary-of-a-finite-forest-in-a-regular-tree.md)
- [Forest](forest.md)
- [Labelled forest count with prescribed roots](labelled-forest-count-with-prescribed-roots.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-122/2/c/solution.md)
