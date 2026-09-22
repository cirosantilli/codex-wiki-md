# Poisson-gamma conjugacy

↑ **Parent:** [Bayesian posterior](bayesian-posterior.md)

For conditionally [independent](independent-random-variables.md) [Poisson](poisson-distribution.md) observations of mean $\theta$ and a [gamma distribution](gamma-distribution.md) prior of shape $r>0$ and rate $\lambda>0$, the [likelihood function](likelihood-function.md) contributes $\theta^{\sum_i x_i}e^{-n\theta}$. Multiplying by the [prior density](prior-density.md) gives a [posterior distribution](bayesian-posterior.md) with shape $r+\sum_i x_i$ and rate $\lambda+n$. The single-observation update is shape $r+X$ and rate $\lambda+1$.

The [posterior mean](posterior-mean.md) is the [convex combination](convex-combination.md)

$$
\frac{r+\sum_i x_i}{\lambda+n}=\frac\lambda{\lambda+n}\frac r\lambda+\frac n{\lambda+n}\bar x.
$$

Thus the [prior mean](prior-mean.md) $r/\lambda$ and the sample [maximum-likelihood estimate](maximum-likelihood-estimator.md) $\bar x$ bracket it. Integrating the next conditional [Poisson distribution](poisson-distribution.md) against this [posterior distribution](bayesian-posterior.md) gives the [Poisson-gamma mixture](poisson-gamma-mixture.md), a [negative binomial distribution](negative-binomial-distribution.md); its spread includes uncertainty in $\theta$ as well as the conditional count variation.

**Table of contents**

- [Log-gamma prior for a Poisson log-intercept](log-gamma-prior-for-a-poisson-log-intercept.md)
- [Poisson-gamma conjugacy with unequal exposures](poisson-gamma-conjugacy-with-unequal-exposures.md)

## ↑ Ancestors (7)

1. [Bayesian posterior](bayesian-posterior.md)
2. [Bayesian statistics](bayesian-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-43/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3/28l/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-d/d13/b/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-1/section-d/d13/a/solution.md)
- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2023/3/b/i/solution.md)
- [Poisson mean equality model comparison](poisson-mean-equality-model-comparison.md)
