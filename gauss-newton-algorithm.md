# Gauss-Newton algorithm

↑ **Parent:** [Non-linear least squares](non-linear-least-squares.md)  
🏷️ **Tags:** [Quasi-Newton method](quasi-newton-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss–Newton_algorithm)

For [nonlinear least squares](non-linear-least-squares.md) $f(x)=\tfrac12\|R(x)\|_2^2$, with residual [Jacobian matrix](jacobian-matrix.md) $J=DR$, the method approximates the Hessian by $J^TJ$. The exact Hessian is $J^TJ+\sum_jR_j\nabla^2R_j$. Full column rank of $J$ makes the approximation positive definite. At a zero-residual solution with full-rank Jacobian, $J(x_k)^TJ(x_k)\to\nabla^2f(x_*)$, so any convergent sequence of full Gauss-Newton steps satisfies the [Dennis-Moré condition](dennis-more-condition.md) and converges superlinearly. A nonzero residual at the solution leaves a generally nonvanishing discarded Hessian term; the same conclusion does not follow automatically.

## ↑ Ancestors (6)

1. [Non-linear least squares](non-linear-least-squares.md)
2. [Least squares](least-squares.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Non-linear least squares](non-linear-least-squares.md)
