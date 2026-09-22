# Engquist-Osher flux

↑ **Parent:** [Engquist-Osher method](engquist-osher-method.md)

The Engquist-Osher [numerical flux](numerical-flux.md) is $F(a,b)=f(0)+\int_0^a\max(f\prime(s),0)ds+\int_0^b\min(f\prime(s),0)ds$. It sends positive-speed contributions from the left state and negative-speed contributions from the right state. Its consistency $F(u,u)=f(u)$ and opposite monotonicities in the two arguments yield a [monotone conservative scheme](monotone-conservative-scheme.md) under the appropriate [Courant–Friedrichs–Lewy condition](courant-friedrichs-lewy-condition.md). For the [Inviscid Burgers equation](inviscid-burgers-equation.md), it is $\tfrac12\max(a,0)^2+\tfrac12\min(b,0)^2$.

**Table of contents**

- [Sonic-point splitting of a convex Engquist-Osher flux](sonic-point-splitting-of-a-convex-engquist-osher-flux.md)

## ↑ Ancestors (8)

1. [Engquist-Osher method](engquist-osher-method.md)
2. [Monotone conservative scheme](monotone-conservative-scheme.md)
3. [Finite volume method](finite-volume-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Engquist-Osher method](engquist-osher-method.md)
- [Godunov numerical flux](godunov-numerical-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/6/solution.md)
- [Sonic-point splitting of a convex Engquist-Osher flux](sonic-point-splitting-of-a-convex-engquist-osher-flux.md)
