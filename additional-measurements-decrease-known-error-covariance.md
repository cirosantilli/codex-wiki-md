# Additional measurements decrease known-error covariance

↑ **Parent:** [Weighted least squares](weighted-least-squares.md)

Independent observations with known errors add a positive-semidefinite [Fisher information matrix](fisher-information-matrix.md) $G$ to the existing information $F$. Writing $F+G=F^{1/2}(I+F^{-1/2}GF^{-1/2})F^{1/2}$ shows its inverse covariance cannot increase in any parameter direction. Improvement can be zero along an uninformative direction. This statement does not assume that data-dependent residual [variance](variance-split.md) estimates or model [systematic errors](systematic-error.md) must decrease.

## ↑ Ancestors (8)

1. [Weighted least squares](weighted-least-squares.md)
2. [Normal linear model](normal-linear-model-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
