<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The wing and its forcing are time independent in the co-moving frame, so after transients have propagated away the perturbation is stationary there. Write the background velocity and field as

$$
\mathbf U=-u_0\mathbf e_x,
\qquad
\mathbf B_0=B_0\mathbf e_z,
$$

and take every perturbation to be independent of $y$. The cold-plasma [linearized ideal magnetohydrodynamic equations](../../../../../../linearized-ideal-magnetohydrodynamic-equations.md) are

$$
-\rho_0u_0\partial_x\delta\mathbf u
=\frac1{4\pi}(\nabla\times\delta\mathbf B)\times\mathbf B_0,
$$



$$
-u_0\partial_x\delta\mathbf B
=(\mathbf B_0\mathbin\cdot\nabla)\delta\mathbf u
-\mathbf B_0\nabla\mathbin\cdot\delta\mathbf u.
$$

Their relevant components are

$$
-\rho_0u_0\partial_x\delta u_x
=\frac{B_0}{4\pi}
(\partial_z\delta B_x-\partial_x\delta B_z),
$$



$$
-u_0\partial_x\delta B_x=B_0\partial_z\delta u_x,
\qquad
-u_0\partial_x\delta B_z=-B_0\partial_x\delta u_x.
$$

Differentiate the momentum equation with respect to $x$ and use the two induction relations. With the [Alfvén speed](../../../../../../alfven-speed.md)

$$
u_A^2=\frac{B_0^2}{4\pi\rho_0},
$$

the result is

$$
\boxed{(u_A^2-u_0^2)\frac{\partial^2\delta u_x}{\partial x^2}
+u_A^2\frac{\partial^2\delta u_x}{\partial z^2}=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
