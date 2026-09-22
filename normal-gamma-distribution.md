# Normal-gamma distribution

↑ **Parent:** [Conjugate prior](conjugate-prior.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal-gamma_distribution)

A normal-gamma [conjugate prior](conjugate-prior.md) for the mean $\mu$ and [precision parameter](precision-parameter.md) $\tau$ of a [Gaussian distribution](normal-distribution.md) specifies a [Gamma distribution](gamma-distribution.md) $\tau\sim\operatorname{Gamma}(\alpha,\beta)$ in the shape-rate convention and a conditional [Gaussian distribution](normal-distribution.md) $\mu\mid\tau\sim N(\mu_0,(K\tau)^{-1})$. Its joint [probability density function](probability-density-function.md) is proportional to $\tau^{\alpha-1}\sqrt\tau\exp[-\beta\tau-K\tau(\mu-\mu_0)^2/2]$, with $\alpha,\beta,K>0$. For $n$ independent observations with [Gaussian distribution](normal-distribution.md) $N(\mu,\tau^{-1})$, multiplication by the [likelihood](likelihood-function.md) and completing the square gives

$$
K_n=K+n,\quad\mu_n=(K\mu_0+n\bar x)/(K+n),\quad\alpha_n=\alpha+n/2,
$$

and $\beta_n=\beta+\sum_i(x_i-\bar x)^2/2+Kn(\bar x-\mu_0)^2/[2(K+n)]$. The identity behind conjugacy is $K(\mu-\mu_0)^2+\sum_i(x_i-\mu)^2=(K+n)(\mu-\mu_n)^2+\sum_i(x_i-\bar x)^2+Kn(\bar x-\mu_0)^2/(K+n)$.

## ↑ Ancestors (8)

1. [Conjugate prior](conjugate-prior.md)
2. [Exponential family](exponential-family-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/27i/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/7h/solution.md)
