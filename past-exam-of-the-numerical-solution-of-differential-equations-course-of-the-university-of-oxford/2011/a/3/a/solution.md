<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\delta_{xx}U_{ij}=(U_{i+1,j}-2U_{ij}+U_{i-1,j})/(\Delta x)^2$, and define $\delta_{yy}$ analogously. The [Crank-Nicolson diffusion scheme](../../../../../crank-nicolson-diffusion-scheme.md) is

$$
\boxed{\frac{U_{ij}^{m+1}-U_{ij}^m}{\Delta t}
=\frac12(\delta_{xx}+\delta_{yy})(U_{ij}^{m+1}+U_{ij}^m),\qquad1\leq i,j\leq N-1.}
$$

Use $U_{ij}^0=u_0(x_i,y_j)$ and zero values on every boundary node for every time level. This is the [theta method](../../../../../theta-method.md) with $\theta=1/2$ applied to the spatial [finite difference method](../../../../../finite-difference-method.md) for the [heat equation](../../../../../heat-equation.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
