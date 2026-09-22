# Bipartite four-cycle count

↑ **Parent:** [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)

If a [bipartite graph](bipartite-graph.md) with parts $X,Y$ has at least $\delta|X||Y|$ [edges](edge-of-a-graph.md), then the number of ordered tuples $(x_1,x_2,y_1,y_2)\in X^2\times Y^2$ for which every $x_iy_j$ is an edge is at least

$$
\delta^4|X|^2|Y|^2.
$$

Indeed, if $d(x_1,x_2)$ is the number of common neighbours of $x_1,x_2$ in $Y$, two applications of the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) give

$$
\sum_{x_1,x_2}d(x_1,x_2)^2
\geq\frac1{|X|^2}\left(\sum_y\deg(y)^2\right)^2
\geq\frac1{|X|^2|Y|^2}\left(\sum_y\deg(y)\right)^4.
$$

**Table of contents**

- [Bipartite four-cycle density](bipartite-four-cycle-density.md)

## ↑ Ancestors (7)

1. [Edge density of a bipartite graph](edge-density-of-a-bipartite-graph.md)
2. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-147/1/i/solution.md)
