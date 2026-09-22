<h1 id="tree-component-expectation-in-the-erdos-renyi-model">Tree-component expectation in the Erdős-Rényi model</h1>

↑ **Parent:** [Erdős-Rényi model](erdos-renyi-model.md)

For $X_j$ the number of [tree components](tree-component.md) of order $j$ in a [binomial random graph](binomial-random-graph.md), choose their [vertices](vertex-graph-theory.md), choose one of $j^{j-2}$ labelled [trees](tree-graph-theory.md) by the [Cayley formula](cayley-s-formula.md), require its $j-1$ [edges](edge-of-a-graph.md), and exclude both the remaining internal [edges](edge-of-a-graph.md) and all crossing [edges](edge-of-a-graph.md). For $j=1$ interpret $j^{j-2}=1$, recovering the [isolated vertex](isolated-vertex.md) count. If $p=\lambda/n$ for fixed positive $\lambda$ and $j=O(\log n)$, the [Stirling formula](stirling-formula.md) gives $\mathbb EX_j\sim n(\lambda e^{1-\lambda})^j/(\lambda\sqrt{2\pi}\,j^{5/2})$. Distinct overlapping vertex sets cannot both be [graph components](component-graph-theory.md); for disjoint sets their joint occurrence gains the factor $(1-p)^{-j^2}$ relative to the product, because their between-set [edges](edge-of-a-graph.md) must be absent only once.

**Table of contents**

- [Fixed-order tree-component window](fixed-order-tree-component-window.md)

## ↑ Ancestors (7)

1. [Erdős-Rényi model](erdos-renyi-model.md)
2. [Random graph](random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/3/ii/solution.md)
- [Rooted-tree generating function](rooted-tree-generating-function.md)
- [Sharp subcritical largest-component scale](sharp-subcritical-largest-component-scale.md)
