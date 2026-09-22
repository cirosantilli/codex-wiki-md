# Tree-graph moment bound for a percolation cluster

↑ **Parent:** [Percolation susceptibility](percolation-susceptibility.md)

For translation-invariant independent [bond percolation](bond-percolation-split.md) with finite [percolation susceptibility](percolation-susceptibility.md) $\chi=\sum_y\mathbb P(0\leftrightarrow y)$, the [BK inequality](van-den-berg-kesten-inequality.md) gives $\mathbb E|C_0|^k\le(2k-3)!!\chi^{2k-1}$ for $k\ge1$, with $(-1)!!=1$. Prune a connecting open [tree](tree-graph-theory.md) for the $k+1$ labelled vertices, suppress unmarked degree-two vertices, and split higher branching into binary branching with zero-length connections. There are $(2k-3)!!$ binary tree topologies and $2k-1$ connections. The connections have disjoint bond witnesses, so the [BK inequality](van-den-berg-kesten-inequality.md) bounds their joint [probability](probability.md) by a product of two-point connection [probabilities](probability.md). Summing successive leaves contributes $\chi$ for each connection. Since $(2k-3)!!\le2^{k-1}(k-1)!$, this proves $\mathbb E e^{t|C_0|}\le1-(2\chi)^{-1}\log(1-2t\chi^2)$ for $0<t<(2\chi^2)^{-1}$. Finite [percolation susceptibility](percolation-susceptibility.md) therefore gives an exponential cluster-volume tail.

## ↑ Ancestors (8)

1. [Percolation susceptibility](percolation-susceptibility.md)
2. [Bond percolation](bond-percolation-split.md)
3. [Percolation theory](percolation-theory.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15/2/i/solution.md)
