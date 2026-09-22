# Threshold semidefinite program for the largest eigenvalues

↑ **Parent:** [Sum of the largest eigenvalues](sum-of-the-largest-eigenvalues.md)

The [sum of the largest eigenvalues](sum-of-the-largest-eigenvalues.md) has the [semidefinite program](semidefinite-programming.md) representation

$$
F_k(X)=\min_{t\in\mathbb R,\ S\succeq0}\{kt+\operatorname{tr}S:S\succeq X-tI\}.
$$

For every feasible $Y$ in the [fantope](fantope.md), [positive semidefinite trace nonnegativity](positive-semidefinite-trace-nonnegativity.md) gives $\operatorname{tr}(XY)\leq kt+\operatorname{tr}S$. To attain equality, use an [orthonormal eigenbasis](orthonormal-eigenbasis.md) of $X$ and choose $S=\operatorname{diag}((\lambda_i-t)_+)$ in that basis, with the same threshold choice as in the [threshold formula for the sum of the largest components](threshold-formula-for-the-sum-of-the-largest-components.md). This argument also covers $k=n$, without requiring strict feasibility of the maximization program.

## ↑ Ancestors (7)

1. [Sum of the largest eigenvalues](sum-of-the-largest-eigenvalues.md)
2. [Support function](support-function.md)
3. [Convex set](convex-set.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/1/e/solution.md)
