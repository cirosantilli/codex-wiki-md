# Sample median

↑ **Parent:** [Median](median.md)

The [sample median](sample-median.md) is a central value of an ordered [statistical sample](statistical-sample.md). The usual numerical convention selects the middle [order statistic](order-statistic.md) for odd sample size and the [arithmetic mean](arithmetic-mean.md) of the two central [order statistics](order-statistic.md) for even sample size:

$$
\widetilde X_n=\begin{cases}
X_{(m+1)},&n=2m+1,\\
\bigl(X_{(m)}+X_{(m+1)}\bigr)/2,&n=2m.
\end{cases}
$$

NIST uses this convention. [NIST: measures of location, median definition](https://www.itl.nist.gov/div898/handbook/eda/section3/eda351.htm). For $(0.7,0.1,0.9,0.4,0.2)$, the [sample median](sample-median.md) is $0.4$; for $(0.1,0.2,0.4,0.7)$, it is $(0.2+0.4)/2=0.3$, which need not be an observed value.

More generally, every value between the two central [order statistics](order-statistic.md) in an even [statistical sample](statistical-sample.md) is a [median](median.md) of its [empirical distribution function](empirical-distribution-function.md). The generalized-inverse [sample quantile](sample-quantile.md) at $p=1/2$ selects the lower central [order statistic](order-statistic.md) in that case, so it can differ from the midpoint convention. Ties are allowed in all these definitions.

The [sample median](sample-median.md) measures the center using sorted positions. Changing the largest observation from $0.9$ to $9$ in the five-value example leaves the [sample median](sample-median.md) at $0.4$, while the [sample mean](sample-mean.md) rises from $0.46$ to $2.08$. Its [sampling distribution](sampling-distribution.md) still depends on the population [probability distribution](probability-distribution-split.md): the [mean](expected-value-split.md) $1/2$ found for five observations from a [uniform distribution](continuous-uniform-distribution.md) is a special calculation, and a [sample median](sample-median.md)'s [expected value](expected-value-split.md) need not equal the population [median](median.md) in general.

For a concrete counterexample, three [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with rate-one [exponential distribution](exponential-distribution.md) have [sample median](sample-median.md) $X_{(2)}$ with [expected value](expected-value-split.md) $1/3+1/2=5/6$, by [independent exponential order-statistic spacings](independent-exponential-order-statistic-spacings.md). The population [median](median.md) instead solves $1-e^{-m}=1/2$, giving $m=\log2\approx0.693147$. Thus even the middle [order statistic](order-statistic.md) can have [mean](expected-value-split.md) different from the population [median](median.md).

**Table of contents**

- [Coordinatewise median](coordinatewise-median.md)

## ↑ Ancestors (7)

1. [Median](median.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Bootstrapping (statistics)](bootstrapping-statistics.md)
- [Coordinatewise median](coordinatewise-median.md)
- [Finite-sample maximum bias](finite-sample-maximum-bias.md)
- [Global argmin may escape a compact convergence set](global-argmin-may-escape-a-compact-convergence-set.md)
- [Huber location estimator](huber-location-estimator.md)
- [Huber location response to one outlier](huber-location-response-to-one-outlier.md)
- [Laplace location and scale maximum likelihood](laplace-location-and-scale-maximum-likelihood.md)
- [Laplace median robustness example](laplace-median-robustness-example.md)
- [Laplace regression](laplace-regression.md)
- [Local influence versus replacement breakdown](local-influence-versus-replacement-breakdown.md)
- [Order statistic](order-statistic.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/6/vi/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-223/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-223/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-223/2/c/solution.md)
- [Sample median](sample-median.md)
- [Uniform order statistic](uniform-order-statistic.md)
