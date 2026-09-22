<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $t_j$ be the distinct observed event times, with $r_j$ individuals at risk just before $t_j$ and $d_j$ events there. Parameterize the event-time distribution by the conditional failure probabilities $q_j=\mathbb P(T=t_j\mid T\geq t_j)$. Under [independent censoring](../../../../../independent-censoring.md), the survival part of the nonparametric [likelihood](../../../../../likelihood-function.md) groups into factors

$$
L(q)\propto\prod_j q_j^{d_j}(1-q_j)^{r_j-d_j}.
$$

An individual still under observation at $t_j$ contributes either a failure factor or a survival factor; later-censored individuals contribute the latter factors until censoring. Maximizing each factor independently gives $\widehat q_j=d_j/r_j$, including the boundary solutions when $d_j=0$ or $d_j=r_j$. Multiplying the conditional survival probabilities yields the [Kaplan–Meier estimator](../../../../../kaplan-meier-estimator.md)

$$
\boxed{\widehat F(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

The notation $F$ here denotes the [survivor function](../../../../../survival-function.md), as in the question. The estimator is constant between event times. Under the usual simultaneous-event convention, individuals censored at $t_j$ remain in its [risk set](../../../../../risk-set.md) while events are processed, and are then removed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
