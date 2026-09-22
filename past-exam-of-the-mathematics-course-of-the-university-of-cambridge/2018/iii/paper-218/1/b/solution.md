<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $r=1,\ldots,16$ for rats and $j$ for repeated observations. With diet 1 as the [reference level in a regression factor](../../../../../../reference-level-in-a-regression-factor.md), the [random-intercept linear mixed model](../../../../../../random-intercept-linear-mixed-model.md) is

$$
Y_{rj}=\beta_0+\beta_Tt_{rj}+\beta_2\mathbf1_{\{D_r=2\}}+\beta_3\mathbf1_{\{D_r=3\}}+b_r+\varepsilon_{rj},
\qquad b_r\overset{\mathrm{iid}}\sim N(0,\tau^2),\quad\varepsilon_{rj}\overset{\mathrm{iid}}\sim N(0,\sigma^2),
$$

with the two families of [normal distributions](../../../../../../normal-distribution.md) independent and the covariates treated as fixed. The reported estimates are

$$
\boxed{(\widehat\beta_0,\widehat\beta_T,\widehat\beta_2,\widehat\beta_3)=(244.06890,\,0.58568,\,220.98864,\,262.07955),\quad\widehat\tau^2=1337.88,\quad\widehat\sigma^2=66.85.}
$$

The corresponding estimated standard deviations are $36.577$ and $8.176$ grams. Individual realized [random intercepts](../../../../../../random-intercept.md) are not parameters in this marginal model, and their predictions are not supplied by this summary. For distinct measurements on the same rat, $\operatorname{Cov}(Y_{rj},Y_{rk})=\tau^2$, while the marginal [variance](../../../../../../variance-split.md) is $\tau^2+\sigma^2$; different rats are independent.

The estimated mean weight rises by $0.58568$ grams per day, adjusting for diet and the rat's [random intercept](../../../../../../random-intercept.md). This common slope is imposed across all diets: there is no time-by-diet [interaction term](../../../../../../interaction-term.md), so these estimates do not compare diet-specific growth slopes. The intercept refers to time zero for diet 1 and a zero rat effect.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
