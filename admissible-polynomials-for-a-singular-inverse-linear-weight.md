# Admissible polynomials for a singular inverse-linear weight

↑ **Parent:** [Weighted least squares](weighted-least-squares.md)

Consider the squared error of approximating $x^n$, $n\ge1$, by a [polynomial](polynomial-split.md) $q$ under a measure containing $dx/x$ on $(0,1)$. This error is finite exactly when $q(0)=0$. A nonzero constant term makes the integrand asymptotic to $q(0)^2/x$, which is not [Lebesgue integrable](lebesgue-integrable-function.md); a vanishing constant term makes $x^n-q(x)=O(x)$, giving an integrable $O(x)$ integrand.

Consequently the full space of [polynomials](polynomial-split.md) of degree at most $n-1$ is not contained in the weighted [L2 space](l2-space-is-a-hilbert-space.md). Its admissible subspace is $\operatorname{span}\{x,\ldots,x^{n-1}\}$, or zero when $n=1$. This finite-dimensional subspace has a unique [orthogonal projection](orthogonal-projection.md) of $x^n$, hence a unique best approximation. Indeed its [Gram matrix](gram-matrix.md) is positive definite: a nonzero polynomial cannot vanish on an interval, so its squared norm is positive. Thus a singular weight can invalidate the proposed full approximation space while still allowing a unique finite-error minimizer in its admissible part. As usual, weighted [L2 spaces](l2-space-is-a-hilbert-space.md) identify functions equal almost everywhere.

## ↑ Ancestors (8)

1. [Weighted least squares](weighted-least-squares.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2008/p/3/d/solution.md)
