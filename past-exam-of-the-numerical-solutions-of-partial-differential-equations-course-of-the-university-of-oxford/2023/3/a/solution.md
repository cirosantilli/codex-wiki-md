<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Backward Euler method](../../../../backward-euler-method.md) in time and the prescribed [central finite differences](../../../../central-finite-difference.md) in space. With $j\in\mathbb Z$ and $m\geq0$, the implicit [finite difference method](../../../../finite-difference-method.md) for the [advection-diffusion equation](../../../../advection-diffusion-equation.md) is

$$
\boxed{\frac{U_j^{m+1}-U_j^m}{\Delta t}+\frac{U_{j+1}^{m+1}-U_{j-1}^{m+1}}{2\Delta x}
=a\frac{U_{j+1}^{m+1}-2U_j^{m+1}+U_{j-1}^{m+1}}{(\Delta x)^2},\qquad U_j^0=u_0(j\Delta x).}
$$

Equivalently, for $\nu=\Delta t/\Delta x$ and $\mu=\Delta t/(\Delta x)^2$, the new time level solves

$$
(\nu/2-a\mu)U_{j+1}^{m+1}+(1+2a\mu)U_j^{m+1}+(-\nu/2-a\mu)U_{j-1}^{m+1}=U_j^m.
$$

The spatial terms are evaluated at the new time level, making this an implicit scheme. On the whole line there are no finite-endpoint [boundary conditions](../../../../boundary-condition.md); in the next part its solution is chosen in the [l2 sequence space](../../../../l2-sequence-space.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
