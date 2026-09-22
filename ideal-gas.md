# Ideal gas

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_gas)

An ideal gas is a model of a dilute [gas](thermodynamics.md#gas) whose particle centres move according to [classical mechanics](classical-mechanics.md) and occupy negligible [volume](thermodynamics.md#volume-thermodynamics) compared with their container. Treating the particles as [point masses](classical-mechanics.md#point-mass) removes the molecular-size correction; neglecting interactions between separated particles removes the intermolecular contribution to [potential energy](energy.md#potential-energy). The usual [kinetic theory](kinetic-theory.md) model retains brief [elastic collisions](classical-mechanics.md#elastic-collision) with the walls and, optionally, with other particles: these transfer [momentum](momentum.md) while conserving the total [kinetic energy](energy.md#kinetic-energy) of the colliding bodies. There is no appreciable interaction [energy](energy.md) stored between [collisions](classical-mechanics.md#collision). These assumptions lead to the [ideal gas law](#ideal-gas-law), $PV=Nk_BT$. [OpenStax University Physics Volume 2, section 2.1: molecular model and ideal gas law](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/2-1-molecular-model-of-an-ideal-gas) [OpenStax University Physics Volume 2, section 2.2: kinetic-model assumptions](https://openstax.org/books/university-physics-volume-2/pages/2-2-pressure-temperature-and-rms-speed)

The model's attraction is its universality: at the same [temperature](temperature.md) and [number density](statistical-physics.md#number-density), different classical [ideal gases](ideal-gas.md) have the same [pressure](pressure.md), even when their particle [masses](classical-mechanics.md#mass) differ. In [ideal gas pressure from wall collisions](#ideal-gas-pressure-from-wall-collisions), heavier particles move more slowly at a given [temperature](temperature.md), and the two effects cancel. For example, one [mole](physics.md#mole-unit) of any [ideal gas](ideal-gas.md) at $300\,\mathrm K$ in $0.025\,\mathrm{m^3}$ has [pressure](pressure.md) approximately $99.774\,\mathrm{kPa}$, as computed under the [ideal gas law](#ideal-gas-law).

The [ideal gas law](#ideal-gas-law) describes the translational contribution to [pressure](pressure.md); it does not specify all of the [internal energy](internal-energy.md) or the [heat capacity](heat.md#heat-capacity). A [monatomic gas](#monatomic-gas) has three classical translational [degrees of freedom](classical-mechanics.md#degree-of-freedom), whereas a [gas](thermodynamics.md#gas) of [molecules](molecule.md) can also store [rotational kinetic energy](energy.md#rotational-kinetic-energy) and [energy](energy.md) in vibrational [normal modes](wave-equation.md#normal-mode). An [equation of state](pressure.md#equation-of-state) alone therefore does not determine how much [heat](heat.md) a chosen [temperature](temperature.md) increase requires. It also does not select a process: [isothermal expansion](second-law-of-thermodynamics.md#isothermal-expansion) and [adiabatic expansion](first-law-of-thermodynamics.md#adiabatic-expansion) need different additional constraints. [OpenStax University Physics Volume 2, section 2.3: internal degrees of freedom and heat capacity](https://openstax.org/books/university-physics-volume-2/pages/2-3-heat-capacity-and-equipartition-of-energy)

A [real gas](thermodynamics.md#real-gas) departs from this approximation when particle size or interactions become important, especially at high [number density](statistical-physics.md#number-density) or low [temperature](temperature.md) near a [phase transition](critical-phenomenon.md#phase-transition). The [Van der Waals equation](pressure.md#van-der-waals-equation) adds such corrections. Independently, at sufficiently low [temperature](temperature.md) or high [number density](statistical-physics.md#number-density), [quantum statistics](quantum-ideal-gas-statistics.md) can become essential: even particles with negligible interactions need not obey the classical [ideal gas law](#ideal-gas-law). The classical statistical assumption is the [nondegenerate gas](#nondegenerate-gas) regime, which is distinct from neglecting interactions. [OpenStax University Physics Volume 2, section 2.1: departures from ideal-gas behavior](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/2-1-molecular-model-of-an-ideal-gas) [3 Quantum Gases](physics-bibliography.md#statistical-physics-by-david-tong/3-quantum-gases)

**Table of contents**

- [Classical ideal-gas entropy limits](#classical-ideal-gas-entropy-limits)
- [Isobaric ideal-gas internal-energy density](#isobaric-ideal-gas-internal-energy-density)
- [Mean particle mass](#mean-particle-mass)
- [Diatomic gas](#diatomic-gas)
- [Specific gas constant](#specific-gas-constant)
- [Two-dimensional ideal gas](#two-dimensional-ideal-gas)
- [Classical grand potential in a harmonic trap](#classical-grand-potential-in-a-harmonic-trap)
- [Partial pressure](#partial-pressure)
- [Molar gas constant](#molar-gas-constant)
- [Ideal gas law](#ideal-gas-law)
  - [Ideal gas pressure from wall collisions](#ideal-gas-pressure-from-wall-collisions)
- [Monatomic gas](#monatomic-gas)
- [Mean free path](#mean-free-path)
  - [Transport mean free path](#transport-mean-free-path)
  - [Mean free path through randomly oriented disc absorbers](#mean-free-path-through-randomly-oriented-disc-absorbers)
- [Mean molecular weight](#mean-molecular-weight)
  - [Stellar gas constant](#stellar-gas-constant)
  - [Mean molecular weight per ion](#mean-molecular-weight-per-ion)
  - [Mean molecular weight per electron](#mean-molecular-weight-per-electron)
- [Heat capacity ratio](#heat-capacity-ratio)
  - [Rüchardt experiment](#ruchardt-experiment)
  - [Clément-Desormes experiment](#clement-desormes-experiment)
- [Nondegenerate gas](#nondegenerate-gas)
- [Internal energy of an ideal gas](#internal-energy-of-an-ideal-gas)
- [Mayer's relation](#mayer-s-relation)

## Classical ideal-gas entropy limits

↑ **Parent:** [Ideal gas](ideal-gas.md)

For constant positive [molar heat capacity](heat.md#molar-heat-capacity), the [ideal gas](ideal-gas.md) [entropy](entropy.md) grows without bound on isothermal dilution to unbounded [volume](geometry-and-topology.md#volume), corresponding to $p\to0$. This is a meaningful limiting configuration count, not an infinite [entropy](entropy.md) in a finite container. Extrapolation to $T\to0$ at fixed positive [pressure](pressure.md) instead predicts negative infinite [entropy](entropy.md). That extrapolation fails: phase changes, [quantum statistics](quantum-ideal-gas-statistics.md) and temperature-dependent [heat capacities](heat.md#heat-capacity) prevent a real equilibrium substance from retaining the same classical formula down to zero [temperature](temperature.md).

## Isobaric ideal-gas internal-energy density

↑ **Parent:** [Ideal gas](ideal-gas.md)

An [ideal gas](ideal-gas.md) with constant [heat capacity ratio](#heat-capacity-ratio) $\gamma$ has $U=n c_{V,m}T$ up to a consistent thermal-energy reference, and $c_{V,m}=R/(\gamma-1)$. Combining this with $pV=nRT$ gives the displayed thermal internal-energy [density](fluid-mechanics.md#density). At fixed [pressure](pressure.md) it does not grow with [temperature](temperature.md): the particle [density](fluid-mechanics.md#density) falls as $1/T$. A fixed-volume space exchanging gas with the atmosphere therefore differs from a sealed fixed-particle system. Composition changes, activated internal modes or a [pressure](pressure.md) change require a modified comparison.

## Mean particle mass

↑ **Parent:** [Ideal gas](ideal-gas.md)

The [mean particle mass](#mean-particle-mass) is the [mass density](fluid-mechanics.md#density) divided by the total [number density](statistical-physics.md#number-density) of freely moving particles. It enters $P=\rho k_BT/\bar m$. [ionization](atomic-physics.md#ionization) changes the particle count without significantly changing the [mass](classical-mechanics.md#mass), so it changes $\bar m$. The [dimensionless](physics.md#dimensionless-quantity) [mean molecular weight](#mean-molecular-weight) is $\bar m$ divided by a stated reference [mass](classical-mechanics.md#mass), commonly the atomic [mass](classical-mechanics.md#mass) unit; it must not be substituted as a [dimensionless](physics.md#dimensionless-quantity) number into a formula requiring a [mass](classical-mechanics.md#mass).

## Diatomic gas

↑ **Parent:** [Ideal gas](ideal-gas.md)

A gas whose constituent molecules have two atoms. In the classical ideal-gas regime with three translational and two rotational degrees of freedom active but vibration frozen, $c_v=5\mathcal R/2$, $c_p=7\mathcal R/2$ and $\gamma=7/5$. Vibrational excitation, rotational freezing or chemical changes alter this heat-capacity model.

## Specific gas constant

↑ **Parent:** [Ideal gas](ideal-gas.md)

The gas constant per unit [mass](classical-mechanics.md#mass) for a specified composition. An [ideal gas](ideal-gas.md) obeys $p=\rho\mathcal RT$. With dimensionless [mean molecular weight](#mean-molecular-weight) $\mu$ relative to an atomic [mass](classical-mechanics.md#mass) unit, $\mathcal R=k_B/(\mu m_u)$; the common astrophysical notation $R^*/\mu$ uses a modified mass-based constant rather than the molar gas constant without a [mass](classical-mechanics.md#mass) conversion.

## Two-dimensional ideal gas

↑ **Parent:** [Ideal gas](ideal-gas.md)

An [ideal gas](ideal-gas.md) whose particles move in an [area](differential-geometry.md#surface-area) $A$ with two independent translational momentum components. In its dilute classical limit the one-particle [translational partition function](canonical-ensemble.md#translational-partition-function) is $q=A/\Lambda^2$, where $\Lambda$ is the [thermal de Broglie wavelength](canonical-ensemble.md#thermal-de-broglie-wavelength), and $Z_N=q^N/N!$. The translational [internal energy](internal-energy.md) is $Nk_{\rm B}T$, and the surface pressure conjugate to [area](differential-geometry.md#surface-area) is $Nk_{\rm B}T/A$. A mobile dilute adsorbed gas is an example; a fully occupied array of fixed [adsorption sites](physical-chemistry.md#adsorption-site) has different state counting.

## Classical grand potential in a harmonic trap

↑ **Parent:** [Ideal gas](ideal-gas.md)

For noninteracting particles in a three-dimensional isotropic [quantum harmonic oscillator](quantum-harmonic-oscillator.md), measure the one-particle ground energy as zero. The single-particle [partition function](canonical-ensemble.md#canonical-partition-function) is $Z_1=(1-e^{-\beta\hbar\omega})^{-3}$, from the product of three [geometric series](sequence-and-series.md#geometric-series). In the dilute [Maxwell–Boltzmann statistics](quantum-ideal-gas-statistics.md#maxwell-boltzmann-statistics) regime, $\ln\Xi=e^{\beta\mu}Z_1$, so the [grand potential](statistical-physics.md#grand-potential) is the displayed expression and $N=e^{\beta\mu}Z_1$. For $k_BT\gg\hbar\omega$,

$$
\Phi\simeq-\frac{(k_BT)^4}{(\hbar\omega)^3}e^{\beta\mu},\qquad\mu\simeq k_BT\ln\left[N\left(\frac{\hbar\omega}{k_BT}\right)^3\right].
$$

The same approximation follows from integrating the [density of states](quantum-ideal-gas-statistics.md#density-of-states) $g(E)\simeq E^2/[2(\hbar\omega)^3]$ against $e^{-\beta E}$. Extrapolating the classical formula until the fugacity is one gives the scale of [Bose condensation in a three-dimensional harmonic trap](quantum-ideal-gas-statistics.md#bose-condensation-in-a-three-dimensional-harmonic-trap), but the quantitative transition temperature requires the Bose occupation law rather than Maxwell-Boltzmann statistics.

## Partial pressure

↑ **Parent:** [Ideal gas](ideal-gas.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_pressure)

The [partial pressure](#partial-pressure) of a component of a [gas](thermodynamics.md#gas) [mixture](mixture.md) is the [pressure](pressure.md) it would exert alone at the same [temperature](temperature.md) and total [volume](thermodynamics.md#volume-thermodynamics). For an ideal [mixture](mixture.md), $p_i=n_iRT/V$ and $p=\sum_i p_i$. The [chemical potential of an ideal gas](chemical-potential.md#chemical-potential-of-an-ideal-gas) uses $p_i$ for that component rather than the total [pressure](pressure.md) $p$.

## Molar gas constant

↑ **Parent:** [Ideal gas](ideal-gas.md)

The molar gas constant is the product of the [Avogadro constant](physics.md#avogadro-constant) and the [Boltzmann constant](thermodynamics.md#boltzmann-constant). It converts the particle-number form of the [ideal gas law](#ideal-gas-law), $pV=Nk_BT$, into the amount-of-substance form $pV=nRT$, using $N=nN_A$ with $n$ measured in [moles](physics.md#mole-unit).

## Ideal gas law

↑ **Parent:** [Ideal gas](ideal-gas.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_gas_law)

The [ideal gas law](#ideal-gas-law) is the [equation of state](pressure.md#equation-of-state) relating the absolute [pressure](pressure.md) $P$, [volume](thermodynamics.md#volume-thermodynamics) $V$, particle count $N$, and absolute [thermodynamic temperature](second-law-of-thermodynamics.md#thermodynamic-temperature) $T$ of a classical [ideal gas](ideal-gas.md):

$$
PV=Nk_BT=n_{\rm mol}RT,\qquad
N=n_{\rm mol}N_{\mathrm A},\qquad R=N_{\mathrm A}k_B.
$$

Here $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant), $N_{\mathrm A}$ is the [Avogadro constant](physics.md#avogadro-constant), $R$ is the [molar gas constant](#molar-gas-constant), and $n_{\rm mol}$ is the [amount of substance](physics.md#amount-of-substance) in [moles](physics.md#mole-unit). The distinct symbol $n_{\rm mol}$ avoids confusing [amount of substance](physics.md#amount-of-substance) with the [number density](statistical-physics.md#number-density) $n=N/V$, measured in $\mathrm{m^{-3}}$: the same law can be written $P=nk_BT$. Use absolute [pressure](pressure.md), relative to a [vacuum](physics.md#vacuum), rather than an unconverted [gauge pressure](fluid-mechanics.md#gauge-pressure). [OpenStax University Physics Volume 2, section 2.1: particle-count and molar forms](physics-bibliography.md#university-physics-volume-2-by-samuel-j-ling-and-others/2-1-molecular-model-of-an-ideal-gas)

The exact [SI](physics.md#international-system-of-units) definitions of the [Avogadro constant](physics.md#avogadro-constant) and [Boltzmann constant](thermodynamics.md#boltzmann-constant) give

$$
R=(6.02214076\times10^{23})(1.380649\times10^{-23})
\,\mathrm{J\,mol^{-1}\,K^{-1}}
=8.31446261815324\,\mathrm{J\,mol^{-1}\,K^{-1}}.
$$

This numerical value is exact; the applicability of the [ideal gas](ideal-gas.md) model to a [real gas](thermodynamics.md#real-gas) is an approximation. [BIPM, exact Avogadro constant in the mole definition](https://www.bipm.org/en/si-base-units/mole) [BIPM, exact Boltzmann constant in the kelvin definition](https://www.bipm.org/en/si-base-units/kelvin)

For $n_{\rm mol}=1\,\mathrm{mol}$, $T=300\,\mathrm K$, and $V=0.025\,\mathrm{m^3}$, direct substitution gives

$$
RT=2494.338785445972\,\mathrm{J\,mol^{-1}},\qquad
P=\frac{n_{\rm mol}RT}{V}
=99773.55141783888\,\mathrm{Pa}
\approx99.774\,\mathrm{kPa}.
$$

At fixed [temperature](temperature.md) and particle count, doubling the [volume](thermodynamics.md#volume-thermodynamics) to $0.050\,\mathrm{m^3}$ halves the [pressure](pressure.md) to approximately $49.887\,\mathrm{kPa}$: this is [Boyle's law](second-law-of-thermodynamics.md#boyle-s-law). At fixed [volume](thermodynamics.md#volume-thermodynamics) and particle count, doubling the [temperature](temperature.md) from $300\,\mathrm K$ to $600\,\mathrm K$ doubles the [pressure](pressure.md) to approximately $199.547\,\mathrm{kPa}$. These ratios use [kelvins](temperature.md#kelvin), not readings in the [degree Celsius](temperature.md#degree-celsius) scale: $300\,\mathrm K$ is $26.85\,{}^\circ\mathrm C$, and $600\,\mathrm K$ is $326.85\,{}^\circ\mathrm C$.

<a id="image-ideal-gas-law-pressure-versus-volume-at-fixed-temperatures-and-pressure-versus-absolute-temperature-at-fixed-volume"></a>
![](ideal-gas-state-slices.png)

**[Figure 1](#image-ideal-gas-law-pressure-versus-volume-at-fixed-temperatures-and-pressure-versus-absolute-temperature-at-fixed-volume). Ideal gas law: pressure versus volume at fixed temperatures, and pressure versus absolute temperature at fixed volume**.

The curved slices show [Boyle's law](second-law-of-thermodynamics.md#boyle-s-law) at three [temperatures](temperature.md); the straight slice shows proportionality to absolute [temperature](temperature.md) at one fixed [volume](thermodynamics.md#volume-thermodynamics). They are relations among equilibrium states, rather than a prescribed process history. Compression could hold the [temperature](temperature.md) fixed through [heat transfer](heat.md#heat-transfer), or raise it during [adiabatic compression](first-law-of-thermodynamics.md#adiabatic-compression). To calculate a process's [heat](heat.md) or [work](energy.md#work), supplement the [ideal gas law](#ideal-gas-law) with the process constraint, the [first law of thermodynamics](first-law-of-thermodynamics.md), and the relevant [internal energy](internal-energy.md) or [heat capacity](heat.md#heat-capacity) information. The graph's extrapolation toward $T=0$ is mathematical; it does not assert that a [real gas](thermodynamics.md#real-gas) remains classical or gaseous there.

For a stellar [mixture](mixture.md) with fixed [mean molecular weight](#mean-molecular-weight), the [ideal gas law](#ideal-gas-law) can be written $P=\mathcal R\rho T/\mu$, where $\rho$ is [mass density](fluid-mechanics.md#density) and $\mathcal R$ is the [stellar gas constant](#stellar-gas-constant). It assumes negligible interaction corrections and a [nondegenerate gas](#nondegenerate-gas); excitation or [ionization](atomic-physics.md#ionization) can change the particle count and thermodynamic response.

In his 1834 memoir on the motive power of [heat](heat.md), Émile Clapeyron combined gas laws into a relation between [pressure](pressure.md), [volume](thermodynamics.md#volume-thermodynamics), and [temperature](temperature.md) while analysing [heat engines](thermodynamics.md#heat-engine) (printed page 164). The equation above uses modern [SI](physics.md#international-system-of-units) notation and absolute [thermodynamic temperature](second-law-of-thermodynamics.md#thermodynamic-temperature); it is not a transcription of his historical temperature convention. [Clapeyron, Mémoire sur la puissance motrice de la chaleur (1834), page 164](https://www3.nd.edu/~powers/ame.20231/clapeyron1834.pdf)

### Ideal gas pressure from wall collisions

↑ **Parent:** [Ideal gas law](#ideal-gas-law)

Consider a particle of [mass](classical-mechanics.md#mass) $m$ in a rigid rectangular box of length $L$ along $x$ and wall [surface area](differential-geometry.md#surface-area) $A$, so $V=AL$ is the [volume](thermodynamics.md#volume-thermodynamics). Choose $+x$ toward the right wall. For an incoming normal [velocity](classical-mechanics.md#velocity) $v_x=v>0$, an [elastic collision](classical-mechanics.md#elastic-collision) reverses the normal [momentum](momentum.md):

$$
p_{x,\rm in}=mv,\qquad p_{x,\rm out}=-mv,\qquad
\Delta p_{x,\rm particle}=-2mv,\qquad
J_{x,\rm wall}=+2mv.
$$

The [impulse](classical-mechanics.md#impulse) delivered to the wall points outward, toward $+x$, by [Newton's third law](force.md#newton-s-third-law). The particle's opposite [momentum](momentum.md) change is not the wall's [impulse](classical-mechanics.md#impulse). A tangential [velocity](classical-mechanics.md#velocity) component is unchanged by the ideal smooth-wall [collision](classical-mechanics.md#collision).

<a id="image-schematic-ideal-gas-model-an-elastic-bounce-transfers-outward-momentum-to-a-wall-this-is-not-a-real-experimental-setup"></a>
![](ideal-gas-wall-momentum.png)

**[Figure 2](#image-schematic-ideal-gas-model-an-elastic-bounce-transfers-outward-momentum-to-a-wall-this-is-not-a-real-experimental-setup). Schematic ideal gas model: an elastic bounce transfers outward momentum to a wall; this is not a real experimental setup**.

Ignoring intervening particle-particle [collisions](classical-mechanics.md#collision) in this counting model, the particle travels a normal distance $2L$ before hitting the same wall again. Its hit rate is $|v_x|/(2L)$; multiplying by the [impulse](classical-mechanics.md#impulse) per hit gives the time-averaged normal [force](force.md) and its contribution to [pressure](pressure.md):

$$
\overline F_{\perp,1}=(2m|v_x|)\frac{|v_x|}{2L}
=\frac{mv_x^2}{L},\qquad
P_1=\frac{\overline F_{\perp,1}}{A}=\frac{mv_x^2}{V}.
$$

For example, stipulate $m=4\times10^{-26}\,\mathrm{kg}$, $|v_x|=500\,\mathrm{m\,s^{-1}}$, $L=0.10\,\mathrm m$, and $A=0.010\,\mathrm{m^2}$. Then $V=0.0010\,\mathrm{m^3}$, the [impulse](classical-mechanics.md#impulse) per hit is $4\times10^{-23}\,\mathrm{N\,s}$, the hit rate is $2500\,\mathrm{s^{-1}}$, and $P_1=10^{-17}\,\mathrm{Pa}$. This is one particle's tiny time-averaged contribution to one wall's [pressure](pressure.md), not an [isotropic](continuum-mechanics.md#isotropy) equilibrium [gas](thermodynamics.md#gas) by itself.

For $N$ particles of equal [mass](classical-mechanics.md#mass), add their [force](force.md) contributions and define $\langle v_x^2\rangle=N^{-1}\sum_{i=1}^Nv_{x,i}^2$. In the [gas](thermodynamics.md#gas)'s rest frame, [isotropy](continuum-mechanics.md#isotropy) gives $\langle v_x^2\rangle=\langle v_y^2\rangle=\langle v_z^2\rangle=\langle v^2\rangle/3$, where $v^2=v_x^2+v_y^2+v_z^2$. Hence

$$
P=\frac{Nm\langle v_x^2\rangle}{V}
=\frac{Nm\langle v^2\rangle}{3V},\qquad
\frac12m\langle v^2\rangle=\frac32k_BT
\quad\Longrightarrow\quad PV=Nk_BT.
$$

The final equality uses the classical [equipartition theorem](canonical-ensemble.md#equipartition-theorem). The [kinetic pressure of an isotropic gas](statistical-physics.md#kinetic-pressure-of-an-isotropic-gas) therefore recovers the [ideal gas law](#ideal-gas-law) from [momentum](momentum.md) transfers. Doubling the normal speed would double both the [impulse](classical-mechanics.md#impulse) per hit and the hit rate, giving four times the [pressure](pressure.md) contribution; [pressure](pressure.md) measures a mean squared speed. Interparticle [elastic collisions](classical-mechanics.md#elastic-collision) redistribute [velocities](classical-mechanics.md#velocity) and help establish [isotropy](continuum-mechanics.md#isotropy); the individual round-trip times need not remain $2L/|v_x|$, but the equilibrium [momentum flux](mathematical-physics.md#momentum-flux) result survives. [OpenStax University Physics Volume 2, section 2.2: wall-collision pressure derivation](https://openstax.org/books/university-physics-volume-2/pages/2-2-pressure-temperature-and-rms-speed)

## Monatomic gas

↑ **Parent:** [Ideal gas](ideal-gas.md)

A monatomic gas consists of individual atoms or ions rather than molecules. In the classical dilute ideal-gas regime, its three translational degrees of freedom give $U=3Nk_BT/2$ by [equipartition theorem](canonical-ensemble.md#equipartition-theorem). Thus $C_V=3Nk_B/2$, while $C_P-C_V=Nk_B$ follows by differentiating the ideal-gas enthalpy $H=U+PV=5Nk_BT/2$. Consequently the [adiabatic index](#heat-capacity-ratio) is $\gamma=C_P/C_V=5/3$ and the [specific internal energy](internal-energy.md#specific-internal-energy) is $e=3P/(2\rho)$. The same translational result applies to a fully ionized mixture when the particle numbers are fixed. This excludes additional excitation, ionization and radiation contributions to the heat capacity.

## Mean free path

↑ **Parent:** [Ideal gas](ideal-gas.md)

The mean free path is the average distance travelled between [collisions](classical-mechanics.md#collision). For dilute targets with [number density](statistical-physics.md#number-density) $n$ and effective [collision cross-section](classical-mechanics.md#collision-cross-section) $\sigma_c$, $\ell\sim1/(n\sigma_c)$; identical-particle conventions introduce factors such as $\sqrt2$.

### Transport mean free path

↑ **Parent:** [Mean free path](#mean-free-path)

The length associated with relaxation of carrier momentum. In a parabolic band, [electron mobility](electric-charge.md#electron-mobility) measures the [momentum relaxation time](electric-charge.md#momentum-relaxation-time), giving the displayed expression. Frequent weak small-angle scattering can make the single-particle scattering time shorter than the transport time, and [electron phase coherence](density-matrix.md#electron-phase-coherence) has its own lifetime.

### Mean free path through randomly oriented disc absorbers

↑ **Parent:** [Mean free path](#mean-free-path)

For an unclustered population of fully covering circular disc absorbers, the inverse [mean free path](#mean-free-path) is proper number density times mean projected area. A comoving number density must first be multiplied by $(1+z)^3$. The incidence then constrains the proper radius; covering factor and multiplicity of detectable lines can change the inference.

## Mean molecular weight

↑ **Parent:** [Ideal gas](ideal-gas.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_molecular_weight)

The mean molecular weight is the average mass per freely moving gas particle in units of the atomic mass unit. A fully ionized hydrogen-helium gas with mass fractions $X,Y$ has $\mu^{-1}=2X+3Y/4$.

### Stellar gas constant

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

In stellar [ideal gas](ideal-gas.md) equations, the [stellar gas constant](#stellar-gas-constant) $\mathcal R=k_B/m_u$ converts a dimensionless [mean molecular weight](#mean-molecular-weight) $\mu$ into the specific thermal relation $P=\mathcal R\rho T/\mu$. Here $m_u$ is the reference atomic mass unit, commonly approximated by the proton mass in simplified hydrogen-helium models. It has units of energy per mass per temperature. It is the molar gas constant divided by the molar mass corresponding to $m_u$, rather than the molar gas constant used with a dimensional molar molecular weight.

### Mean molecular weight per ion

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

The [mean molecular weight](#mean-molecular-weight) per ion counts nuclei rather than nuclei plus free electrons: $\rho/(\mu_i m_u)$ is the ion number density. For species with mass fractions $X_j$ and mass numbers $A_j$, $\mu_i^{-1}=\sum_jX_j/A_j$. It is useful when ions provide a thermal [ideal gas](ideal-gas.md) pressure but [electron degeneracy pressure](quantum-ideal-gas-statistics.md#electron-degeneracy-pressure) supplies a separate contribution.

### Mean molecular weight per electron

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

The mean molecular weight per electron is the mass carried per free electron in units of atomic mass $m_u$. Fully ionized hydrogen has $\mu_e=1$, while helium, carbon, and oxygen have approximately $\mu_e=2$. It converts [electron number density](statistical-physics.md#electron-number-density) to bulk [mass density](fluid-mechanics.md#density) in the [equation of state of a cold electron gas](quantum-ideal-gas-statistics.md#equation-of-state-of-a-cold-electron-gas).

## Heat capacity ratio

↑ **Parent:** [Ideal gas](ideal-gas.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_capacity_ratio)

The heat capacity ratio compares [heat capacity at constant pressure](enthalpy.md#heat-capacity-at-constant-pressure) $C_p$ with [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume) $C_V$ at the same equilibrium state and fixed composition:

$$
\gamma=\frac{C_p}{C_V}
=\frac{C_{p,\mathrm m}}{C_{V,\mathrm m}}
=\frac{c_p}{c_V}.
$$

Here $C_p,C_V$ refer to the whole sample, in $\mathrm{J\,K^{-1}}$; [molar heat capacities](heat.md#molar-heat-capacity) $C_{p,\mathrm m}=C_p/n$ and $C_{V,\mathrm m}=C_V/n$ are per [mole](physics.md#mole-unit); [specific heat capacities](heat.md#specific-heat-capacity) $c_p=C_p/m$ and $c_V=C_V/m$ are per unit [mass](classical-mechanics.md#mass). The [amount of substance](physics.md#amount-of-substance) $n$ or [mass](classical-mechanics.md#mass) $m$ cancels only when both capacities use the same normalization. Thus [heat capacity ratio](#heat-capacity-ratio) is dimensionless and independent of sample size. For a fixed-composition [ideal gas](ideal-gas.md) with positive finite $C_V$, [Mayer's relation](#mayer-s-relation) gives

$$
\gamma(T)=1+\frac{nR}{C_V(T)}=1+\frac{R}{C_{V,\mathrm m}(T)}>1,
$$

where $R$ is the [molar gas constant](#molar-gas-constant). More ways to store [internal energy](internal-energy.md) make a given [temperature](temperature.md) increase require more [heat](heat.md), bringing [heat capacity ratio](#heat-capacity-ratio) closer to unity. [MIT Unified Engineering, Specific heats: definitions and ideal-gas relations](https://web.mit.edu/16.unified/www/FALL/thermodynamics/notes/node18.html)

The [equipartition theorem](canonical-ensemble.md#equipartition-theorem) predicts $C_{V,\mathrm m}=fR/2$ when $f$ independent quadratic terms in molecular [energy](energy.md) are thermally active and their number stays fixed; consequently $\gamma=1+2/f$. A classical [monatomic gas](#monatomic-gas) with no appreciable electronic excitation has $f=3$, giving $C_{V,\mathrm m}=3R/2$ and $\gamma=5/3$. For an [ideal gas](ideal-gas.md) of diatomic [molecules](molecule.md) with three translational and two rotational terms active, but its vibrational [normal mode](wave-equation.md#normal-mode) effectively frozen, $f=5$ gives $C_{V,\mathrm m}=5R/2$ and $\gamma=7/5$. A fully classical harmonic vibration adds both [kinetic energy](energy.md#kinetic-energy) and [potential energy](energy.md#potential-energy), giving $f=7$ and $\gamma=9/7$. These are model regimes, not universal constants of every [gas](thermodynamics.md#gas): rotational freezing, electronic excitation, and changing composition invalidate the simple count.[§§2.2.1 and 2.4: equipartition and diatomic gases](physics-bibliography.md#statistical-physics-by-david-tong/2-classical-gases)

The mechanical significance of [heat capacity ratio](#heat-capacity-ratio) follows from the [first law of thermodynamics](first-law-of-thermodynamics.md). For a fixed amount of [ideal gas](ideal-gas.md) in a reversible [adiabatic process](first-law-of-thermodynamics.md#adiabatic-process), $C_V(T)\,dT=-p\,dV$. Combining this with the [ideal gas law](#ideal-gas-law) gives the local relation

$$
\left(\frac{\partial\ln p}{\partial\ln V}\right)_S=-\gamma(T),\qquad
\int_{T_1}^{T_2}\frac{C_V(T)}{T}\,dT+nR\ln\frac{V_2}{V_1}=0.
$$

The [partial derivative](multivariable-calculus.md#partial-derivative) holds at fixed [entropy](entropy.md) and composition even when [heat capacity ratio](#heat-capacity-ratio) varies with [temperature](temperature.md). The finite-path formulas $pV^\gamma=\mathrm{constant}$ and $TV^{\gamma-1}=\mathrm{constant}$ require the additional approximation of constant [heat capacity ratio](#heat-capacity-ratio). A rapid compression also needs internal equilibration to approximate this path; rapid motion alone does not ensure reversibility. The same local response gives [isentropic compressibility](thermodynamics.md#isentropic-compressibility) $1/(\gamma p)$ and, for small sound disturbances in this [ideal gas](ideal-gas.md) regime, [speed of sound](compressible-flow.md#speed-of-sound) $a=\sqrt{\gamma p/\rho}$, where $\rho$ is [mass density](fluid-mechanics.md#density). Thus thermal storage controls mechanical stiffness, sound propagation and the measurements in [Rüchardt experiment](#ruchardt-experiment) and [Clément-Desormes experiment](#clement-desormes-experiment).

<h3 id="ruchardt-experiment">Rüchardt experiment</h3>

↑ **Parent:** [Heat capacity ratio](#heat-capacity-ratio)

The Rüchardt experiment infers [heat capacity ratio](#heat-capacity-ratio) from the [period of an oscillation](classical-mechanics.md#period-of-an-oscillation) of a piston supported by trapped [gas](thermodynamics.md#gas). Use a vertical precision cylinder with a close-fitting movable piston, known moving [mass](classical-mechanics.md#mass) $M$, face [area](differential-geometry.md#surface-area) $A$, trapped equilibrium [volume](thermodynamics.md#volume-thermodynamics) $V_0$, and local atmospheric [pressure](pressure.md) $p_{\rm atm}$. With negligible static [friction](newtonian-mechanics.md#friction), [force balance](force.md#force-balance) gives the absolute gas [pressure](pressure.md) $p_0=p_{\rm atm}+Mg/A$, where $g$ is gravitational acceleration. Displace the piston slightly and release it: compression raises [pressure](pressure.md), and expansion lowers it, producing a restoring [force](force.md). The [oscillation](wave.md#oscillation) is a mechanical probe of thermal response, without separately measuring two [heat](heat.md) inputs. [Instituto Superior Técnico e-lab, Determination of the Adiabatic Constant: piston apparatus and period model](https://groups.ist.utl.pt/wwwelab/wiki/index.php?title=Determination_of_the_Adiabatic_Constant)

Let $x$ be upward [displacement](classical-mechanics.md#displacement) from equilibrium, so $V=V_0+Ax$. For constant [heat capacity ratio](#heat-capacity-ratio) and a reversible [adiabatic process](first-law-of-thermodynamics.md#adiabatic-process), the net upward [force](force.md), including the ambient load and weight, is

$$
F(x)=A p_0\left[\left(1+\frac{Ax}{V_0}\right)^{-\gamma}-1\right]
\simeq-\frac{\gamma p_0A^2}{V_0}x.
$$

The [linear approximation](calculus.md#linear-approximation) requires $|Ax|/V_0\ll1$. Applying [Newton's second law](force.md#newton-s-second-law) gives [simple harmonic motion](classical-mechanics.md#simple-harmonic-motion) with

$$
\omega_0^2=\frac{\gamma p_0A^2}{MV_0},\qquad
\gamma=\frac{4\pi^2MV_0}{p_0A^2\mathcal T^2},\qquad
\mathcal T=\frac{2\pi}{\omega_0}.
$$

Here $\omega_0$ is the undamped [angular frequency](lagrangian-mechanics.md#angular-frequency) and $\mathcal T$ the undamped [oscillation period](classical-mechanics.md#period-of-an-oscillation), rather than [temperature](temperature.md). Record repeated cycles, measure $M,A,V_0,p_{\rm atm}$ independently, and include all connected trapped [volume](thermodynamics.md#volume-thermodynamics). An illustrative model with $M=0.020\,\mathrm{kg}$, $A=2.0\times10^{-4}\,\mathrm{m^2}$, $V_0=0.010\,\mathrm{m^3}$, $p_{\rm atm}=100000\,\mathrm{Pa}$, $g=9.81\,\mathrm{m\,s^{-2}}$ and $\gamma=1.4$ gives $p_0=100981\,\mathrm{Pa}$ and $\mathcal T\simeq1.182\,\mathrm s$. These stipulated values are not measurements.

<a id="image-ruchardt-experiment-heat-capacity-ratio-sets-the-restoring-stiffness-of-trapped-gas"></a>
![](heat-capacity-ratio-gas-spring.png)

**[Figure 3](#image-ruchardt-experiment-heat-capacity-ratio-sets-the-restoring-stiffness-of-trapped-gas). Rüchardt experiment: heat capacity ratio sets the restoring stiffness of trapped gas**. Original schematic and analytical [ideal gas](ideal-gas.md) curves. Upward piston [displacement](classical-mechanics.md#displacement) increases [volume](thermodynamics.md#volume-thermodynamics); the blue curve uses constant $\gamma=1.4$, its dashed tangent gives the small-[amplitude](wave.md#wave-amplitude) model, and the orange curve is the [isothermal process](second-law-of-thermodynamics.md#isothermal-process) limit. The shaded central interval illustrates a small fractional [volume](thermodynamics.md#volume-thermodynamics) change, without specifying an experimental acceptance threshold. No measured waveform is shown.

In Shearwood and Sloan's implementation, piston-mounted magnets induce an [electromotive force](electric-charge.md#electromotive-force) in a stationary coil through [Faraday's law of induction](maxwell-equations.md#faraday-s-law-of-induction); an oscilloscope records the signal. They observed faster [oscillations](wave.md#oscillation) at smaller trapped [volume](thermodynamics.md#volume-thermodynamics) values and stronger [damping](wave-equation.md#damping) at small cylinder [volume](thermodynamics.md#volume-thermodynamics) values. The signal tracks [velocity](classical-mechanics.md#velocity) locally, so its [amplitude](wave.md#wave-amplitude) is not directly piston [displacement](classical-mechanics.md#displacement). Calibration also identified inlet dead space beyond the graduated cylinder volume. [Chris Shearwood and Peter A. Sloan, The Rüchardt experiment revisited, §§3–4: signal, dead volume and observations](https://arxiv.org/html/2209.03323v1)

Repeat at smaller initial [amplitudes](wave.md#wave-amplitude) to test the [linear approximation](calculus.md#linear-approximation), and compare several $V_0$ values. [Heat transfer](heat.md#heat-transfer) weakens the restoring [force](force.md) toward the [isothermal process](second-law-of-thermodynamics.md#isothermal-process) limit, biasing the inference toward $1$. Check leakage through resting-piston drift and before-and-after trapped [volume](thermodynamics.md#volume-thermodynamics) readings. For viscous [damping](wave-equation.md#damping) with envelope $e^{-t/\tau}$, the measured [angular frequency](lagrangian-mechanics.md#angular-frequency) obeys $\omega_0^2=\omega_d^2+\tau^{-2}$; this correction does not remove thermal leakage. Internal equilibration must be faster than an [oscillation period](classical-mechanics.md#period-of-an-oscillation), with [heat transfer](heat.md#heat-transfer) and leakage slow over a run. Large [amplitude](wave.md#wave-amplitude) or sticking [friction](newtonian-mechanics.md#friction) require a richer model. [Shearwood and Sloan, §§2.1, 2.4 and 3.2: damping, heat exchange and leakage limitations](https://arxiv.org/html/2209.03323v1)

<h3 id="clement-desormes-experiment">Clément-Desormes experiment</h3>

↑ **Parent:** [Heat capacity ratio](#heat-capacity-ratio)

The Clément-Desormes experiment infers [heat capacity ratio](#heat-capacity-ratio) from a rapid [pressure](pressure.md) reduction followed by reheating. Use a rigid bottle, pump or bellows, a quick release valve, and a U-tube [pressure](pressure.md) gauge connected to the bottle and atmosphere. First pump to a small excess [pressure](pressure.md), close the inlet, and wait for [thermal equilibrium](thermal-equilibrium.md) with the room at $T_0$. Measure $p_1>p_a$, where $p_a$ is local absolute atmospheric [pressure](pressure.md). Briefly open the release valve until the bottle reaches $p_a$, then close it promptly. The remaining [gas](thermodynamics.md#gas) is cooler than the room. As it warms back to $T_0$ at fixed bottle [volume](thermodynamics.md#volume-thermodynamics), its [pressure](pressure.md) rises to $p_3$, with $p_a<p_3<p_1$ in the ideal procedure. The rebound reveals cooling during release. [KIT Faculty of Physics, Clément-Desormes laboratory protocol: release and pressure rebound](https://labs.physik.kit.edu/prakt-nebenfach-manuals/Experiments/Adiabatenexponent_Luft/)

The bottle loses [molecules](molecule.md) while the valve is open: it is not a [closed system](thermodynamics.md#closed-system) whose geometrical [volume](thermodynamics.md#volume-thermodynamics) expands. In the well-mixed, negligible-[heat transfer](heat.md#heat-transfer) discharge model with constant [heat capacity ratio](#heat-capacity-ratio), the remaining [gas](thermodynamics.md#gas) obeys $T_2/T_0=(p_a/p_1)^{(\gamma-1)/\gamma}$. Subsequent heating at fixed [amount of substance](physics.md#amount-of-substance) and bottle [volume](thermodynamics.md#volume-thermodynamics) gives $p_3/p_a=T_0/T_2$ by the [ideal gas law](#ideal-gas-law). Eliminating the unmeasured $T_2$ yields

$$
\gamma=\frac{\ln(p_1/p_a)}{\ln(p_1/p_3)}
\simeq\frac{\Delta p_1}{\Delta p_1-\Delta p_3}
=\frac{h_1}{h_1-h_3},\qquad
\Delta p_i=p_i-p_a=\rho_{\rm liquid}gh_i.
$$

The [logarithms](calculus.md#logarithm) use absolute [pressure](pressure.md) ratios. The approximation requires small [gauge pressures](fluid-mechanics.md#gauge-pressure) $\Delta p_i\ll p_a$; $h_i$ are signed height differences between the two liquid surfaces, and the final equality uses the same liquid in both readings with [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). It is not an instruction to insert gauge readings into the logarithmic formula. For synthetic states generated with $p_a=100000\,\mathrm{Pa}$, $p_1=102000\,\mathrm{Pa}$ and $\gamma=1.4$, the model gives $p_3\simeq100567.39\,\mathrm{Pa}$. The logarithmic inference recovers $1.4$; the small-[pressure](pressure.md) approximation gives approximately $1.3961$.

Wait for a stable initial [pressure](pressure.md) after pumping and for a stable final [pressure](pressure.md) after closing. Vary the valve-open interval and initial excess [pressure](pressure.md) across repeated trials: closing too early leaves residual excess [pressure](pressure.md), while leaving the valve open during warming lets more [gas](thermodynamics.md#gas) escape and suppresses the rebound. Test the seal for leaks, and read both liquid levels consistently. In a variant with incomplete release, measure the actual immediate post-release absolute [pressure](pressure.md) $p_2$ and replace the numerator by $\ln(p_1/p_2)$. The Zurich laboratory manual explains that liquid-column [oscillations](wave.md#oscillation) can delay this reading until appreciable reheating has occurred; its proposed backward extrapolation assumes an exponential thermal relaxation and must be checked against the recorded readings. These controls separate a thermal signal from valve timing, instrumental lag and leakage. [University of Zurich, PHY112/122 laboratory manual, §1.3 and Appendix 1.4(a): pressure readings and reheating correction](https://www.physik.uzh.ch/~matthias/espace-assistant/manuals/en/anleitung-cd_e.pdf)

## Nondegenerate gas

↑ **Parent:** [Ideal gas](ideal-gas.md)

A gas is nondegenerate when its occupation numbers are low enough that [quantum statistics](quantum-ideal-gas-statistics.md) reduce to the [Maxwell-Boltzmann distribution](quantum-ideal-gas-statistics.md#maxwell-boltzmann-distribution). A common criterion is $n\lambda_{\rm th}^3\ll1$, where $\lambda_{\rm th}$ is the thermal de Broglie wavelength.

For an [ideal gas](ideal-gas.md), this is the classical statistical regime; nondegeneracy alone does not assert the absence of interactions.

## Internal energy of an ideal gas

↑ **Parent:** [Ideal gas](ideal-gas.md)

For a fixed [amount of substance](physics.md#amount-of-substance) and composition of classical [ideal gas](ideal-gas.md), [internal energy](internal-energy.md) depends only on [temperature](temperature.md): $U=U(T,n)$, with no independent [volume](thermodynamics.md#volume-thermodynamics) dependence. This does not require constant [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume). Between equilibrium endpoints,

$$
dU=C_V(T)\,dT=nC_{V,\mathrm m}(T)\,dT,
\qquad U(T_2)-U(T_1)=n\int_{T_1}^{T_2}C_{V,\mathrm m}(T)\,dT.
$$

Here $C_V$ is total [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume), $C_{V,\mathrm m}$ is [molar heat capacity](heat.md#molar-heat-capacity), and $U/m$ for sample [mass](classical-mechanics.md#mass) $m$ is [specific internal energy](internal-energy.md#specific-internal-energy), whose change is $\int_{T_1}^{T_2}c_V(T)\,dT$. These endpoint relations apply even when the intervening process is not at fixed [volume](thermodynamics.md#volume-thermodynamics); they do not say that transferred [heat](heat.md) always equals $\Delta U$. With constant $C_V$, the safe statement is $U(T)=U(T_*)+C_V(T-T_*)$. Writing $U=C_VT$ additionally chooses the reference [energy](energy.md); it does not prove that a physical [gas](thermodynamics.md#gas) remains classical and ideal down to zero [temperature](temperature.md). [Richard Feynman, Robert Leighton and Matthew Sands, §45-1: internal-energy derivatives and heat capacity](https://www.feynmanlectures.caltech.edu/I_45.html#Ch45-S1)

A thermodynamic proof outline uses the [first law of thermodynamics](first-law-of-thermodynamics.md) in equilibrium form, $dU=T\,dS-p\,dV$, and the [Maxwell relation](thermodynamics.md#maxwell-relations) $(\partial S/\partial V)_T=(\partial p/\partial T)_V$:

$$
\left(\frac{\partial U}{\partial V}\right)_T
=T\left(\frac{\partial p}{\partial T}\right)_V-p
=T\frac{nR}{V}-\frac{nRT}{V}=0.
$$

The last step uses the [ideal gas law](#ideal-gas-law) and the [molar gas constant](#molar-gas-constant) $R$, with fixed composition and [amount of substance](physics.md#amount-of-substance). Microscopically, separated [ideal gas](ideal-gas.md) particles store no intermolecular interaction [energy](energy.md); their translational [kinetic energy](energy.md#kinetic-energy) and any internal molecular [energy](energy.md) are determined by [temperature](temperature.md). Negligible intermolecular interactions still allow a [molecule](molecule.md) to have internal vibrational [potential energy](energy.md#potential-energy).

An original analytical model makes the distinction between an [ideal gas](ideal-gas.md) and constant [heat capacity](heat.md#heat-capacity) concrete. Assume classical translation, two fully active rotational terms, and one independent [quantum harmonic oscillator](quantum-harmonic-oscillator.md) per diatomic [molecule](molecule.md), with fixed [angular frequency](lagrangian-mechanics.md#angular-frequency) $\omega$. Define the vibrational [temperature](temperature.md) scale $\Theta=\hbar\omega/k_B$, using the reduced [Planck constant](quantum-mechanics.md#planck-constant) $\hbar=h/(2\pi)$ and [Boltzmann constant](thermodynamics.md#boltzmann-constant) $k_B$. Summing its thermal occupations gives

$$
\frac{U(T)-U_*}{nR}=\frac52T+\frac{\Theta}{e^{\Theta/T}-1},\qquad
\frac{C_{V,\mathrm m}(T)}{R}=\frac52+\frac{x^2e^{-x}}{(1-e^{-x})^2},\qquad x=\frac{\Theta}{T}.
$$

The constant $U_*$ includes the chosen reference and [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy), whose [temperature](temperature.md) derivative vanishes. When $T\ll\Theta$ the vibrational contribution to [heat capacity](heat.md#heat-capacity) is exponentially small; when $T\gg\Theta$ it tends to $R$ per [mole](physics.md#mole-unit). This model assumes rotations remain active throughout the interval and excludes dissociation, electronic excitation and [real gas](thermodynamics.md#real-gas) corrections. Its low-$T/\Theta$ edge is not a model of rotational freezing or of an actual substance at absolute zero.[§3.4: quantum vibrational spectrum, thermal occupations and zero-point energy](physics-bibliography.md#statistical-physics-by-david-tong/3-quantum-gases)

<a id="image-temperature-dependent-internal-energy-of-an-ideal-gas-molar-heat-capacities-and-heat-capacity-ratio-in-a-vibrational-model"></a>
![](heat-capacity-ratio-vibrational-model.png)

**[Figure 4](#image-temperature-dependent-internal-energy-of-an-ideal-gas-molar-heat-capacities-and-heat-capacity-ratio-in-a-vibrational-model). Temperature-dependent internal energy of an ideal gas, molar heat capacities and heat capacity ratio in a vibrational model**. Analytical illustration with active rotations and one [quantum harmonic oscillator](quantum-harmonic-oscillator.md) per [molecule](molecule.md). Left: [Mayer's relation](#mayer-s-relation) keeps the capacity difference equal to $R$. Middle: [heat capacity ratio](#heat-capacity-ratio) falls from $7/5$ toward $9/7$. Right: the [internal energy](internal-energy.md) change from $T=0.2\Theta$ is an [integral](integral.md) of varying [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume); the dashed line suppresses the vibrational contribution. No measured gas curve or material-specific vibrational frequency is implied.

For this stipulated model, heating from $T_1=0.2\Theta$ to $T_2=\Theta$ gives $\Delta U/(nR\Theta)\simeq2.57519$. Holding the frozen-vibration value $C_{V,\mathrm m}=5R/2$ throughout would give $2$, underestimating the required [internal energy](internal-energy.md) increase by about $22.3\%$ of the model's full value. The [integral](integral.md) measures all thermal storage activated along the interval. At fixed [volume](thermodynamics.md#volume-thermodynamics) with only [heat](heat.md) input, this is also the supplied [heat](heat.md); at fixed [pressure](pressure.md), expansion [work](energy.md#work) must be added through [Mayer's relation](#mayer-s-relation).

[Joule's free-expansion experiment](thermodynamics.md#joule-s-free-expansion-experiment) tests the independence from [volume](thermodynamics.md#volume-thermodynamics) in a different way: an insulated rigid vessel allows [gas](thermodynamics.md#gas) into an evacuated compartment, so no external [work](energy.md#work) is delivered and ideally no [heat](heat.md) is exchanged. The [first law of thermodynamics](first-law-of-thermodynamics.md) gives $\Delta U=0$; positive $C_V$ then predicts equal initial and final equilibrium [temperatures](temperature.md) for the [ideal gas](ideal-gas.md). The apparatus, thermal-capacity controls and limitations of this inference are described in [Joule's free-expansion experiment](thermodynamics.md#joule-s-free-expansion-experiment) and [temperature sensitivity of a free-expansion experiment](thermodynamics.md#temperature-sensitivity-of-a-free-expansion-experiment). This endpoint test differs from the reversible [adiabatic expansion](first-law-of-thermodynamics.md#adiabatic-expansion) of a loaded piston, which delivers [work](energy.md#work) and lowers [internal energy](internal-energy.md).

<h2 id="mayer-s-relation">Mayer's relation</h2>

↑ **Parent:** [Ideal gas](ideal-gas.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mayer's_relation)

Mayer's relation states that the difference between [heat capacity at constant pressure](enthalpy.md#heat-capacity-at-constant-pressure) and [heat capacity at constant volume](heat.md#heat-capacity-at-constant-volume) for a fixed-composition [ideal gas](ideal-gas.md) is

$$
C_p(T)-C_V(T)=nR=Nk_B.
$$

Here both capacities are total [heat capacities](heat.md#heat-capacity) in $\mathrm{J\,K^{-1}}$, $n$ is [amount of substance](physics.md#amount-of-substance), $N$ is the number of particles, $R$ is the [molar gas constant](#molar-gas-constant) and $k_B$ is the [Boltzmann constant](thermodynamics.md#boltzmann-constant). In other normalizations the same statement is

$$
C_{p,\mathrm m}(T)-C_{V,\mathrm m}(T)=R,\qquad
c_p(T)-c_V(T)=\frac{nR}{m}.
$$

The first is a difference of [molar heat capacities](heat.md#molar-heat-capacity), in $\mathrm{J\,mol^{-1}\,K^{-1}}$; the second uses [specific heat capacities](heat.md#specific-heat-capacity), in $\mathrm{J\,kg^{-1}\,K^{-1}}$. Writing $C_p-C_V=R$ with total capacities would omit the sample's [amount of substance](physics.md#amount-of-substance). The relation holds pointwise even when the capacities depend on [temperature](temperature.md). [Samuel J. Ling, William Moebs and Jeff Sanny, University Physics Volume 2, §3.5: ideal-gas capacity difference](https://openstax.org/books/university-physics-volume-2/pages/3-5-heat-capacities-of-an-ideal-gas)

The proof outline is short: [enthalpy](enthalpy.md) is $H=U+pV=U+nRT$, and [internal energy of an ideal gas](#internal-energy-of-an-ideal-gas) is independent of [volume](thermodynamics.md#volume-thermodynamics) at fixed [temperature](temperature.md). Differentiating at fixed composition and [amount of substance](physics.md#amount-of-substance) therefore gives $C_p=dH/dT=dU/dT+nR=C_V+nR$. It uses the [ideal gas law](#ideal-gas-law), rather than assuming any particular number of molecular [degrees of freedom](classical-mechanics.md#degree-of-freedom). At fixed [pressure](pressure.md), the additional [heat](heat.md) supplies expansion [work](energy.md#work), $p\,dV=nR\,dT$. The two processes can have the same [temperature](temperature.md) endpoints and equal $\Delta U$ while requiring different [heat](heat.md) inputs.

For one [mole](physics.md#mole-unit) of the rigid-rotation diatomic [ideal gas](ideal-gas.md) model, $C_V=5R/2$ and $C_p=7R/2$. Heating by $10\,\mathrm K$ with $R\simeq8.31446\,\mathrm{J\,mol^{-1}\,K^{-1}}$ gives $Q_V\simeq207.86\,\mathrm J$ in a rigid sealed vessel and $Q_p\simeq291.01\,\mathrm J$ under a frictionless piston at fixed [pressure](pressure.md). Both gain $207.86\,\mathrm J$ of [internal energy](internal-energy.md), while the piston delivers approximately $83.14\,\mathrm J$ of [work](energy.md#work). This is a calculated model budget. If the capacities vary with [temperature](temperature.md), the corresponding finite statement is still

$$
Q_p-Q_V=nR(T_2-T_1),\qquad
Q_V=n\int_{T_1}^{T_2}C_{V,\mathrm m}(T)\,dT,
$$

under the fixed-[pressure](pressure.md) and fixed-[volume](thermodynamics.md#volume-thermodynamics) heating assumptions in [heat capacity](heat.md#heat-capacity). Their final [volume](thermodynamics.md#volume-thermodynamics) values generally differ. Combining [Mayer's relation](#mayer-s-relation) with [heat capacity ratio](#heat-capacity-ratio) also gives $C_V=nR/(\gamma-1)$ and $C_p=\gamma nR/(\gamma-1)$ locally; constant values cannot be extrapolated across intervals in which $\gamma(T)$ changes.

For a smooth stable single [thermodynamic phase](thermodynamics.md#thermodynamic-phase) of a general [simple compressible system](thermodynamics.md#simple-compressible-system), the broader [Maxwell relation](thermodynamics.md#maxwell-relations) identity is

$$
C_p-C_V=T\left(\frac{\partial p}{\partial T}\right)_V\left(\frac{\partial V}{\partial T}\right)_p
=\frac{TV\alpha^2}{\kappa_T},
$$

where $\alpha$ is the [coefficient of thermal expansion](thermodynamics.md#coefficient-of-thermal-expansion) and $\kappa_T$ the [isothermal compressibility](thermodynamics.md#isothermal-compressibility), with composition fixed throughout. Substituting the [ideal gas law](#ideal-gas-law) gives $nR$; a [real gas](thermodynamics.md#real-gas) need not do so. This distinction matters near a [phase transition](critical-phenomenon.md#phase-transition) or when interactions appreciably change the [equation of state](pressure.md#equation-of-state). It explains why [Mayer's relation](#mayer-s-relation) is useful: thermal measurements under different constraints become linked to a mechanical response, while the difference retains a particularly simple value for an [ideal gas](ideal-gas.md).[§4.4.2: Maxwell relations and the general heat-capacity difference](physics-bibliography.md#statistical-physics-by-david-tong/4-classical-thermodynamics)

## ↑ Ancestors (5)

1. [Thermodynamics](thermodynamics.md)
2. [Statistical physics](statistical-physics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (282)

- [Adiabat](first-law-of-thermodynamics.md#adiabat)
- [Adiabatic compression](first-law-of-thermodynamics.md#adiabatic-compression)
- [Adiabatic expansion](first-law-of-thermodynamics.md#adiabatic-expansion)
- [Adiabatic exponents of a monatomic gas-radiation mixture](stellar-structure.md#adiabatic-exponents-of-a-monatomic-gas-radiation-mixture)
- [Adiabatic parcel gradient in a hydrostatic environment](exoplanet.md#adiabatic-parcel-gradient-in-a-hydrostatic-environment)
- [Adsorption confinement free energy](physical-chemistry.md#adsorption-confinement-free-energy)
- [Argon detection in a binary gas mixture](chemical-substance.md#argon-detection-in-a-binary-gas-mixture)
- [Ballistic marginal-escape stellar wind](stellar-astrophysics.md#ballistic-marginal-escape-stellar-wind)
- [Bose condensation in a three-dimensional harmonic trap](quantum-ideal-gas-statistics.md#bose-condensation-in-a-three-dimensional-harmonic-trap)
- [Bose condensation temperature from a fermionic density scale](quantum-ideal-gas-statistics.md#bose-condensation-temperature-from-a-fermionic-density-scale)
- [Boyle's law](second-law-of-thermodynamics.md#boyle-s-law)
- [Brayton cycle](thermodynamics.md#brayton-cycle)
- [Buoyancy frequency of an ideal-gas stratification](gravity-wave.md#buoyancy-frequency-of-an-ideal-gas-stratification)
- [Carnot cycle](second-law-of-thermodynamics.md#carnot-cycle)
- [Chemical potential](chemical-potential.md)
- [Chemical potential and Helmholtz free energy](chemical-potential.md#chemical-potential-and-helmholtz-free-energy)
- [Chemical potential equality for particle exchange](chemical-potential.md#chemical-potential-equality-for-particle-exchange)
- [Chemical potential of an ideal gas](chemical-potential.md#chemical-potential-of-an-ideal-gas)
- [Classical ideal-gas entropy limits](#classical-ideal-gas-entropy-limits)
- [Closed-vessel thermal transpiration](kinetic-theory.md#closed-vessel-thermal-transpiration)
- [Cloud-chamber expansion model](particle-detection.md#cloud-chamber-expansion-model)
- [Coefficient of thermal expansion](thermodynamics.md#coefficient-of-thermal-expansion)
- [Compressibility](thermodynamics.md#compressibility)
- [Compressibility factor](pressure.md#compressibility-factor)
- [Conservative energy flux of a polytropic ideal gas](euler-equations-for-an-inviscid-fluid.md#conservative-energy-flux-of-a-polytropic-ideal-gas)
- [Convective contraction with power-law opacity](stellar-astrophysics.md#convective-contraction-with-power-law-opacity)
- [Convective instability of a square-root exponential atmospheric profile](exoplanet.md#convective-instability-of-a-square-root-exponential-atmospheric-profile)
- [Convective stability of a constant-opacity irradiated atmosphere](exoplanet.md#convective-stability-of-a-constant-opacity-irradiated-atmosphere)
- [Dilute-gas Bose-Einstein condensation](quantum-ideal-gas-statistics.md#dilute-gas-bose-einstein-condensation)
- [Dry adiabatic lapse rate](exoplanet.md#dry-adiabatic-lapse-rate)
- [Dry parcel buoyancy in a homogeneous atmosphere](gravity-wave.md#dry-parcel-buoyancy-in-a-homogeneous-atmosphere)
- [Effusion](kinetic-theory.md#effusion)
- [Effusive beam speed distribution](physics.md#effusive-beam-speed-distribution)
- [Entropy change in free expansion](thermodynamics.md#entropy-change-in-free-expansion)
- [Entropy dependence of a polytropic mass-radius relation](stellar-structure.md#entropy-dependence-of-a-polytropic-mass-radius-relation)
- [Entropy excess of a van der Waals gas](pressure.md#entropy-excess-of-a-van-der-waals-gas)
- [Entropy loss of an isolated convective planet](stellar-astrophysics.md#entropy-loss-of-an-isolated-convective-planet)
- [Equipartition theorem](canonical-ensemble.md#equipartition-theorem)
- [Exobase](exoplanet.md#exobase)
- [Finite-rate isothermal piston model](second-law-of-thermodynamics.md#finite-rate-isothermal-piston-model)
- [Finite-size normalization of the isothermal-isobaric ensemble](statistical-physics.md#finite-size-normalization-of-the-isothermal-isobaric-ensemble)
- [First law of thermodynamics](first-law-of-thermodynamics.md)
- [Free expansion](thermodynamics.md#free-expansion)
- [Fully convective homology with tenth-power surface opacity](stellar-structure.md#fully-convective-homology-with-tenth-power-surface-opacity)
- [Gas density](fluid-mechanics.md#gas-density)
- [Gas-syringe measurement of Boyle's law](second-law-of-thermodynamics.md#gas-syringe-measurement-of-boyle-s-law)
- [Gas thermometer](temperature.md#gas-thermometer)
- [Gas thermometer dead-space correction](temperature.md#gas-thermometer-dead-space-correction)
- [Gibbs free energy of an ideal-gas mixture](thermodynamic-potential.md#gibbs-free-energy-of-an-ideal-gas-mixture)
- [Gibbs paradox](canonical-ensemble.md#gibbs-paradox)
- [Grand-canonical chemical potential of a classical ideal gas](chemical-potential.md#grand-canonical-chemical-potential-of-a-classical-ideal-gas)
- [Gravitational energy generation in a homologously contracting ideal-gas star](stellar-astrophysics.md#gravitational-energy-generation-in-a-homologously-contracting-ideal-gas-star)
- [Grey-atmosphere convection onset with eighth-power temperature opacity](stellar-structure.md#grey-atmosphere-convection-onset-with-eighth-power-temperature-opacity)
- [Grey-atmosphere convection onset with seventeenth-power opacity](stellar-structure.md#grey-atmosphere-convection-onset-with-seventeenth-power-opacity)
- [Heat capacity](heat.md#heat-capacity)
- [Heat capacity at constant pressure](enthalpy.md#heat-capacity-at-constant-pressure)
- [Heat capacity ratio](#heat-capacity-ratio)
- [Helium liquefaction](temperature.md#helium-liquefaction)
- [Homologous vertical structure of a constant-opacity alpha disk](astrophysical-disk.md#homologous-vertical-structure-of-a-constant-opacity-alpha-disk)
- [Homology scaling of central stellar pressure](stellar-structure.md#homology-scaling-of-central-stellar-pressure)
- [Hydrogen rotational heat capacity](molecule.md#hydrogen-rotational-heat-capacity)
- [Hydrostatic atmosphere with a constant temperature lapse rate](fluid-mechanics.md#hydrostatic-atmosphere-with-a-constant-temperature-lapse-rate)
- [Ideal gas](ideal-gas.md)
- [Ideal gas law](#ideal-gas-law)
- [Ideal solution](mixture.md#ideal-solution)
- [Ideal-solution vapor-liquid equilibrium test](mixture.md#ideal-solution-vapor-liquid-equilibrium-test)
- [Intensive and extensive thermodynamic quantities](thermodynamics.md#intensive-and-extensive-thermodynamic-quantities)
- [Internal energy](internal-energy.md)
- [Internal energy of an ideal gas](#internal-energy-of-an-ideal-gas)
- [Isentropic compressibility](thermodynamics.md#isentropic-compressibility)
- [Isentropic temperature-volume derivative](thermodynamics.md#isentropic-temperature-volume-derivative)
- [Isobaric ideal-gas internal-energy density](#isobaric-ideal-gas-internal-energy-density)
- [Isobaric thermal stability of a heated ideal gas](astrophysical-fluid-dynamics.md#isobaric-thermal-stability-of-a-heated-ideal-gas)
- [Isotherm](second-law-of-thermodynamics.md#isotherm)
- [Isothermal compressibility](thermodynamics.md#isothermal-compressibility)
- [Isothermal compression](second-law-of-thermodynamics.md#isothermal-compression)
- [Isothermal expansion](second-law-of-thermodynamics.md#isothermal-expansion)
- [Isothermal gas syringe experiment](second-law-of-thermodynamics.md#isothermal-gas-syringe-experiment)
- [Isothermal ideal-gas work](second-law-of-thermodynamics.md#isothermal-ideal-gas-work)
- [Isothermal process](second-law-of-thermodynamics.md#isothermal-process)
- [Isothermal stellar and gas density equivalence](galaxy.md#isothermal-stellar-and-gas-density-equivalence)
- [Joule-Thomson coefficient](enthalpy.md#joule-thomson-coefficient)
- [Joule-Thomson effect](enthalpy.md#joule-thomson-effect)
- [Joule-Thomson inversion curve](enthalpy.md#joule-thomson-inversion-curve)
- [Kamerlingh Onnes's 1908 helium liquefaction experiment](temperature.md#kamerlingh-onnes-s-1908-helium-liquefaction-experiment)
- [Kelvin-Planck statement of the second law](second-law-of-thermodynamics.md#kelvin-planck-statement-of-the-second-law)
- [Kinetic theory](kinetic-theory.md)
- [Lagrangian perturbation of a fluid variable](fluid-mechanics.md#lagrangian-perturbation-of-a-fluid-variable)
- [Langmuir adsorption model](physical-chemistry.md#langmuir-adsorption-model)
- [Linear-density stellar model](stellar-structure.md#linear-density-stellar-model)
- [Low-temperature heat capacity of a three-dimensional Fermi gas](quantum-ideal-gas-statistics.md#low-temperature-heat-capacity-of-a-three-dimensional-fermi-gas)
- [Matching of a white-dwarf envelope to a degenerate core](stellar-astrophysics.md#matching-of-a-white-dwarf-envelope-to-a-degenerate-core)
- [Maxwell-Boltzmann distribution](quantum-ideal-gas-statistics.md#maxwell-boltzmann-distribution)
- [Maxwell relations](thermodynamics.md#maxwell-relations)
- [Mayer's relation](#mayer-s-relation)
- [Mean molecular weight per ion](#mean-molecular-weight-per-ion)
- [Mixture measurements and the Gibbs-Duhem constraint](thermodynamics.md#mixture-measurements-and-the-gibbs-duhem-constraint)
- [Molar mass measurement model](chemistry.md#molar-mass-measurement-model)
- [Mole fraction](mathematical-biology.md#mole-fraction)
- [Negative hydrogen ion opacity](stellar-structure.md#negative-hydrogen-ion-opacity)
- [Nondegenerate gas](#nondegenerate-gas)
- [Observation of Bose-Einstein condensation in rubidium in 1995](quantum-ideal-gas-statistics.md#observation-of-bose-einstein-condensation-in-rubidium-in-1995)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2012/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1.md#4/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#1/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1.md#3/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017.md#3/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018.md#section-a/a1/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018.md#section-b/b2/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019.md#section-b/5/solution)
- [Solution](past-exam-of-the-atmospheric-physics-course-of-the-university-of-cambridge/2012/paper-1.md#1/b/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#2/solution)
- [Solution](past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#3/c/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2021/paper-2.md#a8/b/i/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2.md#a6/d/solution)
- [Solution](past-exam-of-the-chemistry-a-course-of-the-university-of-cambridge/2022/paper-2.md#a8/a/i/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#4/a/ii/solution)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-id.md#2/a/solution)
- [Solution](past-exam-of-the-exoplanets-and-planetary-systems-course-of-the-university-of-cambridge/2016/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2013/paper-1.md#2/solution)
- [Solution](past-exam-of-the-formation-of-structure-in-the-universe-course-of-the-university-of-cambridge/2014/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-46.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-63.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-65.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-70.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-72.md#1/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-73.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-73.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#38c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-70.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-71.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-74.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#34d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#15a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-65.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-66.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-66.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#34e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-70.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-71.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-63.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#35c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-61.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-63.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#2/solution)
- [B](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#3/b)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-55.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-59.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-315.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-317.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-317.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-317.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-321.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#34d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#34d/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#1/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-315.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-317.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-321.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#2/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-315.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-317.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-321.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-321.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-321.md#2/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2.md#35d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-317.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-347.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#35a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#9d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#36c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-315.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-317.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-317.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#36a/d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#36a/d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#35a/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-317.md#3/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#35a/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#39c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-317.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-317.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-347.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-317.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2.md#9/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2.md#section-b/5/b/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-2.md#section-a/3/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-2.md#section-d/d13/a/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-2.md#section-d/d12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-c/c10/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-1.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2010/paper-2a.md#section-a/1/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2011/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-a/a1/solution)
- [Solution (cycle calculations)](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2.md#section-c/c10/solution-cycle-calculations)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c10/diesel-cycle-geometry/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-c/c12/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-a/a4/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-2.md#section-c/c13/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1.md#section-a/a5/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-2.md#section-c/c10/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-1.md#section-a/a5/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2021/paper-2.md#section-c/c9/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/a/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/b/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2022/paper-2.md#section-c/c8/f/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b7/a/solution)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004.md#section-b/b8/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2012/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1.md#1/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2014/paper-1.md#2/c/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/a/solution)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021.md#section-b/4/e/solution)
- [Polytropic constant](astrophysical-fluid-dynamics.md#polytropic-constant)
- [Polytropic vertical structure in stellar gravity](astrophysical-disk.md#polytropic-vertical-structure-in-stellar-gravity)
- [Power-law opacity radiative envelope](stellar-structure.md#power-law-opacity-radiative-envelope)
- [Pressure scale height](statistical-physics.md#pressure-scale-height)
- [Quasistatic process](thermodynamics.md#quasistatic-process)
- [Radiation budget of monatomic cloud collapse](classical-mechanics.md#radiation-budget-of-monatomic-cloud-collapse)
- [Radiative-zero white-dwarf envelope](stellar-astrophysics.md#radiative-zero-white-dwarf-envelope)
- [Raoult's law](mixture.md#raoult-s-law)
- [Real gas](thermodynamics.md#real-gas)
- [Relative energy fluctuation of a monatomic ideal gas](canonical-ensemble.md#relative-energy-fluctuation-of-a-monatomic-ideal-gas)
- [Rüchardt experiment](#ruchardt-experiment)
- [Second virial coefficient](statistical-physics.md#second-virial-coefficient)
- [Specific gas constant](#specific-gas-constant)
- [Specific heats of a monatomic gas-radiation mixture](stellar-structure.md#specific-heats-of-a-monatomic-gas-radiation-mixture)
- [Speed distribution](kinetic-theory.md#speed-distribution)
- [Stellar gas constant](#stellar-gas-constant)
- [Stellar gas-pressure fraction](stellar-structure.md#stellar-gas-pressure-fraction)
- [Stellar thermal-wind balance](stellar-astrophysics.md#stellar-thermal-wind-balance)
- [Stipulated bond dissociation model](chemical-bond.md#stipulated-bond-dissociation-model)
- [Temperature](temperature.md)
- [Thermal expansion](thermodynamics.md#thermal-expansion)
- [Thermodynamic internal pressure](internal-energy.md#thermodynamic-internal-pressure)
- [Thermodynamic state](thermodynamics.md#thermodynamic-state)
- [Translational and two-level energy variance](canonical-ensemble.md#translational-and-two-level-energy-variance)
- [Two-dimensional ideal gas](#two-dimensional-ideal-gas)
- [Two reversible ideal-gas paths between the same states](thermodynamics.md#two-reversible-ideal-gas-paths-between-the-same-states)
- [Uniform-sphere pressure-work collapse criterion](stellar-astrophysics.md#uniform-sphere-pressure-work-collapse-criterion)
- [Volume derivative form of the heat-capacity difference](enthalpy.md#volume-derivative-form-of-the-heat-capacity-difference)
- [Volume fluctuations of a closed gas bubble](statistical-physics.md#volume-fluctuations-of-a-closed-gas-bubble)
- [Volume mixing ratio](mathematical-biology.md#volume-mixing-ratio)
- [Zero-radiative-flux obstruction for a polytropic ideal gas](astrophysical-disk.md#zero-radiative-flux-obstruction-for-a-polytropic-ideal-gas)
