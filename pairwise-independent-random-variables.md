# Pairwise independent random variables

↑ **Parent:** [Independent random variables](independent-random-variables.md)

[Random variables](random-variable-split.md) are pairwise independent when every two distinct members are [independent random variables](independent-random-variables.md). Each pair's [joint probability distribution](joint-probability-distribution.md) must factor for all its [events](event.md); examining only a pair's [covariance](covariance.md) is insufficient. Full [independence](independent-random-variables.md) implies pairwise independence by taking the other sets in the definition to be the whole target spaces. The reverse implication fails once there are three or more variables.

Pairwise independence is enough to add [variances](variance-split.md): for a finite family of [square-integrable](square-integrable-function.md) pairwise independent [random variables](random-variable-split.md),

$$
\operatorname{Var}\!\left(\sum_{i=1}^n X_i\right)=\sum_{i=1}^n\operatorname{Var}(X_i),
$$

because all cross [covariances](covariance.md) vanish in the [variance of a sum](variance-of-a-sum.md). Thus pairwise independence can support calculations about the size of fluctuations while failing to determine the full [joint probability distribution](joint-probability-distribution.md). The following example makes that distinction visible.

**Table of contents**

- [Pairwise independence does not imply joint independence](pairwise-independence-does-not-imply-joint-independence.md)

## ↑ Ancestors (7)

1. [Independent random variables](independent-random-variables.md)
2. [Random variable](random-variable-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Parity construction of pairwise independent bits](parity-construction-of-pairwise-independent-bits.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/27k/c/solution.md)
- [Variance of a sample mean](variance-of-a-sample-mean.md)
