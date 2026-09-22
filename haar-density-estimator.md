# Haar density estimator

↑ **Parent:** [Density estimation](density-estimation.md)

A Haar density estimator estimates the [Haar scaling function](haar-scaling-function.md) coefficients by sample averages. It is exactly the [histogram](histogram.md) with cells of width $2^{-j}$. Its expectation is the [Haar projection](haar-projection.md) of the density. If the density has bounded derivative $L$ and is bounded by $B$, its pointwise expected absolute error is at most $L2^{-j}+\sqrt{B2^j/n}$: the first term is the [Haar projection error for a Lipschitz function](haar-projection-error-for-a-lipschitz-function.md), and the second follows from the [variance](variance-split.md) of a cell count and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Choosing $2^j\asymp n^{1/3}$ gives error $O(n^{-1/3})$ while preserving nonnegativity and integral one.

## ↑ Ancestors (7)

1. [Density estimation](density-estimation.md)
2. [Nonparametric statistics](nonparametric-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/3/solution.md)
