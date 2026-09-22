# Trapezoidal rule fails B-stability

↑ **Parent:** [Trapezoidal rule](trapezoidal-rule.md)

The [trapezoidal rule](trapezoidal-rule.md) is [A-stable](a-stability.md) but is not [B-stable](b-stability.md). For the [dissipative vector field](dissipative-vector-field.md) $f(y)=-y^3$ at step size one, its uniquely defined step map $T$ obeys $T+T^3/2=y-y^3/2$. At $y=\sqrt2$, $T=0$ and implicit differentiation gives $T'=-2$, so nearby states expand rather than contract. This is a concrete nonlinear obstruction, rather than merely failure of the sufficient [algebraic stability](algebraic-stability-of-a-runge-kutta-method.md) criterion.

## ↑ Ancestors (8)

1. [Trapezoidal rule](trapezoidal-rule.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
