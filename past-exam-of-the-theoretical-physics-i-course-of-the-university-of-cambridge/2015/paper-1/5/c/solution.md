<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Treat $\phi$ and $\phi^*$ as independent fields, keep $A_\mu(x)$ as the prescribed background, and use the source's interaction with no added $e^2A^2|\phi|^2$ term. The momentum derivatives are

$$
\frac{\partial\mathcal L}{\partial(\partial_\mu\phi)}
=\partial^\mu\phi^*-ieA^\mu\phi^*,\qquad
\frac{\partial\mathcal L}{\partial(\partial_\mu\phi^*)}
=\partial^\mu\phi+ieA^\mu\phi.
$$

Varying $\phi^*$ and $\phi$ gives respectively

$$
\boxed{(\Box+m^2)\phi+ie(\partial_\mu A^\mu)\phi
+2ieA^\mu\partial_\mu\phi=0,}
$$



$$
\boxed{(\Box+m^2)\phi^*-ie(\partial_\mu A^\mu)\phi^*
-2ieA^\mu\partial_\mu\phi^*=0.}
$$

No [Lorenz gauge condition](../../../../../lorenz-gauge-condition.md) has been assumed. The background [divergence](../../../../../divergence.md) term must be retained unless such a condition is separately imposed.

The [canonical momenta](../../../../../canonical-momentum.md) conjugate to the two scalar fields are

$$
\pi=\dot\phi^*-ieA_0\phi^*,\qquad
\pi^*=\dot\phi+ieA_0\phi,
$$

so $\dot\phi=\pi^*-ieA_0\phi$ and $\dot\phi^*=\pi+ieA_0\phi^*$. Define the physical three-vector potential by $A_\mu=(A_0,-\mathbf A)$. The [Legendre transform](../../../../../convex-conjugate.md) in the proper [canonical variables](../../../../../canonical-variables.md) is

$$
\boxed{\begin{aligned}
\mathcal H(\phi,\phi^*,\pi,\pi^*;x,t)
={}&(\pi+ieA_0\phi^*)(\pi^*-ieA_0\phi)
+\boldsymbol\nabla\phi^*\cdot\boldsymbol\nabla\phi+m^2|\phi|^2\\
&-ie\mathbf A\cdot(\phi\boldsymbol\nabla\phi^*-\phi^*\boldsymbol\nabla\phi).
\end{aligned}}
$$

Equivalently the first product is $\pi\pi^*+ieA_0(\phi^*\pi^*-\phi\pi)+e^2A_0^2|\phi|^2$. The last quadratic term arises from replacing velocities by [canonical momenta](../../../../../canonical-momentum.md) even though the original [Lagrangian](../../../../../lagrangian.md) has no quadratic interaction. It is not permission to modify the specified [Lagrangian](../../../../../lagrangian.md). An explicitly time-dependent background generally makes the scalar-field energy time dependent.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
