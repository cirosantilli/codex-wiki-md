# Inverse Gaussian mean estimation

↑ **Parent:** [Inverse Gaussian distribution](inverse-gaussian-distribution.md)

For an independent [statistical sample](statistical-sample.md) from an [Inverse Gaussian distribution](inverse-gaussian-distribution.md) with mean $\mu>0$ and known shape $\lambda>0$, the [maximum-likelihood estimator](maximum-likelihood-estimator.md) of $\mu$ is the [sample mean](sample-mean.md). To prove this, expand the [log-likelihood function](log-likelihood.md) to get $\ell(\mu)=C-\lambda\sum_i y_i/(2\mu^2)+n\lambda/\mu$. Its [score function](informant-function.md) is $\lambda(\sum_i y_i-n\mu)/\mu^3$, positive below $\bar y$ and negative above it. Taking the negative expected second derivative gives one-observation [Fisher information](fisher-information-matrix.md) $I_1(\mu)=\lambda/\mu^3$. Thus the regular [asymptotic normality of a maximum likelihood estimator](asymptotic-normality-of-a-maximum-likelihood-estimator.md) yields $\sqrt n(\bar Y-\mu)\xrightarrow d N(0,\mu^3/\lambda)$. The same conclusion follows from the [central limit theorem](central-limit-theorem.md) and the distribution's [variance](variance-split.md) $\mu^3/\lambda$.

## ↑ Ancestors (8)

1. [Inverse Gaussian distribution](inverse-gaussian-distribution.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2023/1/b/i/solution.md)
