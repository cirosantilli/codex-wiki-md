<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one-dimensional [inviscid flow](../../../../inviscid-flow.md), [conservation of mass](../../../../mass-conservation.md) and the [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) are

$$
\partial_t\rho+\partial_x(\rho u)=0,\qquad
\partial_tu+u\partial_xu=-\rho^{-1}\partial_xp.
$$

Substitute $u=U_0+v_1$ and the stated background-plus-perturbation expressions. Dropping products of perturbations gives the [linearization](../../../../linearization.md)

$$
D_0\rho_1+\rho_0\partial_xv_1=0,\qquad
\rho_0D_0v_1=-\partial_xp_1,\qquad D_0=\partial_t+U_0\partial_x.
$$

The [Taylor expansion](../../../../taylor-expansion.md) of the [equation of state](../../../../equation-of-state.md) gives

$$
p_0\left(1+\frac{\rho_1}{\rho_0}\right)^\gamma
=p_0+\frac{\gamma p_0}{\rho_0}\rho_1+O(\rho_1^2),\qquad
\boxed{p_1=c_0^2\rho_1,\quad c_0^2=\left.\frac{dp}{d\rho}\right|_{\rho_0}=\frac{\gamma p_0}{\rho_0}.}
$$

Since the background coefficients are constant, $D_0$ commutes with $\partial_x$. Applying $D_0$ to the linearized [continuity equation](../../../../continuity-equation.md) and using the linearized [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) therefore yields

$$
D_0^2\rho_1=-\rho_0\partial_xD_0v_1=\partial_x^2p_1,
\qquad
\boxed{(\partial_t+U_0\partial_x)^2\rho_1=c_0^2\partial_x^2\rho_1.}
$$

This is the [convected acoustic wave equation](../../../../convected-acoustic-wave-equation.md): in the coordinate $x-U_0t$, it becomes the ordinary [one-dimensional wave equation](../../../../one-dimensional-wave-equation.md). Positive $c_0^2$ is required for propagating [sound waves](../../../../acoustic-wave.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
