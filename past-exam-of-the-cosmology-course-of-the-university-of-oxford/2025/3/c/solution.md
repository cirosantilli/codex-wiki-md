<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p(z)$ be the normalized galaxy [probability density](../../../../probability-density.md) per unit [cosmological redshift](../../../../cosmological-redshift.md), $\int p(z)\,dz=1$, and let $b_g$ be its linear [galaxy bias](../../../../galaxy-bias.md). In a spatially flat background with $c=1$, $d\chi=dz/H(z)$. Thus the projected [galaxy density contrast](../../../../galaxy-density-contrast.md) is

$$
\delta_g(\hat{\mathbf n})=\int dz\,p(z)b_g\delta(\chi(z)\hat{\mathbf n},z)
=\int d\chi\,H(z)p(z)b_g\delta(\chi\hat{\mathbf n},z),
$$

so its radial kernel is $q_g=Hbp$. The [cosmological Poisson equation](../../../../cosmological-poisson-equation.md) in [Fourier transform](../../../../fourier-transform-split.md) variables gives

$$
-k^2\psi(\mathbf k,a)=4\pi Ga^2\bar\rho_m\delta(\mathbf k,a)
=\frac32H_0^2\Omega_m a^{-1}\delta(\mathbf k,a).
$$

Here $\Omega_m$ denotes today's [matter density parameter](../../../../matter-density-parameter.md), not its time-dependent value. For a growing [linear cosmological density perturbation](../../../../linear-cosmological-density-perturbation-split.md), write $\delta(\mathbf k,a)=D(a)\delta_{\rm ini}(\mathbf k)$, where $D$ is the [linear growth factor](../../../../linear-growth-factor.md), and define the [logarithmic linear growth rate](../../../../logarithmic-linear-growth-rate.md) $f=d\ln D/d\ln a$. At fixed [comoving coordinate](../../../../comoving-coordinate.md),

$$
\left(\frac\delta a\right)'=\mathcal H(f-1)\frac\delta a=H(f-1)\delta.
$$

Consequently

$$
\boxed{\psi'(\mathbf k,z)=\frac{3H_0^2\Omega_m}{2k^2}H(z)[1-f(z)]\delta(\mathbf k,z).}
$$

In particular, $f=1$ during [matter domination](../../../../matter-domination.md) makes the linear potential constant and eliminates this [Integrated Sachs-Wolfe effect](../../../../integrated-sachs-wolfe-effect.md).

To use the supplied [Limber approximation](../../../../limber-approximation.md) without hiding its scale dependence in a radial kernel, take $U=\delta$, $V=\psi'$, $q_g=Hbp$, and $q_T=2$. The corresponding three-dimensional [cross-power spectrum](../../../../cross-spectrum.md) is

$$
P_{\delta\psi'}(k,z)=\frac{3H_0^2\Omega_m}{2k^2}H(z)[1-f(z)]P(k,z),
$$

where $P$ is the [matter power spectrum](../../../../matter-power-spectrum.md). Substitution gives

$$
C_\ell^{gT}=3H_0^2\Omega_m\int\frac{d\chi}{\chi^2}\,\frac{H^2(z)[1-f(z)]b_gp(z)}{k^2}P(k,z)\bigg|_{k=(\ell+1/2)/\chi}.
$$

The [Limber approximation](../../../../limber-approximation.md) relation $k\chi=\ell+1/2$ cancels $\chi^{-2}k^{-2}$, yielding

$$
\boxed{C_\ell^{\delta_g\,\delta T/T}=\frac{3H_0^2\Omega_m}{(\ell+1/2)^2}\int d\chi\,H^2(z)[1-f(z)]b_gp(z)P\left(\frac{\ell+1/2}{\chi},z\right),\qquad z=z(\chi).}
$$

Both powers of $H$ are necessary: one converts the redshift selection to a distance kernel, and the other differentiates the potential in [conformal time](../../../../conformal-time.md). The factor two in the [Integrated Sachs-Wolfe effect](../../../../integrated-sachs-wolfe-effect.md) cancels the factor $1/2$ from the [cosmological Poisson equation](../../../../cosmological-poisson-equation.md). For positive [galaxy bias](../../../../galaxy-bias.md) and $f<1$, the predicted correlation is positive: an overdense region whose negative potential becomes shallower gives a positive integrated [temperature](../../../../temperature-split.md) shift. The result assumes linear, scale-independent growth and the Newtonian [cosmological Poisson equation](../../../../cosmological-poisson-equation.md); the [Limber approximation](../../../../limber-approximation.md) becomes less accurate at the very lowest angular multipoles.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the cosmology course of the University of Oxford](../../../split.md)
5. [Cosmology course of the University of Oxford](../../../../cosmology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
