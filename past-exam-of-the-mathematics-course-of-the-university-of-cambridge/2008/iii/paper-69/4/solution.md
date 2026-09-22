<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $m(r)$ be the background [enclosed mass](../../../../../enclosed-mass.md), so $g=Gm/r^2$ and $m'=4\pi r^2\rho$. The background [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) is $p'=-\rho g$. Use a Lagrangian [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $\xi=\xi_r$ of each spherical mass shell; $\Delta$ denotes its Lagrangian perturbation. Conservation of shell mass gives

$$
\frac{\Delta\rho}{\rho}=-\frac1{r^2}(r^2\xi)'=-(\xi'+2\xi/r),
$$

and the adiabatic [pressure](../../../../../pressure.md) law gives the [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md)

$$
\boxed{\Delta p=-\gamma p(\xi'+2\xi/r).}
$$

This retains perturbed self-gravity: a shell keeps its enclosed mass while its gravitational acceleration changes with its radius.

In mass coordinates, the exact radial shell equation is $\ddot r=-4\pi r^2\partial p/\partial m-Gm/r^2$. Its first-order perturbation is

$$
\ddot\xi=-4\pi r^2\partial_m\Delta p
-8\pi r\xi\partial_m p+2g\xi/r.
$$

Hydrostatic equilibrium gives $\partial_m p=-g/(4\pi r^2)$, and $\partial_m\Delta p=(\Delta p)'/(4\pi r^2\rho)$. Thus the perturbation of the [pressure](../../../../../pressure.md)-force geometry contributes another $2g\xi/r$, in addition to the gravity term:

$$
\ddot\xi=-\frac1\rho(\Delta p)'+4g\xi/r
=\frac1\rho[\gamma p(\xi'+2\xi/r)]'+4g\xi/r.
$$

Put $\eta=\xi/r$, so $\xi'+2\xi/r=r\eta'+3\eta$. Expanding the derivative, using constant $\gamma$ and $p'=-\rho g$, yields the [radial stellar pulsation equation](../../../../../radial-stellar-pulsation-equation.md):

$$
\boxed{\frac{\partial^2\xi_r}{\partial t^2}
=\frac1{\rho r^3}\frac{\partial}{\partial r}
 \left[\gamma p r^4\frac{\partial}{\partial r}(\xi_r/r)\right]
-(3\gamma-4)\frac{g\xi_r}{r}.}
$$

The coefficient $4$ includes both geometric [pressure](../../../../../pressure.md) and self-gravity effects; dropping the gravitational perturbation would not give this equation.

For a [normal mode](../../../../../normal-mode.md) $\xi(r,t)=\xi(r)e^{-i\omega t}$, multiply by $\rho r^2\xi^*$ and integrate. Since $\xi^*/r=\eta^*$, integration by parts gives

$$
\omega^2\int_0^R\rho r^2|\xi|^2dr
=\int_0^R\left[\gamma p r^4|\eta'|^2
 +(3\gamma-4)\rho gr|\xi|^2\right]dr
-\left[\gamma p r^4\eta^*\eta'\right]_0^R.
$$

Regularity at the center requires $\xi=O(r)$ with finite $\eta$, so the lower endpoint vanishes. For an isolated star take $p(R)=0$ and the free-surface condition $\Delta p=0$, with a regular finite-energy displacement; these eliminate the upper boundary term. Hence

$$
\boxed{\omega^2\int_0^R\rho r^2|\xi_r|^2dr
=\int_0^R\left[\gamma p r^4\left|\frac d{dr}(\xi_r/r)\right|^2
 +(3\gamma-4)\rho gr|\xi_r|^2\right]dr.}
$$

These boundary conditions give the self-adjoint radial [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) behind the [weighted stellar pulsation Rayleigh quotient](../../../../../weighted-stellar-pulsation-rayleigh-quotient.md).

Use the homologous trial [fluid displacement](../../../../../lagrangian-displacement-fluid-mechanics.md) $\xi_r=r$, or $\eta=1$. It is regular at the center, and $\Delta p=-3\gamma p$ vanishes at the free surface. The derivative term in the [Rayleigh quotient](../../../../../rayleigh-quotient.md) is zero, leaving

$$
\omega_{\min}^2\leq\mathcal R[r]
=(3\gamma-4)\frac{\int_0^R\rho g r^3dr}{\int_0^R\rho r^4dr}.
$$

The ratio is a positive weighted average of $g/r$. Since the central [mass density](../../../../../density.md) is its maximum,

$$
m(r)=4\pi\int_0^r\rho(s)s^2ds\leq\frac{4\pi}3\rho_c r^3,\qquad
\frac{g(r)}r=\frac{Gm(r)}{r^3}\leq\frac{4\pi}3G\rho_c.
$$

For $\gamma>4/3$ multiplication preserves this inequality, proving the [central-density upper bound for a radial stellar frequency](../../../../../central-density-upper-bound-for-a-radial-stellar-frequency.md):

$$
\boxed{\omega_{\min}^2\leq(3\gamma-4)\frac{4\pi}3G\rho_c.}
$$

The full positive quadratic form also shows radial stability for constant $\gamma>4/3$ under these assumptions. A uniform-density equilibrium has constant $g/r$, making the homologous displacement an exact mode and saturating the bound.

If $\gamma<4/3$, the same trial value is strictly negative. Therefore **$\omega_{\min}^2<0$: the star has an exponentially growing radial instability**, with growth rate $\sqrt{-\omega_{\min}^2}$. One must use this negative trial quotient, rather than carrying the central-density inequality across the sign change unchanged. At the limiting value $\gamma=4/3$, the homologous displacement has zero restoring force and is a neutral radial mode in this constant-exponent model.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
