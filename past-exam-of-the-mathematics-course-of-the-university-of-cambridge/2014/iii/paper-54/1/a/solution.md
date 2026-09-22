<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D_t=\partial_t+\mathbf u\cdot\nabla$ and $\mathbf L=(\nabla\times\mathbf B)\times\mathbf B/\mu_0$. The [continuity equation](../../../../../../continuity-equation.md) converts a material specific-energy balance into a conservative [energy density](../../../../../../energy-density.md) balance. Dot the [ideal magnetohydrodynamic momentum equation](../../../../../../ideal-magnetohydrodynamic-momentum-equation.md) with $\mathbf u$, and use the time independence of the [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md):

$$
\partial_t\!\left[\rho\left(\frac{u^2}{2}+\Phi\right)\right]+\nabla\cdot\!\left[\rho\mathbf u\left(\frac{u^2}{2}+\Phi\right)\right]=-\mathbf u\cdot\nabla p+\mathbf u\cdot\mathbf L.
$$

For the [energy density](../../../../../../energy-density.md) $U=p/(\gamma-1)$ associated with [internal energy](../../../../../../internal-energy.md), the adiabatic [pressure](../../../../../../pressure.md) equation gives

$$
\partial_tU+\nabla\cdot(U\mathbf u)=-p\nabla\cdot\mathbf u.
$$

The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and the cross-product [divergence](../../../../../../divergence.md) identity give the [magnetic energy](../../../../../../magnetic-energy.md) balance

$$
\partial_t\frac{B^2}{2\mu_0}=\frac1{\mu_0}\nabla\cdot[(\mathbf u\times\mathbf B)\times\mathbf B]-\mathbf u\cdot\mathbf L.
$$

Indeed $(\mathbf u\times\mathbf B)\cdot(\nabla\times\mathbf B)=-\mu_0\mathbf u\cdot\mathbf L$. The magnetic work cancels the kinetic magnetic work. The remaining [pressure](../../../../../../pressure.md) terms are $-\nabla\cdot(p\mathbf u)$. Adding all three balances proves [ideal magnetohydrodynamic energy conservation](../../../../../../ideal-magnetohydrodynamic-energy-conservation.md):

$$
\boxed{\partial_t\mathcal E+\nabla\cdot\mathbf F=0,\quad \mathcal E=\frac{\rho u^2}{2}+\rho\Phi+\frac{p}{\gamma-1}+\frac{B^2}{2\mu_0},}
$$

where

$$
\mathbf F=\rho\mathbf u\left(\frac{u^2}{2}+\Phi+\frac{\gamma p}{(\gamma-1)\rho}\right)-\frac{(\mathbf u\times\mathbf B)\times\mathbf B}{\mu_0}.
$$

The last term is the [Poynting vector](../../../../../../poynting-vector.md) with the ideal electric field $\mathbf E=-\mathbf u\times\mathbf B$. A time-dependent imposed potential would instead supply the source $\rho\partial_t\Phi$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
