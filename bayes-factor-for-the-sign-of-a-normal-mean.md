# Bayes factor for the sign of a normal mean

↑ **Parent:** [Bayes factor](bayes-factor.md)

For a [random sample](independent-and-identically-distributed-random-variables.md) $X_i\mid\theta\sim N(\theta,\sigma^2)$ with known $\sigma>0$ and [prior distribution](prior-probability.md) $\theta\sim N(0,\tau^2)$ with $\tau>0$, compare $H_0:\theta<0$ to $H_1:\theta\geq0$. The [prior odds](prior-odds.md) are one by symmetry. [Normal-normal conjugacy](normal-normal-conjugacy-with-known-observation-variance.md) gives a normal [posterior distribution](bayesian-posterior.md) with

$$
\mu_n=\frac{n\tau^2\overline X}{\sigma^2+n\tau^2},\qquad
v_n=\frac{\sigma^2\tau^2}{\sigma^2+n\tau^2}.
$$

Its negative and nonnegative masses are $\Phi(-z)$ and $\Phi(z)$, where

$$
z=\frac{\mu_n}{\sqrt{v_n}}=
\frac{n\tau\overline X}{\sigma\sqrt{\sigma^2+n\tau^2}}.
$$

Since the [Bayes factor](bayes-factor.md) is the [posterior odds](posterior-odds.md) divided by the [prior odds](prior-odds.md),

$$
\boxed{B_{01}=\frac{\Phi(-z)}{\Phi(z)}.}
$$

Here $\Phi$ is the [cumulative distribution function](cumulative-distribution-function.md) of the [standard normal distribution](standard-normal-distribution.md). The ratio decreases with the [sample mean](sample-mean.md). For any threshold $b>0$, the inequality $B_{01}<b$ is equivalent to $\Phi(z)>1/(1+b)$ and hence to

$$
\overline X>
\frac{\sigma\sqrt{\sigma^2+n\tau^2}}{n\tau}
\Phi^{-1}\!\left(\frac1{1+b}\right).
$$

For $b=1/10$, the [quantile](quantile-function.md) is $\Phi^{-1}(10/11)\approx1.33518$, and the equivalent [posterior probability](posterior-probability.md) threshold for $H_0$ is $1/11$. The symmetry and proper normalization of the two hypothesis-conditional priors are essential to replacing the [Bayes factor](bayes-factor.md) by the [posterior odds](posterior-odds.md) directly.

## ↑ Ancestors (8)

1. [Bayes factor](bayes-factor.md)
2. [Bayesian model evidence](bayesian-model-evidence.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2015/3/b/iii/solution.md)
