# Wolfe conditions

↑ **Parent:** [Line search](line-search.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wolfe_conditions)

For a [continuously differentiable function](continuously-differentiable-function.md), a [descent direction](descent-direction.md) $s$ and $0<\beta_1<\beta_2<1$, the [Wolfe conditions](wolfe-conditions.md) require both the [Armijo condition](armijo-condition.md) and

$$
\nabla f(x+\alpha s)^Ts\geq\beta_2\nabla f(x)^Ts.
$$

This second inequality is the weak curvature condition: the slope must have become less negative. The strong variant instead requires $|\nabla f(x+\alpha s)^Ts|\leq\beta_2|\nabla f(x)^Ts|$. The weak version already guarantees a positive curvature pair for the [Quasi-Newton secant equation](quasi-newton-secant-equation.md).

**Table of contents**

- [Existence of a Wolfe step](existence-of-a-wolfe-step.md)

## ↑ Ancestors (5)

1. [Line search](line-search.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Backtracking line search](backtracking-line-search.md)
- [Existence of a Wolfe step](existence-of-a-wolfe-step.md)
- [Line search](line-search.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/2/i/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/2/ii/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2011/2/iii/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/b/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/6/b/i/solution.md)
- [Quasi-Newton secant equation](quasi-newton-secant-equation.md)
- [Wolfe conditions](wolfe-conditions.md)
- [Zoutendijk theorem](zoutendijk-theorem.md)
