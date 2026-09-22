<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $\delta\mathbf u=-i\omega\boldsymbol\xi$. The continuity and adiabatic equations give the Lagrangian perturbations

$$
\frac{\Delta_L\rho}{\rho}=-\Delta,
\qquad
\frac{\Delta_Lp}{p}=-\gamma\Delta,
\qquad
\Delta=ik_x\xi_x+\frac{d\xi_z}{dz}.
$$

Because the equilibrium is a [neutrally stratified polytropic atmosphere](../../../../../../neutrally-stratified-polytropic-atmosphere.md), $p\propto\rho^\gamma$, so the displacement terms cancel and

$$
\boxed{\frac{\delta p}{p}=\gamma\frac{\delta\rho}{\rho}}.
$$

Using $dp/dz=-\rho g$ then gives

$$
\boxed{\Psi=\frac{\delta p}{\rho}
=g\xi_z-v_s^2\Delta},
\qquad
v_s^2=\frac{\gamma p}{\rho}.
$$

Eliminating $\xi_y$ from the two horizontal momentum equations and combining gravity with the vertical pressure force yields

$$
\boxed{-(\omega^2-4\Omega^2)\xi_x=-ik_x\Psi},
\qquad
\boxed{-\omega^2\xi_z=-\frac{d\Psi}{dz}}.
$$

Thus

$$
\xi_x=\frac{ik_x\Psi}{\omega^2-4\Omega^2},
$$

and the requested coupled first-order system is

$$
\boxed{
\frac{d\Psi}{dz}=\omega^2\xi_z,
\qquad
\frac{d\xi_z}{dz}
=\frac{g}{v_s^2}\xi_z
+\left(\frac{k_x^2}{\omega^2-4\Omega^2}
-\frac1{v_s^2}\right)\Psi}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
