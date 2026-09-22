<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Begin by defining the scientific target: prediction for a new patient, or [estimation](../../../../../statistical-estimation.md) of adjusted covariate effects. Check event definitions, follow-up origins, right-censoring codes and any [delayed entry](../../../../../left-truncation.md). The analysis assumes independent patients and censoring that is noninformative conditional on modeled covariates. For fixed explanatory variables $z_i$, the [Cox proportional-hazards model](../../../../../cox-proportional-hazards-model.md) is

$$
h_i(t)=h_0(t)\exp(z_i^{\mathsf T}\beta),
$$

with an unrestricted [baseline hazard](../../../../../baseline-hazard.md) and coefficients constant over time. Report $\exp(\beta_k)$ as the conditional [hazard ratio](../../../../../hazard-ratio.md) for a one-unit change in the coded variable, not as a [risk ratio](../../../../../risk-ratio.md) or automatically a causal effect.

For untied event times, fit the coefficients by maximizing the [Cox partial likelihood](../../../../../cox-partial-likelihood.md)

$$
L_p(\beta)=\prod_{j:\,\mathrm{event}}
\frac{\exp(z_{i(j)}^{\mathsf T}\beta)}
{\sum_{i\in R(t_j)}\exp(z_i^{\mathsf T}\beta)}.
$$

The baseline cancels within each event [risk set](../../../../../risk-set.md). Use an appropriate tied-event method, such as an Efron approximation or an exact method for a genuinely discrete event scale; the [Breslow approximation for tied event times](../../../../../breslow-approximation-for-tied-event-times.md) is another explicit approximation. Numerical score/information methods fit the model, and inverse information gives conventional covariance estimates for independent subjects. Report coefficient estimates, [hazard ratios](../../../../../hazard-ratio.md), uncertainty and the coding that makes their interpretation meaningful. After fitting, the [Breslow estimator](../../../../../breslow-estimator.md) gives $\widehat H_0(t)=\sum_{t_j\leq t}d_j/\sum_{i\in R(t_j)}e^{z_i^{\mathsf T}\widehat\beta}$, from which $\widehat S(t\mid z)=\exp[-\widehat H_0(t)e^{z^{\mathsf T}\widehat\beta}]$ provides predicted survival.

Adequacy is broader than significance of coefficients. Inspect influential observations, [deviance residuals](../../../../../deviance-residual.md) and data errors. [Cox–Snell residuals](../../../../../cox-snell-residual.md) $\widehat H_0(x_i)e^{z_i^{\mathsf T}\widehat\beta}$ should have approximately unit-exponential survival under a well-fitting model, retaining the original censoring indicators; a cumulative-hazard plot of these residuals should be near the 45-degree line. This is an overall diagnostic, not a substitute for the functional-form and proportionality checks below. For prediction, assess held-out discrimination and [survival prediction calibration](../../../../../survival-prediction-calibration.md) at prespecified time horizons with methods accounting for censoring. A high [concordance index](../../../../../concordance-index.md) alone does not establish good calibration or correct hazard structure.

Use [bootstrap](../../../../../bootstrapping-statistics.md) or held-out [cross-validation](../../../../../cross-validation.md) that repeats the complete modeling procedure, including imputation, variable selection and tuning. Validation of only the final fitted coefficients understates overfitting from earlier decisions. Report any substantive lack of fit rather than presenting a single time-independent [hazard ratio](../../../../../hazard-ratio.md) when the data do not support that representation.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
