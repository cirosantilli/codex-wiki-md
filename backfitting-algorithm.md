# Backfitting algorithm

↑ **Parent:** [Generalized additive model](generalized-additive-model.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Backfitting_algorithm)

The backfitting algorithm estimates each additive mean function by smoothing its [partial residual](partial-residual.md), obtained after subtracting the current fits of all other terms, and cycling through terms until convergence. Centering each smooth separates its constant part from the intercept. For fixed quadratic smoothness penalties it is block coordinate minimization of a penalized least-squares objective; identifiability and positive definiteness of the constrained problem ensure a unique converged fit. Non-Gaussian [generalized additive models](generalized-additive-model.md) can use weighted backfitting inside [iteratively reweighted least squares](iteratively-reweighted-least-squares.md).

**Table of contents**

- [Linear backfitting equations](linear-backfitting-equations.md)

## ↑ Ancestors (8)

1. [Generalized additive model](generalized-additive-model.md)
2. [Generalized linear model](generalized-linear-model.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Additive regression model](additive-regression-model.md)
- [Linear backfitting equations](linear-backfitting-equations.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/5/d/solution.md)
