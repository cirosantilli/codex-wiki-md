# Asymptotic normality of a normal sample standard deviation

↑ **Parent:** [Sample variance](sample-variance.md)

For a [normal sample](normal-sample.md) of [variance](variance-split.md) $\sigma^2>0$, define $S^2=(n-1)^{-1}\sum_i(X_i-\overline X)^2$. The exact [chi-squared distribution](chi-squared-distribution.md) identity $(n-1)S^2/\sigma^2\sim\chi^2_{n-1}$ and the [central limit theorem](central-limit-theorem.md) for [independent](independent-random-variables.md) squared [standard normal random variables](standard-normal-random-variable.md) imply

$$
\sqrt n(S^2-\sigma^2)\xrightarrow dN(0,2\sigma^4).
$$

The [delta method](delta-method.md) for $g(v)=\sqrt v$, with [derivative](derivative.md) $g'(\sigma^2)=1/(2\sigma)$, therefore gives the displayed limit for $S$. Exact [independence of the normal sample mean and sample variance](independence-of-the-normal-sample-mean-and-sample-variance.md) also makes $S$ independent of $\overline X$. The resulting joint limit supports combining location and scale estimates when a model relates their parameters.

## ↑ Ancestors (7)

1. [Sample variance](sample-variance.md)
2. [Jackknife bias correction](jackknife-bias-correction.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Optimal asymptotic combination of a normal sample mean and standard deviation](optimal-asymptotic-combination-of-a-normal-sample-mean-and-standard-deviation.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2017/1/b/iii/solution.md)
