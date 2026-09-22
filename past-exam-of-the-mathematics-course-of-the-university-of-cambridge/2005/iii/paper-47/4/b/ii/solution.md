<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each [bootstrap](../../../../../../../bootstrapping-statistics.md) replicate form the studentized pivot

$$
T^*=\frac{\widehat\theta^*-\widehat\theta}{\widehat s^*}.
$$

Let $t^*_{.025},t^*_{.975}$ be its empirical [quantiles](../../../../../../../quantile-function.md). The [bootstrap-t confidence interval](../../../../../../../bootstrap-t-confidence-interval.md) approximates

$$
\mathbb P\!\left(t^*_{.025}\leq\frac{\widehat\theta-\theta}{\widehat s}
\leq t^*_{.975}\right)\simeq0.95.
$$

Solving both inequalities for $\theta$ reverses the [quantile](../../../../../../../quantile-function.md) order, giving

$$
\boxed{[\widehat\theta-t^*_{.975}\widehat s,\quad
\widehat\theta-t^*_{.025}\widehat s].}
$$

Using the same fixed [standard error](../../../../../../../standard-error.md) in every [bootstrap](../../../../../../../bootstrapping-statistics.md) numerator would not implement this studentized procedure; each replicate needs its own $\widehat s^*$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
