# Likelihood support reduction under censoring

↑ **Parent:** [Empirical likelihood with mixed censoring](empirical-likelihood-with-mixed-censoring.md)

Partition the time axis into cells on which membership in each observed exact-event or [censoring](censoring-statistics.md) set is constant. Let $w_j$ be a cell's probability mass and $A_{ij}$ indicate whether cell $j$ is permitted by observation $i$. The [empirical likelihood](empirical-likelihood.md) has the displayed form, with nonnegative masses summing to one. Columns of $A$ that agree can be combined. If column $j$ is componentwise dominated by another column $k$, moving all mass from $j$ to $k$ cannot reduce any factor, so an unconstrained [nonparametric maximum-likelihood estimator](nonparametric-maximum-likelihood-estimator.md) can omit column $j$. The remaining [log-likelihood](log-likelihood.md) is a [concave function](concave-function.md) of the masses. Extra constraints can prevent a domination move; for a fixed [survivor function](survival-function.md) value, split cells at the constrained time and retain the associated linear mass constraint.

## ↑ Ancestors (8)

1. [Empirical likelihood with mixed censoring](empirical-likelihood-with-mixed-censoring.md)
2. [Empirical likelihood](empirical-likelihood.md)
3. [Nonparametric statistics](nonparametric-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-44/3/solution.md)
