# Entropy density of a photon gas

↑ **Parent:** [Photon gas](photon-gas.md)

The [entropy density of a photon gas](entropy-density-of-a-photon-gas.md) is its [entropy](entropy.md) per physical [volume](volume-thermodynamics.md), $s=S/V$. For homogeneous equilibrium vacuum radiation with two states of [electromagnetic polarization](polarization-of-an-electromagnetic-wave.md) and zero [photon chemical potential](photon-chemical-potential.md),

$$
s=\frac{u+p}{T}=\frac{4}{3}a_RT^3,\qquad
S=\frac{4}{3}a_RT^3V.
$$

The first equality is the [entropy density at zero chemical potential](entropy-density-at-zero-chemical-potential.md), obtained from the [thermodynamic Euler relation](euler-relation-in-thermodynamics.md) $U=TS-pV+\mu_\gamma N_\gamma$ with [internal energy](internal-energy.md) $U=uV$. The second uses the [photon gas](photon-gas.md) [equation of state](equation-of-state.md), $u=a_RT^4$ and $p=u/3$. If an independently constrained [photon](photon.md) number gives a nonzero [chemical potential](chemical-potential.md), the general [entropy density](entropy-density.md) is $(u+p-\mu_\gamma n_\gamma)/T$ and $u=a_RT^4$ need not hold. This distinction explains why the absence of a conserved number matters for [entropy](entropy.md) as well as for the spectral shape. [David Tong, Statistical Physics, §4.4: Gibbs free energy and the thermodynamic Euler relation](https://davidtong.org/teaching/statistical-physics/statmechhtml/S4#S4.SS4)

A short [first law of thermodynamics](first-law-of-thermodynamics.md) check, for neighboring equilibrium states with $\mu_\gamma=0$, is

$$
T\,dS=dU+p\,dV
 =4a_RT^3V\,dT+\frac{4}{3}a_RT^4\,dV,
\qquad
dS=\frac{4}{3}a_R\,d(T^3V).
$$

The [thermodynamic Euler relation](euler-relation-in-thermodynamics.md) fixes the additive normalization. Equivalently, this radiation [entropy](entropy.md) tends to zero with [temperature](temperature.md) at fixed [volume](volume-thermodynamics.md); no contribution from the containing walls is included. Interpreting $T\,dS$ as transferred [heat](heat.md) and $p\,dV$ as boundary [work](work.md) requires a [reversible thermodynamic process](reversible-thermodynamic-process.md). For a [reversible thermodynamic process](reversible-thermodynamic-process.md) that is also an [adiabatic process](adiabatic-process.md), there is no [entropy production](entropy-production.md) or [entropy](entropy.md) exchange, so

$$
T^3V=\text{constant},\qquad
T=T_0\left(\frac{V_0}{V}\right)^{1/3},\qquad
pV^{4/3}=\text{constant},\qquad
U=U_0\left(\frac{V_0}{V}\right)^{1/3}.
$$

An irreversible [adiabatic process](adiabatic-process.md) can produce [entropy](entropy.md) even without [heat](heat.md) exchange, so the word adiabatic alone is insufficient to infer $T^3V=\text{constant}$.

For an analytic example, expand an initially equilibrated [photon gas](photon-gas.md) reversibly from $V_0$ to $8V_0$, keeping only the same two [photon](photon.md) states of [electromagnetic polarization](polarization-of-an-electromagnetic-wave.md). Its [temperature](temperature.md) halves, its [energy density](energy-density.md) becomes $u_0/16$, its [entropy density of a photon gas](entropy-density-of-a-photon-gas.md) becomes $s_0/8$, and its total [entropy](entropy.md) stays $S_0$. The [internal energy](internal-energy.md) halves rather than remaining fixed: the missing half leaves as [work](work.md) against [radiation pressure](radiation-pressure.md),

$$
W=\int_{V_0}^{8V_0}p(V)\,dV=\frac{U_0}{2},\qquad
\Delta U=-W.
$$

This is a stipulated reversible radiation model, not a report of a piston experiment. Maintaining a real cavity along this path requires controlling wall [heat](heat.md) exchange and including the wall [heat capacity](heat-capacity.md) in any actual apparatus balance.

<a id="image-analytic-reversible-photon-gas-expansion-entropy-conservation-and-pressure-work"></a>
![](photon-gas-entropy-adiabatic-work.png)

**[Figure 2](#image-analytic-reversible-photon-gas-expansion-entropy-conservation-and-pressure-work). Analytic reversible photon gas expansion: entropy conservation and pressure work**. Original fixed-species model with $r=V/V_0$ from 1 to 8 and no [entropy production](entropy-production.md). The left panel shows $T/T_0=r^{-1/3}$, $u/u_0=r^{-4/3}$ and $s/s_0=r^{-1}$ on a logarithmic vertical scale. The right panel plots $pV_0/U_0=r^{-4/3}/3$; the shaded [integral](integral.md) is $W/U_0=1-8^{-1/3}=1/2$. Total [entropy](entropy.md) remains constant even though both [entropy density](entropy-density.md) and [internal energy](internal-energy.md) decrease.

For a computed scale at stipulated $T=2.725\,\mathrm K$, $s\simeq2.04122\times10^{-14}\,\mathrm{J\,K^{-1}\,m^{-3}}$. Combining this with the [photon number density](photon-number-density.md) gives

$$
\frac{S}{N_\gamma}=\frac{s}{n_\gamma}
 =\frac{2\pi^4}{45\zeta(3)}k_B\simeq3.60157\,k_B.
$$

This is the total equilibrium radiation [entropy](entropy.md) divided by its mean [photon](photon.md) number, not a separately assigned [entropy](entropy.md) carried by each labeled particle. During the ideal expansion, $n_\gamma\propto T^3$ and $T^3V$ is fixed, so the mean number $N_\gamma=n_\gamma V$ also stays constant. This follows from the path; it was not imposed as the independent number constraint used to establish [chemical potential](chemical-potential.md).

The beautiful connection is that expansion lowers each typical [photon](photon.md) [energy](energy.md) and dilutes the radiation in just the proportions needed to retain its equilibrium spectral shape and total [entropy](entropy.md). For the [cosmic microwave background](cosmic-microwave-background.md), homogeneous [expansion of the universe](expansion-of-the-universe.md) has physical [volume](volume-thermodynamics.md) proportional to the cube of the [scale factor](scale-factor-cosmology.md); fixed-species [cosmological entropy conservation](cosmological-entropy-conservation.md) therefore gives $T\propto a^{-1}$. This describes preservation of an already established [Planck photon distribution](planck-photon-distribution.md) and connects the FIRAS spectral observation in [photon gas](photon-gas.md) to an [entropy](entropy.md) prediction; FIRAS did not perform a direct [entropy](entropy.md) measurement. When other equilibrated species disappear and transfer [energy](energy.md) into radiation, use the [effective number of relativistic entropy degrees of freedom](effective-number-of-relativistic-degrees-of-freedom.md), $g_{*s}$: the conserved quantity for the combined sector is $g_{*s}T^3V$, under the corresponding equilibrium and no-[entropy production](entropy-production.md) assumptions. A changing species population, separate decoupled sectors or [entropy production](entropy-production.md) requires an appropriate [entropy](entropy.md) balance rather than the pure [photon gas](photon-gas.md) formula. [David Tong, Cosmology, §2.5.2: entropy conservation and heating when relativistic species disappear](https://davidtong.org/teaching/cosmology/cosmohtml/S2#S2.SS5.SSS2)

## ↑ Ancestors (5)

1. [Photon gas](photon-gas.md)
2. [Statistical physics](statistical-physics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Entropy density of a photon gas](entropy-density-of-a-photon-gas.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/10e/solution.md)
- [Photon gas](photon-gas.md)
