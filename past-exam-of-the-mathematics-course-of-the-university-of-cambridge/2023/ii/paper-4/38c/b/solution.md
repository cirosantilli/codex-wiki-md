<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [velocity potentials](../../../../../../velocity-potential.md) in the upper, middle and lower domains as $\phi_+$, $\phi_0$ and $\phi_-$. [Irrotational flow](../../../../../../irrotational-flow.md) and [incompressible flow](../../../../../../incompressible-flow.md) imply the [Laplace equation](../../../../../../laplace-equation.md)

$$
\nabla^2\phi_j=0,\qquad j\in\{+,0,-\}.
$$

The [far-field boundary conditions](../../../../../../far-field-boundary-condition.md) are

$$
\nabla\phi_+\longrightarrow U\mathbf e_x\quad(y\to+\infty),
\qquad
\nabla\phi_-\longrightarrow U\mathbf e_x\quad(y\to-\infty).
$$

Every shear layer is a material interface. The exact [kinematic boundary condition](../../../../../../kinematic-boundary-condition.md) at $y=h+\eta$ is

$$
\phi_{+,y}=\eta_t+\phi_{+,x}\eta_x,
\qquad
\phi_{0,y}=\eta_t+\phi_{0,x}\eta_x,
$$

and at $y=-h-\eta$ it is

$$
\phi_{-,y}=-\eta_t-\phi_{-,x}\eta_x,
\qquad
\phi_{0,y}=-\eta_t-\phi_{0,x}\eta_x.
$$

Here each equation is evaluated on the indicated moving interface.

Finally, [pressure continuity](../../../../../../pressure-continuity.md) is the [dynamic boundary condition for an inviscid interface](../../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md). The [Unsteady Bernoulli equation](../../../../../../unsteady-bernoulli-equation.md) gives

$$
\phi_{+,t}+\frac12|\nabla\phi_+|^2
=\phi_{0,t}+\frac12|\nabla\phi_0|^2
\quad(y=h+\eta),
$$



$$
\phi_{-,t}+\frac12|\nabla\phi_-|^2
=\phi_{0,t}+\frac12|\nabla\phi_0|^2
\quad(y=-h-\eta),
$$

after absorbing spatially constant functions of time into the potentials.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
