# Central limit theorem for the sample variance

↑ **Parent:** [Sample variance](sample-variance.md)

Let $X_i$ be real [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md), with [mean](expected-value-split.md) $m$, [variance](variance-split.md) $v$ and finite fourth [central moment](central-moment.md) $\mu_4=\mathbb E[(X_i-m)^4]$. For the [sample variance](sample-variance.md) $S_n^2=(n-1)^{-1}\sum_i(X_i-\overline X_n)^2$, the displayed [convergence in distribution](convergence-in-distribution.md) holds.

Indeed $n^{-1}\sum_i(X_i-\overline X_n)^2=n^{-1}\sum_i(X_i-m)^2-(\overline X_n-m)^2$. The [central limit theorem](central-limit-theorem.md) for the [sample mean](sample-mean.md) implies that $\sqrt n(\overline X_n-m)^2$ tends to zero in [probability](probability.md). Changing the divisor from $n$ to $n-1$ also has negligible effect at this scale, by the [law of large numbers](law-of-large-numbers.md). Apply the [central limit theorem](central-limit-theorem.md) to the [independent](independent-random-variables.md) variables $(X_i-m)^2$, whose [variance](variance-split.md) is $\mu_4-v^2$, and use [Slutsky's theorem](slutsky-theorem.md). Standardization gives a [standard normal distribution](standard-normal-distribution.md) limit when $\mu_4>v^2$. The familiar special case $2v^2$ holds for the [normal distribution](normal-distribution.md) because then $\mu_4=3v^2$.

## ↑ Ancestors (7)

1. [Sample variance](sample-variance.md)
2. [Jackknife bias correction](jackknife-bias-correction.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2021/3/b/ii/solution.md)
