# Uncorrelated random variables

↑ **Parent:** [Covariance](covariance.md)

Two [square-integrable](square-integrable-function.md) [random variables](random-variable-split.md) $X,Y$ are [uncorrelated random variables](uncorrelated-random-variables.md) when $\operatorname{Cov}(X,Y)=0$. [Independent random variables](independent-random-variables.md) with finite [second moments](second-moment.md) are [uncorrelated random variables](uncorrelated-random-variables.md), but zero [covariance](covariance.md) does not generally imply [independence](independent-random-variables.md).

For an explicit counterexample, let $X$ take $-1$, $0$, $1$ with equal [probabilities](probability.md), and let $Y=X^2$. Then $\mathbb E X=\mathbb E X^3=0$, so $\operatorname{Cov}(X,Y)=\mathbb E X^3-\mathbb E X\,\mathbb E X^2=0$. Nevertheless, $Y$ is completely determined by $X$: $\mathbb P(Y=0\mid X=0)=1$, while $\mathbb P(Y=0)=1/3$. Thus these are [uncorrelated random variables](uncorrelated-random-variables.md) with [statistical dependence](statistical-dependence.md). In this example, opposite contributions from the [odd function](odd-function.md) $x^3$ cancel; the [even function](even-function.md) $x^2$ still retains information about $|X|$. The last panel of the [covariance](covariance.md) diagram shows the relationship.

There are useful special cases. [Uncorrelated jointly normal variables are independent](uncorrelated-jointly-normal-variables-are-independent.md), and the [Bernoulli independence from zero covariance](bernoulli-independence-from-zero-covariance.md) result supplies another setting where the converse holds. Their distribution assumptions do the extra work; zero [covariance](covariance.md) alone does not.

**Table of contents**

- [Bernoulli independence from zero covariance](bernoulli-independence-from-zero-covariance.md)

## ↑ Ancestors (8)

1. [Covariance](covariance.md)
2. [Variance](variance-split.md)
3. [Expected value](expected-value-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Autocorrelation](autocorrelation.md)
- [Autocovariance](autocovariance.md)
- [Bernoulli independence from zero covariance](bernoulli-independence-from-zero-covariance.md)
- [Independent random variables](independent-random-variables.md)
- [Law of total variance](law-of-total-variance.md)
- [Martingale difference sequence](martingale-difference-sequence.md)
- [Moving average](moving-average.md)
- [Moving-average process of order one](moving-average-process-of-order-one.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/10f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-2/9f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/1/1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202/1/a/ii/solution.md)
- [Pearson correlation coefficient](pearson-correlation-coefficient.md)
- [Probability generating function of an independent sum](probability-generating-function-of-an-independent-sum.md)
- [Strong law for uniformly L2-bounded uncorrelated random variables](strong-law-for-uniformly-l2-bounded-uncorrelated-random-variables.md)
- [Uncorrelated random variables](uncorrelated-random-variables.md)
- [Weak white noise](weak-white-noise.md)
- [White noise](white-noise.md)
