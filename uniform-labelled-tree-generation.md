# Uniform labelled tree generation

↑ **Parent:** [Prüfer sequence](prufer-sequence.md)

For $n\geq2$, choose $n-2$ [independent random variables](independent-random-variables.md), each with the [uniform distribution on a finite set](discrete-uniform-distribution.md) $\{1,\ldots,n\}$, and decode their values as a [Prüfer sequence](prufer-sequence.md). Every [sequence](sequence.md) has [probability](probability.md) $n^{-(n-2)}$, and the [bijection](bijection.md) gives each [labelled tree](labelled-tree.md) the same [probability](probability.md). This produces a [uniform spanning tree](uniform-spanning-tree.md) of the [complete graph](complete-graph.md) without repeatedly proposing sets of [edges](edge-of-a-graph.md) and rejecting those that fail to be [trees](tree-graph-theory-split.md). It supplies random inputs for testing implementations of [breadth-first search](breadth-first-search.md) and a tractable model of random connections. [Doron Zeilberger, Rutgers Math 454 (2020), Lecture 23: generate random labelled trees by sampling and inverting Prüfer codes](https://sites.math.rutgers.edu/~zeilberg/Combo20/hw.html)

This distribution is uniform over fixed-label [trees](tree-graph-theory-split.md), rather than over [unlabelled trees](unlabelled-tree.md). With four labels, the [star graph](star-graph-theory.md) shape has [probability](probability.md) $4/16=1/4$ and the [path graph](path-graph.md) shape has [probability](probability.md) $12/16=3/4$. Also, for a fixed label $v$, the [Prüfer degree formula](prufer-degree-formula.md) gives

$$
\deg_T(v)-1\sim\operatorname{Binomial}(n-2,1/n),
\qquad
\mathbb E[\deg_T(v)]=1+\frac{n-2}{n}=2-\frac2n.
$$

Here the [binomial distribution](binomial-distribution.md) counts the [independent](independent-random-variables.md) code positions equal to $v$. The [expected value](expected-value-split.md) agrees with the average [vertex degree](degree-graph-theory.md) from the [degree-sum formula](degree-sum-formula.md). Individual labels have the same distribution by symmetry, though their [vertex degrees](degree-graph-theory.md) are constrained together by their fixed sum. When $n=1$, simply return the single isolated [vertex](vertex-graph-theory.md).

## ↑ Ancestors (7)

1. [Prüfer sequence](prufer-sequence.md)
2. [Cayley's formula](cayley-s-formula.md)
3. [Tree (graph theory)](tree-graph-theory-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cayley's formula](cayley-s-formula.md)
