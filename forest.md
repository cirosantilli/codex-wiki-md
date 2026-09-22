# Forest

↑ **Parent:** [Tree (graph theory)](tree-graph-theory-split.md)

A [forest](forest.md) is an [undirected graph](undirected-graph.md) with no [graph cycle](cycle-in-a-graph.md); each of its [connected components of a graph](component-graph-theory.md) is a [tree](tree-graph-theory-split.md), including any isolated [vertex](vertex-graph-theory.md). A finite [forest](forest.md) with $n$ [vertices](vertex-graph-theory.md) and $c$ [connected components of a graph](component-graph-theory.md) has

$$
|E|=n-c.
$$

Indeed, a [connected component of a graph](component-graph-theory.md) with $n_i$ [vertices](vertex-graph-theory.md) contributes $n_i-1$ [edges](edge-of-a-graph.md); adding these counts gives $n-c$. Equivalently, start with $n$ isolated [vertices](vertex-graph-theory.md): every added [edge](edge-of-a-graph.md) must join different [connected components of a graph](component-graph-theory.md), reducing their number by one. Joining [vertices](vertex-graph-theory.md) already connected would create a [graph cycle](cycle-in-a-graph.md). [MIT, counting notes, p. 4: building forests by merging components](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec05-06.pdf)

Deleting $13$ in our example gives $n=7$, $c=2$, and five [edges](edge-of-a-graph.md): the two [trees](tree-graph-theory-split.md) contribute $3+2=5=7-2$. Deleting $67$ as well leaves $7$ isolated, so $c=3$ and four [edges](edge-of-a-graph.md). A [forest](forest.md) therefore describes separate hierarchies or the intermediate stages of building a [spanning tree](spanning-tree.md). The [acyclic graph](forest.md) condition accounts for missing connections without assuming that all locations are mutually reachable.

**Table of contents**

- [Star forest](star-forest.md)
- [Two-component spanning forest](two-component-spanning-forest.md)
- [Minimum spanning forest](minimum-spanning-forest.md)
  - [Minimum-weight acyclic subgraph](minimum-weight-acyclic-subgraph.md)

## ↑ Ancestors (5)

1. [Tree (graph theory)](tree-graph-theory-split.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (51)

- [2-core of a graph](2-core-of-a-graph.md)
- [Acyclic orientation](acyclic-orientation.md)
- [Admissible crystallographic Coxeter graph](admissible-crystallographic-coxeter-graph.md)
- [Breadth-first search](breadth-first-search.md)
- [Bridges and connectivity in the 2-core](bridges-and-connectivity-in-the-2-core.md)
- [Coordinatewise minimum spanning-tree weight vector](coordinatewise-minimum-spanning-tree-weight-vector.md)
- [Cutset conditioning](cutset-conditioning.md)
- [Cycle cutset](cycle-cutset.md)
- [Depth-first search](depth-first-search.md)
- [Depth-first search parenthesis property](depth-first-search-parenthesis-property.md)
- [DFS lowpoint](dfs-lowpoint.md)
- [Disjoint-set forest](disjoint-set-forest.md)
- [Edge boundary of a finite forest in a regular tree](edge-boundary-of-a-finite-forest-in-a-regular-tree.md)
- [Forest](forest.md)
- [Forest polytope](forest-polytope.md)
- [Fractional support graph of a matching relaxation](fractional-support-graph-of-a-matching-relaxation.md)
- [Girth determines initial chromatic coefficients](girth-determines-initial-chromatic-coefficients.md)
- [Graphic matroid](graphic-matroid.md)
- [Kruskal's algorithm](kruskal-s-algorithm.md)
- [Kruskal's algorithm worked example](kruskal-s-algorithm-worked-example.md)
- [Kruskal safe edge](kruskal-safe-edge.md)
- [Labelled forest count with prescribed roots](labelled-forest-count-with-prescribed-roots.md)
- [Matroid](matroid.md)
- [Minimum spanning forest](minimum-spanning-forest.md)
- [Minimum-weight acyclic subgraph](minimum-weight-acyclic-subgraph.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms/3/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/3/c/iii/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/2/d/solution.md)
- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2010/a/1/c/solution.md)
- [Solution](past-exam-of-the-graph-theory-course-of-the-university-of-oxford/2023/2/c/solution.md)
- [Solution](past-exam-of-the-graph-theory-course-of-the-university-of-oxford/2023/2/d/solution.md)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/b/solution.md)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/d/solution.md)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-122/2/c/solution.md)
- [Solution](past-exam-of-the-probability-statistics-and-options-i-course-of-the-university-of-oxford/2007/r/1/x/solution.md)
- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2021/7/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/functional-programming-design-and-analysis-of-algorithms/7/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/functional-programming-design-and-analysis-of-algorithms/7/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/2/h/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/functional-programming-design-and-analysis-of-algorithms-resit/8/c/solution.md)
- [Skew-binary random-access list](skew-binary-random-access-list.md)
- [Star forest](star-forest.md)
