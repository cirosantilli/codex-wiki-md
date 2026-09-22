<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $u_i=u(x_i)$ for the sampled exact solution, and let $e_i=U_i-u_i$. The [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) imply $e_0=e_N=0$. The definition of the [truncation error](../../../../truncation-error.md) $\varphi$ gives the exact discrete equation

$$
-D_x^+D_x^-u_i+u_i+u_i^3=f_i-\varphi_i.
$$

Subtracting it from the numerical equation therefore gives

$$
-D_x^+D_x^-e_i+e_i+(U_i^3-u_i^3)=\varphi_i.
$$

The sign on the right is positive because $\varphi_i$ was defined as the difference approximation minus the exact [second derivative](../../../../second-derivative.md). Multiply by $he_i$, sum over the interior nodes and apply [discrete summation by parts](../../../../discrete-summation-by-parts.md):

$$
\|D_x^-e]\!\|_h^2+\|e\|_h^2+h\sum_{i=1}^{N-1}(U_i^3-u_i^3)e_i=(\varphi,e)_h.
$$

Again $(U_i^3-u_i^3)e_i=e_i^2(U_i^2+U_iu_i+u_i^2)\geq0$. By [Young's inequality for products](../../../../young-s-inequality-for-products.md), $(\varphi,e)_h\leq\tfrac12\|\varphi\|_h^2+\tfrac12\|e\|_h^2$. Hence

$$
\boxed{\|D_x^-U-D_x^-u]\!\|_h^2+\frac12\|U-u\|_h^2\leq\frac12\|\varphi\|_h^2.}
$$

No fourth [derivative](../../../../derivative.md) is needed for this step: the assumed twice continuous differentiability suffices to define $\varphi$ and obtain the discrete [energy estimate](../../../../energy-estimate.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
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
