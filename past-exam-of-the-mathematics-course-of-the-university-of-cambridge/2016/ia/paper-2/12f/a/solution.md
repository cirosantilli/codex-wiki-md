<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each unordered triple of distinct [vertices](../../../../../../vertex-graph-theory.md), let $I_A$ be the [indicator variable](../../../../../../indicator-variable.md) that its three [edges](../../../../../../edge-of-a-graph.md) are present. This is a [binomial random graph](../../../../../../binomial-random-graph.md), so edge independence gives $\mathbb E[I_A]=p^3$. The [triangle count in a binomial random graph](../../../../../../triangle-count-in-a-binomial-random-graph.md) is $T=\sum_A I_A$. There are $\binom n3$ such triples; all are triangles in the [complete graph](../../../../../../complete-graph.md).

**The combinatorial maximum and expectation are**

$$
\boxed{T_{\max}=\binom n3,\qquad \mathbb E[T]=\binom n3p^3.}
$$

The maximum is attainable with positive probability if $p>0$; for $p=0$, the [random variable](../../../../../../random-variable-split.md) is identically zero. The [linearity of expectation](../../../../../../linearity-of-expectation.md) requires no independence between different triangle indicators.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
