# Non-linear least squares

↑ **Parent:** [Least squares](least-squares.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-linear_least_squares)

Here the residual map $R$ may be nonlinear. Its [Jacobian matrix](jacobian-matrix.md) $J=DR$ gives $\nabla f=J^TR$ and $\nabla^2f=J^TJ+\sum_jR_j\nabla^2R_j$. The [Gauss-Newton algorithm](gauss-newton-algorithm.md) drops the second term to obtain an approximation using only first derivatives of the residuals. Full column rank of $J$ makes $J^TJ$ positive definite; at a zero-residual solution this approximation equals the exact Hessian.

**Table of contents**

- [Gauss-Newton algorithm](gauss-newton-algorithm.md)

## ↑ Ancestors (5)

1. [Least squares](least-squares.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
