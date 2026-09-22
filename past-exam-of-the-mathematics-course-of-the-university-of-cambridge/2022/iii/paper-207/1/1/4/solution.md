<h1 id="1/1/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $G$ be the genetic instrument, $X$ vitamin-D concentration, $U$ an unmeasured cause of vitamin D and mortality, and $Y$ mortality. The [causal directed acyclic graph](../../../../../../../causal-directed-acyclic-graph.md) contains

$$
G\longrightarrow X\longleftarrow U\longrightarrow Y.
$$

Although $G$ and $U$ are marginally independent, $X$ is a [collider](../../../../../../../collider.md). Conditioning on $X$ opens the path $G\leftrightarrow U\to Y$, violating [instrumental-variable independence](../../../../../../../instrumental-variable-independence.md) within the resulting strata. [Residual exposure stratification](../../../../../../../residual-exposure-stratification.md) instead removes the component of $X$ predicted by $G$ before stratification; under the additive first-stage model, the stratifying variable is no longer caused by $G$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
