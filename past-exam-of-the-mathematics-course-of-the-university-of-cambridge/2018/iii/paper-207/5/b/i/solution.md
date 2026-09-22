<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $R_i=\{j:x_j\geq x_i\}$ be the [risk set](../../../../../../../risk-set.md) at an observed event time $x_i$. In the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md), conditional on one member of this set failing then and on the preceding history, the probability that it is individual $i$ is

$$
\frac{e^{\beta z_i}h_0(x_i)}{\sum_{j\in R_i}e^{\beta z_j}h_0(x_i)}
=\frac{e^{\beta z_i}}{\sum_{j\in R_i}e^{\beta z_j}}.
$$

The [baseline hazard](../../../../../../../baseline-hazard.md) cancels. Multiplying these conditional contributions gives the [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md)

$$
\boxed{L_p(\beta)=\prod_{i:v_i=1}\frac{e^{\beta z_i}}{\sum_{j:x_j\geq x_i}e^{\beta z_j}}.}
$$

The no-ties assumption avoids the need for a tied-event approximation. This construction assumes [independent censoring](../../../../../../../independent-censoring.md) conditional on the modelled covariates. The printed phrase calling $z$ a scalar parameter is read as a scalar observed covariate $z_i$; $\beta$ is the unknown regression parameter.

## ↑ Ancestors (12)

1. [I](../i.md)
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
