<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [forward Euler method](../../../../euler-method.md) in time and evaluate both spatial [finite difference operators](../../../../finite-difference-operator.md) at the old time level:

$$
\boxed{\frac{U_j^{m+1}-U_j^m}{\Delta t}+\frac{U_{j+1}^{m}-U_{j-1}^{m}}{2\Delta x}
=a\frac{U_{j+1}^{m}-2U_j^{m}+U_{j-1}^{m}}{(\Delta x)^2},\qquad U_j^0=u_0(j\Delta x).}
$$

With $\nu=\Delta t/\Delta x$ and $\mu=\Delta t/(\Delta x)^2$, the explicit update is

$$
\boxed{U_j^{m+1}=(a\mu+\nu/2)U_{j-1}^m+(1-2a\mu)U_j^m+(a\mu-\nu/2)U_{j+1}^m.}
$$

Every value on the new time level is computed directly from three old values. The sum of the stencil weights is one, as required to preserve constant solutions of the [advection-diffusion equation](../../../../advection-diffusion-equation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
