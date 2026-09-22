<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\boldsymbol\xi$ be the [Lagrangian displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md). Linearized mass conservation and adiabaticity give

$$
\delta\rho=-\boldsymbol\xi\mathbin\cdot\nabla\rho-\rho\nabla\mathbin\cdot\boldsymbol\xi,
\qquad
\delta p=-\boldsymbol\xi\mathbin\cdot\nabla p-\gamma p\nabla\mathbin\cdot\boldsymbol\xi.
$$

The fixed potential has no Eulerian perturbation, so the linearized momentum equation is

$$
\rho\,\partial_t^2\boldsymbol\xi
=-\nabla\delta p-\delta\rho\,\nabla\Phi.
$$

For the stated [spherical harmonic](../../../../../../spherical-harmonic.md) decomposition,

$$
\Delta\equiv\nabla\mathbin\cdot\boldsymbol\xi
=\frac1{r^2}\frac{d(r^2\xi_r)}{dr}
-\frac{\ell(\ell+1)}{r^2}\xi_h.
$$

Taking radial and horizontal components and using $g=\Omega^2r$ gives

$$
\boxed{-\rho\omega^2\xi_r=-g\delta\rho-\frac{d\delta p}{dr}},
\qquad
\boxed{-\rho\omega^2\xi_h=-\delta p},
$$



$$
\boxed{\delta\rho=-\xi_r\frac{d\rho}{dr}-\rho\Delta},
\qquad
\boxed{\delta p=-\xi_r\frac{dp}{dr}-\gamma p\Delta}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
