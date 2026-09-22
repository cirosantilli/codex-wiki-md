# Natural conjugate credibility identity

↑ **Parent:** [Natural conjugate prior](natural-conjugate-prior.md)

For a positive-support [exponential family](exponential-family-split.md) $f(x\mid\theta)=p(x)e^{-\theta x}/q(\theta)$, normalization gives $m(\theta)=-q'(\theta)/q(\theta)$. The [natural conjugate prior](natural-conjugate-prior.md) proportional to $q(\theta)^{-k}e^{-k\mu\theta}$ has logarithmic derivative $k(m(\theta)-\mu)$. If its endpoint density values vanish, integration gives prior [expected value](expected-value.md) $\mathbb E[m(\Theta)]=\mu$. Observations update $k$ to $k+n$ and $\mu$ to $(k\mu+\sum_i x_i)/(k+n)$. The [endpoint control for a Laplace-family conjugate posterior](endpoint-control-for-a-laplace-family-conjugate-posterior.md) justifies the same mean identity after updating, giving an exact [credibility estimate](credibility-estimate.md) with [credibility factor](credibility-factor.md) $n/(n+k)$.

**Table of contents**

- [Endpoint control for a Laplace-family conjugate posterior](endpoint-control-for-a-laplace-family-conjugate-posterior.md)

## ↑ Ancestors (9)

1. [Natural conjugate prior](natural-conjugate-prior.md)
2. [Conjugate prior](conjugate-prior.md)
3. [Exponential family](exponential-family-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Credibility estimate](credibility-estimate.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40/4/solution.md)
