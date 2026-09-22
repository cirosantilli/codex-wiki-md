<h1 id="11c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Combining the electric-field equations gives the [Poisson equation](../../../../../../poisson-equation.md) $\nabla^2\phi_i=-\rho_i/\varepsilon_0$. Apply the [product rule for divergence](../../../../../../product-rule-for-divergence.md) to

$$
\mathbf F=\phi_1\nabla\phi_2-\phi_2\nabla\phi_1.
$$

The two cross terms in its [divergence](../../../../../../divergence.md) cancel, leaving

$$
\nabla\cdot\mathbf F=\phi_1\nabla^2\phi_2-\phi_2\nabla^2\phi_1
=\frac{\phi_2\rho_1-\phi_1\rho_2}{\varepsilon_0}.
$$

This [electrostatic reciprocity identity](../../../../../../electrostatic-reciprocity-identity.md) follows from the [divergence theorem](../../../../../../divergence-theorem.md), and is exactly [Green's second identity](../../../../../../green-second-identity.md) for these potentials. Integrating and rearranging gives

$$
\boxed{\frac1{\varepsilon_0}\int_V\phi_1\rho_2\,dV
+\int_{\partial V}\phi_1\nabla\phi_2\cdot d\mathbf S
=\frac1{\varepsilon_0}\int_V\phi_2\rho_1\,dV
+\int_{\partial V}\phi_2\nabla\phi_1\cdot d\mathbf S.}
$$

The boundary orientation is outward from the chosen region. For smooth charge densities this follows directly from classical differentiation. For isolated [point charges](../../../../../../point-charge.md), one may excise small spheres and take their radii to zero, provided the other potential is regular at each charge.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
