<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the product-limit estimate in (b). Between consecutive event times there are no mortality jumps, so

$$
\frac{d\widehat F_E(t)}{dt}=\overline h_B(t)\widehat F_E(t).
$$

Thus **the estimated relative survivor curve rises between events** when background mortality is positive, and is constant if it is zero. [Censoring](../../../../../../censoring-statistics.md) changes the [risk set](../../../../../../risk-set.md) and can change the slope, but supplies no downward event jump. At the next event time the curve is multiplied by $1-d_k/r_k$.

Provided the curve is still positive, the ratio of the post-event estimates at the two consecutive event times is

$$
\frac{\widehat F_E(t_k)}{\widehat F_E(t_j)}
=\exp\left[\int_{t_j}^{t_k}\overline h_B(u)\,du\right]
\left(1-\frac{d_k}{r_k}\right).
$$

For $d_k<r_k$, the later value is larger precisely when

$$
\boxed{\int_{t_j}^{t_k}\overline h_B(u)\,du>
-\log\left(1-\frac{d_k}{r_k}\right).}
$$

For example, suppose there are 100 individuals in the [risk set](../../../../../../risk-set.md) after the earlier event, no intervening [censoring](../../../../../../censoring-statistics.md), a 20-day gap, and one death at its end. If every [background hazard](../../../../../../background-hazard.md) is $0.001$ per day, then the integrated background contribution is $0.02$ and

$$
\frac{\widehat F_E(t_k)}{\widehat F_E(t_j)}=e^{0.02}(1-1/100)\simeq1.010>1.
$$

The individual [background hazards](../../../../../../background-hazard.md) are small, but the interval contains less observed mortality than expected from that background. This can occur by chance in a small event sample or when the cohort is healthier than the life-table reference on other dimensions.

A nonnegative true [excess hazard](../../../../../../excess-hazard.md) makes $F_E$ nonincreasing, but this unconstrained [estimator](../../../../../../estimator.md) need not inherit that restriction. An increase is therefore not proof of a clinical survival benefit. If the exponential cumulative-hazard version is chosen instead, its corresponding condition is $\int_{t_j}^{t_k}\overline h_B>d_k/r_k$; the qualitative explanation remains the same. If the [risk set](../../../../../../risk-set.md) is exhausted by deaths, the product-limit factor is zero and no later increase is possible.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
