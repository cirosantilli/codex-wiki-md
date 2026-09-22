<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [relative potential](../../../../../../relative-potential.md) $\Psi=\Phi_*-\Phi$ and integrate the stated, untruncated [Maxwell-Boltzmann velocity distribution](../../../../../../maxwell-boltzmann-velocity-distribution.md) over $\mathbb R^3$. The normalization cancels its three [Gaussian integrals](../../../../../../gaussian-integral.md):

$$
\boxed{\rho(r)=\rho_1e^{\Psi(r)/\sigma^2}.}
$$

The [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) sign reverses under the relative-potential convention, so the spherical [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) is

$$
\boxed{\frac1{r^2}\frac{d}{dr}\left(r^2\frac{d\Psi}{dr}\right)=-4\pi G\rho_1e^{\Psi/\sigma^2}.}
$$

Also $\Psi'=-Gm(r)/r^2$, with $m'=4\pi r^2\rho$. Differentiating the density relation yields

$$
\sigma^2\rho'=-\rho\frac{Gm(r)}{r^2}.
$$

An [ideal gas](../../../../../../ideal-gas.md) with constant [temperature](../../../../../../temperature.md) has $P=\rho k_BT/m_0$. Its [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) equation is precisely the same when

$$
\boxed{\sigma^2=\frac{k_BT}{m_0}.}
$$

Together with the same enclosed-mass equation, central density and [boundary conditions](../../../../../../boundary-condition.md), this proves the [isothermal stellar and gas density equivalence](../../../../../../isothermal-stellar-and-gas-density-equivalence.md). In dimensionless terms, $y=-[\Psi-\Psi(0)]/\sigma^2$ and $x=r\sqrt{4\pi G\rho(0)}/\sigma$ obey $x^{-2}(x^2y')'=e^{-y}$ with $y(0)=y'(0)=0$ in both systems.

This calculation uses the distribution as printed for all [velocities](../../../../../../velocity.md). Imposing an additional cutoff at positive [relative energy](../../../../../../relative-energy.md) changes the integral to $\rho_1[e^W\operatorname{erf}\sqrt W-2\sqrt W/\sqrt\pi]$, where $W=\Psi/\sigma^2\geq0$, and no longer gives an exactly isothermal gas profile. An untruncated self-gravitating isothermal sphere also needs an outer modification for finite total [mass](../../../../../../mass.md). The function $\operatorname{erf}$ here is the [error function](../../../../../../error-function.md). Finally, the half-line [Gaussian integral](../../../../../../gaussian-integral.md) printed in the note lacks a factor: the correct value is **$\int_0^\infty e^{-\alpha x^2}\,dx=\tfrac12\sqrt{\pi/\alpha}$**.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
