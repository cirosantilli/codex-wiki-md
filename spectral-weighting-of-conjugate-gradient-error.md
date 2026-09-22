# Spectral weighting of conjugate gradient error

↑ **Parent:** [Conjugate gradient method](conjugate-gradient-method.md)

For a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md), choose an orthonormal eigenbasis and write the exact solution as $x=\sum_i\alpha_iv_i$. Starting at zero, the [conjugate gradient method](conjugate-gradient-method.md) chooses an admissible polynomial $p(0)=1$ of degree at most the iteration count that minimizes the displayed error. The weights depend on both the eigenvalues and the solution coefficients. For two eigenvalues $1,L$, the first polynomial is $1-\eta t$, with $\eta=(\alpha^2+\beta^2L^2)/(\alpha^2+\beta^2L^3)$. Comparable nonzero coefficients and large $L$ give $\eta\approx1/L$, so the high-eigenvalue error is removed first. A sufficiently tiny high-mode coefficient changes this behavior; the spectrum alone does not determine the first step.

## ↑ Ancestors (7)

1. [Conjugate gradient method](conjugate-gradient-method.md)
2. [Gradient descent](gradient-descent-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-approximation-course-of-the-university-of-oxford/2008/4/b/solution.md)
