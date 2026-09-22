# Estimation of a beta shape parameter

↑ **Parent:** [Beta distribution](beta-distribution.md)

For an independent [statistical sample](statistical-sample.md) from the [beta distribution](beta-distribution.md) with parameters $(\theta,1)$, $\theta>0$, the [probability density function](probability-density-function.md) is $\theta x^{\theta-1}$ on $(0,1)$. Its [raw moments](raw-moment.md) are $\mathbb E X^r=\theta/(\theta+r)$ for $r> -\theta$, by direct [integration](integral-split.md). Consequently the [method of moments](method-of-moments-statistics.md) gives $T_1=\bar X/(1-\bar X)$, whereas the [maximum-likelihood estimator](maximum-likelihood-estimator.md) is $T_2=-n/\sum_i\log X_i$.

The second formula follows by setting the [score function](informant-function.md) $n/\theta+\sum_i\log X_i$ to zero; its [derivative](derivative.md) is negative. Also $-\log X_i$ has an [exponential distribution](exponential-distribution.md) of rate $\theta$, since $\mathbb P(-\log X_i>u)=e^{-\theta u}$. The [central limit theorem](central-limit-theorem.md) and [delta method](delta-method.md) give

$$
\sqrt n(T_1-\theta)\xrightarrow dN\left(0,\frac{\theta(\theta+1)^2}{\theta+2}\right),\qquad
\sqrt n(T_2-\theta)\xrightarrow dN(0,\theta^2).
$$

Thus the [asymptotic relative efficiency](asymptotic-relative-efficiency.md) of $T_1$ relative to $T_2$ is $1-(\theta+1)^{-2}$. The transformed sum has a [gamma distribution](gamma-distribution.md) of shape $n$ and rate $\theta$, which also gives $\mathbb E T_2=n\theta/(n-1)$ for $n>1$ and $\operatorname{Var}(T_2)=n^2\theta^2/[(n-1)^2(n-2)]$ for $n>2$.

## ↑ Ancestors (7)

1. [Beta distribution](beta-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/1/a/i/solution.md)
