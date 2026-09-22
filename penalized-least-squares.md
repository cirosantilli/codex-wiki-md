# Penalized least squares

↑ **Parent:** [Regularization](regularization.md)

For $\lambda\geq0$, a full-column-rank [design matrix](design-matrix.md) $B$, and a [positive semidefinite matrix](positive-semidefinite-matrix.md) $\Omega$, minimize $\|y-B\beta\|^2+\lambda\beta^T\Omega\beta$. Differentiation gives $(B^TB+\lambda\Omega)\widehat\beta=B^Ty$. The fitted-value matrix is $B(B^TB+\lambda\Omega)^{-1}B^T$, whose trace measures the [effective degrees of freedom](effective-degrees-of-freedom.md).

**Table of contents**

- [Penalized least-squares estimator](penalized-least-squares-estimator.md)
  - [Basic inequality for a penalized least-squares estimator](basic-inequality-for-a-penalized-least-squares-estimator.md)

## ↑ Ancestors (8)

1. [Regularization](regularization.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-206/3/c/solution.md)
- [Roughness-matrix formula for a natural cubic smoothing spline](roughness-matrix-formula-for-a-natural-cubic-smoothing-spline.md)
