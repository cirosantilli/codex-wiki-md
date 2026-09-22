<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $m=\mathbb EX$ and $v=\operatorname{Var}(X)$, evaluated from the given [polylogarithm](../../../../../polylogarithm.md) formulas. Generate a large sample of [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with `r_sample_f`, and compute its [sample mean](../../../../../sample-mean.md) $\overline X_n$ and [sample variance](../../../../../sample-variance.md) $S_n^2$ using `mean` and `var`. The [central limit theorem](../../../../../central-limit-theorem.md) gives the first standardized check:

$$
\boxed{Z_m=\frac{\sqrt n(\overline X_n-m)}{\sqrt v}\ \Rightarrow\ N(0,1).}
$$

For the second check, the correct asymptotic [variance](../../../../../variance-split.md) of the [sample variance](../../../../../sample-variance.md) involves the fourth [central moment](../../../../../central-moment.md) $\mu_4=\mathbb E[(X-m)^4]$:

$$
\boxed{Z_v=\frac{\sqrt n(S_n^2-v)}{\sqrt{\mu_4-v^2}}\ \Rightarrow\ N(0,1).}
$$

The denominator is not $\sqrt{2v^2}$ unless the [probability distribution](../../../../../probability-distribution-split.md) has the requisite fourth [central moment](../../../../../central-moment.md), as does the [normal distribution](../../../../../normal-distribution.md). Here the [probability density function](../../../../../probability-density-function.md) decays exponentially, so all required [moments](../../../../../moment.md) are finite.

To compute $\mu_4$, expand the denominator of the [probability density function](../../../../../probability-density-function.md) as a [geometric series](../../../../../geometric-series.md) and integrate each nonnegative term. The [gamma function](../../../../../gamma-function.md) integral gives the [raw moments](../../../../../raw-moment.md)

$$
m_j:=\mathbb E[X^j]
=-\frac{j!\operatorname{Li}_{j+1}(1-p)}{\beta^j\log p},\qquad j\geq1.
$$

Thus $v=m_2-m_1^2$ and $\mu_4=m_4-4m_1m_3+6m_1^2m_2-3m_1^4$. The following [R](../../../../../r-programming-language.md) code implements both checks for chosen interior parameters and large `n`:

```
p <- 0.4
beta <- 1.3
n <- 100000
raw_m <- vapply(1:4, function(j) {
  -factorial(j) * polylog(j + 1, 1 - p) / (beta^j * log(p))
}, numeric(1))
m <- raw_m[1]
v <- raw_m[2] - m^2
mu4 <- raw_m[4] - 4 * m * raw_m[3] +
  6 * m^2 * raw_m[2] - 3 * m^4
x <- r_sample_f(n, p, beta)
c(mean_check = sqrt(n) * (mean(x) - m) / sqrt(v),
  variance_check = sqrt(n) * (var(x) - v) / sqrt(mu4 - v^2))
```

For each check separately, an absolute value below $1.96$ is consistent with its approximate $95\%$ [confidence interval](../../../../../confidence-interval.md). Repeat with many [independent](../../../../../independent-random-variables.md) samples: the two standardized statistics should each resemble a [standard normal distribution](../../../../../standard-normal-distribution.md), with about $5\%$ outside that range. Also vary $p$, $\beta$ and `n`; a systematic discrepancy that grows with $\sqrt n$ suggests a bias. The two checks from the same sample are generally dependent, so passing both is not itself a joint $95\%$ statement, nor can a finite test prove that a generator is correct.

The second [central limit theorem](../../../../../central-limit-theorem.md) follows from the [central limit theorem for the sample variance](../../../../../central-limit-theorem-for-the-sample-variance.md): $\sqrt n(S_n^2-v)$ differs by a quantity tending to zero in [probability](../../../../../probability.md) from $n^{-1/2}\sum_i[(X_i-m)^2-v]$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
