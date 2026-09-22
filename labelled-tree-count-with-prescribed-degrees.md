# Labelled tree count with prescribed degrees

↑ **Parent:** [Prüfer degree formula](prufer-degree-formula.md)

For $n\geq2$ and positive integers $d_1,\ldots,d_n$ with $\sum_v d_v=2(n-1)$, the number of [labelled trees](labelled-tree.md) having [vertex degree](degree-graph-theory.md) $d_v$ at label $v$ is

$$
\frac{(n-2)!}{\prod_{v=1}^n(d_v-1)!}.
$$

By the [Prüfer degree formula](prufer-degree-formula.md), this is the [multinomial coefficient](multinomial-coefficient.md) counting [sequences](sequence.md) with $d_v-1$ occurrences of each label. If a degree is zero or the sum is wrong, there are no such [trees](tree-graph-theory.md). For the example [degree sequence](degree-sequence.md) $(2,1,3,1,2,1)$, there are $4!/(1!0!2!0!1!0!)=12$ [labelled trees](labelled-tree.md), one for each ordering of the labels $1,3,3,5$. Knowing the [vertex degrees](degree-graph-theory.md) thus constrains, but usually does not determine, the [tree](tree-graph-theory.md).

## ↑ Ancestors (8)

1. [Prüfer degree formula](prufer-degree-formula.md)
2. [Prüfer sequence](prufer-sequence.md)
3. [Cayley's formula](cayley-s-formula.md)
4. [Tree (graph theory)](tree-graph-theory.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
