# Dissipative vector field

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)

A real [vector field](vector-field.md) $f$ is dissipative in an [inner product](inner-product.md) if

$$
\langle f(x)-f(y),x-y\rangle\leq0
$$

for all $x,y$. Two solutions of the [ordinary differential equation](ordinary-differential-equation.md) $y'=f(y)$ satisfy

$$
\frac{d}{dt}\|x(t)-y(t)\|^2
=2\langle f(x(t))-f(y(t)),x(t)-y(t)\rangle\leq0.
$$

Thus their distance never increases. The linear case $f(y)=Ay$ recovers the [dissipative operator](dissipative-operator.md) condition. [B-stability](b-stability.md) asks whether a [Runge-Kutta method](runge-kutta-method.md) preserves this contraction for every positive [step size](step-size.md).

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Butcher contractivity theorem](butcher-contractivity-theorem.md)
- [One-sided Lipschitz condition](one-sided-lipschitz-condition.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/6/solution.md)
- [Runge-Kutta contractivity identity](runge-kutta-contractivity-identity.md)
- [Stage solvability of an implicit Runge-Kutta method](stage-solvability-of-an-implicit-runge-kutta-method.md)
- [Trapezoidal rule fails B-stability](trapezoidal-rule-fails-b-stability.md)
