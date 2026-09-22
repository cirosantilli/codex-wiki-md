<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If the final individual experiences an event at $t_1$, the [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md) acquires the factor $1-1/1=0$. Thus

$$
\boxed{\phi_1=0.}
$$

The conventional fitted curve is zero thereafter. Its area gives the finite plug-in estimate

$$
\boxed{\widehat{\mathbb ET}_{\mathrm{KM}}=\int_0^{t_1}\widehat F(t)\,dt.}
$$

The area is a sum of rectangles: if $a_0=0<a_1<\cdots<a_m=t_1$ are the event times, it equals $\sum_{j=0}^{m-1}\widehat F(a_j)(a_{j+1}-a_j)$. Censoring times within a constant segment do not alter its area.

Both terminal estimates have poor reliability because the last [risk set](../../../../../../../risk-set.md) has size one: one observed outcome determines whether the entire remaining fitted tail stays positive or collapses to zero. The zero tail is an empirical endpoint convention, not evidence that every future member of the population must fail by $t_1$. With earlier [right censoring](../../../../../../../right-censoring.md), the displayed finite area can be especially sensitive to this last event and does not remove uncertainty about the population tail. In the final-censoring case the full mean lacks a determined tail area; in the final-event case the conventional full fitted mean is finite and calculable, but should be reported with this limitation. A [restricted mean survival time](../../../../../../../restricted-mean-survival-time.md) at a prespecified cutoff within reliable follow-up often avoids the unstable terminal extrapolation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
