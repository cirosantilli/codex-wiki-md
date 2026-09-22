<h1 id="kaplan-meier-estimator">Kaplan–Meier estimator</h1>

↑ **Parent:** [Survival analysis](survival-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kaplan–Meier_estimator)

At distinct observed event times $t_1<t_2<\cdots$, let $n_j$ be the [risk set](risk-set.md) size immediately before $t_j$, and let $d_j$ count events at $t_j$. The [Kaplan–Meier estimator](kaplan-meier-estimator.md) of the [survival function](survival-function.md) is

$$
\widehat S(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{n_j}\right).
$$

The empty product is one. Each factor estimates a conditional survival [probability](probability.md) among those still observed and event-free; their product joins the successive steps. This is [nonparametric statistics](nonparametric-statistics-split.md): no specified shape for the [survival distribution](survival-distribution.md) is imposed. Use [independent censoring](independent-censoring.md) and the appropriate [risk sets](risk-set.md) to interpret the result as an estimate for the intended population.

The [Kaplan–Meier estimator](kaplan-meier-estimator.md) is a [right-continuous function](right-continuous-function.md) with downward jumps at event times. [Right censoring](right-censoring.md) changes later denominators without causing a jump. A tick on the curve marks [right censoring](right-censoring.md), rather than a failure. For a tied group of $d_j$ events, use the one factor $(n_j-d_j)/n_j$; subjects [right-censored](right-censoring.md) at that recorded time remain in $n_j$ for this factor. The fraction $d_j/n_j$ estimates a [discrete hazard](discrete-hazard.md), not a continuous [hazard function](hazard-function.md) in inverse-time units. With no [censoring](censoring-statistics.md), the factors telescope to the fraction of the original cohort whose observed [survival times](survival-time.md) exceed $t$, the complement of its [empirical distribution function](empirical-distribution-function.md).

Edward L. Kaplan and Paul Meier published [Nonparametric Estimation from Incomplete Observations, Journal of the American Statistical Association 53(282), 457–481 (1958)](https://doi.org/10.1080/01621459.1958.10501452). Their paper addresses lifetime estimation when observation ends before failure and explicitly calls attention to the assumption of [independence](independent-random-variables.md) between lifetime and potential observation loss. The date 1958 is the original publication year; the publisher's later online-posting date is not the discovery date.

In his [1983 Citation Classic recollection](https://garfield.library.upenn.edu/classics1983/A1983QS51100001.pdf), Kaplan traces Meier's interest to cancer-duration data in 1952 and his own to the lifetimes of vacuum tubes in undersea telephone-cable equipment a year later. The journal encouraged them to combine their manuscripts. The shared mathematical question was how to estimate a [survival function](survival-function.md) when some lifetimes are still running or disappear from observation.

**Table of contents**

- [Kaplan–Meier six-subject cohort](kaplan-meier-six-subject-cohort.md)
- [Kaplan–Meier median survival time](kaplan-meier-median-survival-time.md)
- [Constrained Kaplan–Meier estimator](constrained-kaplan-meier-estimator.md)
- [Kaplan–Meier telescoping across a censor-free interval](kaplan-meier-telescoping-across-a-censor-free-interval.md)
- [Greenwood formula](greenwood-formula.md)
- [Kaplan–Meier estimator with delayed entry](kaplan-meier-estimator-with-delayed-entry.md)
- [Self-consistency of Kaplan–Meier estimation](self-consistency-of-kaplan-meier-estimation.md)
- [Fractional event imputation](fractional-event-imputation.md)
- [Terminal censoring and survival-mean identifiability](terminal-censoring-and-survival-mean-identifiability.md)
- [Potential right-censoring time](potential-right-censoring-time.md)
- [Potential event time](potential-event-time.md)

## ↑ Ancestors (5)

1. [Survival analysis](survival-analysis-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (66)

- [Cohort pooling under administrative censoring](cohort-pooling-under-administrative-censoring.md)
- [Constrained Kaplan–Meier estimator](constrained-kaplan-meier-estimator.md)
- [Cox–Snell residual](cox-snell-residual.md)
- [Cox–Snell residual survival diagnostic](cox-snell-residual-survival-diagnostic.md)
- [Cumulative hazard function](cumulative-hazard-function.md)
- [Discrete hazard](discrete-hazard.md)
- [Fractional event imputation](fractional-event-imputation.md)
- [Greenwood formula](greenwood-formula.md)
- [Independent censoring](independent-censoring.md)
- [Informative censoring](informative-censoring.md)
- [Kaplan–Meier estimator](kaplan-meier-estimator.md)
- [Kaplan–Meier estimator with delayed entry](kaplan-meier-estimator-with-delayed-entry.md)
- [Kaplan–Meier median survival time](kaplan-meier-median-survival-time.md)
- [Kaplan–Meier six-subject cohort](kaplan-meier-six-subject-cohort.md)
- [Kaplan–Meier telescoping across a censor-free interval](kaplan-meier-telescoping-across-a-censor-free-interval.md)
- [Net survival](net-survival.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-28/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-40/2/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-38/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-46/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/5/b/iii/solution.md)
- [4](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/4.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/4/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/4/b/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-207/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-207/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-207/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-207/5/viii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-207/6/b/ii/solution.md)
- [Potential event time](potential-event-time.md)
- [Potential right-censoring time](potential-right-censoring-time.md)
- [Restricted mean survival time](restricted-mean-survival-time.md)
- [Risk-set-adjusted relative survivor estimator](risk-set-adjusted-relative-survivor-estimator.md)
- [Self-consistency of Kaplan–Meier estimation](self-consistency-of-kaplan-meier-estimation.md)
- [Shared-fit Cox–Snell residuals reproduce the fitted survival curve](shared-fit-cox-snell-residuals-reproduce-the-fitted-survival-curve.md)
- [Small-jump comparison of cumulative hazard estimators](small-jump-comparison-of-cumulative-hazard-estimators.md)
- [Survival analysis](survival-analysis-split.md)
- [Survival function](survival-function.md)
- [Terminal censoring and survival-mean identifiability](terminal-censoring-and-survival-mean-identifiability.md)
