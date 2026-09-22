# Pseudo-Poisson process

↑ **Parent:** [Markov jump process](markov-jump-process.md)

A [Markov chain](markov-chain-split.md) $Z$ with [transition kernel](markov-kernel.md) $K$, sampled at an independent [Poisson process](poisson-process-split.md) $N$ of rate $r$, is a pseudo-Poisson process. Its [infinitesimal generator](infinitesimal-generator-stochastic-processes.md) is $r(K-I)$ and its [transition semigroup](markov-semigroup.md) is $e^{-rt}\sum_{n\geq0}(rt)^nK^n/n!$. Conditioning on $N_t$ proves the latter formula, and differentiation at zero gives the former. Its [resolvent operator](resolvent-of-an-operator.md) is $(\lambda+r)^{-1}\sum_{n\geq0}[r/(\lambda+r)]^nK^n$ for $\lambda>0$, by integrating the nonnegative scalar Poisson weights. The series converge in [operator norm](operator-norm.md) on bounded [Borel measurable functions](borel-measurable-function.md).

## ↑ Ancestors (9)

1. [Markov jump process](markov-jump-process.md)
2. [Continuous-time Markov chain](continuous-time-markov-chain-split.md)
3. [Markov chain](markov-chain-split.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford/2025/1/a/solution.md)
