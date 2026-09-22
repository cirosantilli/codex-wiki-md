# Gaussian-process characterization of Brownian motion

↑ **Parent:** [Brownian motion](brownian-motion-split.md)

A centered [Gaussian process](gaussian-process.md) with [almost surely](almost-sure-convergence.md) continuous [sample paths](sample-path.md) and [covariance](covariance.md) $\mathbb E[B_sB_t]=\min(s,t)$ is standard [Brownian motion](brownian-motion-split.md). Here [Gaussian process](gaussian-process.md) means that every [finite-dimensional distribution](finite-dimensional-distribution.md) is a [multivariate normal distribution](multivariate-normal-distribution.md); having separate [normal distributions](normal-distribution.md) at each time would not suffice. This characterization is stated in [Pitman, Basic Properties of Brownian Motion, Definition 15.2](https://www.stat.berkeley.edu/~pitman/s205s03/lecture15.pdf).

To compute the [Brownian covariance kernel](brownian-covariance-kernel.md) directly, suppose $0\leq s\leq t$. Since $B_t=B_s+(B_t-B_s)$ and the added [Brownian increment](brownian-increment.md) is centered and [independent](independent-random-variables.md) of $B_s$,

$$
\operatorname{Cov}(B_s,B_t)=\mathbb E B_s^2+\mathbb E[B_s(B_t-B_s)]=s+0=s.
$$

Symmetry gives $\min(s,t)$ for arbitrary nonnegative times. For instance, $\operatorname{Cov}(B_1,B_4)=1$ and their [correlation](pearson-correlation-coefficient.md) is $1/\sqrt{1\cdot4}=1/2$. Positions are therefore related even though disjoint [Brownian increments](brownian-increment.md) are [independent](independent-random-variables.md): both positions contain the displacement accumulated during the first unit of time. Conversely, taking differences of $\min(s,t)$ gives zero [covariance](covariance.md) for disjoint increments; their joint [multivariate normal distribution](multivariate-normal-distribution.md) turns this into [independence](independent-random-variables.md).

## ↑ Ancestors (7)

1. [Brownian motion](brownian-motion-split.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/29k/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-201/2/a/ii/solution.md)
