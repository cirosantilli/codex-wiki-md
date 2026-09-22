<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The linearized azimuthal [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) is

$$
\partial_tv_\phi+\frac{u'_R}{R}\frac{d(R^2\Omega)}{dR}=0.
$$

For the time dependence $e^{-i\omega t}$ and $u'_R=-i\omega\xi_R$, it gives

$$
\boxed{v_\phi=-\frac{\xi_R}{R}\frac{d(R^2\Omega)}{dR}.}
$$

This expresses conservation of the displaced element's [specific angular momentum](../../../../../../specific-angular-momentum.md). It applies directly to nonzero-[frequency](../../../../../../frequency.md) modes, with the zero-[frequency](../../../../../../frequency.md) limit taken in the displacement formulation.

The radial advective acceleration supplies $-2\Omega v_\phi$, while the [pressure](../../../../../../pressure.md) force perturbation is $\delta\rho\,\nabla p/\rho^2-\nabla\delta p/\rho$. Eliminate $v_\phi$ and retain the vertical equation. Under the [Cowling approximation](../../../../../../cowling-approximation.md), $\delta\Phi=0$, so

$$
\boxed{-\omega^2\boldsymbol\xi=\mathcal F\boldsymbol\xi=\frac{\delta\rho}{\rho^2}\nabla p-\frac1\rho\nabla\delta p-\kappa^2\xi_R\mathbf e_R,\qquad \kappa^2=\frac{2\Omega}{R}\frac{d(R^2\Omega)}{dR}.}
$$

The [continuity equation](../../../../../../continuity-equation.md) gives $\delta\rho=-\nabla\cdot(\rho\boldsymbol\xi)$. The Lagrangian adiabatic relation $\Delta p/p=\gamma\Delta\rho/\rho$, with $\Delta\rho=-\rho\nabla\cdot\boldsymbol\xi$, gives

$$
\boxed{\delta\rho=-\nabla\cdot(\rho\boldsymbol\xi),\qquad \delta p=-\boldsymbol\xi\cdot\nabla p-\gamma p\nabla\cdot\boldsymbol\xi.}
$$

Here $\kappa$ is the [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md). These formulas define the [axisymmetric adiabatic displacement operator](../../../../../../axisymmetric-adiabatic-displacement-operator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
