# Negative binomial information in capture-recapture sampling

↑ **Parent:** [Negative binomial distribution](negative-binomial-distribution.md)

When each observation counts untagged captures before the $r$th tagged capture with immediate replacement, its [negative binomial distribution](negative-binomial-distribution.md) has success probability $p=k/N$. For $n$ independent runs, the log-likelihood is $nr\log p+(\sum_i x_i)\log(1-p)$ plus a constant. Differentiation gives the displayed estimator and expected [Fisher information](fisher-information-matrix.md). For an interior true parameter, its asymptotic variance is $p^2(1-p)/(nr)$. A confidence interval $(L,U)$ for $p$ transforms to $(k/U,k/L)$ for the population size, with endpoint order reversed.

## ↑ Ancestors (8)

1. [Negative binomial distribution](negative-binomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
