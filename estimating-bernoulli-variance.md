# Estimating Bernoulli variance

↑ **Parent:** [Bernoulli distribution](bernoulli-distribution.md)

For $n\geq2$ independent Bernoulli observations with sum $K$, the extended maximum-likelihood estimator is $\widehat\phi=(K/n)(1-K/n)$. Its unbiased improvement is $K(n-K)/[n(n-1)]=n\widehat\phi/(n-1)$, obtained by conditioning $X_1(1-X_2)$ on $K$. The [Rao-Blackwell theorem](rao-blackwell-theorem.md) gives strict variance reduction for $0<\theta<1$. With a uniform prior on $\theta$ and squared-error loss for $\phi$, the Bayes estimator is $(K+1)(n-K+1)/[(n+2)(n+3)]$. For parameter space strictly $(0,1)$, samples with $K=0$ or $n$ have only a boundary likelihood supremum, not an attained maximum.

## ↑ Ancestors (8)

1. [Bernoulli distribution](bernoulli-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/18c/i/solution.md)
