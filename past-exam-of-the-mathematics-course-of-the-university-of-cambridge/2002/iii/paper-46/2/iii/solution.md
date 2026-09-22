<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $\mathcal R=k/(\mu_m m_H)$, so $p_g=\mathcal R\rho T$ and the prescribed [dynamic viscosity](../../../../../../dynamic-viscosity.md) is $\mu=\alpha\mathcal R\rho T/\Omega$. Keplerian shear and [radiative diffusion](../../../../../../radiative-diffusion.md) then give

$$
F_z=\frac94\alpha\mathcal R\Omega\rho T,\qquad F=-\frac{4\sigma}{3\kappa\rho}(T^4)_z.
$$

Differentiating the second expression, equating it to the first and dividing by $\rho$ gives

$$
\boxed{\frac1\rho\frac{d}{dz}\left(\frac1\rho\frac{dT^4}{dz}\right)+A\Omega T=0,\qquad A=\frac{27\alpha\kappa\mathcal R}{16\sigma}=\frac{27\alpha\kappa k}{16\sigma\mu_m m_H}.}
$$

This reduction uses the gas-pressure [viscosity](../../../../../../dynamic-viscosity.md) closure, not an assumption that [gas pressure](../../../../../../gas-pressure.md) dominates the hydrostatic support.

For $z\ge0$, introduce the [vertical mass coordinate of a disk](../../../../../../vertical-mass-coordinate-of-a-disk.md)

$$
m(z)=\int_0^z\rho(z')\,dz',\qquad \frac{d}{dm}=\frac1\rho\frac{d}{dz}.
$$

Let $\Sigma=\int_{-z_s}^{z_s}\rho\,dz$ be the full [surface density](../../../../../../surface-density-of-a-disk.md) of a reflection-symmetric disk. The upper surface is at $m_s=\Sigma/2$. With $\zeta=2m/\Sigma$, the [temperature](../../../../../../temperature.md) equation becomes

$$
\frac4{\Sigma^2}\frac{d^2T^4}{d\zeta^2}+A\Omega T=0.
$$

Write $T=T_*t(\zeta)$ and choose

$$
\boxed{T_*^3=\frac{A\Omega\Sigma^2}4=\frac{27\alpha\kappa\mathcal R\Omega\Sigma^2}{64\sigma}.}
$$

The equation reduces exactly to $(t^4)''+t=0$. Midplane symmetry gives $t'(0)=0$, and the zero surface [temperature](../../../../../../temperature.md) gives $t(1)=0$. The stipulated unique positive nontrivial dimensionless solution therefore applies at every radius and [surface density](../../../../../../surface-density-of-a-disk.md), with all physical dependence contained in $T_*$ and the mass-coordinate scaling. A zero [temperature](../../../../../../temperature.md) at the ideal surface does not mean zero escaping flux: $F=-(4\sigma/(3\kappa))\partial_mT^4$ can have a finite nonzero surface value.

The required [viscosity](../../../../../../dynamic-viscosity.md) is the [density-weighted mean kinematic viscosity](../../../../../../density-weighted-mean-kinematic-viscosity.md), not an unweighted vertical mean. Since $\rho\nu=\mu$,

$$
\bar\nu=\frac1\Sigma\int_{-z_s}^{z_s}\mu\,dz=\frac{2\alpha\mathcal R}{\Omega\Sigma}\int_0^{\Sigma/2}T(m)\,dm.
$$

Substituting the dimensionless solution gives, with $I_t=\int_0^1t(\zeta)\,d\zeta$,

$$
\boxed{\bar\nu=\frac{\alpha\mathcal R}{\Omega}\left(\frac{A\Omega\Sigma^2}4\right)^{1/3}I_t=\frac{3I_t}{4}\left(\frac{\alpha^4\kappa\mathcal R^4}{\sigma}\right)^{1/3}\Sigma^{2/3}\Omega^{-2/3}.}
$$

For central [mass](../../../../../../mass.md) $M_*$, $\Omega=(GM_*/r^3)^{1/2}$, so the requested explicit radius and surface-density dependence is

$$
\boxed{\bar\nu(r,\Sigma)=\frac{3I_t}{4}\left(\frac{\alpha^4\kappa k^4}{\sigma(\mu_m m_H)^4GM_*}\right)^{1/3}r\Sigma^{2/3}.}
$$

The universal [integral](../../../../../../integral.md) need not be evaluated. No separate solution for $\rho(z)$ is needed to find this mean: the mass-coordinate transformation removes it from both the [temperature](../../../../../../temperature.md) equation and the [viscosity](../../../../../../dynamic-viscosity.md) [integral](../../../../../../integral.md). The result is the [gas-pressure viscosity closure with mixed pressure support](../../../../../../gas-pressure-viscosity-closure-with-mixed-pressure-support.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
