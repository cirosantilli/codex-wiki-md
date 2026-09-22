<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The ordinary [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) adds $d_j/r_j$ at event time $t_j$. Under a fitted [proportional hazards model](../../../../../../proportional-hazards-model.md), replace the number at risk by the sum of fitted [hazard multipliers](../../../../../../hazard-multiplier.md):

$$
\widehat H_0(t)=\sum_{t_j\leq t}\frac{d_j}{\sum_{i\in R(t_j)}\widehat\phi_i}.
$$

This is the [Breslow estimator](../../../../../../breslow-estimator.md) of the integrated [baseline hazard](../../../../../../baseline-hazard.md), using fitted [regression coefficients](../../../../../../regression-coefficient.md) obtained by maximizing the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md). The denominator arises because the total event intensity is $h_0(t)\sum_{i\in R(t)}\phi_i$; with every multiplier equal to one it reduces to the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md).

The estimator is right-continuous, so $\widehat H_0(t_a)$ already includes the event at $t_a$. Subtracting it leaves only the events at $t_c$ and $t_d$, whose [risk sets](../../../../../../risk-set.md) are $\{c,d\}$ and $\{d\}$. Hence

$$
\boxed{\widehat H_0(t_d)-\widehat H_0(t_a)=\frac1{\widehat\phi_c+\widehat\phi_d}+\frac1{\widehat\phi_d}.}
$$

There is no increment at the censoring time $t_b$. If the lower endpoint had instead been $t_a-$, an additional $1/(\widehat\phi_a+\widehat\phi_b+\widehat\phi_c+\widehat\phi_d)$ would be present. The final singleton event can increase the [baseline hazard](../../../../../../baseline-hazard.md) estimate even though its [partial likelihood](../../../../../../partial-likelihood.md) contribution is one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
