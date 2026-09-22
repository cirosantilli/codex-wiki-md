# Exponential Laplace martingale of a compound Poisson process

↑ **Parent:** [Compound Poisson process](compound-poisson-process.md)

Let $Y_t=\sum_{j=1}^{N_t}X_j$ for a rate-$\lambda$ [Poisson process](poisson-process.md) and [independent and identically distributed](independent-and-identically-distributed-random-variables.md) nonnegative marks independent of that process, with $\phi(q)=\mathbb E e^{-qX_1}$. The [Laplace transform of a nonnegative random variable](laplace-transform-of-a-nonnegative-random-variable.md) for the increment over $[s,t]$ is $\exp[\lambda(t-s)(\phi(q)-1)]$. That increment is independent of the past of $Y$, so the displayed nonnegative process has mean one and satisfies $\mathbb E[Z_t\mid\sigma(Y_u:u\leq s)]=Z_s$. No finite first moment of the marks is needed for this [martingale](martingale-split.md) when $q\geq0$.

## ↑ Ancestors (8)

1. [Compound Poisson process](compound-poisson-process.md)
2. [Lévy process](levy-process.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/5/c/solution.md)
