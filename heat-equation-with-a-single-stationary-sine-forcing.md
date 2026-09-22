# Heat equation with a single stationary sine forcing

↑ **Parent:** [Heat equation](heat-equation.md)

On $0<x<L$, let $u_t=\nu u_{xx}+G\sin(n\pi x/L)$, with $\nu>0$, zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md), and zero initial data. Write $k_n=n\pi/L$. Its stationary solution is $u_s=G\sin(k_nx)/(\nu k_n^2)$. Subtracting it removes the forcing from the [partial differential equation](partial-differential-equation-split.md) and leaves a [heat equation](heat-equation.md) with initial data $-u_s$.

Because the forcing is a single spatial [eigenfunction](eigenfunction.md), [separation of variables](separation-of-variables.md) gives the entire solution without mixing modes:

$$
u(x,t)=\frac{G}{\nu k_n^2}(1-e^{-\nu k_n^2t})\sin(k_nx).
$$

Its integral is $G[1-(-1)^n](1-e^{-\nu k_n^2t})/(\nu k_n^3)$; [even](even-function.md) modes have zero signed net integral. Removing forcing from the evolution equation does not remove its amplitude from the initial data for the transient.

## ↑ Ancestors (7)

1. [Heat equation](heat-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/20/c/solution.md)
