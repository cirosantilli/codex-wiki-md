# Variance of a sample mean

↑ **Parent:** [Expected value](expected-value-split.md)

Let $X_1,\ldots,X_n$ be an [IID sample](independent-and-identically-distributed-random-variables.md) of real-valued [random variables](random-variable-split.md) with finite [expected value](expected-value-split.md) $\mu$ and finite [variance](variance-split.md) $\sigma^2$, where $n\geq1$. Its [sample mean](sample-mean.md) $\overline X=n^{-1}\sum_iX_i$ satisfies

$$
\boxed{\mathbb E[\overline X]=\mu,\qquad\operatorname{Var}(\overline X)=\frac{\sigma^2}{n}.}
$$

[Linearity of expectation](linearity-of-expectation.md) gives the first identity. The [variance of a sum](variance-of-a-sum.md) and vanishing cross [covariances](covariance.md) give $\operatorname{Var}(\sum_iX_i)=n\sigma^2$; scaling by $1/n$ scales the [variance](variance-split.md) by $1/n^2$. [Pairwise independent random variables](pairwise-independent-random-variables.md) with the same [expected value](expected-value-split.md) and [variance](variance-split.md) suffice for these identities, even without full [independence](independent-random-variables.md). Grinstead and Snell state the corresponding finite-variance independent-trials result.[§6.2, Theorems 6.7–6.9, printed pp. 259–260: scaling variance and sums of independent trials](introduction-to-probability-by-charles-m-grinstead-and-j-laurie-snell.md)

The [standard deviation](standard-deviation.md) of the [sample mean](sample-mean.md) is $\sigma/\sqrt n$. Four times as many observations halve this scale; they do not divide it by four. In the fair [Bernoulli distribution](bernoulli-distribution.md) example, $\sigma=1/2$, so sample sizes $4$ and $64$ give standard deviations $1/4$ and $1/16$, respectively. The [common-coin averaging](common-coin-averaging.md) example shows why merely repeating observations with a common marginal law does not justify this calculation.

[Chebyshev's inequality](chebyshev-s-inequality.md) turns the [variance](variance-split.md) identity into a probability bound: for $\varepsilon>0$,

$$
\mathbb P(|\overline X-\mu|\geq\varepsilon)\leq\frac{\sigma^2}{n\varepsilon^2}.
$$

This proves [convergence in probability](convergence-in-probability.md) of the [sample mean](sample-mean.md) to $\mu$ in this finite-variance setting, a form of the [weak law of large numbers](weak-law-of-large-numbers.md). It is an upper bound, so values above one convey no improvement over the universal [probability](probability.md) bound one. [Cauchy sample mean stability](cauchy-sample-mean-has-an-unchanged-distribution.md) lies outside these hypotheses.

## ↑ Ancestors (6)

1. [Expected value](expected-value-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chebyshev's inequality](chebyshev-s-inequality.md)
- [Independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/4/solution.md)
