<h1 id="38d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The momentum equation is

$$
\rho\left(\partial_tu+(u\cdot\nabla)u\right)
=f+\nabla\cdot\sigma,
\qquad \nabla\cdot u=0.
$$

Taking its scalar product with $u$ gives

$$
\partial_t\left(\frac12\rho|u|^2\right)
+\nabla\cdot\left(\frac12\rho|u|^2u\right)
=u\cdot f+\nabla\cdot(u\cdot\sigma)-\sigma:\nabla u.
$$

For the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) $\sigma=-pI+2\mu e$, its contraction with the velocity gradient is

$$
\sigma:\nabla u=2\mu e:e,
$$

because incompressibility removes the pressure term and the symmetric [rate-of-strain tensor](../../../../../../strain-rate-tensor.md) is orthogonal to the antisymmetric part of $\nabla u$. Integration over $\mathcal D$ and the divergence theorem therefore give the [kinetic-energy balance for an incompressible Newtonian fluid](../../../../../../kinetic-energy-balance-for-an-incompressible-newtonian-fluid.md):

$$
\frac{d}{dt}\int_{\mathcal D}\frac12\rho|u|^2\,dV
+\int_{\partial\mathcal D}\frac12\rho|u|^2u\cdot n\,dS
=\int_{\mathcal D}u\cdot f\,dV
+\int_{\partial\mathcal D}u\cdot\sigma\cdot n\,dS
-2\mu\int_{\mathcal D}e:e\,dV.
$$

The terms are respectively the rate of change of kinetic energy, outward advective flux of kinetic energy, power supplied by the body force, power supplied by surface traction, and irreversible viscous dissipation. Since $f=-\nabla\psi$, the body-force power may also be written $-\nabla\cdot(\psi u)$ and interpreted as exchange with potential energy.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38D](../../38d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
