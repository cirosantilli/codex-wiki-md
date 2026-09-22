<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Within the [risk set](../../../../../../../risk-set.md) $R_i$, the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md) makes the conditional failure probabilities proportional to $e^{\beta z_j}$. Thus

$$
\mathbb E_\beta[z_{\text{failing individual}}\mid\mathcal F_{x_i-},\text{one event at }x_i]
=\overline z_\beta(x_i)
=\frac{\sum_{j\in R_i}z_je^{\beta z_j}}{\sum_{j\in R_i}e^{\beta z_j}}.
$$

The [score function](../../../../../../../informant-function.md) sums observed minus expected covariates at event times. At a finite interior maximum of the [Cox partial likelihood](../../../../../../../cox-partial-likelihood.md),

$$
\boxed{\sum_{i:v_i=1}z_i=\sum_{i:v_i=1}\overline z_{\widehat\beta}(x_i).}
$$

The balance holds in aggregate, not separately at every event. The log [partial likelihood](../../../../../../../partial-likelihood.md) is concave because

$$
S''(\beta)=-\sum_{i:v_i=1}\operatorname{Var}_\beta(z\mid R_i)\leq0.
$$

When there is informative covariate variation in the [risk sets](../../../../../../../risk-set.md), this gives a unique finite solution if it exists. A completely separated event pattern can instead have its maximum only as $\beta\to\pm\infty$; the question's finite $\widehat\beta$ implicitly excludes that case.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
