# Junction tree algorithm

↑ **Parent:** [Junction tree](junction-tree.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Junction_tree_algorithm)

The junction tree algorithm performs exact inference in a finite [probabilistic graphical model](probabilistic-graphical-model.md). First moralize a [Bayesian network](bayesian-network.md) if necessary; then apply [triangulation of an undirected graph](triangulation-of-an-undirected-graph.md), organize its [maximal cliques](maximal-clique.md) into a [junction tree](junction-tree.md), and assign each original factor to one containing clique. Inward and outward [junction-tree sum-product messages](junction-tree-sum-product-message.md) compute the [normalizing constant](normalizing-constant.md) and [marginal distributions](marginal-distribution.md). Its cost depends exponentially on the largest clique's number of variables, rather than necessarily on the total number of variables.

## ↑ Ancestors (7)

1. [Junction tree](junction-tree.md)
2. [Probabilistic graphical model](probabilistic-graphical-model.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-39/3/f/solution.md)
