# Within-group and between-group scatter decomposition

↑ **Parent:** [Multivariate analysis of variance](multivariate-analysis-of-variance.md)

For groups with sizes $n_r$, means $\bar x_r$, and overall mean $\bar x$, define $W=\sum_{r,i}(x_{ri}-\bar x_r)(x_{ri}-\bar x_r)^T$ and $B=\sum_r n_r(\bar x_r-\bar x)(\bar x_r-\bar x)^T$. Expanding $x_{ri}-\bar x=(x_{ri}-\bar x_r)+(\bar x_r-\bar x)$ gives total scatter $T=W+B$ because each within-group residual sum vanishes. Both matrices are [positive semidefinite](positive-semidefinite-matrix.md), and $\operatorname{rank}B\leq\min(p,g-1)$. They separate within-group noise from between-group mean separation.

## ↑ Ancestors (10)

1. [Multivariate analysis of variance](multivariate-analysis-of-variance.md)
2. [Analysis of variance](analysis-of-variance.md)
3. [Linear regression](linear-regression-split.md)
4. [Normal linear model](normal-linear-model.md)
5. [Statistical modelling](statistical-modelling-split.md)
6. [Statistical model](statistical-model-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/2/iii/solution.md)
