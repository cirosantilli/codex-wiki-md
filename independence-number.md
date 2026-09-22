# Independence number

↑ **Parent:** [Independent set (graph theory)](independent-set-graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Independence_number)

The [independence number](independence-number.md) is the largest [cardinality](cardinality.md) of an [independent set](independent-set-graph-theory.md) in a finite [simple graph](simple-graph.md):

$$
\alpha(G)=\max\{|I|:I\subseteq V(G),\ I\text{ is an independent set of }G\}.
$$

It answers "how many mutually compatible objects can be selected at once?", while the [chromatic number](chromatic-number.md) asks how many compatible groups are needed for all the [vertices](vertex-graph-theory.md). Diestel uses this notation for a largest [independent set](independent-set-graph-theory.md).[Diestel, Graph Theory, Chapter 2, Exercise 23](https://diestel-graph-theory.com/Sample.pdf)

For the [cycle graph](cycle-graph.md) $C_5$, the [independent set](independent-set-graph-theory.md) $\{0,2\}$ shows that $\alpha(C_5)\geq2$. Three selected [vertices](vertex-graph-theory.md) would require at least three unselected [vertices](vertex-graph-theory.md) separating them around the [cycle graph](cycle-graph.md), which has only five [vertices](vertex-graph-theory.md). Thus $\alpha(C_5)=2$. There are five largest [independent sets](independent-set-graph-theory.md), obtained by rotating $\{0,2\}$ around the [cycle graph](cycle-graph.md), and five corresponding [minimum vertex covers](minimum-vertex-cover.md).

For the [complete bipartite graph](complete-bipartite-graph.md) $K_{2,3}$, an [independent set](independent-set-graph-theory.md) cannot contain a [vertex](vertex-graph-theory.md) from each side, since every such pair is joined by an [edge](edge-of-a-graph.md). The larger side has three [vertices](vertex-graph-theory.md), so $\alpha(K_{2,3})=3$. A [triangle in a graph](triangle-in-a-graph.md) has [independence number](independence-number.md) one. A [graph](graph-split.md) with no [edges](edge-of-a-graph.md) and $n$ [vertices](vertex-graph-theory.md) has [independence number](independence-number.md) $n$, including $\alpha(G)=0$ when $n=0$.

The complement correspondence between [vertex covers](vertex-cover.md) and [independent sets](independent-set-graph-theory.md) gives, with $n=|V(G)|$,

$$
\tau(G)+\alpha(G)=n.
$$

Every extra [vertex](vertex-graph-theory.md) that can be left in an [independent set](independent-set-graph-theory.md) is one fewer [vertex](vertex-graph-theory.md) needed in a [minimum vertex cover](minimum-vertex-cover.md). This identity holds for all finite [simple graphs](simple-graph.md), including the [triangle in a graph](triangle-in-a-graph.md) and the [cycle graph](cycle-graph.md) $C_5$; it does not require the [bipartite graph](bipartite-graph.md) hypothesis of [Kőnig's theorem for bipartite matching](konig-s-theorem-graph-theory.md).

For a nonempty [graph](graph-split.md), every [colour class](colour-class.md) of a [proper vertex colouring](proper-vertex-coloring.md) contains at most $\alpha(G)$ [vertices](vertex-graph-theory.md). Counting all the [vertices](vertex-graph-theory.md) therefore gives

$$
\chi(G)\geq\frac{|V(G)|}{\alpha(G)}.
$$

Since the [chromatic number](chromatic-number.md) is an [integer](integer.md), the bound rounds up: for the [cycle graph](cycle-graph.md) $C_5$, $\chi(C_5)\geq\lceil5/2\rceil=3$. It is attained by assigning colour $A$ to $0,2$, colour $B$ to $1,3$, and colour $C$ to $4$. All five [edges](edge-of-a-graph.md), including $40$, have differently coloured endpoints.

**Table of contents**

- [Caro-Wei bound](caro-wei-bound.md)
- [Triangle-free graph with sub-power independence number](triangle-free-graph-with-sub-power-independence-number.md)

## ↑ Ancestors (6)

1. [Independent set (graph theory)](independent-set-graph-theory.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Chromatic number of the half-density binomial random graph](chromatic-number-of-the-half-density-binomial-random-graph.md)
- [Circuit-cover bound by independence number](circuit-cover-bound-by-independence-number.md)
- [Cyclic stability of a digraph order](cyclic-stability-of-a-digraph-order.md)
- [Entropy weight of a graph cover](entropy-weight-of-a-graph-cover.md)
- [Independence number](independence-number.md)
- [Independent set (graph theory)](independent-set-graph-theory.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-14/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/17i/solution.md)
- [Strong product of graphs](strong-product-of-graphs.md)
- [Vertex cover number](vertex-cover-number.md)
