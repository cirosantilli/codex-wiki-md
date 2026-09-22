# Quasi-Newton secant equation

↑ **Parent:** [Quasi-Newton method](quasi-newton-method.md)

For $p_k=x_{k+1}-x_k$ and $y_k=\nabla f(x_{k+1})-\nabla f(x_k)$, the [Quasi-Newton secant equation](quasi-newton-secant-equation.md) requires $B_{k+1}p_k=y_k$. It reproduces the observed change of [gradient](gradient.md) along the latest step. If $B_{k+1}$ is a [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) and $p_k\ne0$, necessarily $p_k^Ty_k=p_k^TB_{k+1}p_k>0$. A [line search](line-search.md) satisfying the weak [Wolfe conditions](wolfe-conditions.md) ensures this: with $p_k=\alpha_ks_k$,

$$
p_k^Ty_k\geq\alpha_k(\beta_2-1)\nabla f(x_k)^Ts_k>0.
$$

This necessary curvature condition is also sufficient for the existence of some [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) mapping $p_k$ to $y_k$. In an [orthonormal basis](orthonormal-basis.md) whose first vector is $p_k/\|p_k\|$, its first column must be $(a,b)^T=y_k/\|p_k\|$, with $a=p_k^Ty_k/\|p_k\|^2>0$. The block [matrix](matrix.md) with first row $(a,b^T)$ and lower-right block $bb^T/a+I$ has a positive [Schur complement](schur-complement.md), so is [positive-definite](positive-definite-bilinear-form.md).

## ↑ Ancestors (6)

1. [Quasi-Newton method](quasi-newton-method.md)
2. [Newton's method in optimization](newton-s-method-in-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [BFGS method](bfgs-method.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/5/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/discrete-mathematics-probability-and-continuous-mathematics/5/c/iii/solution.md)
- [Quasi-Newton method](quasi-newton-method.md)
- [Quasi-Newton secant equation](quasi-newton-secant-equation.md)
- [Wolfe conditions](wolfe-conditions.md)
