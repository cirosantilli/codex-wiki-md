<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $I_{ij}$ be the [indicator random variable](../../../../../../../indicator-random-variable.md) that the unordered [vertex](../../../../../../../vertex-graph-theory.md) pair $\{i,j\}$ has no [common neighbour](../../../../../../../common-neighbour.md). For each of the other $n-2$ [vertices](../../../../../../../vertex-graph-theory.md), the two required [edges](../../../../../../../edge-of-a-graph.md) are both present with probability $p^2$. The edge pairs for different candidate neighbours are disjoint sets of independent random choices. Thus $\mathbb E I_{ij}=(1-p^2)^{n-2}$. [Linearity of expectation](../../../../../../../linearity-of-expectation.md) yields

$$
\boxed{\mathbb E X=\binom n2(1-p^2)^{n-2}},
$$

the [missing common-neighbour count in a binomial random graph](../../../../../../../missing-common-neighbour-count-in-a-binomial-random-graph.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 36](../../../../paper-36-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
