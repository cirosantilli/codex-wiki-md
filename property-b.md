# Property B

↑ **Parent:** [Hypergraph colouring](hypergraph-colouring.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Property_B)

A [hypergraph](hypergraph-split.md) has [Property B](property-b.md) if its [vertices of a hypergraph](vertex-of-a-hypergraph.md) can be coloured with two colours so that every [hypergraph edge](edge-of-a-hypergraph.md) meets both [colour classes](colour-class.md). An $r$-[uniform hypergraph](uniform-hypergraph.md) with fewer than $2^{r-1}$ [edges](edge-of-a-graph.md) has [Property B](property-b.md), by a fair [independent](independent-random-variables.md) colouring and the [union bound](boole-s-inequality.md). Conversely, for $r\geq2$, take $N=2r^2$ vertices and independently sample $m=\lceil(N\log2+1)2^r\rceil$ uniformly random $r$-subsets. In any fixed colouring an [edge](edge-of-a-graph.md) is [monochromatic](monochromatic-set.md) with [probability](probability.md) at least $2^{-r}$: [convexity](convex-function.md) of [binomial coefficients](binomial-coefficient.md) reduces to the balanced colouring, and $\binom{r^2}{r}/\binom{2r^2}{r}\geq2^{-r-1}$. The [union bound](boole-s-inequality.md) over $2^N$ colourings gives a [probability](probability.md) at most $2^N e^{-m2^{-r}}<1$ of any proper colouring. Removing repeated [edges](edge-of-a-graph.md) leaves a [hypergraph](hypergraph-split.md) without [Property B](property-b.md) and with $O(r^22^r)$ [edges](edge-of-a-graph.md).

**Table of contents**

- [Bipartite three-uniform hypergraph](bipartite-three-uniform-hypergraph.md)

## ↑ Ancestors (7)

1. [Hypergraph colouring](hypergraph-colouring.md)
2. [Hypergraph](hypergraph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Fano-plane Turán theorem](fano-plane-turan-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11/4/solution.md)
- [Property B](property-b.md)
