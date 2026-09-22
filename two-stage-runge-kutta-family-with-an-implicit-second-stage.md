# Two-stage Runge-Kutta family with an implicit second stage

↑ **Parent:** [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)

For stages $k_1=f(y)$ and $k_2=f(y+(1-a)hk_1+ahk_2)$ with update $y+h(k_1+k_2)/2$, the method has order two for every fixed real $a$. The third-order coefficient of $f''f^2$ is always $1/4$, not $1/6$, so no parameter gives third order on general nonlinear equations. The displayed [stability function](stability-function.md) is bounded throughout the left half-plane only when $a=1/2$, when it is the A-stable trapezoidal function $(1+z/2)/(1-z/2)$. It is not L-stable.

## ↑ Ancestors (7)

1. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
2. [Runge-Kutta method](runge-kutta-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/38a/a/solution.md)
