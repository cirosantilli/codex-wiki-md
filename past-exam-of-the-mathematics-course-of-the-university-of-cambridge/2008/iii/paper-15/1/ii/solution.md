<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), $\sum_i\beta_i\leq\sqrt{n\sum_i\beta_i^2}<\lambda$. The [total influence](../../../../../../total-influence.md) identity in part (i) therefore gives $\boxed{\sum_{S\ne\varnothing}|S|\alpha_S^2<\lambda/4}$.

The [Holder inequality](../../../../../../holder-inequality.md) gives $\sum_i\beta_i^{2/p}\leq n^{1-1/p}(\sum_i\beta_i^2)^{1/p}<\lambda^{2/p}n^{1-2/p}$. Substitute this into the [hypercontractive weighted influence bound](../../../../../../hypercontractive-weighted-influence-bound.md) and multiply by $\delta$ to obtain

$$
\sum_{S\ne\varnothing}|S|\delta^{|S|}\alpha_S^2<\frac\delta4\lambda^{2/p}n^{1-2/p}\leq\boxed{\frac14\lambda^{2/p}n^{1-2/p}},
$$

as required. The version with $\delta^{|S|-1}$ is slightly stronger and will also be useful below.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
