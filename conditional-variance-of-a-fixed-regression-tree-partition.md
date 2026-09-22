# Conditional variance of a fixed regression-tree partition

↑ **Parent:** [Regression tree](regression-tree.md)

For a deterministic partition $R_1,\ldots,R_J$ and

$$
\widetilde\gamma_j=\frac1{N_j+1}
\sum_{i=1}^nY_i\mathbf1_{R_j}(X_i),
$$

conditional independence gives

$$
\operatorname{Var}(\widetilde\gamma_j\mid X_{1:n})
=\frac{\sum_i\operatorname{Var}(Y_i\mid X_i)\mathbf1_{R_j}(X_i)}
{(N_j+1)^2}.
$$

If the conditional response variance is at most $\sigma^2$, the prediction variance at an independent test point is at most $\sigma^2J/n$.

## ↑ Ancestors (7)

1. [Regression tree](regression-tree.md)
2. [Decision tree learning](decision-tree-learning.md)
3. [Statistical learning theory](statistical-learning-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-2/31k/b/solution.md)
