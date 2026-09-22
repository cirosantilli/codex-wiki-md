<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R(t^*)$ be the [risk set](../../../../../../risk-set.md) immediately before $t^*$, conditional on the preceding history. Only its members can experience the next event. In a short interval $[t^*,t^*+dt)$, the conditional probability that subject $j$ fails is $h_0(t^*)e^{\beta z_j}dt+o(dt)$, whereas the probability of one event from the [risk set](../../../../../../risk-set.md) is $h_0(t^*)\sum_{i\in R(t^*)}e^{\beta z_i}dt+o(dt)$. Dividing and taking the small-interval limit gives

$$
\boxed{P_\beta\{\pi(t^*)=j\mid\mathcal F_{t^*-},\text{one event}\}
=\frac{e^{\beta z_j}}{\sum_{i\in R(t^*)}e^{\beta z_i}},\qquad j\in R(t^*).}
$$

It is zero outside the [risk set](../../../../../../risk-set.md). The common [baseline hazard](../../../../../../baseline-hazard.md) cancels. This is the conditional event-label probability underlying the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md). Conditioning at an exact continuous event time is understood by this limiting conditional-intensity argument, rather than as division by the zero unconditional probability of an event at a fixed time. We use the standard simple event process with no simultaneous events and [independent censoring](../../../../../../independent-censoring.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
