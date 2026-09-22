<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A stellar [equation of state](../../../../../equation-of-state.md) supplies [pressure](../../../../../pressure.md) and [internal energy](../../../../../internal-energy.md) as functions of density, [temperature](../../../../../temperature.md) and composition, together with thermodynamic derivatives needed for stability and transport. [Hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) fixes the [pressure gradient](../../../../../pressure-gradient.md), but does not determine which microscopic components provide the [pressure](../../../../../pressure.md). In ordinary dense interiors [local thermodynamic equilibrium](../../../../../local-thermodynamic-equilibrium.md) is a useful starting point. A consistent mixture is

$$
\boxed{P=P_i+P_e(\rho,T,\{X_A\})+P_\gamma+P_{\rm int},}
$$

where ions, [Electrons](../../../../../electron.md), radiation and interaction corrections are distinguished. **The classical [Electron](../../../../../electron.md) [pressure](../../../../../pressure.md) and [electron degeneracy pressure](../../../../../electron-degeneracy-pressure.md) are two limits of the same [Electron](../../../../../electron.md) contribution**, and must not be added as if they belonged to different particles. The [finite-temperature electron equation of state](../../../../../finite-temperature-electron-equation-of-state.md) interpolates between them.

In a fully ionized, nondegenerate, nonrelativistic gas, $P_g=\rho k_BT/(\mu m_u)$ and specific thermal energy is $u_g=3k_BT/(2\mu m_u)$. With nuclear mass fractions $X_A$, charges $Z_A$ and mass numbers $A_A$, the [mean molecular weight](../../../../../mean-molecular-weight.md) satisfies $\mu^{-1}=\sum_A X_A(1+Z_A)/A_A$, and $\mu_e^{-1}=\sum_A X_AZ_A/A_A$ is the [mean molecular weight per electron](../../../../../mean-molecular-weight-per-electron.md). This regime describes much of an ordinary [main sequence](../../../../../main-sequence.md) interior. Toward cooler layers, [ionization](../../../../../ionization.md) and molecular dissociation change particle numbers and consume heat. The [Saha equation](../../../../../saha-ionization-equation.md) relates [ionization](../../../../../ionization.md) to both [temperature](../../../../../temperature.md) and [Electron](../../../../../electron.md) density: there is no universal horizontal [ionization](../../../../../ionization.md) boundary. These regions have larger [heat capacity](../../../../../heat-capacity.md) and can have a reduced [stellar adiabatic exponent](../../../../../stellar-adiabatic-exponent.md). The simple fully ionized formula is then insufficient.

Equilibrium [photons](../../../../../photon.md) give [radiation pressure](../../../../../radiation-pressure.md) $P_\gamma=a_rT^4/3$ and energy per volume $a_rT^4$, or specific energy $u_\gamma=a_rT^4/\rho$. In the nondegenerate gas regime, equality with gas [pressure](../../../../../pressure.md) gives the [radiation-to-gas pressure boundary](../../../../../radiation-to-gas-pressure-boundary.md)

$$
\boxed{T^3=\frac{3k_B\rho}{a_r\mu m_u},}
$$

a line of slope $1/3$ on a $(\log\rho,\log T)$ plot. Higher temperatures at fixed [mass density](../../../../../density.md) favor [photon](../../../../../photon.md) support. A monatomic gas has [stellar adiabatic exponent](../../../../../stellar-adiabatic-exponent.md) $5/3$, while radiation alone has $4/3$; their [adiabatic exponents of a monatomic gas-radiation mixture](../../../../../adiabatic-exponents-of-a-monatomic-gas-radiation-mixture.md) are not obtained by assuming a fixed [pressure](../../../../../pressure.md) fraction during compression. Radiation support is particularly important in massive stars.

For [Electrons](../../../../../electron.md), [Pauli exclusion principle](../../../../../pauli-exclusion-principle.md) and the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) determine occupation numbers. The net [Electron](../../../../../electron.md) density is $n_e=\rho/(\mu_em_u)$ and the [Fermi momentum](../../../../../fermi-momentum.md) is $p_F=\hbar(3\pi^2n_e)^{1/3}$. Define the kinetic [electron Fermi temperature](../../../../../electron-fermi-temperature.md)

$$
\boxed{k_BT_F=\sqrt{m_e^2c^4+p_F^2c^2}-m_ec^2.}
$$

For $T\gg T_F$ the [Electrons](../../../../../electron.md) are nearly classical; for $T\ll T_F$ they are strongly degenerate and their [pressure](../../../../../pressure.md) depends primarily on density. The intermediate region requires [finite-temperature electron equation of state](../../../../../finite-temperature-electron-equation-of-state.md) integrals, not a discontinuous switch of formulas.

The [equation of state of a cold electron gas](../../../../../equation-of-state-of-a-cold-electron-gas.md) gives, in its two limits,

$$
\boxed{P_e\simeq\frac{\hbar^2(3\pi^2)^{2/3}}{5m_e}n_e^{5/3}
\quad(p_F\ll m_ec),\qquad
P_e\simeq\frac{\hbar c(3\pi^2)^{1/3}}4n_e^{4/3}
\quad(p_F\gg m_ec).}
$$

These are respectively the $n=3/2$ and $n=3$ pressure-density powers, explaining the approximate [white dwarf](../../../../../white-dwarf.md) [polytropic mass-radius relation](../../../../../polytropic-mass-radius-relation.md) sequence and the [Chandrasekhar limit](../../../../../chandrasekhar-limit.md). The kinetic energy per volume is $3P_e/2$ in the nonrelativistic limit and $3P_e$ in the ultrarelativistic limit. Ions can still supply much of the [heat capacity](../../../../../heat-capacity.md) even when the [Electron](../../../../../electron.md) [pressure](../../../../../pressure.md) supplies the mechanical support.

The [Electron](../../../../../electron.md) degeneracy crossover $T\sim T_F$ has slope $2/3$ at low [mass density](../../../../../density.md) and $1/3$ at high [mass density](../../../../../density.md). The [electron relativistic density threshold](../../../../../electron-relativistic-density-threshold.md) is

$$
\rho_*=\frac{\mu_em_u}{3\pi^2}\left(\frac{m_ec}{\hbar}\right)^3
\simeq9.74\times10^5\mu_e\,\mathrm{g\,cm^{-3}},
$$

a vertical marker where $p_F=m_ec$. It is different from the [thermal electron relativistic threshold](../../../../../thermal-electron-relativistic-threshold.md) $k_BT\sim m_ec^2$, near $5.93\times10^9\,\mathrm K$, a horizontal [temperature](../../../../../temperature.md) scale. Hot dilute matter can have relativistic thermal [Electrons](../../../../../electron.md) without degeneracy; cold dense matter can have relativistic degenerate [Electrons](../../../../../electron.md) without reaching that [temperature](../../../../../temperature.md).

[Electron](../../../../../electron.md) degeneracy also does not automatically imply that [Electrons](../../../../../electron.md) dominate the total [pressure](../../../../../pressure.md). Comparing the cold [Electron](../../../../../electron.md) limit with radiation gives the [radiation-to-degeneracy pressure boundary](../../../../../radiation-to-degeneracy-pressure-boundary.md)

$$
\boxed{T=\left(\frac{3P_e(\rho,0)}{a_r}\right)^{1/4}.}
$$

Its logarithmic slopes are $5/12$ for nonrelativistic [Electrons](../../../../../electron.md) and $1/3$ for ultrarelativistic [Electrons](../../../../../electron.md). One must compare the pressures separately from the degeneracy criterion; extrapolating the classical gas-radiation line into a degenerate region is incorrect.

<a id="4/image-density-temperature-crossover-diagram-for-classical-gas-radiation-and-electron-degeneracy-illustrated-for-fully-ionized-carbon"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55-eos-regimes.png)

**[Figure 2](#4/image-density-temperature-crossover-diagram-for-classical-gas-radiation-and-electron-degeneracy-illustrated-for-fully-ionized-carbon). Density-temperature crossover diagram for classical gas, radiation and electron degeneracy, illustrated for fully ionized carbon**.

The [stellar equation-of-state regime diagram](../../../../../stellar-equation-of-state-regime-diagram.md) uses an illustrative fully ionized [carbon](../../../../../carbon.md) composition, $\mu_e=2$, $\mu=12/7$. It displays the electron-degeneracy crossover, both radiation-pressure comparisons, and distinct thermal and density-driven relativity scales. The curves are limiting-model comparisons, not sharp phase boundaries or a calibrated complete equation of state. Partial [ionization](../../../../../ionization.md), molecular physics and interactions modify the low-temperature regions indicated on the plot.

At sufficiently high [temperature](../../../../../temperature.md), [electron-positron thermal pair abundance](../../../../../electron-positron-thermal-pair-abundance.md) can become important. The pair abundance depends on density and [chemical potential](../../../../../chemical-potential.md) as well as [temperature](../../../../../temperature.md); $k_BT=m_ec^2$ is not a universal onset line. In the dilute ultrarelativistic limit, both pair species together add energy density $7a_rT^4/4$ to the [photons](../../../../../photon.md)' $a_rT^4$, and have [pressure](../../../../../pressure.md) one third of their energy density. While pairs are being created, thermal energy is spent on rest mass, which can reduce the [stellar adiabatic exponent](../../../../../stellar-adiabatic-exponent.md) below $4/3$ and contribute to [pair-instability supernova](../../../../../pair-instability-supernova.md) physics.

At high [mass density](../../../../../density.md) and low [temperature](../../../../../temperature.md), Interactions governed by [Coulomb's law](../../../../../coulomb-s-law.md) invalidate the noninteracting-ion approximation. The [ionic Coulomb coupling parameter](../../../../../ionic-coulomb-coupling-parameter.md) $\Gamma=Z^2e^2/(4\pi\epsilon_0a_i k_BT)$, where $a_i=(3/(4\pi n_i))^{1/3}$, grows as $\rho^{1/3}/T$. Corrections become significant when $\Gamma$ is of order one, and a sufficiently strongly coupled plasma can crystallize. At still greater [mass density](../../../../../density.md), [electron capture](../../../../../electron-capture.md) alters $\mu_e$ and nuclear matter replaces the ideal electron-ion model; [neutron star](../../../../../neutron-star.md) interiors require strong-interaction and relativistic equations of state. These further regimes lie beyond the simple [pressure](../../../../../pressure.md) curves plotted here. **A useful stellar EOS is thermodynamically consistent across the crossovers**, rather than just the maximum of unrelated [pressure](../../../../../pressure.md) laws.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
