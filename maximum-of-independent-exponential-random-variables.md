# Maximum of independent exponential random variables

↑ **Parent:** [Extreme value theory](extreme-value-theory-split.md)

Let $n\geq1$ be an [integer](integer-split.md) and let $X_1,\ldots,X_n$ be [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with an [exponential distribution](exponential-distribution.md) of rate $\lambda>0$. Their [sample maximum](sample-maximum.md) $M_n$ is nonnegative. Substituting the [exponential distribution](exponential-distribution.md)'s [cumulative distribution function](cumulative-distribution-function.md) into the [distribution functions of independent minima and maxima](distribution-functions-of-independent-minima-and-maxima.md) gives the exact law

$$
\mathbb P(M_n\leq x)=
\begin{cases}
(1-e^{-\lambda x})^n,&x\geq0,\\
0,&x<0.
\end{cases}
$$

For example, at $x=(\log2)/\lambda$ each observation is below the threshold with [probability](probability.md) $1/2$, but all $n$ observations are below it with [probability](probability.md) $2^{-n}$. Thus an individual observation's [median](median.md) becomes an increasingly unlikely upper bound for the whole batch. The general [order statistic](order-statistic.md) density in Siegrist's treatment, with $k=n$, also gives this law on [integration](integral-split.md). [Siegrist, Random Services: exponential order statistics](https://www.randomservices.org/random/sample/OrderStatistics.html).

Solving $(1-e^{-\lambda x})^n=p$ gives the exact [quantile function](quantile-function.md), for $0<p<1$,

$$
q_n(p)=-\frac1\lambda\log(1-p^{1/n}),\qquad
m_n=q_n(1/2)=-\frac1\lambda\log(1-2^{-1/n}).
$$

In a toy model with $\lambda=1\,\mathrm{s}^{-1}$, the [median](median.md) maximum is $0.693147$ seconds for $n=1$, $2.703555$ seconds for $n=10$, and $4.975147$ seconds for $n=100$. All three use the exact [distribution function](cumulative-distribution-function.md); the increase comes from taking a [maximum](maximum-of-a-subset-of-a-total-order.md) over more observations. The $n=2$ case connects to the existing [maximum of two exponentials as a scaled sum](maximum-of-two-exponentials-as-a-scaled-sum.md).

<a id="image-exact-cumulative-distribution-functions-of-exponential-sample-maxima-with-rate-one-per-second-and-median-markers"></a>
![](exponential-sample-maximum-distributions.png)

**[Figure 1](#image-exact-cumulative-distribution-functions-of-exponential-sample-maxima-with-rate-one-per-second-and-median-markers). Exact cumulative distribution functions of exponential sample maxima, with rate one per second and median markers**.

The [Gumbel distribution](gumbel-distribution.md) explains the logarithmic shift visible here: after subtracting $(\log n)/\lambda$ and measuring deviations in units of $1/\lambda$, the [distribution functions](cumulative-distribution-function.md) approach one fixed shape. The next derivation makes that [convergence in distribution](convergence-in-distribution.md) explicit.

## ↑ Ancestors (6)

1. [Extreme value theory](extreme-value-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Extreme value theory](extreme-value-theory-split.md)
- [Gumbel distribution](gumbel-distribution.md)
