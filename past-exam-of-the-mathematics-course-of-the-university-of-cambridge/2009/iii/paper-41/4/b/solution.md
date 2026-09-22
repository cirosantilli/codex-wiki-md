<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the usual cohort setup: all individuals enter at time zero, each contributes one event or [censoring](../../../../../../censoring-statistics.md) time, and every such observation is included. Order these distinct observation times as $t_1<\cdots<t_m$. The [risk set](../../../../../../risk-set.md) size just before $t_k$ is then $r_k=m-k+1$. Write $\delta_k=1$ for an event and zero for [censoring](../../../../../../censoring-statistics.md). Including the jump at an event time, the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) is

$$
\widehat H_j=\sum_{k=1}^{j}\frac{\delta_k}{m-k+1}.
$$

Exchange the two finite sums:

$$
\sum_{j=1}^{m}\widehat H_j
=\sum_{k=1}^{m}\frac{\delta_k}{m-k+1}\sum_{j=k}^{m}1
=\sum_{k=1}^{m}\delta_k.
$$

Thus **the sum equals the number of observed events**. Each event increment appears once for each individual still at risk at that event, exactly cancelling its denominator. This is the [event-count identity for Nelson–Aalen cumulative hazards](../../../../../../event-count-identity-for-nelson-aalen-cumulative-hazards.md). The cohort and entry convention matter: delayed entry would invalidate the simple equation $r_k=m-k+1$ and require a modified identity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
