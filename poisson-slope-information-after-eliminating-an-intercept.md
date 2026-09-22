# Poisson slope information after eliminating an intercept

↑ **Parent:** [Poisson regression](poisson-regression.md)

In [Poisson regression](poisson-regression.md) with log means $a+\beta x_i$, the [Fisher information matrix](fisher-information-matrix.md) is $\begin{pmatrix}S_0&S_1\\S_1&S_2\end{pmatrix}$, where $S_j=\sum_i x_i^j\mu_i$. Inverting this matrix gives slope [variance](variance-split.md) $S_0/(S_0S_2-S_1^2)$. Writing $\bar x_\mu=S_1/S_0$ reduces it to the displayed reciprocal weighted sum of squares. Thus a common intercept consumes information about the overall rate, while slope information comes from the spread of the covariates under the mean-count weights. Constant covariates make the two parameters unidentifiable.

## ↑ Ancestors (8)

1. [Poisson regression](poisson-regression.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/2/solution.md)
