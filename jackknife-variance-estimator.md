# Jackknife variance estimator

↑ **Parent:** [Jackknife resampling](jackknife-resampling.md)

The [jackknife variance estimator](jackknife-variance-estimator.md) estimates the [sampling variance](variance-of-an-estimator.md) of the full-data [estimator](estimator.md), using the deletion estimates and their [mean](expected-value.md) from [jackknife resampling](jackknife-resampling.md):

$$
\widehat V_J=\frac{n-1}{n}\sum_{i=1}^n
(\widehat\theta_{(-i)}-\overline\theta_J)^2,\qquad
\widehat{\operatorname{SE}}_J=\sqrt{\widehat V_J}.
$$

The square root is the estimated [standard error](standard-error.md). The factor $n-1$ multiplies the divisor-$n$ [variance](variance-split.md) of the deletion estimates: those estimates vary less than estimates from new [independent](independent-random-variables.md) experiments because almost all their observations are shared. Ryan Tibshirani's [Carnegie Mellon notes on computing jackknife standard errors](https://www.stat.cmu.edu/~ryantibs/statcomp-F15/lectures/design.html) give the same scaling in terms of the divisor-$(n-1)$ [sample variance](sample-variance.md) of the deletion estimates.

For the [sample mean](sample-mean.md), this formula has an exact algebraic simplification. With $s_n^2$ denoting the usual [sample variance](sample-variance.md),

$$
\widehat\theta_{(-i)}=\frac{n\overline x-x_i}{n-1},\qquad
\overline\theta_J=\overline x,\qquad
\widehat\theta_{(-i)}-\overline\theta_J
=-\frac{x_i-\overline x}{n-1},
$$

and therefore

$$
\widehat V_J=\frac{1}{n(n-1)}\sum_{i=1}^n(x_i-\overline x)^2
=\frac{s_n^2}{n}.
$$

Under the [independent and identically distributed](independent-and-identically-distributed-random-variables.md) assumption and a finite second [moment](moment.md), $s_n^2$ is an [unbiased estimator](unbiased-estimator.md) of the population [variance](variance-split.md) $\sigma^2$. Consequently $\widehat V_J$ is an [unbiased estimator](unbiased-estimator.md) of the [sample mean](sample-mean.md)'s [sampling variance](variance-of-an-estimator.md) $\sigma^2/n$. The equality $\widehat V_J=s_n^2/n$ itself holds for any observed data with $n>1$; its sampling interpretation uses the stated assumptions.

For $(1,2,3,4,10)$, the sum of squared deviations from the [sample mean](sample-mean.md) is $50$, giving [sample variance](sample-variance.md) $s_5^2=50/4=12.5$. The deletion [sample means](sample-mean.md) have squared deviations totaling $3.125$, so

$$
\widehat V_J=\frac45(3.125)=2.5=\frac{12.5}{5},\qquad
\widehat{\operatorname{SE}}_J=\sqrt{2.5}\approx1.58114.
$$

Here $12.5$ estimates the [variance](variance-split.md) of individual observations, while $2.5$ estimates the [sampling variance](variance-of-an-estimator.md) of their [sample mean](sample-mean.md). These answer different questions.

For more general [statistics](statistic.md), validity requires regularity beyond the deletion formula, such as a sufficiently [smooth function](smooth-function.md) of [sample means](sample-mean.md) with suitable [moments](moment.md). Ordinary delete-one [jackknife resampling](jackknife-resampling.md) can fail for nonsmooth [quantiles](quantile-function.md), including the [median](median.md); see Larry Wasserman's [All of Nonparametric Statistics, Section 3.1](https://www.stat.cmu.edu/~brian/valerie/617-2022/0%20-%20books/2006%20-%20Wasserman%20All%20Of%20Nonparametric%20Statistics.pdf). With [statistical dependence](statistical-dependence.md), deleting individual observations need not reproduce the relevant [sampling variance](variance-of-an-estimator.md); the deletion scheme must reflect that [statistical dependence](statistical-dependence.md). Shalizi's [jackknife notes, Sections 4 and 7](https://stat.cmu.edu/~cshalizi/490/23/2023-11-29-jackknife.pdf) distinguish the basic [independent and identically distributed](independent-and-identically-distributed-random-variables.md) case from extensions.

**Table of contents**

- [Jackknife and bootstrap variance of a sample second moment](jackknife-and-bootstrap-variance-of-a-sample-second-moment.md)

## ↑ Ancestors (6)

1. [Jackknife resampling](jackknife-resampling.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Jackknife and bootstrap variance of a sample second moment](jackknife-and-bootstrap-variance-of-a-sample-second-moment.md)
- [Jackknife bias correction](jackknife-bias-correction.md)
- [Jackknife resampling](jackknife-resampling.md)
- [Jackknife variance estimator](jackknife-variance-estimator.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/c/solution.md)
