# Four-clique threshold in a binomial 3-uniform hypergraph

↑ **Parent:** [Binomial random hypergraph](binomial-random-hypergraph.md)

A complete three-[uniform hypergraph](uniform-hypergraph.md) on four [vertices](vertex-graph-theory.md) has four [edges](edge-of-a-graph.md). In the [binomial random hypergraph](binomial-random-hypergraph.md) $H^{(3)}(n,p)$, its count $X$ has [mean](expected-value-split.md) $\mu=\binom n4p^4$. If $np\to0$, the [first moment method](first-moment-method.md) gives $\mathbb P(X>0)\to0$. Two distinct four-sets have [independent](independent-random-variables.md) [clique](clique-graph-theory.md) indicators unless they share three [vertices](vertex-graph-theory.md); in that case their combined [edge set](edge-set.md) has seven triples. There are $O(n^5)$ such ordered pairs, so $\operatorname{Var}(X)\leq\mu+O(n^5p^7)$. Consequently $\operatorname{Var}(X)/\mu^2=O((np)^{-4}+(n^3p)^{-1})\to0$ if $np\to\infty$. The [second moment method](second-moment-method.md) then gives $\mathbb P(X>0)\to1$. These two implications establish the [threshold function](threshold-function.md).

## ↑ Ancestors (8)

1. [Binomial random hypergraph](binomial-random-hypergraph.md)
2. [Uniform hypergraph](uniform-hypergraph.md)
3. [Hypergraph](hypergraph-split.md)
4. [Graph theory](graph-theory-split.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2011/b/4/b/solution.md)
