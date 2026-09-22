# Wilson score interval

↑ **Parent:** [Binomial proportion confidence interval](binomial-proportion-confidence-interval.md)

For $K\sim\operatorname{Bin}(n,p)$, $n>0$, put $\widehat p=K/n$ and let $z$ be the $1-\alpha/2$ [quantile](quantile-function.md) of the [standard normal distribution](standard-normal-distribution.md). Inverting the approximate [score test](score-test.md) retains precisely the parameters satisfying

$$
\frac{n(\widehat p-p)^2}{p(1-p)}\le z^2.
$$

Multiplication and collection of terms gives the [quadratic inequality](quadratic-inequality.md)

$$
(n+z^2)p^2-(2n\widehat p+z^2)p+n\widehat p^2\le0.
$$

Its two roots are the displayed endpoints. The [Wilson score interval](wilson-score-interval.md) stays within $[0,1]$ and remains nontrivial when $K=0$ or $K=n$, unlike the unmodified [Wald confidence interval](wald-confidence-interval.md). Its [coverage probability](coverage-probability.md) is approximate and varies with $p$; it is not a uniformly exact 95% guarantee. Separate pointwise intervals for several groups are not a simultaneous confidence statement. The method is named after [Edwin Bidwell Wilson](edwin-bidwell-wilson.md).[§7.2.4.1: inversion of the score statistic and endpoint formulas](binomial-proportion-confidence-intervals-by-nist.md)

## ↑ Ancestors (7)

1. [Binomial proportion confidence interval](binomial-proportion-confidence-interval.md)
2. [Confidence interval](confidence-interval.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Binomial Proportion Confidence Intervals by NIST](binomial-proportion-confidence-intervals-by-nist.md)
- [Edwin Bidwell Wilson](edwin-bidwell-wilson.md)
- [Wilson score interval](wilson-score-interval.md)
