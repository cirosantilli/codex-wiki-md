<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a_\xi=\boldsymbol\xi\cdot\nabla\Psi$, $d_\xi=\nabla\cdot\boldsymbol\xi$ and $\rho_\Psi=d\rho/d\Psi$. Since $\nabla p=-\rho\nabla\Psi$, the [pressure](../../../../../../pressure.md) and [mass density](../../../../../../density.md) perturbations are $\delta p_\xi=\rho a_\xi-\gamma p d_\xi$ and $\delta\rho_\xi=-\rho d_\xi-\rho_\Psi a_\xi$. Integrating the [pressure](../../../../../../pressure.md)-[gradient](../../../../../../gradient.md) term by parts in the [mass density](../../../../../../density.md)-weighted [inner product](../../../../../../inner-product.md) gives

$$
\langle\eta,\mathcal F\xi\rangle=\int\left[-\gamma p d_\eta^*d_\xi+\rho(a_\eta^*d_\xi+d_\eta^*a_\xi)+\rho_\Psi a_\eta^*a_\xi-\rho\kappa^2\eta_R^*\xi_R\right]d\tau.
$$

The boundary term vanishes for regular admissible displacements because $p,\rho$ vanish there and $\delta p=\rho a-\gamma p d$. Completing the [pressure](../../../../../../pressure.md) square gives

$$
\langle\eta,\mathcal F\xi\rangle=-\int\left[\frac{\delta p_\eta^*\delta p_\xi}{\gamma p}+\rho\mathcal N^2a_\eta^*a_\xi+\rho\kappa^2\eta_R^*\xi_R\right]d\tau,
$$

where

$$
\mathcal N^2=-\frac{\rho}{\gamma p}-\frac{\rho_\Psi}{\rho}=-\frac1\rho\frac{dp}{d\Psi}\left(\frac1\gamma\frac{d\ln p}{d\Psi}-\frac{d\ln\rho}{d\Psi}\right).
$$

This [effective-potential stratification coefficient](../../../../../../effective-potential-stratification-coefficient.md) is real. All coefficients of the bilinear form are real, so $\langle\eta,\mathcal F\xi\rangle=\langle\mathcal F\eta,\xi\rangle$: the operator is symmetric on the stated boundary domain, giving the usual [self-adjoint](../../../../../../self-adjoint-operator.md) realization of the stellar normal-mode problem.

Set $\eta=\xi$ and use $\mathcal F\xi=-\omega^2\xi$. The [Cowling energy principle for a rotating barotropic star](../../../../../../cowling-energy-principle-for-a-rotating-barotropic-star.md) is

$$
\boxed{\omega^2\int\rho|\xi|^2d\tau=Q[\xi]=\int\left[\frac{|\delta p|^2}{\gamma p}+\rho\mathcal N^2|\xi\cdot\nabla\Psi|^2+\rho\kappa^2|\xi_R|^2\right]d\tau.}
$$

The [Rayleigh quotient](../../../../../../rayleigh-quotient.md) $Q[\xi]/\int\rho|\xi|^2$ tests stability. If $Q\ge0$ for every admissible displacement, no mode has $\omega^2<0$, so there is no exponentially growing mode. If an admissible trial displacement has $Q<0$, the [Rayleigh-Ritz variational principle](../../../../../../rayleigh-ritz-variational-principle.md) puts negative spectrum below zero; in the usual discrete stellar mode problem this gives a mode with $\omega=i\sigma$, $\sigma>0$. Equality allows neutral modes, rather than establishing strictly positive [frequencies](../../../../../../frequency.md). A locally negative coefficient alone is not a complete instability proof: a trial function must also control the [pressure](../../../../../../pressure.md) and other positive terms.

## ↑ Ancestors (11)

1. [C](../c.md)
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
