# Persistent claim intensity can destroy the discount Markov property

↑ **Parent:** [No claims discount system](no-claims-discount-system.md)

Let a policyholder have one fixed [exponential distribution](exponential-distribution.md) intensity $\Lambda$ of rate $\nu$, with conditionally independent annual [Poisson distribution](poisson-distribution.md) counts. Its one-year marginal count is geometric, but averaging that count does not make the discount process a [Markov chain](markov-chain.md). In the three-level rule, start at zero discount. At time three, the histories $0,\alpha,\beta,\beta$ and $0,0,\alpha,\beta$ both end at the same top level. The first means three no-claim years, giving next no-claim probability $(\nu+3)/(\nu+4)$. The second means a positive count followed by two zero counts, giving $(\nu+2)/(\nu+4)$: divide the integrals of $(1-e^{-\lambda})e^{-(\nu+3)\lambda}$ and $(1-e^{-\lambda})e^{-(\nu+2)\lambda}$. These are distinct, so the [Markov property](markov-property.md) fails when only the current discount is recorded. Conditioning on the intensity, or recording its [Bayesian posterior](bayesian-posterior.md), restores the required predictive information.

## ↑ Ancestors (6)

1. [No claims discount system](no-claims-discount-system.md)
2. [Actuarial statistics](actuarial-statistics-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-35/4/a/solution.md)
