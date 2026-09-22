<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Efficient [convection](../../../../../../convection.md) makes the interior follow a nearly [adiabatic process](../../../../../../adiabatic-process.md) and maintains uniform [specific entropy](../../../../../../specific-entropy.md). For the fully ionized monatomic [ideal gas](../../../../../../ideal-gas.md), the [specific-heat ratio](../../../../../../heat-capacity-ratio.md) is $5/3$, so the [adiabatic temperature gradient](../../../../../../adiabatic-temperature-gradient.md) gives $d\log T/d\log P=2/5$. Integrating at a fixed time gives

$$
\boxed{P=K(t)T^{5/2}.}
$$

The coefficient is spatially constant because the composition and [specific entropy](../../../../../../specific-entropy.md) are uniform. It can change as the star loses energy. Equivalently the gas is an [adiabatic stellar polytrope](../../../../../../adiabatic-stellar-polytrope.md) with $P=K_\rho\rho^{5/3}$ and [polytropic index](../../../../../../polytropic-index.md) $n=3/2$; $K_\rho$ and the pressure-temperature coefficient $K$ are different quantities.

This fixes the dimensionless [Lane-Emden equation](../../../../../../lane-emden-equation.md) profile throughout a [stellar homology](../../../../../../stellar-homology.md) sequence. Writing $\rho(r)=\rho_cf(r/R)$ in the mass integral gives $\rho_c=C_\rho M/R^3$, with a fixed positive shape constant $C_\rho$. Integrating the [stellar hydrostatic equation](../../../../../../hydrostatic-pressure-support-equation.md) through the same profile, with negligible surface pressure compared with central pressure, gives $P_c=C_PGM^2/R^4$. Hence

$$
\boxed{\rho_c\propto M/R^3,\qquad P_c\propto GM^2/R^4,\qquad
T_c=\frac{\mu P_c}{\mathcal R\rho_c}\propto\frac{\mu GM}{\mathcal R R}.}
$$

These are [homology scalings of central stellar pressure](../../../../../../homology-scaling-of-central-stellar-pressure.md). Substituting the central quantities into $K=P_c/T_c^{5/2}$ yields

$$
\boxed{K=K_0\mu^{-5/2}M^{-1/2}R^{-3/2},\qquad
K_0=C_\rho^{5/2}C_P^{-3/2}\mathcal R^{5/2}G^{-3/2}.}
$$

Thus $K_0$ is constant for the fixed [stellar polytrope](../../../../../../stellar-polytrope.md) family.

At the approximate [photosphere](../../../../../../photosphere.md), take $T=T_e$ and use the [ideal gas](../../../../../../ideal-gas.md) relation $\rho=\mu P/(\mathcal RT)$. The prescribed [opacity](../../../../../../opacity.md) gives

$$
\kappa P=\frac{\kappa_0\mu}{\mathcal R}P^2T^3
=\frac{\kappa_0\mu}{\mathcal R}K^2T^8.
$$

The [stellar surface boundary condition](../../../../../../stellar-surface-boundary-condition.md) and [surface gravity of a star](../../../../../../surface-gravity-of-a-star.md) therefore imply

$$
\boxed{T_e^8=\frac{2G\mathcal R}{3\kappa_0K_0^2}\,\mu^4M^2R.}
$$

This is the temperature-four special case of [convective contraction with power-law opacity](../../../../../../convective-contraction-with-power-law-opacity.md).

Using the [Stefan–Boltzmann law](../../../../../../stefan-boltzmann-law.md), the [luminosity](../../../../../../luminosity.md) is

$$
L=4\pi\sigma\left(\frac{2G\mathcal R}{3\kappa_0}\right)^{1/2}
K_0^{-1}\mu^2M R^{5/2}.
$$

For $n=3/2$, the supplied gravitational-energy formula is $\Omega=-6GM^2/(7R)$. The [stellar virial theorem](../../../../../../stellar-virial-theorem.md) for a monatomic gas gives $2U+\Omega=0$, so the total energy is $E=U+\Omega=-3GM^2/(7R)$. During [Kelvin-Helmholtz contraction](../../../../../../kelvin-helmholtz-mechanism.md), with constant mass and no significant nuclear source, $L=-dE/dt$. Thus

$$
\dot R=-\frac{28\pi\sigma}{3}
\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}
K_0^{-1}\mu^2M^{-1}R^{9/2}.
$$

Multiplying by $-(7/2)R^{-9/2}$ and integrating gives

$$
\boxed{R^{-7/2}-R_0^{-7/2}
=\frac{98\pi\sigma}{3}
\left(\frac{2\mathcal R}{3\kappa_0G}\right)^{1/2}
K_0^{-1}\mu^2M^{-1}(t-t_0).}
$$

The sign makes the radius decrease as time increases.

When the accumulated contraction term dominates the initial-radius term, this yields $R\propto\mu^{-4/7}M^{2/7}(t-t_0)^{-2/7}$. Combining it with the central [ideal gas](../../../../../../ideal-gas.md) temperature gives the **late-time central-temperature scaling**

$$
\boxed{T_c\propto\mu^{11/7}M^{5/7}(t-t_0)^{2/7}.}
$$

Replacing $t-t_0$ by $t$ gives the stated late-time form. The asymptotic step also requires a time long enough to forget the initial radius, not merely a choice of zero for the age.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
