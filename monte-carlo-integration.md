# Monte Carlo integration

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

To calculate $I=\int h(x)p(x)\,dx$, generate independent $X_s$ with density $p$ and average $h(X_s)$. Integrability gives convergence by the [strong law of large numbers](strong-law-of-large-numbers.md); finite [variance](variance-split.md) gives an unbiased estimate with variance $\operatorname{Var}(h(X))/S$. Applying this to indicators estimates probabilities. Correlated [Markov chain Monte Carlo](markov-chain-monte-carlo.md) samples can also approximate the integral, but their error is determined by the chain's dependence rather than the independent-sample variance formula.

**Table of contents**

- [Antithetic variates](antithetic-variates.md)
  - [Antithetic Cauchy-tail integration on a finite interval](antithetic-cauchy-tail-integration-on-a-finite-interval.md)
  - [Minimum-variance combination of unbiased sample means](minimum-variance-combination-of-unbiased-sample-means.md)
    - [Cross-fitted combination of unbiased sample means](cross-fitted-combination-of-unbiased-sample-means.md)

## ↑ Ancestors (5)

1. [Monte Carlo method](monte-carlo-method.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/2/d/solution.md)
- [Pseudorandom number generator](pseudorandom-number-generator.md)
