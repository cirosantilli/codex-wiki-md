# Stationarity from uniformly bounded quasi-Newton matrices

↑ **Parent:** [Quasi-Newton method](quasi-newton-method.md)

Suppose $f$ is bounded below, $0\prec B_k\preceq MI$ for one fixed $M$, $B_ks_k=-\nabla f(x_k)$, and $x_{k+1}=x_k+\alpha_ks_k$ satisfies the [Armijo condition](armijo-condition.md) with $\alpha_k\geq C>0$. Then

$$
f(x_k)-f(x_{k+1})\geq\beta_1\alpha_k\nabla f(x_k)^TB_k^{-1}\nabla f(x_k)\geq\frac{\beta_1C}{M}\|\nabla f(x_k)\|^2.
$$

A [telescoping sum](telescoping-sum.md) proves the displayed convergence of a nonnegative [series](series-mathematics.md) and hence $\nabla f(x_k)\to0$. A uniform positive lower bound on the [eigenvalues](eigenvalue.md) of $B_k$ is unnecessary for this conclusion. The conclusion is first-order stationarity; without further assumptions it does not assert convergence of the iterates or attainment of a [global minimum](global-minimum.md).

## ↑ Ancestors (6)

1. [Quasi-Newton method](quasi-newton-method.md)
2. [Newton's method in optimization](newton-s-method-in-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/iii/solution.md)
