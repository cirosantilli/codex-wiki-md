<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) $\boldsymbol\xi$, with velocity perturbation $\delta\mathbf u=\partial_t\boldsymbol\xi$. Denote Eulerian perturbations by $\delta$ and the corresponding [Lagrangian pressure perturbation](../../../../../../lagrangian-pressure-perturbation.md) by $\Delta_Lp=\delta p+\boldsymbol\xi\cdot\nabla p$. For adiabatic perturbations, the linearized [mass conservation](../../../../../../mass-conservation.md), momentum, [adiabatic equation of state](../../../../../../adiabatic-equation-of-state.md) and [Poisson equation](../../../../../../poisson-equation.md) are

$$
\boxed{\begin{aligned}
\delta\rho&=-\nabla\cdot(\rho\boldsymbol\xi),\\
\rho\,\partial_t^2\boldsymbol\xi
&=-\nabla\delta p-\delta\rho\,\nabla\Phi-\rho\nabla\delta\Phi,\\
\delta p+\boldsymbol\xi\cdot\nabla p
&=-\gamma p\,\nabla\cdot\boldsymbol\xi,\\
\nabla^2\delta\Phi&=4\pi G\,\delta\rho.
\end{aligned}}
$$

These [self-gravitating adiabatic displacement equations](../../../../../../self-gravitating-adiabatic-displacement-equations.md) retain the perturbation of the star's own [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md). In the uniform-density interior, $\delta\rho=-\rho\nabla\cdot\boldsymbol\xi$, $\nabla\Phi=\omega_d^2\mathbf r$, and $\nabla p=-\rho\omega_d^2\mathbf r$. The [dynamical frequency of a uniform-density star](../../../../../../dynamical-frequency-of-a-uniform-density-star.md) $\omega_d=(GM/R^3)^{1/2}$ sets the natural timescale. For a [normal mode](../../../../../../normal-mode.md) with time factor $e^{-i\omega t}$, replace $\partial_t^2$ by $-\omega^2$. The requested interior analysis needs no surface or exterior matching conditions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
