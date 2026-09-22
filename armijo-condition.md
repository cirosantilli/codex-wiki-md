# Armijo condition

↑ **Parent:** [Line search](line-search.md)

For $0<\beta_1<1$ and a [descent direction](descent-direction.md) $s$, the [Armijo condition](armijo-condition.md) asks for a decrease at least a fixed fraction $\beta_1$ of the decrease predicted by the first-order [Taylor expansion](taylor-expansion.md). Put $d=\nabla f(x)^Ts<0$. [Differentiability](differentiability.md) gives $f(x+\alpha s)-f(x)-\beta_1\alpha d=(1-\beta_1)\alpha d+o(\alpha)<0$ for all sufficiently small positive $\alpha$. Thus the condition is satisfiable without a second derivative.

## ↑ Ancestors (5)

1. [Line search](line-search.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Armijo condition](armijo-condition.md)
- [Backtracking line search](backtracking-line-search.md)
- [Existence of a Wolfe step](existence-of-a-wolfe-step.md)
- [Line search](line-search.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/a/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/b/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/ii/solution.md)
- [Solution](past-exam-of-the-continuous-optimisation-course-of-the-university-of-oxford/2025/1/c/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/7/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/7/iii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2007/b/7/v/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/4/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2009/b/4/c/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/4/ii/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford/2010/b/4/iii/solution.md)
- [Stationarity from uniformly bounded quasi-Newton matrices](stationarity-from-uniformly-bounded-quasi-newton-matrices.md)
- [Wolfe conditions](wolfe-conditions.md)
