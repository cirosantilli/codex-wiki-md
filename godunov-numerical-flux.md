# Godunov numerical flux

↑ **Parent:** [Numerical flux](numerical-flux.md)

For a [scalar conservation law](scalar-conservation-law.md) whose flux is a [convex function](convex-function.md), the [Godunov numerical flux](godunov-numerical-flux.md) is the physical flux at the origin of the [entropy solution](entropy-solution.md) of the [Riemann problem](riemann-problem.md) between states $a,b$. It is $\min_{u\in[a,b]}f(u)$ for $a\le b$ and $\max_{u\in[b,a]}f(u)$ for $a>b$. For a [rarefaction wave](rarefaction-wave.md), the [characteristic speed](characteristic-speed.md) is monotone across its states, so the origin sees either an endpoint or a zero-speed minimizing state. For a [shock wave](shock-wave.md), its speed is $(f(a)-f(b))/(a-b)$; the origin sees the left state if this speed is positive and the right state if negative, selecting the larger endpoint flux. Unlike the [Godunov flux](godunov-numerical-flux.md), the [Engquist-Osher flux](engquist-osher-flux.md) at reversed transsonic states may equal $f(a)+f(b)-f(s_*)$.

## ↑ Ancestors (7)

1. [Numerical flux](numerical-flux.md)
2. [Finite volume method](finite-volume-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Godunov numerical flux](godunov-numerical-flux.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/6/solution.md)
