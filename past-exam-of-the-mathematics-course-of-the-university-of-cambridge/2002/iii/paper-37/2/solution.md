<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the numerical [competing risks](../../../../../competing-risks.md) update, the estimated probability of remaining event-free just before the tied time is

$$
\widehat S(7.8-)=1-0.285-0.241=0.474.
$$

There were no intervening events, so the [cumulative incidence functions](../../../../../cumulative-incidence-function.md) did not jump between the two stated times. The [Aalen–Johansen estimator](../../../../../aalen-johansen-estimator.md) uses the [risk set](../../../../../risk-set.md) immediately before the event time, including the subject censored at that same time under the usual events-before-censoring tie convention. Therefore the cause-$A$ increment is $0.474(2/20)$, and

$$
\boxed{\widehat F_A(7.8)=0.285+0.474\frac2{20}=0.3324.}
$$

For a consistency check, $\widehat F_B(7.8)=0.241+0.474/20=0.2647$ and $\widehat S(7.8)=0.474(1-3/20)=0.4029$; these sum to one. The censoring does not create an incidence jump and leaves $16$ subjects for subsequent follow-up. Dividing by $19$ would instead assume that the censored subject had already left before the event time, contrary to the stated immediately preceding [risk set](../../../../../risk-set.md). This is a [cumulative incidence update with tied censoring](../../../../../cumulative-incidence-update-with-tied-censoring.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
