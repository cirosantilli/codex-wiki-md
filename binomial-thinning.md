# Binomial thinning

↑ **Parent:** [Random sum](random-sum.md)

Retain each of $N$ objects independently with [probability](probability.md) $r$, independently of the nonnegative integer-valued [random variable](random-variable-split.md) $N$. The retained count $Y$ has the displayed conditional [binomial distribution](binomial-distribution.md). The [probability generating function of an independent random sum](probability-generating-function-of-an-independent-random-sum.md) gives $G_Y(s)=G_N(1-r+rs)$. If $N$ has finite [variance](variance-split.md), the [law of total expectation](law-of-total-expectation.md) and [law of total variance](law-of-total-variance.md) give

$$
\mathbb E Y=r\mathbb E N,\qquad\operatorname{Var}(Y)=r(1-r)\mathbb E N+r^2\operatorname{Var}(N).
$$

The first term is the average conditional [variance](variance-split.md) of the independent retention decisions; the second is the [variance](variance-split.md) in their conditional [expected value](expected-value-split.md).

**Table of contents**

- [Binomial thinning of a geometric random variable](binomial-thinning-of-a-geometric-random-variable.md)

## ↑ Ancestors (7)

1. [Random sum](random-sum.md)
2. [Random variable](random-variable-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Binomial thinning of a geometric random variable](binomial-thinning-of-a-geometric-random-variable.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/8/b/i/solution.md)
