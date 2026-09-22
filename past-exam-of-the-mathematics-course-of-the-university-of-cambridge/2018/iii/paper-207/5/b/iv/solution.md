<h1 id="5/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

In the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md), replace the number at risk in the [Nelson–Aalen estimator](../../../../../../../nelson-aalen-estimator.md) by the sum of relative hazards:

$$
W_\beta(u)=\sum_jY_j(u)e^{\beta z_j}.
$$

The total event [counting process](../../../../../../../counting-process.md) has conditional rate $W_\beta(u)h_0(u)$, so the estimated [baseline hazard](../../../../../../../baseline-hazard.md) increment is $dN(u)/W_{\widehat\beta}(u)$. Integrating gives the [Breslow estimator](../../../../../../../breslow-estimator.md)

$$
\boxed{\widehat H_0(t)=\sum_{i:x_i\leq t}\frac{v_i}{\sum_{j:x_j\geq x_i}e^{\widehat\beta z_j}}.}
$$

When $\widehat\beta=0$, all relative hazards are 1 and this reduces to the [Nelson–Aalen estimator](../../../../../../../nelson-aalen-estimator.md). The denominator is positive at each observed event time.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
