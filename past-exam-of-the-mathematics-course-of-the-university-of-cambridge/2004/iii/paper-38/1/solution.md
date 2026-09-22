<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [censoring](../../../../../censoring-statistics.md) observation means an event time is not observed exactly: the information supplies a bound or interval instead. Under [right censoring](../../../../../right-censoring.md), one observes $X=\min(T,C)$ and the event indicator $\delta=\mathbf1_{\{T\le C\}}$; if $\delta=0$, one knows only $T>C$. Left [censoring](../../../../../censoring-statistics.md) gives an upper bound, while interval [censoring](../../../../../censoring-statistics.md) locates the event between two observations.

[Uninformative censoring](../../../../../independent-censoring.md) means that, conditional on the covariates used in the analysis, the [censoring](../../../../../censoring-statistics.md) mechanism supplies no additional information about the event time. [Independence](../../../../../independent-random-variables.md) $T\perp C$ within those covariate strata is a sufficient formulation: subjects remaining in the observed [risk set](../../../../../risk-set.md) have the same future [hazard](../../../../../hazard-function.md) as the corresponding event-free population. A fixed study cutoff unrelated to prognosis is an example of [administrative censoring](../../../../../administrative-censoring.md).

[Informative censoring](../../../../../informative-censoring.md) occurs when that condition fails. For example, students at high risk of leaving may also become harder to contact before their departure is formally recorded; [censoring](../../../../../censoring-statistics.md) at loss of contact selectively removes high-risk students. Ordinary [Kaplan–Meier estimator](../../../../../kaplan-meier-estimator.md) and [Nelson–Aalen estimator](../../../../../nelson-aalen-estimator.md) calculations then use an unrepresentative [risk set](../../../../../risk-set.md). **The distinction determines whether ordinary survival estimates can be interpreted as population survival.** Merely knowing that an observation is censored does not establish [independence](../../../../../independent-random-variables.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 38](../../paper-38-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
