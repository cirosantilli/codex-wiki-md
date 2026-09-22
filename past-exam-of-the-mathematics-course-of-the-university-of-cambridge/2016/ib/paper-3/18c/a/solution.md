<h1 id="18c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard ideal-fluid assumptions of [incompressible flow](../../../../../../incompressible-flow.md), [inviscid flow](../../../../../../inviscid-flow.md), gravity $-g\mathbf e_y$, and no surface tension. [Irrotational flow](../../../../../../irrotational-flow.md) gives $\mathbf u_j=\nabla\varphi_j$ in each layer, and incompressibility gives [Laplace equation](../../../../../../laplace-equation.md)

$$
\nabla^2\varphi_1=0\quad(\eta<y<h_1),\qquad
\nabla^2\varphi_2=0\quad(-h_2<y<\eta).
$$

The rigid-wall [boundary conditions](../../../../../../boundary-condition.md) are $\varphi_{1y}=0$ at $y=h_1$ and $\varphi_{2y}=0$ at $y=-h_2$. At the moving interface, each fluid has the same normal velocity as the interface:

$$
\boxed{\eta_t+\varphi_{jx}\eta_x=\varphi_{jy}\quad\text{at }y=\eta,\quad j=1,2.}
$$

The dynamic condition is continuity of pressure, $p_1=p_2$ at $y=\eta$. [Bernoulli equation](../../../../../../bernoulli-equation.md) in each fluid reads $\varphi_{jt}+\tfrac12|\nabla\varphi_j|^2+p_j/\rho_j+gy=C_j(t)$. Choosing the potential gauges to subtract a common reference pressure, the interface condition becomes

$$
\boxed{\rho_1\left(\varphi_{1t}+\tfrac12|\nabla\varphi_1|^2+g\eta\right)
=\rho_2\left(\varphi_{2t}+\tfrac12|\nabla\varphi_2|^2+g\eta\right).}
$$

Tangential velocities need not agree across an inviscid interface.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18C](../../18c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
