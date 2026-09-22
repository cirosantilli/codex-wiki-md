<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For an event at $t_j$ from subject $i_j$, with covariate vector $z_i$, define the [Schoenfeld function](../../../../../schoenfeld-function.md)

$$
\boxed{s_j(\beta)=z_{i_j}-\bar z(\beta,t_j),\qquad \bar z(\beta,t_j)=\frac{\sum_{i\in R_j}z_i e^{\beta^Tz_i}}{\sum_{i\in R_j}e^{\beta^Tz_i}}.}
$$

The second term is the hazard-weighted mean covariate in the [risk set](../../../../../risk-set.md) just before the event. The [Schoenfeld residual](../../../../../schoenfeld-residual.md) is this function evaluated at the fitted coefficient, $r_j=s_j(\widehat\beta)$. Calculate one residual vector per event, using every at-risk subject, including those who will subsequently be censored. There is no ordinary event residual assigned at a [right censoring](../../../../../right-censoring.md) time.

The [Cox partial likelihood](../../../../../cox-partial-likelihood.md) [score function](../../../../../informant-function.md) is $\sum_j s_j(\beta)$. At the true constant coefficient in a [Cox proportional-hazards model](../../../../../cox-proportional-hazards-model.md), the conditional event subject is selected with weights proportional to $e^{\beta^Tz_i}$, so each [Schoenfeld function](../../../../../schoenfeld-function.md) has conditional mean zero. If the coefficient varies with time, that centering changes. Plot residuals against event time or a transformation of it, smooth them, and investigate departures from zero. [Scaled Schoenfeld residuals](../../../../../scaled-schoenfeld-residual.md) account for the risk-set covariate [variance](../../../../../variance-split.md) and can display departures in coefficient units; [score function](../../../../../informant-function.md) tests based on residual-time association provide a formal check. Risk-set composition affects unscaled residual [variance](../../../../../variance-split.md), and the total residual [score function](../../../../../informant-function.md) can be zero by fitting even when a time trend is present.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
