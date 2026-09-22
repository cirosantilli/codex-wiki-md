<h1 id="30a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\widehat f(\xi)=\int e^{-ix\xi}f(x)dx$. For a [Schwartz function](../../../../../../schwartz-function.md), [Fourier inversion](../../../../../../fourier-inversion-theorem.md) is $f(x)=(2\pi)^{-1}\int e^{ix\xi}\widehat f(\xi)d\xi$. For a [tempered distribution](../../../../../../tempered-distribution.md) define $\langle\widehat T,\phi\rangle=\langle T,\widehat\phi\rangle$ for [Schwartz functions](../../../../../../schwartz-function.md); this agrees with the function transform in the stated convention. The half-indicator kernel has transform

$$
\widehat F_t(\xi)=\frac12\int_{-t}^t e^{-ix\xi}dx
=\frac{\sin(t\xi)}\xi,
$$

with value $t$ at zero. Transforming the [wave equation](../../../../../../wave-equation-split.md) gives $\widehat u_{tt}+\xi^2\widehat u=0$, zero initial value and initial derivative $\widehat g$. Hence $\widehat u=\widehat g\sin(t\xi)/\xi$, and convolution yields

$$
\boxed{u(t,x)=\frac12\int_{x-t}^{x+t}g(s)ds}.
$$

[Finite propagation speed](../../../../../../finite-propagation-speed.md) means that the solution at $(t,x)$ depends only on initial data in this interval, so disturbances cannot travel faster than one. The formula also makes sense for any smooth $g$, regardless of its growth at infinity, because the integration interval is compact. Direct differentiation verifies the equation and both initial conditions. Equivalently, locally replace $g$ by a compactly supported smooth function agreeing throughout the relevant domain of dependence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30A](../../30a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
