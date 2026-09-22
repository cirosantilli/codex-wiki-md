<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a gas-pressure-supported, [optically thick](../../../../../../../optically-thick-medium.md) [alpha disk](../../../../../../../alpha-disk.md), with $\mathcal R=k/(\mu_m m_p)$ and positive parameters. Here $\sigma$ is the Stefan–Boltzmann constant in the [Stefan–Boltzmann law](../../../../../../../stefan-boltzmann-law.md), and $F_+$ and $F_-$ below are heating and cooling flux estimates per disk face. [Hydrostatic equilibrium](../../../../../../../hydrostatic-equilibrium.md) and the [ideal gas](../../../../../../../ideal-gas.md) relation give $\mathcal R T\sim\Omega^2H^2$, while $\rho\sim\Sigma/H$. Integrating viscous heating over one semi-thickness and estimating [radiative diffusion](../../../../../../../radiative-diffusion.md) give

$$
F_+\sim\mu\Omega^2H\sim\alpha\Sigma\mathcal R T\Omega\sim\alpha\Sigma\Omega^3H^2,\qquad F_-\sim\frac{\sigma T^4}{\kappa\rho H}\sim\frac{\sigma}{\kappa_0}T^{-6}\Sigma^{-4/3}H^{1/3}.
$$

Here the stipulated [negative hydrogen ion opacity](../../../../../../../negative-hydrogen-ion-opacity.md) exponent is $\kappa=\kappa_0\rho^{1/3}T^{10}$, which is a local approximation distinct from other empirical [opacity](../../../../../../../opacity.md) fits. Substituting $T\sim\Omega^2H^2/\mathcal R$ and equating heating and cooling gives

$$
\boxed{H^{41/3}\sim\frac{\sigma}{\kappa_0}\mathcal R^6\Omega^{-15}\alpha^{-1}\Sigma^{-7/3}.}
$$

Dropping numerical constants of order one is essential here. This is the [negative-hydrogen-opacity alpha-disk thickness scaling](../../../../../../../negative-hydrogen-opacity-alpha-disk-thickness-scaling.md). Its angular thickness estimate is

$$
\boxed{\frac Hr\sim\left(\frac{\sigma}{\alpha\kappa_0}\right)^{3/41}\mathcal R^{18/41}\Sigma^{-7/41}\frac{\Omega^{-45/41}}r.}
$$

For a central mass $M$, [Keplerian rotation](../../../../../../../keplerian-disk.md) gives $\Omega=(GM/r^3)^{1/2}$, so $H/r\propto r^{53/82}\Sigma(r)^{-7/41}$. The isothermal [sound speed](../../../../../../../speed-of-sound.md) $c_s^2=\mathcal R T$ is

$$
\boxed{c_s\sim\Omega H\propto\Omega^{-4/41}\Sigma^{-7/41}\propto r^{6/41}\Sigma(r)^{-7/41}.}
$$

An adiabatic [sound speed](../../../../../../../speed-of-sound.md) differs by the constant factor $\sqrt\gamma$ if the adiabatic index is fixed. For $\Sigma\propto r^{-p}$, constant $\alpha$, and fixed composition, the [disk aspect ratio](../../../../../../../disk-aspect-ratio.md) grows as $r^{(53+14p)/82}$, so there is [disk flaring](../../../../../../../disk-flaring.md) when $p>-53/14$; $c_s\propto r^{(6+7p)/41}$. The problem supplies no numerical parameters or specified $\Sigma(r)$, so no unique numerical $H/r$ or unconditional radial power can be inferred.

If the additional standard closure of a constant inward [accretion rate](../../../../../../../accretion-rate.md) well outside a zero-torque edge is intended, $\bar\nu\sim\alpha\Omega H^2$ and $\bar\nu\Sigma\simeq\dot M/(3\pi)$ imply $\Sigma\propto(\alpha\Omega H^2)^{-1}$. Eliminating it gives $H^9\propto\Omega^{-38/3}$ at fixed $\dot M,\alpha$, hence $H/r\propto r^{10/9}$ and $c_s\propto r^{11/18}$. These stronger powers use that extra steady-flow assumption. All these local scalings cease to apply if the [thin disk](../../../../../../../thin-disk.md) or the stated [opacity](../../../../../../../opacity.md) regime fails.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
