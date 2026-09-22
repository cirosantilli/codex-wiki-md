# Bernoulli distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_distribution)

A [Bernoulli random variable](bernoulli-distribution.md) records one success as $1$ and one failure as $0$. For $0\leq p\leq1$, its [probability mass function](probability-mass-function.md) is

$$
\mathbb P(B=1)=p,\qquad \mathbb P(B=0)=1-p,
$$

with zero mass elsewhere. The terms success and failure merely name outcomes; success need not be desirable. Any event $A$ produces such a variable through its [indicator random variable](indicator-random-variable.md) $B=\mathbf1_A$, with $p=\mathbb P(A)$. A single [Bernoulli distribution](bernoulli-distribution.md) requires no [independence](independent-random-variables.md) assumption; [independence](independent-random-variables.md) becomes relevant when several trials are combined.

Because $B^2=B$, the [expected value](expected-value.md) and [variance](variance-split.md) follow immediately:

$$
\mathbb E B=0(1-p)+1p=p,\qquad
\operatorname{Var}(B)=\mathbb E[B^2]-(\mathbb E B)^2=p-p^2=p(1-p).
$$

For a constructed trial with $p=0.3$, these are $0.3$ and $0.21$. The [variance](variance-split.md) is greatest at $p=1/2$, where it equals $1/4$, since $p(1-p)=1/4-(p-1/2)^2$. At $p=0$ or $p=1$, the outcome is certain and the [variance](variance-split.md) vanishes.

The beauty of an [indicator random variable](indicator-random-variable.md) is that counting becomes addition: summing such indicators counts successes, and the [linearity of expectation](linearity-of-expectation.md) gives the expected count even when the indicators are dependent. With [independence](independent-random-variables.md) and a shared $p$, the full count law is the [binomial distribution](binomial-distribution.md). These models are summarized in [Penn State STAT 504, discrete distributions](https://online.stat.psu.edu/stat504/Lesson01).

A historical anchor is Bernoulli's posthumous _Ars conjectandi_: its original title page identifies the author and records publication at Basel in 1713. This documents the book's publication, rather than establishing priority for the modern name [Bernoulli distribution](bernoulli-distribution.md). See [Ars conjectandi, original title page, ETH Library](https://www.e-rara.ch/download/pdf/2645768.pdf).

**Table of contents**

- [Estimating Bernoulli variance](estimating-bernoulli-variance.md)
- [Bernoulli trial](bernoulli-trial.md)
- [Bernoulli thinning](bernoulli-thinning.md)

## ↑ Ancestors (7)

1. [Discrete probability distribution](discrete-probability-distribution-split.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (101)

- [Bernoulli coupling by a shared uniform random variable](bernoulli-coupling-by-a-shared-uniform-random-variable.md)
- [Bernoulli distribution](bernoulli-distribution.md)
- [Bernoulli invariant laws of finite symmetric exclusion](bernoulli-invariant-laws-of-finite-symmetric-exclusion.md)
- [Bernoulli process](bernoulli-process.md)
- [Bernoulli trial](bernoulli-trial.md)
- [Binary cross-entropy](binary-cross-entropy.md)
- [Bond percolation](bond-percolation-split.md)
- [Brier score](brier-score.md)
- [Central limit theorem](central-limit-theorem.md)
- [Chernoff information for complementary Bernoulli distributions](chernoff-information-for-complementary-bernoulli-distributions.md)
- [Conditional independence](conditional-independence.md)
- [Conditional logistic model for longitudinal binary data](conditional-logistic-model-for-longitudinal-binary-data.md)
- [Coordinate-splitting proof of the BK inequality](coordinate-splitting-proof-of-the-bk-inequality.md)
- [Coupling](coupling.md)
- [Dependence in Poisson thinning](dependence-in-poisson-thinning.md)
- [Discrete probability distribution](discrete-probability-distribution-split.md)
- [Disjoint occurrence of increasing events](disjoint-occurrence-of-increasing-events.md)
- [Expected value premium principle](expected-value-premium-principle.md)
- [Fair-coin doubling martingale](fair-coin-doubling-martingale.md)
- [Graph cut](graph-cut.md)
- [Independent random variables](independent-random-variables.md)
- [Independent record indicators](independent-record-indicators.md)
- [Indicator random variable](indicator-random-variable.md)
- [Itinerary of an interval map](itinerary-of-an-interval-map.md)
- [Kullback-Leibler divergence](kullback-leibler-divergence.md)
- [Linear probability score](linear-probability-score.md)
- [Logarithmic scoring rule](logarithmic-scoring-rule.md)
- [Maximum-likelihood estimator](maximum-likelihood-estimator.md)
- [Moment matching for a beta prior](moment-matching-for-a-beta-prior.md)
- [Monotone coupling of Bernoulli percolation](monotone-coupling-of-bernoulli-percolation.md)
- [Negative correlation of increasing and decreasing events](negative-correlation-of-increasing-and-decreasing-events.md)
- [Non-uniqueness of maximal ancillary statistics](non-uniqueness-of-maximal-ancillary-statistics.md)
- [Parity construction of pairwise independent bits](parity-construction-of-pairwise-independent-bits.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/1/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37/6/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-38/5/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3/5i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/4/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-41/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/2/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/5/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/5/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-204/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/9f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/8h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/13j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/5j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/26k/c/ii/solution.md)
- [Posterior predictive probability](posterior-predictive-probability.md)
- [Proper scoring rule](proper-scoring-rule.md)
- [Randomly shifted lattice point process](randomly-shifted-lattice-point-process.md)
- [Return period](return-period.md)
- [Saturated statistical model](saturated-statistical-model.md)
- [Scoring rule](scoring-rule.md)
- [Spectral norm bound for a centered Bernoulli adjacency matrix](spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix.md)
- [Stationarity without ergodicity in an information source](stationarity-without-ergodicity-in-an-information-source.md)
- [Strictly proper scoring rule](strictly-proper-scoring-rule.md)
- [Strong law of large numbers](strong-law-of-large-numbers.md)
- [Total variation distance under a measurable map](total-variation-distance-under-a-measurable-map.md)
- [Weak law of large numbers](weak-law-of-large-numbers.md)
