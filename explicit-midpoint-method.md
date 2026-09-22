# Explicit midpoint method

↑ **Parent:** [Midpoint method](midpoint-method.md)

This [explicit numerical method](explicit-numerical-method.md) is a two-stage [Runge-Kutta method](runge-kutta-method-split.md) and a [one-step method](one-step-method.md). For a sufficiently smooth [ordinary differential equation](ordinary-differential-equation.md), the [chain rule](chain-rule.md) gives $y''=f_x+f_yf$, and [Taylor's theorem](taylor-s-theorem.md) shows that its [local truncation error](local-truncation-error.md) is $O(h^3)$. Uniform [Lipschitz continuity](lipschitz-continuity.md) of $f$ in its solution argument gives an increment-function [Lipschitz constant](lipschitz-constant.md) at most $L(1+hL/2)$. The [Lipschitz one-step error bound](lipschitz-one-step-error-bound.md) then proves second-order [numerical convergence](convergence-of-a-numerical-method.md) on a fixed time interval. This method uses an intermediate prediction from $y_n$; the [explicit midpoint linear multistep method](explicit-midpoint-linear-multistep-method.md) instead requires a separate previous value $y_{n-1}$.

## ↑ Ancestors (6)

1. [Midpoint method](midpoint-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2020/1/b/solution.md)
- [Solution](past-exam-of-the-numerical-linear-algebra-and-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2020/1/c/solution.md)
