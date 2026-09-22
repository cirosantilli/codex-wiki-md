# Bayesian rejection sampling for a segregating-site count

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

With proper prior $\pi(\theta)$ independent of the neutral [Kingman's coalescent](kingman-s-coalescent.md) times, propose $(\theta,T)$ from their joint prior and accept with probability $e^{-\theta L/2}(\theta L/2)^k/k!$. The accepted density is proportional to the prior times the observed-count likelihood, hence is the posterior given $S=k$. The acceptance rate is the prior predictive probability $P(S=k)$. For $k>0$, divide the acceptance function by its maximum $M_k=e^{-k}k^k/k!$, achieved at $\theta L/2=k$, to improve the rate to $P(S=k)/M_k$ without altering the accepted distribution. For $k=0$, $M_0=1$.

**Table of contents**

- [Joint posterior of mutation rate and coalescent times](joint-posterior-of-mutation-rate-and-coalescent-times.md)

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-45/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45/4/d/solution.md)
