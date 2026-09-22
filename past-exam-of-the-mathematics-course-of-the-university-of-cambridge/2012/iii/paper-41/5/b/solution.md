<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [frailty model](../../../../../../frailty-model.md) uses an unobserved nonnegative random [hazard multiplier](../../../../../../hazard-multiplier.md) to represent variation in individual risk. In a [proportional frailty model](../../../../../../proportional-frailty-model.md), conditional on $U=u$ the [cumulative hazard function](../../../../../../cumulative-hazard-function.md) is $uH_0(t)$, giving survivor $e^{-uH_0(t)}$. Averaging over the [frailty random variable](../../../../../../frailty-random-variable.md) by the [law of total probability](../../../../../../law-of-total-probability.md) yields

$$
\boxed{S(t)=\int_0^\infty e^{-uH_0(t)}g(u)\,du
=\widetilde g(H_0(t)),}
$$

the [Laplace transform](../../../../../../laplace-transform.md) of the frailty distribution evaluated at the baseline integrated hazard. This also applies to atoms by integration against the probability measure; the printed Dirac expression is not an ordinary continuous density.

In the given two-atom case, the [Dirac delta function](../../../../../../dirac-delta-function.md) notation assigns probabilities $1/4$ and $3/4$ to $U=4/7$ and $U=8/7$. These have mean one, fixing the frailty scale relative to the [baseline hazard](../../../../../../baseline-hazard.md). With $H_0(t)=7t/4$, the two conditional integrated hazards are $t$ and $2t$. Therefore

$$
\boxed{S(t)=\tfrac14e^{-t}+\tfrac34e^{-2t}=w(t).}
$$

The [frailty distribution among survivors](../../../../../../frailty-distribution-among-survivors.md) shifts toward the smaller multiplier $4/7$ over time, reproducing the declining population hazard and limit one without changing either individual's constant conditional hazard.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
