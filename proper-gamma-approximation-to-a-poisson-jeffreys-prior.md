# Proper gamma approximation to a Poisson Jeffreys prior

↑ **Parent:** [Jeffreys prior](jeffreys-prior.md)

A [Poisson distribution](poisson-distribution.md) with mean $E\lambda$ and positive known exposure has [Fisher information](fisher-information-matrix.md) $E/\lambda$, so its [Jeffreys prior](jeffreys-prior.md) kernel is $\lambda^{-1/2}$. The proper shape-rate [gamma distribution](gamma-distribution.md) $\operatorname{Gamma}(1/2,\varepsilon)$ has kernel $\lambda^{-1/2}e^{-\varepsilon\lambda}$, approximating the improper kernel where $\varepsilon\lambda$ is small. Its posterior is $\operatorname{Gamma}(y+1/2,E+\varepsilon)$, converging to $\operatorname{Gamma}(y+1/2,E)$. There is no normalized Jeffreys prior to which the proper priors converge weakly; this is kernel approximation and posterior convergence.

## ↑ Ancestors (9)

1. [Jeffreys prior](jeffreys-prior.md)
2. [Fisher information matrix](fisher-information-matrix.md)
3. [Informant function](informant-function.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/2/c/solution.md)
