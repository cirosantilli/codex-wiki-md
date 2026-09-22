# Bootstrapping (statistics)

↑ **Parent:** [Statistical modelling](statistical-modelling-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bootstrapping_(statistics))

The [bootstrap](bootstrapping-statistics.md) approximates a [sampling distribution](sampling-distribution.md) by repeatedly [sampling with replacement](sampling-with-replacement.md) from the [empirical measure](empirical-measure.md) of the observed data. In the ordinary nonparametric version, observations are assumed [independent and identically distributed](independent-and-identically-distributed-random-variables.md); a [bootstrap sample](bootstrap-sample.md) has the same size as the original [statistical sample](statistical-sample.md). A [statistic](statistic.md), such as a [sample mean](sample-mean.md) or [sample median](sample-median.md), is recomputed on each resample. Its variation across resamples estimates how the original [statistic](statistic.md) would vary across repeated sampling from the unknown [probability distribution](probability-distribution-split.md).[UW STAT 535: Statistical Machine Learning, Autumn 2026; The Bootstrap, resampling procedure; High level idea of how bootstrap works, conditional empirical sampling law](uw-stat-535-statistical-machine-learning-autumn-2026/lecture-12-the-bootstrap.md)

The key distinction is between the observed [statistical sample](statistical-sample.md) and its still-unknown source [probability distribution](probability-distribution-split.md). Condition on the observed values $x_1,\ldots,x_n$ and form the [empirical measure](empirical-measure.md)

$$
\widehat P_n=\frac1n\sum_{i=1}^n\delta_{x_i}.
$$

Here $\delta_{x_i}$ is a [Dirac measure](dirac-measure.md). Draw [independent](independent-random-variables.md) indices $I_1,\ldots,I_n$ from the [uniform distribution on a finite set](discrete-uniform-distribution.md) $\{1,\ldots,n\}$ and set $X_j^*=x_{I_j}$. Each observed slot has [probability](probability.md) $1/n$ on every draw. If equal values occupy several slots, their total [probability](probability.md) is the sum of those slot [probabilities](probability.md); distinct observed values need not be equally likely. A star denotes this conditional resampling experiment. There are $n^n$ equally likely ordered index sequences, although [bootstrap count vectors](bootstrap-count-vectors.md) and [statistics](statistic.md) can combine many such sequences.

<a id="image-sampling-with-replacement-reuses-observed-slots-while-keeping-the-original-data-fixed"></a>
![](bootstrap-resampling-observed-slots.png)

**[Figure 7](#image-sampling-with-replacement-reuses-observed-slots-while-keeping-the-original-data-fixed). Sampling with replacement reuses observed slots while keeping the original data fixed**. Original schematic for observations $(1,2,4)$. Three possible ordered [bootstrap samples](bootstrap-sample.md) have different [sample means](sample-mean.md). Their colors identify source slots; none of these samples is new evidence about the unknown [probability distribution](probability-distribution-split.md).

A complicated [sampling distribution](sampling-distribution.md) need not stop [statistical inference](statistical-inference-split.md) when recomputing the [statistic](statistic.md) is easy. The [bootstrap](bootstrapping-statistics.md) reuses that calculation on simulated datasets. The [plug-in estimator](plug-in-estimator.md) principle replaces the unknown [probability measure](probability-measure.md) by $\widehat P_n$ in the whole repeated-sampling experiment. Whether that substitution approximates the target [sampling distribution](sampling-distribution.md) needs an appropriate [bootstrap consistency theorem for the sample mean](bootstrap-consistency-theorem-for-the-sample-mean.md) or a result for the particular [statistic](statistic.md). A larger number of resamples reduces [Monte Carlo error](monte-carlo-error.md); it cannot repair the [bootstrap failure for a uniform endpoint](bootstrap-failure-for-a-uniform-endpoint.md), an unrepresentative [statistical sample](statistical-sample.md) or ignored [statistical dependence](statistical-dependence.md).[UW STAT 535: Statistical Machine Learning, Autumn 2026; High level idea of how bootstrap works; Bootstrap and Statistical Functionals, conditional variance and bootstrap variance consistency; Failure of the bootstrap, uniform-endpoint counterexample](uw-stat-535-statistical-machine-learning-autumn-2026/lecture-12-the-bootstrap.md)

**Table of contents**

- [Exact bootstrap distribution for three observations](exact-bootstrap-distribution-for-three-observations.md)
- [Bootstrap publication history](bootstrap-publication-history.md)
- [Bootstrap failure for a uniform endpoint](bootstrap-failure-for-a-uniform-endpoint.md)
- [Bootstrap standard error](bootstrap-standard-error.md)
- [Bootstrap confidence interval](bootstrap-confidence-interval.md)
  - [Bootstrap inference for a product of regression coefficients](bootstrap-inference-for-a-product-of-regression-coefficients.md)
  - [Bootstrap-t confidence interval](bootstrap-t-confidence-interval.md)
  - [Percentile bootstrap confidence interval](percentile-bootstrap-confidence-interval.md)
  - [Basic bootstrap confidence interval](basic-bootstrap-confidence-interval.md)
- [Bootstrap consistency theorem for the sample mean](bootstrap-consistency-theorem-for-the-sample-mean.md)
- [Bootstrap sample](bootstrap-sample.md)
  - [Wild bootstrap](wild-bootstrap.md)
  - [Paired bootstrap](paired-bootstrap.md)
  - [Conditional bootstrap variance of a sample mean](conditional-bootstrap-variance-of-a-sample-mean.md)
  - [Bootstrap count vectors](bootstrap-count-vectors.md)
- [Parametric bootstrap](parametric-bootstrap.md)

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling-split.md)
2. [Statistical model](statistical-model-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3/28j/c/solution.md)
