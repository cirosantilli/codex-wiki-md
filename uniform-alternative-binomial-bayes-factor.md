# Uniform-alternative binomial Bayes factor

↑ **Parent:** [Bayes factor](bayes-factor.md)

For a [binomial distribution](binomial-distribution.md) count, compare a point null $\theta=1/2$ with the uniform alternative [prior distribution](prior-probability.md) on $(0,1)$. The alternative [Bayesian model evidence](bayesian-model-evidence.md) is

$$
\binom ny\int_0^1\theta^y(1-\theta)^{n-y}\,d\theta=\frac1{n+1},
$$

so the exact [Bayes factor](bayes-factor.md) favouring the point null is $(n+1)\binom ny2^{-n}$. With standardized deviation $z=2(y-n/2)/\sqrt n$, the local [normal distribution](normal-distribution.md) approximation is $B_{01}\approx\sqrt{2n/\pi}e^{-z^2/2}$. At fixed $z$ the frequentist [p-value](p-value.md) remains approximately constant, while the factor grows like $\sqrt n$. This demonstrates the prior-width mechanism behind the [Jeffreys-Lindley paradox for a Gaussian point null](jeffreys-lindley-paradox-for-a-gaussian-point-null.md) in a discrete sampling model.

## ↑ Ancestors (8)

1. [Bayes factor](bayes-factor.md)
2. [Bayesian model evidence](bayesian-model-evidence.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/d/solution.md)
