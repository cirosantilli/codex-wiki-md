<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If some choice $\omega$ produced a [graph](../../../../../../graph-split.md) with [largest component of a graph](../../../../../../largest-component-of-a-graph.md) smaller than $2n/3$, the [balanced component cut](../../../../../../balanced-component-cut.md) result with packing parameter one would give an empty [graph cut](../../../../../../graph-cut.md) whose sides both have at least $n/3$ [vertices](../../../../../../vertex-graph-theory.md). For any fixed such vertex [set partition](../../../../../../set-partition.md), a uniform [edge](../../../../../../edge-of-a-graph.md) of the [complete graph](../../../../../../complete-graph.md) crosses with [probability](../../../../../../probability.md)

$$
q=\frac{2|V_1||V_2|}{n(n-1)}\geq\frac49.
$$

To avoid crossing in row $i$, at least one of its $k$ offered [edges](../../../../../../edge-of-a-graph.md) must be noncrossing. The row's [probability](../../../../../../probability.md) is $1-q^k\leq1-(4/9)^k$. The rows consist of [independent random variables](../../../../../../independent-random-variables.md), so at $m=cn$ a [union bound](../../../../../../boole-s-inequality.md) over at most $2^n$ vertex [set partitions](../../../../../../set-partition.md) gives

$$
\mathbb P(\exists\omega:\ L_1(G_\omega)<2n/3)
\leq 2^n[1-(4/9)^k]^{cn}.
$$

For example, the positive integer

$$
\boxed{c_k=\left\lceil\frac{\log2+1}{-\log[1-(4/9)^k]}\right\rceil}
$$

makes this bound at most $e^{-n}$. Therefore **every choice has a component of order at least $2n/3$, with probability tending to one**. The [simultaneous giant for fixed random-edge choice](../../../../../../simultaneous-giant-for-fixed-random-edge-choice.md) estimate includes choices made after seeing the entire array; it does not assume a particular online selection rule.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
