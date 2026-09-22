<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $a_1<a_2<\cdots$ be the distinct observed event times, $r_j$ the [risk set](../../../../../../../risk-set.md) size immediately before $a_j$, and $d_j$ the events there. Under [independent censoring](../../../../../../../independent-censoring.md), the [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md) is

$$
\boxed{\widehat F(t)=\prod_{a_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

It starts at one, jumps down at events, and is unchanged by a pure censoring time; [right censoring](../../../../../../../right-censoring.md) removes people from subsequent [risk sets](../../../../../../../risk-set.md). If events and censorings coincide, the convention here processes events before censoring, so those censored at the recorded time are included just before the event. The estimated [median](../../../../../../../median.md) is the first time the curve reaches or falls below $1/2$. If it never does during observation, the median is not estimable from the observed curve without tail assumptions.

With one remaining individual censored at $t_1$, no event factor is introduced. Hence

$$
\boxed{\phi_1=\phi_0.}
$$

This is the terminal observed step value. With an empty [risk set](../../../../../../../risk-set.md) after $t_1$, continued horizontal plotting is a convention and supplies no information about the true later [survivor function](../../../../../../../survival-function.md). The tail rests on one person and is imprecise; this is [terminal censoring and survival-mean identifiability](../../../../../../../terminal-censoring-and-survival-mean-identifiability.md). If $\phi_0>0$, the unrestricted mean cannot be obtained nonparametrically from this censored tail: extending the last positive step to infinity would give an infinite area, which does not establish an infinite population mean. A [restricted mean survival time](../../../../../../../restricted-mean-survival-time.md) up to a suitably supported finite cutoff remains estimable.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
