<h1 id="10f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [waiting time for a new record after a fixed sample](../../../../../../waiting-time-for-a-new-record-after-a-fixed-sample.md), given $U=F(Y_n)$, no overflow in the first $k$ subsequent years has [probability](../../../../../../probability.md) $U^k$. Averaging as in part (c) yields

$$
P(\tau>k)=n\int_0^1u^{n+k-1}\,du=\frac n{n+k},\qquad k\geq0.
$$

The [tail-sum formula for expectation](../../../../../../tail-sum-formula-for-expectation.md) therefore gives

$$
E\tau=\sum_{k=0}^\infty P(\tau>k)
=n\sum_{k=0}^\infty\frac1{n+k}=\infty.
$$

**The answer is $\boxed{E\tau=\infty}$.** This does not contradict almost-sure finiteness: the [tail probability](../../../../../../tail-probability.md) tends to zero, but too slowly for its sum to converge.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
