# Studentized normal sample mean

↑ **Parent:** [Student's t-distribution](student-s-t-distribution.md)

Suppose $X_1,\ldots,X_n$, $n\geq2$, are [independent and identically distributed](independent-and-identically-distributed-random-variables.md) with [normal distribution](normal-distribution.md) $N(\mu,\sigma^2)$, where the [mean](expected-value-split.md) $\mu$ and [standard deviation](standard-deviation.md) $\sigma>0$ are unknown. Define the [sample mean](sample-mean.md) and [sample variance](sample-variance.md) by

$$
\bar X=\frac1n\sum_{i=1}^nX_i,\qquad S^2=\frac1{n-1}\sum_{i=1}^n(X_i-\bar X)^2.
$$

Under these assumptions,

$$
Z=\frac{\sqrt n(\bar X-\mu)}{\sigma}\sim N(0,1),\qquad V=\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1},\qquad Z\text{ and }V\text{ are independent}.
$$

Substitution gives the exact ratio

$$
\frac{Z}{\sqrt{V/(n-1)}}=\frac{\bar X-\mu}{S/\sqrt n}\sim t_{n-1}.
$$

The unknown $\sigma$ cancels. The denominator $S/\sqrt n$ estimates the [standard error](standard-error.md) of the [sample mean](sample-mean.md); its sampling variability is precisely why the [Student's t-distribution](student-s-t-distribution.md) has wider tails than the [standard normal distribution](standard-normal-distribution.md).

The crucial [independence](independent-random-variables.md) has a geometric explanation. Apply an [orthogonal transformation](orthogonal-transformation.md) to the standardized observations $(X_i-\mu)/\sigma$, choosing its first coordinate along $(1,\ldots,1)/\sqrt n$. That coordinate is $Z$; the remaining $n-1$ coordinates are [independent](independent-random-variables.md) [standard normal random variables](standard-normal-random-variable.md) whose squared sum is $V$. Their [joint probability density](joint-probability-density.md) factorizes because the transformation preserves the squared length. This also explains the loss of one [statistical degree of freedom](statistical-degrees-of-freedom.md) when estimating the [mean](expected-value-split.md). Uncorrelatedness alone would not establish the required [independence](independent-random-variables.md) for arbitrary data.

The result is exact for every $n\geq2$ under the stated [normal distribution](normal-distribution.md) model. A small [sample size](sample-size.md) by itself does not justify it: a sample from an arbitrary [probability distribution](probability-distribution-split.md) need not have the displayed [chi-squared distribution](chi-squared-distribution.md) or the necessary [independence](independent-random-variables.md).

**Table of contents**

- [Small normal sample mean confidence interval](small-normal-sample-mean-confidence-interval.md)

## ↑ Ancestors (8)

1. [Student's t-distribution](student-s-t-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [History of Student's t-distribution](history-of-student-s-t-distribution.md)
- [Small normal sample mean confidence interval](small-normal-sample-mean-confidence-interval.md)
