# Coverage probability

↑ **Parent:** [Confidence interval](confidence-interval.md)

The [coverage probability](coverage-probability.md) is the repeated-sampling [probability](probability.md) that a random [confidence interval](confidence-interval.md) contains the fixed true [statistical parameter](statistical-parameter.md). A finite-sample level-$1-\alpha$ procedure has [coverage probability](coverage-probability.md) at least $1-\alpha$ at every admissible [statistical parameter](statistical-parameter.md); exact nominal coverage means equality. An asymptotically calibrated procedure approaches the nominal value as [sample size](sample-size.md) grows, under its stated assumptions. Higher-order [Edgeworth expansions](edgeworth-series.md) can quantify the discrepancy from nominal [coverage probability](coverage-probability.md) when their regularity conditions hold.

Observed coverage in finitely many repetitions is itself random. For $m$ independent repetitions of the exact [normal mean confidence interval with known variance](normal-mean-confidence-interval-with-known-variance.md), the count $K$ of covering [confidence intervals](confidence-interval.md) has [binomial distribution](binomial-distribution.md) $\operatorname{Binomial}(m,0.95)$. At $m=40$, its [expectation](expected-value-split.md) is $38$, but

$$
\mathbb P(K=39)=\binom{40}{39}0.95^{39}0.05\approx0.270552.
$$

Consequently, the 39 successes in the figure are compatible with exact 95% [coverage probability](coverage-probability.md). The guarantee follows from the [pivotal quantity](pivotal-quantity.md)'s [probability distribution](probability-distribution-split.md); the finite observed fraction is an illustration. Also distinguish a [confidence interval](confidence-interval.md) for a fixed [mean](expected-value-split.md) from a [prediction interval](prediction-interval.md) for a future observation: the latter must accommodate the new observation's variation as well as estimation uncertainty.

## ↑ Ancestors (6)

1. [Confidence interval](confidence-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Binomial proportion confidence interval](binomial-proportion-confidence-interval.md)
- [Confidence interval](confidence-interval.md)
- [Consistency identities for a two-sided t-test](consistency-identities-for-a-two-sided-t-test.md)
- [Coverage probability](coverage-probability.md)
- [Credible interval](credible-interval.md)
- [Exponential-mean confidence interval by pivot inversion](exponential-mean-confidence-interval-by-pivot-inversion.md)
- [Normal mean confidence interval with known variance](normal-mean-confidence-interval-with-known-variance.md)
- [Parameter space](parameter-space.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-41/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/undated/prelims/mathematics-iii-resit/9/a/ii/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2014/1/a/ii/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2014/3/a/i/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/1/b/ii/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/1/a/v/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2023/1/b/ii/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2023/3/a/i/solution.md)
- [Sample mean under simple random sampling](sample-mean-under-simple-random-sampling.md)
- [Small normal sample mean confidence interval](small-normal-sample-mean-confidence-interval.md)
- [Statistical inference](statistical-inference-split.md)
- [Wilson score interval](wilson-score-interval.md)
