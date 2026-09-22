# BFGS method

↑ **Parent:** [Quasi-Newton method](quasi-newton-method.md)

A [quasi-Newton method](quasi-newton-method.md) that maintains a symmetric curvature approximation for differentiable [optimization](mathematical-optimization-split.md). For a [positive-definite symmetric matrix](symmetric-positive-definite-matrix.md) $H$ approximating inverse curvature, step $s$, gradient change $y$ and $\rho=1/(y^{\mathsf T}s)>0$, its inverse update is

$$
H_+=(I-\rho sy^{\mathsf T})H(I-\rho ys^{\mathsf T})+\rho ss^{\mathsf T}.
$$

Multiplying by $y$ gives $H_+y=s$, the inverse form of the [Quasi-Newton secant equation](quasi-newton-secant-equation.md). The update is a [symmetric matrix](symmetric-matrix.md). For any nonzero $v$,

$$
v^{\mathsf T}H_+v=[(I-\rho ys^{\mathsf T})v]^{\mathsf T}H[(I-\rho ys^{\mathsf T})v]+\rho(s^{\mathsf T}v)^2>0.
$$

Both terms are nonnegative, and both can vanish only if $s^{\mathsf T}v=0$ and then $v=0$. Thus positive definiteness is preserved when $y^{\mathsf T}s>0$, making $-H_+\nabla f$ a [descent direction](descent-direction.md) away from a stationary point. Full updates use quadratic storage in the dimension; the method does not require explicit [Hessian matrix](hessian-matrix.md) evaluations. [Superlinear convergence](superlinear-convergence.md) requires additional local smoothness and [line search](line-search.md) assumptions.[Secant condition and low-rank curvature updating; BFGS is the zero-parameter member of the displayed family.](quasi-newton-methods-by-neos-guide.md)

**Table of contents**

- [Limited-memory BFGS](limited-memory-bfgs.md)

## ↑ Ancestors (6)

1. [Quasi-Newton method](quasi-newton-method.md)
2. [Newton's method in optimization](newton-s-method-in-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/i/solution.md)
