# Exposure time for a Poisson rate at fixed fractional precision

↑ **Parent:** [Poisson exposure model](poisson-exposure-model.md)

For an independent count with a [Poisson distribution](poisson-distribution.md) of mean $RT$, the rate estimator $N/T$ has [variance](variance-split.md) $R/T$. Its fractional [standard deviation](standard-deviation.md) is $1/\sqrt{RT}$, so achieving target fractional precision $\epsilon$ requires expected count $RT=\epsilon^{-2}$ and exposure $T=1/(\epsilon^2R)$.

For independently acquired settings with rates $R_i$, the required total exposure is $\epsilon^{-2}\sum_iR_i^{-1}$. Rare settings dominate because they require the same expected count but collect it more slowly. Simultaneous acquisition is a different design, and backgrounds or correlated systematic errors require a different uncertainty calculation.

## ↑ Ancestors (8)

1. [Poisson exposure model](poisson-exposure-model.md)
2. [Generalized linear model](generalized-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-1/section-c/c8/d/solution.md)
