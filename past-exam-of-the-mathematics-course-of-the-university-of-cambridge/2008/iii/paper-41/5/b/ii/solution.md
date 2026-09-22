<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Converting size to a [regression factor](../../../../../../../regression-factor.md) allows two unrestricted contrasts rather than imposing a linear trend on numerical size codes. The command relevel with a numeric second argument selects the second existing factor level as its [reference level](../../../../../../../reference-level-in-a-regression-factor.md). For sorted codes $0,1,2$ this is medium, coded $1$. However, the displayed coefficient labels size1 and size3 instead correspond to codes $1,2,3$ with code $2$ as reference. **The printed coding and coefficient labels are inconsistent.** The actual factor levels and labels must be checked. Under the intended medium-size reference, the two reported contrasts compare small and large businesses with medium ones; with literal $0,1,2$ coding their printed names would be size0 and size2.

Using B's delayed-entry survival object, the [Cox proportional-hazards model](../../../../../../../cox-proportional-hazards-model.md) is

$$
h(t\mid c,s)=h_0(t)\exp\{\beta_c c+\beta_{\mathrm{small}}\mathbf1_{\{s=\mathrm{small}\}}+\beta_{\mathrm{large}}\mathbf1_{\{s=\mathrm{large}\}}\}.
$$

Here $h_0$ is the unspecified [baseline hazard](../../../../../../../baseline-hazard.md) for a medium-size village business and $c$ is the Cambridge indicator. The fitted [hazard ratios](../../../../../../../hazard-ratio.md) are conditional on the other [covariates](../../../../../../../covariate.md) and constant over business age under the [proportional hazards](../../../../../../../proportional-hazards-model.md) assumption. The function fits [regression coefficients](../../../../../../../regression-coefficient.md) through [partial likelihood](../../../../../../../partial-likelihood.md); its survival object must actually be B's version, rather than A's earlier object with the same name.

The location coefficient $-0.803$, with [standard error](../../../../../../../standard-error.md) $0.344$, gives $z=-2.335$ and a two-sided [Wald test](../../../../../../../wald-test.md) [p-value](../../../../../../../p-value.md) about $0.02$. Its reported [hazard ratio](../../../../../../../hazard-ratio.md) is $0.448$, with 95% [confidence interval](../../../../../../../confidence-interval.md) $(0.228,0.879)$. At the same age and size, a Cambridge business therefore has an estimated closure hazard about 55.2% lower than a village business. The reciprocal ratio is $2.23$. **A hazard ratio is not a survival-probability ratio or a proportional increase in lifetime.**

The intended small-versus-medium contrast is $-0.322$, with [standard error](../../../../../../../standard-error.md) $0.482$, $z=-0.669$ and [p-value](../../../../../../../p-value.md) $0.50$. Its [hazard ratio](../../../../../../../hazard-ratio.md) is $0.724$, with 95% [confidence interval](../../../../../../../confidence-interval.md) $(0.282,1.863)$. The intended large-versus-medium contrast is $-0.224$, with [standard error](../../../../../../../standard-error.md) $0.375$, $z=-0.598$ and [p-value](../../../../../../../p-value.md) $0.55$; its [hazard ratio](../../../../../../../hazard-ratio.md) is $0.799$, with interval $(0.383,1.666)$. Neither size contrast provides convincing evidence of an effect. The wide intervals also show why these results do not establish equality of size-specific hazards.

The sample has $60$ businesses. The [likelihood-ratio test](../../../../../../../likelihood-ratio-test.md), [Wald test](../../../../../../../wald-test.md) and [score test](../../../../../../../score-test.md) jointly test all three coefficients being zero; their statistics are $5.45$, $5.76$ and $6.01$ on three [degrees of freedom](../../../../../../../degree-of-freedom.md), with [p-values](../../../../../../../p-value.md) $0.142$, $0.124$ and $0.111$. None rejects at 5%. This is compatible with the significant one-coefficient location test: testing a specified one-dimensional contrast and testing three coefficients together are different questions. The location result offers some adjusted evidence, but the joint output does not demonstrate a strong overall improvement, and interpretation should acknowledge the uncertainty and the number of comparisons.

The reported $R^2=0.087$ is a [Cox–Snell likelihood pseudo-R-squared](../../../../../../../cox-snell-likelihood-pseudo-r-squared.md), here $1-e^{-5.45/60}\approx0.087$. It measures likelihood improvement rather than a literal fraction of variance in lifetimes explained. Its attainable maximum is reported as $0.979$. It does not validate the [proportional hazards](../../../../../../../proportional-hazards-model.md) assumption or establish useful predictive performance. Adjusted survival predictions would require estimating the [baseline survival function](../../../../../../../baseline-survival-function.md) as well: $S(t\mid z)=S_0(t)^{e^{\beta^Tz}}$. The coefficient summary alone does not supply adjusted five- or ten-year survival probabilities.

Before reporting results, check the size coding discrepancy, the precise sampling dates and the survival records. The stated January 2000–December 2005 span is six calendar years, despite being called five years. Check nonnegative ages, entry no later than exit, correctly recorded closure indicators and the same opening-based clock throughout. Establish whether inclusion and [censoring](../../../../../../../censoring-statistics.md) are plausibly independent of lifetime given the [covariates](../../../../../../../covariate.md), and whether different opening cohorts or calendar environments can reasonably share the fitted lifetime model. Simply including delayed entry does not cure informative selection, omitted [confounders](../../../../../../../confounder.md) or dependence between businesses.

Assess [proportional hazards](../../../../../../../proportional-hazards-model.md) using [Schoenfeld residuals](../../../../../../../schoenfeld-residual.md) against time and a [proportional hazards assumption test](../../../../../../../proportional-hazards-assumption-test.md), supplemented by groupwise log-minus-log survival plots. Investigate influential observations with coefficient-deletion diagnostics and [deviance residuals](../../../../../../../deviance-residual.md), and inspect overall fit using [Cox–Snell residuals](../../../../../../../cox-snell-residual.md). Consider a city-by-size [interaction](../../../../../../../interaction-statistics.md) or time-varying effects if supported by the available events, rather than relying on the displayed three main effects. Finally, report the uncertainty and declining late [risk sets](../../../../../../../risk-set.md)—only six remain at the final listed event—and distinguish a conditional association from a causal explanation or a prediction for all future businesses.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 41](../../../../paper-41-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
