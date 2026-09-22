# Thermodynamics

↑ **Parent:** [Statistical physics](statistical-physics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermodynamics)

Thermodynamics relates energy, entropy, temperature, pressure, volume, work, and heat through state functions and process laws.

**Table of contents**

- [Thermodynamic phase](#thermodynamic-phase)
- [Laws of thermodynamics](#laws-of-thermodynamics)
  - [Zeroth law of thermodynamics](#zeroth-law-of-thermodynamics)
- [Compressibility](#compressibility)
  - [Isothermal compressibility](#isothermal-compressibility)
- [Maxwell relations](#maxwell-relations)
- [Diffusion](#diffusion)
  - [Molecular diffusion](#molecular-diffusion)
  - [Rotational diffusion](#rotational-diffusion)
- [Thermal expansion](#thermal-expansion)
  - [Coefficient of thermal expansion](#coefficient-of-thermal-expansion)
  - [Thermal expansion coefficient](#thermal-expansion-coefficient)
- [Stochastic thermodynamics](#stochastic-thermodynamics)
  - [Local detailed balance](#local-detailed-balance)
    - [Microscopic reversibility](#microscopic-reversibility)
  - [Entropy production](#entropy-production)
    - [Thermodynamic entropy flux](#thermodynamic-entropy-flux)
    - [Fluctuation theorem](#fluctuation-theorem)
  - [Fluctuation-dissipation relation for a Langevin particle](#fluctuation-dissipation-relation-for-a-langevin-particle)
    - [Vector noise normalization in inertial Langevin dynamics](#vector-noise-normalization-in-inertial-langevin-dynamics)
- [Boltzmann constant](#boltzmann-constant)
- [Boltzmann distribution](#boltzmann-distribution)
- [Temperature](#temperature)
  - [Inverse temperature](#inverse-temperature)
- [Thermal equilibrium](#thermal-equilibrium)
  - [Tolman–Ehrenfest relation](#tolman-ehrenfest-relation)
  - [Boltzmann suppression](#boltzmann-suppression)
    - [Boltzmann suppression of a nonrelativistic relic](#boltzmann-suppression-of-a-nonrelativistic-relic)
  - [Kinetic equilibrium](#kinetic-equilibrium)
  - [Heat bath](#heat-bath)
  - [Entropy maximization under thermal contact](#entropy-maximization-under-thermal-contact)
- [Entropy](#entropy)
  - [Specific entropy](#specific-entropy)
  - [Boltzmann's entropy formula](#boltzmann-s-entropy-formula)
  - [Entropy density](#entropy-density)
    - [Comoving entropy](#comoving-entropy)
    - [Entropy density at zero chemical potential](#entropy-density-at-zero-chemical-potential)
      - [Nonrelativistic entropy at zero chemical potential](#nonrelativistic-entropy-at-zero-chemical-potential)
- [Second law of thermodynamics](#second-law-of-thermodynamics)
  - [Reversible thermodynamic process](#reversible-thermodynamic-process)
  - [Clausius statement of the second law](#clausius-statement-of-the-second-law)
  - [Kelvin-Planck statement of the second law](#kelvin-planck-statement-of-the-second-law)
  - [Carnot's theorem](#carnot-s-theorem)
    - [Thermodynamic temperature](#thermodynamic-temperature)
    - [Carnot cycle](#carnot-cycle)
      - [Isothermal process](#isothermal-process)
        - [Boyle's law](#boyle-s-law)
        - [Isothermal compression](#isothermal-compression)
        - [Isothermal expansion](#isothermal-expansion)
- [Heat](#heat)
  - [Sensible heat](#sensible-heat)
  - [Heat transfer](#heat-transfer)
    - [Nusselt number](#nusselt-number)
    - [Thermal inertia](#thermal-inertia)
    - [Radiative cooling](#radiative-cooling)
      - [Compton cooling by the cosmic microwave background](#compton-cooling-by-the-cosmic-microwave-background)
      - [Dust thermal emission](#dust-thermal-emission)
      - [Inverse Compton cooling](#inverse-compton-cooling)
      - [Astrophysical cooling function](#astrophysical-cooling-function)
        - [Molecular line cooling](#molecular-line-cooling)
        - [Cooling suppression by photoionization](#cooling-suppression-by-photoionization)
        - [Optically thin gas cooling time](#optically-thin-gas-cooling-time)
          - [Cooling-to-free-fall equality curve](#cooling-to-free-fall-equality-curve)
        - [Primordial atomic cooling curve](#primordial-atomic-cooling-curve)
        - [Atomic line cooling](#atomic-line-cooling)
          - [Metal-line cooling](#metal-line-cooling)
  - [Heat flux density](#heat-flux-density)
  - [Thermal conduction](#thermal-conduction)
    - [Temperature dipole around an insulating sphere](#temperature-dipole-around-an-insulating-sphere)
    - [Isobaric conductive cooling in mass coordinates](#isobaric-conductive-cooling-in-mass-coordinates)
      - [Error-function isobaric cooling front](#error-function-isobaric-cooling-front)
    - [Temperature gradient](#temperature-gradient)
    - [Fourier's law](#fourier-s-law)
      - [Thermal conductivity](#thermal-conductivity)
        - [Thermal conductivity tensor](#thermal-conductivity-tensor)
        - [Thermal diffusivity](#thermal-diffusivity)
          - [Prandtl number](#prandtl-number)
          - [Thermal diffusion time](#thermal-diffusion-time)
            - [Thermal diffusion rate of a Fourier mode](#thermal-diffusion-rate-of-a-fourier-mode)
  - [Stefan–Boltzmann law](#stefan-boltzmann-law)
    - [Stefan-Boltzmann constant](#stefan-boltzmann-constant)
    - [Emissivity](#emissivity)
    - [Radiative equilibrium](#radiative-equilibrium)
  - [Heat capacity](#heat-capacity)
    - [Entropy from heat capacity](#entropy-from-heat-capacity)
    - [Entropy concavity and positive heat capacity](#entropy-concavity-and-positive-heat-capacity)
    - [Specific heat capacity](#specific-heat-capacity)
      - [Specific heat capacity at constant volume](#specific-heat-capacity-at-constant-volume)
      - [Specific heat capacity at constant pressure](#specific-heat-capacity-at-constant-pressure)
        - [Pure-radiation constant-pressure heat-capacity singularity](#pure-radiation-constant-pressure-heat-capacity-singularity)
    - [Heat capacity at constant volume](#heat-capacity-at-constant-volume)
      - [Dulong-Petit law](#dulong-petit-law)
    - [Heat capacity at constant area](#heat-capacity-at-constant-area)
- [Third law of thermodynamics](#third-law-of-thermodynamics)
- [Pressure](#pressure)
  - [Kinematic pressure](#kinematic-pressure)
  - [Pressure tensor](#pressure-tensor)
  - [Gas pressure](#gas-pressure)
  - [Radiation pressure](#radiation-pressure)
  - [Equation of state](#equation-of-state)
    - [Barotropic stellar equation of state](#barotropic-stellar-equation-of-state)
    - [Clausius gas](#clausius-gas)
    - [Van der Waals equation](#van-der-waals-equation)
      - [Van der Waals law of corresponding states](#van-der-waals-law-of-corresponding-states)
    - [Equation of state of an ideal ultrarelativistic gas](#equation-of-state-of-an-ideal-ultrarelativistic-gas)
    - [Adiabatic equation of state](#adiabatic-equation-of-state)
- [Volume (thermodynamics)](#volume-thermodynamics)
- [Internal energy](#internal-energy)
  - [Specific internal energy](#specific-internal-energy)
- [Thermodynamic free energy](#thermodynamic-free-energy)
  - [Free-energy functional](#free-energy-functional)
  - [Helmholtz free energy](#helmholtz-free-energy)
- [Chemical potential](#chemical-potential)
  - [Chemical potential of a composition field](#chemical-potential-of-a-composition-field)
  - [Chemical equilibrium](#chemical-equilibrium)
    - [Chemical disequilibrium](#chemical-disequilibrium)
    - [Zero chemical potential from number-changing reactions](#zero-chemical-potential-from-number-changing-reactions)
    - [Chemical relaxation time](#chemical-relaxation-time)
    - [Equilibrium constant](#equilibrium-constant)
    - [Photon chemical potential](#photon-chemical-potential)
- [Ideal gas](#ideal-gas)
  - [Ideal gas law](#ideal-gas-law)
  - [Monatomic gas](#monatomic-gas)
  - [Mean free path](#mean-free-path)
    - [Mean free path through randomly oriented disc absorbers](#mean-free-path-through-randomly-oriented-disc-absorbers)
  - [Mean molecular weight](#mean-molecular-weight)
    - [Stellar gas constant](#stellar-gas-constant)
    - [Mean molecular weight per ion](#mean-molecular-weight-per-ion)
    - [Mean molecular weight per electron](#mean-molecular-weight-per-electron)
  - [Heat capacity ratio](#heat-capacity-ratio)
  - [Nondegenerate gas](#nondegenerate-gas)
  - [Internal energy of an ideal gas](#internal-energy-of-an-ideal-gas)
  - [Mayer's relation](#mayer-s-relation)
- [Real gas](#real-gas)
  - [Dieterici equation](#dieterici-equation)
- [Intensive and extensive thermodynamic quantities](#intensive-and-extensive-thermodynamic-quantities)
  - [Extensive quantity](#extensive-quantity)
    - [Euler relation in thermodynamics](#euler-relation-in-thermodynamics)
- [Gibbs-Duhem equation](#gibbs-duhem-equation)
- [Gibbs free energy](#gibbs-free-energy)
  - [Gibbs free energy of an ideal-gas mixture](#gibbs-free-energy-of-an-ideal-gas-mixture)
  - [Gibbs free-energy Maxwell relation](#gibbs-free-energy-maxwell-relation)
  - [Chemical-potential balance for a reaction](#chemical-potential-balance-for-a-reaction)
    - [Thermochemical equilibrium](#thermochemical-equilibrium)
      - [Constrained Gibbs minimization for chemical equilibrium](#constrained-gibbs-minimization-for-chemical-equilibrium)
      - [Reverse reaction rate from equilibrium thermodynamics](#reverse-reaction-rate-from-equilibrium-thermodynamics)
  - [Phase coexistence curve](#phase-coexistence-curve)
    - [Maxwell construction](#maxwell-construction)
    - [Phase diagram](#phase-diagram)
      - [Solidus](#solidus)
      - [Lever rule](#lever-rule)
      - [Bicritical point](#bicritical-point)
      - [Liquidus](#liquidus)
        - [Freezing-point depression](#freezing-point-depression)
      - [Eutectic system](#eutectic-system)
        - [Eutectic composition](#eutectic-composition)
        - [Eutectic temperature](#eutectic-temperature)
    - [First-order phase transition](#first-order-phase-transition)
      - [Two-phase scalar coexistence endpoint conditions](#two-phase-scalar-coexistence-endpoint-conditions)
      - [Spin-flop transition](#spin-flop-transition)
      - [Classical nucleation theory](#classical-nucleation-theory)
        - [Critical nucleus](#critical-nucleus)
        - [Arrhenius nucleation time](#arrhenius-nucleation-time)
    - [Latent heat](#latent-heat)
      - [Stefan number](#stefan-number)
        - [Latent-to-sensible heat ratio](#latent-to-sensible-heat-ratio)
      - [Clausius-Clapeyron relation](#clausius-clapeyron-relation)
        - [Common-pressure melting-point slope](#common-pressure-melting-point-slope)
- [Conjugate variables (thermodynamics)](#conjugate-variables-thermodynamics)
- [First law of thermodynamics](#first-law-of-thermodynamics)
  - [Adiabatic process](#adiabatic-process)
    - [Adiabatic compression](#adiabatic-compression)
    - [Adiabatic expansion](#adiabatic-expansion)
    - [Isentropic process](#isentropic-process)
    - [Reversible ideal-gas adiabat](#reversible-ideal-gas-adiabat)
- [Enthalpy](#enthalpy)
  - [Joule-Thomson coefficient](#joule-thomson-coefficient)
    - [Virial criterion for Joule-Thomson cooling](#virial-criterion-for-joule-thomson-cooling)
  - [Specific enthalpy](#specific-enthalpy)
    - [Polytropic enthalpy](#polytropic-enthalpy)
  - [Enthalpy Maxwell relation](#enthalpy-maxwell-relation)
  - [Heat capacity at constant pressure](#heat-capacity-at-constant-pressure)
    - [Difference between constant-pressure and constant-volume heat capacities](#difference-between-constant-pressure-and-constant-volume-heat-capacities)
- [Diatomic ideal-gas enthalpy](#diatomic-ideal-gas-enthalpy)
- [Irreversible adiabatic piston compression](#irreversible-adiabatic-piston-compression)
- [Constant-pressure heating of an ideal gas](#constant-pressure-heating-of-an-ideal-gas)
- [Thermodynamic cycle](#thermodynamic-cycle)
  - [Thermal efficiency](#thermal-efficiency)
  - [Otto cycle](#otto-cycle)
  - [Diesel cycle](#diesel-cycle)

## Thermodynamic phase

↑ **Parent:** [Thermodynamics](thermodynamics.md)

A thermodynamic phase is a form of macroscopic equilibrium characterized by its structure, symmetries and thermodynamic response. Away from [phase transitions](critical-phenomenon.md#phase-transition), its [free-energy density](statistical-physics.md#free-energy-density) varies smoothly with the control parameters. Different phases can share a [phase coexistence](critical-phenomenon.md#phase-coexistence) boundary. An ordered magnetic phase is distinguished from a disordered phase by its spontaneous [order parameter](critical-phenomenon.md#order-parameter); positive and negative ordered states are different [pure thermodynamic phases](critical-phenomenon.md#pure-thermodynamic-phase) related by [spin inversion symmetry](statistical-physics.md#spin-inversion-symmetry).

## Laws of thermodynamics

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laws_of_thermodynamics)

The laws organize the equilibrium and process constraints of [thermodynamics](thermodynamics.md): the [zeroth law of thermodynamics](#zeroth-law-of-thermodynamics) makes thermal equilibrium transitive, the [first law of thermodynamics](#first-law-of-thermodynamics) expresses energy balance, the [Second law of thermodynamics](#second-law-of-thermodynamics) restricts entropy changes, and the [Third law of thermodynamics](#third-law-of-thermodynamics) describes the zero-temperature limit. Their analogy with horizon mechanics becomes quantitative through [Hawking temperature](general-relativity.md#hawking-temperature) and [Bekenstein-Hawking entropy](general-relativity.md#bekenstein-hawking-entropy).

### Zeroth law of thermodynamics

↑ **Parent:** [Laws of thermodynamics](#laws-of-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Zeroth_law_of_thermodynamics)

If two systems are each in [thermal equilibrium](#thermal-equilibrium) with a third, they are in thermal equilibrium with each other. Equilibrium classes can therefore be labelled by a common [thermodynamic temperature](#thermodynamic-temperature). The corresponding [Zeroth law of black-hole mechanics](general-relativity.md#zeroth-law-of-black-hole-mechanics) states constancy of [surface gravity](general-relativity.md#surface-gravity) over an equilibrium horizon; [Hawking radiation](general-relativity.md#hawking-radiation) identifies that quantity with physical temperature up to its universal conversion factor.

## Compressibility

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressibility)

Compressibility measures fractional volume reduction per increase in [pressure](#pressure), with another thermodynamic variable held fixed. Holding [temperature](#temperature) fixed gives isothermal compressibility; holding [entropy](#entropy) fixed gives adiabatic compressibility for a reversible process. Its reciprocal is the bulk modulus. The constraint matters: these responses need not agree.

### Isothermal compressibility

↑ **Parent:** [Compressibility](#compressibility)

The [compressibility](#compressibility) measured at fixed [temperature](#temperature). For a mechanically stable equilibrium it is positive; its reciprocal is the isothermal bulk modulus.

## Maxwell relations

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maxwell_relations)

A Maxwell relation equates mixed derivatives of a thermodynamic potential. For $dF=-S\,dT-P\,dV$, equality of mixed derivatives gives $(\partial S/\partial V)_T=(\partial P/\partial T)_V$. For $dG=-S\,dT+V\,dP$, it gives $(\partial S/\partial P)_T=-(\partial V/\partial T)_P$. These identities connect experimentally accessible response functions to [heat capacities](#heat-capacity) and [compressibility](#compressibility).

## Diffusion

↑ **Parent:** [Thermodynamics](thermodynamics.md)

Diffusion is the spreading of heat or material by microscopic random motion. A [concentration](physics.md#concentration) gradient produces flux down that gradient; with uniform [diffusion coefficient](brownian-motion.md#diffusion-coefficient) $D$, conservation gives the [diffusion equation](diffusion-equation.md) $C_t=D\nabla^2C$. In a moving carrier, [advection](fluid-mechanics.md#advection) must also be included. Physical diffusion is a transport mechanism, distinct from the general probabilistic class of [Markov diffusion](stochastic-calculus.md#markov-diffusion).

### Molecular diffusion

↑ **Parent:** [Diffusion](#diffusion)

Molecular diffusion transports material through random molecular motion rather than coherent fluid [advection](fluid-mechanics.md#advection). Its continuum limit gives a concentration flux $-\kappa\nabla\chi$, with molecular [diffusivity](brownian-motion.md#diffusion-coefficient) $\kappa$, and a [diffusion equation](diffusion-equation.md) when no bulk motion is present. Molecular diffusion acts on the small scalar gradients produced by stretching, even when the macroscopic effective transport is much faster than molecular transport.

### Rotational diffusion

↑ **Parent:** [Diffusion](#diffusion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotational_diffusion)

Rotational diffusion randomizes orientation. For a unit orientation vector on a sphere, isotropic rotational diffusion contributes $D_r\nabla_p^2f$ to the [Fokker-Planck equation](probability-theory.md#fokker-planck-equation), where $\nabla_p^2$ is the [Laplace-Beltrami operator](differential-geometry.md#laplace-beltrami-operator). Its coefficient has units inverse time. It differs from the translational [diffusion coefficient](brownian-motion.md#diffusion-coefficient), whose units are length squared per time.

## Thermal expansion

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_expansion)

### Coefficient of thermal expansion

↑ **Parent:** [Thermal expansion](#thermal-expansion)

The fractional [mass density](fluid-mechanics.md#density) decrease per [temperature](#temperature) increase at fixed [pressure](#pressure). In the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), a [temperature](#temperature) excess $\theta$ gives [reduced gravity](reduced-gravity.md) $g'=g\alpha_T\theta$. It converts a [heat](#heat) budget into a buoyancy budget in [natural ventilation](fluid-mechanics.md#natural-ventilation).

### Thermal expansion coefficient

↑ **Parent:** [Thermal expansion](#thermal-expansion)

For a fluid at fixed [pressure](#pressure), the volumetric thermal expansion coefficient obeys $\rho(T_0+\theta)\simeq\rho(T_0)(1-\alpha\theta)$. Under the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) it determines the [buoyancy](fluid-mechanics.md#buoyancy) proportional to $g\alpha\theta$, while [mass density](fluid-mechanics.md#density) is otherwise held constant.

## Stochastic thermodynamics

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_thermodynamics)

Stochastic thermodynamics assigns work, heat, and entropy production to individual fluctuating trajectories while recovering ordinary thermodynamics after ensemble averaging.

### Local detailed balance

↑ **Parent:** [Stochastic thermodynamics](#stochastic-thermodynamics)

Local detailed balance states that the logarithm of the probability ratio between a trajectory and its time reverse equals the entropy delivered to the environment in units of $k_B$. For one heat bath, $\log(P_F/P_B)=\Delta Q/(k_BT)$ when positive $\Delta Q$ flows into the bath.

#### Microscopic reversibility

↑ **Parent:** [Local detailed balance](#local-detailed-balance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Microscopic_reversibility)

For an equilibrium process, a path and its physically time-reversed path have equal probability after including their equilibrium starting weights. Conditional on their endpoints, this means

$$
\frac{P_F}{P_B}=\exp[-(F_2-F_1)/(k_BT)].
$$

This is the path version of [detailed balance](markov-process.md#detailed-balance). A time-even [order parameter](critical-phenomenon.md#order-parameter) is read backward without changing sign, while a transport flux changes sign. The [Onsager--Machlup path probability](critical-phenomenon.md#onsager-machlup-path-probability) implements this reversal in a coarse-grained stochastic description.

### Entropy production

↑ **Parent:** [Stochastic thermodynamics](#stochastic-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_production)

Entropy production is the sum of the entropy changes of a system and its environment. Under local detailed balance it is represented by a forward-to-reversed path-probability logarithm and has nonnegative expectation.

#### Thermodynamic entropy flux

↑ **Parent:** [Entropy production](#entropy-production)

Local equilibrium associates the outgoing [heat flux](#heat-flux-density) $q$ with outgoing [entropy](#entropy) flux $q/\theta$ at positive [temperature](#temperature) $\theta$. Its [divergence](calculus.md#divergence) appears in the [Lagrangian entropy inequality](continuum-mechanics.md#lagrangian-entropy-inequality), with the appropriate nominal flux in reference coordinates.

#### Fluctuation theorem

↑ **Parent:** [Entropy production](#entropy-production)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fluctuation_theorem)

A fluctuation theorem relates probabilities of positive and negative entropy production. In a steady-state large-deviation form, the rate function often obeys $I(s)-I(-s)=-s$ in units where $s$ is the entropy-production rate.

### Fluctuation-dissipation relation for a Langevin particle

↑ **Parent:** [Stochastic thermodynamics](#stochastic-thermodynamics)

For a Langevin particle with drag coefficient $\zeta$ and white-force covariance amplitude $\sigma^2$, detailed balance at temperature $T$ requires $\sigma^2=2\zeta k_BT$.

#### Vector noise normalization in inertial Langevin dynamics

↑ **Parent:** [Fluctuation-dissipation relation for a Langevin particle](#fluctuation-dissipation-relation-for-a-langevin-particle)

Divide the inertial [Langevin equation](stochastic-process.md#langevin-dynamics) by mass and let $\zeta=\gamma/m$. An isotropic three-dimensional equilibrium velocity has $\langle|\mathbf u|^2\rangle=3k_BT/m$ by the [equipartition theorem](statistical-physics.md#equipartition-theorem). Its white acceleration dot-covariance amplitude is therefore $6\zeta k_BT/m$, while the amplitude per Cartesian component is $2\zeta k_BT/m$. A scalar moment formula must use the component variance rather than the trace.

## Boltzmann constant

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann_constant)

The Boltzmann constant converts temperature into an energy scale.

## Boltzmann distribution

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann_distribution)

At thermal equilibrium, the Boltzmann distribution assigns a state of energy $E_i$ probability $P_i=Z^{-1}e^{-\beta E_i}$, where $\beta=(k_BT)^{-1}$ and the partition function $Z$ normalizes the probabilities.

## Temperature

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Temperature)

Temperature is the intensive variable thermodynamically conjugate to entropy; at equilibrium it determines the direction of heat transfer.

### Inverse temperature

↑ **Parent:** [Temperature](#temperature)

[Inverse temperature](#inverse-temperature) is $\beta=1/(k_BT)$, where $k_B$ is the [Boltzmann constant](#boltzmann-constant) and $T$ is the absolute [temperature](#temperature). A [canonical ensemble](statistical-physics.md#canonical-ensemble) weights an energy $E$ by its [Boltzmann factor](statistical-physics.md#boltzmann-factor) $e^{-\beta E}$. Calling couplings dimensionless means absorbing this factor $\beta$ into their energy coefficients. The alternative convention $k_B=1$ makes [inverse temperature](#inverse-temperature) $1/T$; physical and dimensionless couplings must not be mixed.

In a thermal [Euclidean worldline path integral](quantum-field-theory.md#euclidean-worldline-path-integral) with $\hbar=1$, $\beta$ is also the circumference of the imaginary-time circle.

## Thermal equilibrium

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_equilibrium)

Systems are in thermal equilibrium when no net heat flows between them; their temperatures are equal.

<h3 id="tolman-ehrenfest-relation">Tolman–Ehrenfest relation</h3>

↑ **Parent:** [Thermal equilibrium](#thermal-equilibrium)

In static [thermal equilibrium](#thermal-equilibrium), the local temperature times the stationary lapse is constant. Energy measured locally redshifts to conserved Killing energy by that same lapse; requiring a single equilibrium Boltzmann exponent gives the relation. The [Killing vector field](general-relativity.md#killing-vector-field) normalization fixes the constant but not the ratio of temperatures at different locations.

### Boltzmann suppression

↑ **Parent:** [Thermal equilibrium](#thermal-equilibrium)

[Boltzmann suppression](#boltzmann-suppression) is the exponential reduction of an equilibrium population when creating it costs energy much greater than the temperature. For a nonrelativistic species with negligible [chemical potential](#chemical-potential), the leading factor is $e^{-m/T}$, multiplied by its momentum phase-space volume. It concerns the equilibrium abundance; freeze-out can preserve a larger population than the instantaneous equilibrium value at later times.

#### Boltzmann suppression of a nonrelativistic relic

↑ **Parent:** [Boltzmann suppression](#boltzmann-suppression)

A nonrelativistic species with $g$ states and negligible [chemical potential](#chemical-potential) has equilibrium density $g(mT/(2\pi))^{3/2}e^{-m/T}$. If particle-antiparticle annihilation maintains equilibrium after the species becomes massive, its eventual freeze-out population can be much smaller than a relativistically decoupled population. The nonrelativistic annihilation rate and any asymmetry determine the final abundance.

### Kinetic equilibrium

↑ **Parent:** [Thermal equilibrium](#thermal-equilibrium)

Momentum-exchange collisions maintain a common [temperature](#temperature) and an equilibrium-shaped momentum [probability distribution](probability-theory.md#probability-distribution). Particle abundances and [chemical potentials](#chemical-potential) need not have their [chemical equilibrium](#chemical-equilibrium) values: elastic scattering alone conserves particle number. Thus kinetic equilibrium does not by itself imply either zero [chemical potential](#chemical-potential) or conserved comoving [entropy](#entropy).

### Heat bath

↑ **Parent:** [Thermal equilibrium](#thermal-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_bath)

A heat bath, or thermal reservoir, is an idealized system so large that exchanging a finite amount of [heat](#heat) does not appreciably change its [temperature](#temperature).

### Entropy maximization under thermal contact

↑ **Parent:** [Thermal equilibrium](#thermal-equilibrium)

If two otherwise isolated systems freely exchange energy while $E_1+E_2$ remains fixed, their total entropy is

$$
S_{\mathrm{tot}}(E_1)=S_1(E_1)+S_2(E-E_1).
$$

At an interior maximum, $\partial S_1/\partial E_1=\partial S_2/\partial E_2$. Since [thermodynamic temperature](#thermodynamic-temperature) satisfies $1/T=\partial S/\partial E$, the systems have equal temperatures at [thermal equilibrium](#thermal-equilibrium).

## Entropy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy)

Entropy is an extensive state function satisfying $dS=\delta Q_{\rm rev}/T$ for a reversible transfer of heat.

### Specific entropy

↑ **Parent:** [Entropy](#entropy)

Specific entropy is [entropy](#entropy) per unit mass. For a [perfect gas](#ideal-gas) with constant [specific heat capacity](#specific-heat-capacity) $c_v$ at constant volume and [specific-heat ratio](#heat-capacity-ratio) $\gamma$, differences obey

$$
s_2-s_1=c_v\log\left[\frac{p_2}{p_1}\left(\frac{\rho_1}{\rho_2}\right)^\gamma\right],
$$

where $p$ is [pressure](#pressure) and $\rho$ is [mass density](fluid-mechanics.md#density). Thus a [homentropic flow](compressible-flow.md#homentropic-flow) has constant $p/\rho^\gamma$.

<h3 id="boltzmann-s-entropy-formula">Boltzmann's entropy formula</h3>

↑ **Parent:** [Entropy](#entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boltzmann's_entropy_formula)

For a macrostate containing $\Omega$ equally likely microstates, the Boltzmann entropy is $S=k_B\log\Omega$.

### Entropy density

↑ **Parent:** [Entropy](#entropy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entropy_density)

For a homogeneous equilibrium system with [energy density](statistical-physics.md#energy-density) $\rho$, [pressure](#pressure) $P$, [chemical potential](#chemical-potential) $\mu$, and [number density](statistical-physics.md#number-density) $n$, the entropy density is

$$
s=\frac{\rho+P-\mu n}{T}.
$$

#### Comoving entropy

↑ **Parent:** [Entropy density](#entropy-density)

Comoving entropy is the [entropy density](#entropy-density) multiplied by the physical volume factor $a^3$ for a fixed comoving region in an expanding homogeneous universe. In adiabatic expansion it is conserved. Separate decoupled radiation sectors conserve their own comoving entropy, so disappearance of massive species can heat the still-equilibrated sector relative to a decoupled species.

#### Entropy density at zero chemical potential

↑ **Parent:** [Entropy density](#entropy-density)

For an extensive equilibrium system, the [thermodynamic Euler relation](#euler-relation-in-thermodynamics) gives $E=TS-PV+\mu N$. At zero [chemical potential](#chemical-potential), divide by $V$ to obtain $s=(\rho+P)/T$. Equivalently, $dP=(\rho+P)dT/T$ makes

$$
d\left(\frac{(\rho+P)V}{T}\right)=\frac{d(\rho V)+P\,dV}{T}.
$$

The [first law of thermodynamics](#first-law-of-thermodynamics) identifies this as $dS$; the [thermodynamic Euler relation](#euler-relation-in-thermodynamics) fixes the entropy normalization. For adiabatic expansion satisfying the [cosmological perfect-fluid continuity equation](cosmology.md#cosmological-perfect-fluid-continuity-equation), the numerator on the right vanishes, proving [cosmological entropy conservation](cosmology.md#cosmological-entropy-conservation).

##### Nonrelativistic entropy at zero chemical potential

↑ **Parent:** [Entropy density at zero chemical potential](#entropy-density-at-zero-chemical-potential)

For a dilute nonrelativistic gas with $x=m/T\gg1$ and zero [chemical potential](#chemical-potential), the [Bose-Einstein distribution](statistical-physics.md#bose-einstein-distribution) approaches the [Maxwell-Boltzmann distribution](statistical-physics.md#maxwell-boltzmann-distribution). Expanding $E=m+p^2/(2m)+\cdots$ in the [number density](statistical-physics.md#number-density) integral gives $n\sim g(mT/(2\pi))^{3/2}e^{-x}$. Since $\rho=mn+3nT/2+\cdots$ and $P=nT$, the [entropy density at zero chemical potential](#entropy-density-at-zero-chemical-potential) gives $s=n(x+5/2+\cdots)$ and hence the displayed leading expression. This includes the internal multiplicity $g$; a single real [scalar field](quantum-field-theory.md#scalar-field) has $g=1$.

## Second law of thermodynamics

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_law_of_thermodynamics)

The second law forbids cyclic devices whose sole effect is complete conversion of heat from one reservoir into work or unassisted heat transfer from cold to hot. For a closed system it implies nondecrease of total entropy.

### Reversible thermodynamic process

↑ **Parent:** [Second law of thermodynamics](#second-law-of-thermodynamics)

A thermodynamically reversible process can be reversed without a net change of the system and surroundings. Its entropy change equals reversible heat transfer divided by temperature. A reversible [adiabatic process](#adiabatic-process) conserves [entropy](#entropy); adiabaticity alone does not forbid internal entropy production in an irreversible evolution.

### Clausius statement of the second law

↑ **Parent:** [Second law of thermodynamics](#second-law-of-thermodynamics)

No cyclic device can have as its sole effect the transfer of heat from a colder reservoir to a hotter reservoir.

### Kelvin-Planck statement of the second law

↑ **Parent:** [Second law of thermodynamics](#second-law-of-thermodynamics)

No cyclic device can have as its sole effect the extraction of heat from one reservoir and its complete conversion into work.

<h3 id="carnot-s-theorem">Carnot's theorem</h3>

↑ **Parent:** [Second law of thermodynamics](#second-law-of-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carnot's_theorem_(thermodynamics))

No heat engine operating between two fixed reservoirs is more efficient than a reversible engine, and all reversible engines between those reservoirs have the same efficiency.

#### Thermodynamic temperature

↑ **Parent:** [Carnot's theorem](#carnot-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermodynamic_temperature)

Absolute thermodynamic temperature can be defined so that a reversible engine exchanging heats $Q_h$ and $Q_c$ with reservoirs at $T_h$ and $T_c$ satisfies

$$
\frac{Q_c}{Q_h}=\frac{T_c}{T_h},
\qquad
\eta=1-\frac{T_c}{T_h}.
$$

A choice of one reference temperature fixes the scale.

#### Carnot cycle

↑ **Parent:** [Carnot's theorem](#carnot-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carnot_cycle)

A Carnot cycle consists of two reversible [isothermal changes](#isothermal-process), one at each reservoir temperature, joined by two reversible [adiabatic processes](#adiabatic-process). It attains the maximum [thermal efficiency](#thermal-efficiency) permitted between those reservoirs, $1-T_c/T_h$.

##### Isothermal process

↑ **Parent:** [Carnot cycle](#carnot-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isothermal_process)

An isothermal process is a thermodynamic change at constant [temperature](#temperature). In a reversible isothermal step, the working substance remains in thermal equilibrium with a reservoir while exchanging [heat](#heat).

<h6 id="boyle-s-law">Boyle's law</h6>

↑ **Parent:** [Isothermal process](#isothermal-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boyle's_law)

For a fixed amount of an ideal gas at constant temperature, pressure times volume is constant. Equivalently its density is proportional to pressure. In a dilute bubbly flow, this allows bubble volume and its contribution to [buoyancy](fluid-mechanics.md#buoyancy) to increase as hydrostatic pressure decreases, provided gas mass is retained and dissolution is negligible.

###### Isothermal compression

↑ **Parent:** [Isothermal process](#isothermal-process)

###### Isothermal expansion

↑ **Parent:** [Isothermal process](#isothermal-process)

## Heat

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat)

Heat is energy transferred because of a temperature difference.

### Sensible heat

↑ **Parent:** [Heat](#heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sensible_heat)

[Sensible heat](#sensible-heat) changes [temperature](#temperature) without changing the phase. For constant [specific heat capacity](#specific-heat-capacity), its change per unit mass is $c_p\Delta T$, whereas [latent heat](#latent-heat) accompanies a [phase transition](critical-phenomenon.md#phase-transition).

### Heat transfer

↑ **Parent:** [Heat](#heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_transfer)

#### Nusselt number

↑ **Parent:** [Heat transfer](#heat-transfer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nusselt_number)

The [Nusselt number](#nusselt-number) is the ratio of total [heat transfer](#heat-transfer) to conductive [heat transfer](#heat-transfer) across the same length scale: $\mathrm{Nu}=qh/(k_T\Delta T)$, where $q$ is heat flux and $k_T$ is [thermal conductivity](#thermal-conductivity).

#### Thermal inertia

↑ **Parent:** [Heat transfer](#heat-transfer)

For a homogeneous material, thermal inertia is $\Gamma=\sqrt{k\rho c_p}$, where $k$ is [thermal conductivity](#thermal-conductivity), $\rho$ is density and $c_p$ is specific [heat capacity](#heat-capacity). It measures the resistance of the surface temperature to periodic heating and controls the phase lag relevant to the [Yarkovsky effect](planetary-science.md#yarkovsky-effect).

#### Radiative cooling

↑ **Parent:** [Heat transfer](#heat-transfer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiative_cooling)

A body loses [internal energy](#internal-energy) by emitting [thermal radiation](electromagnetism.md#thermal-radiation) faster than it absorbs radiation or receives other heating. In a gravitating gas this can remove pressure support and allow further contraction.

##### Compton cooling by the cosmic microwave background

↑ **Parent:** [Radiative cooling](#radiative-cooling)

Hot electrons can transfer energy to [cosmic microwave background](cosmology.md#cosmic-microwave-background) photons through [Compton scattering](physics.md#compton-scattering). For a fixed electron fraction $x_e$ and electron temperature well above the radiation temperature, the [optically thin gas cooling time](#optically-thin-gas-cooling-time) scales approximately as $(1+z)^{-4}/x_e$. Its volume loss scales with electron density, not with $n_H^2$, because the radiation density is independent of local gas density. The process tends toward the radiation temperature; it heats rather than cools electrons colder than that radiation.

##### Dust thermal emission

↑ **Parent:** [Radiative cooling](#radiative-cooling)

Dust grains emit thermal radiation after absorbing energy from radiation or collisions. Collisions can transfer thermal energy from dense gas to grains, whose radiation then cools the gas. This channel requires dust and does not operate in strictly pristine hydrogen-helium material without prior enrichment.

##### Inverse Compton cooling

↑ **Parent:** [Radiative cooling](#radiative-cooling)

Thermal electrons can transfer energy to lower-energy radiation photons through [Compton scattering](physics.md#compton-scattering). In the nonrelativistic Thomson regime, the net cooling power per electron is $4\sigma_TcU_\gamma k_B(T_e-T_\gamma)/(m_ec^2)$ for a blackbody photon bath. A sufficiently hot electron population therefore loses energy; a colder population is heated instead. The [cosmic microwave background](cosmology.md#cosmic-microwave-background) radiation energy density grows as $(1+z)^4$, making this channel more important for high-redshift diffuse ionized gas.

##### Astrophysical cooling function

↑ **Parent:** [Radiative cooling](#radiative-cooling)

An [astrophysical cooling function](#astrophysical-cooling-function) packages radiative losses of a plasma into a temperature-dependent coefficient. In the hydrogen-density-squared convention, the volume energy loss is $n_H^2\Lambda(T)$, so the coefficient has units $\mathrm{erg\,cm^3\,s^{-1}}$. Its dependence on [ionization](physics.md#ionization) state, chemical abundances and radiation field must be specified; a low-density collisional-equilibrium curve is not universal.

###### Molecular line cooling

↑ **Parent:** [Astrophysical cooling function](#astrophysical-cooling-function)

Radiation from rotational and vibrational transitions of molecules removes gas thermal energy. In primordial gas below the atomic threshold, [molecular hydrogen](chemistry.md#molecular-hydrogen) is a principal coolant; [hydrogen deuteride](chemistry.md#hydrogen-deuteride) can matter in suitable chemical conditions. Molecular formation, photodissociation, optical depth and density-dependent level populations control the rate. This allows some small systems below the atomic [virial temperature](classical-mechanics.md#virial-temperature) threshold to form stars.

###### Cooling suppression by photoionization

↑ **Parent:** [Astrophysical cooling function](#astrophysical-cooling-function)

[Photoionization](physics.md#photoionization) changes the ion population, often removing bound-state coolants at temperatures where collisional equilibrium would retain them. It can therefore suppress primordial line-cooling peaks. It also supplies [photoionization heating](physics.md#photoionization-heating). The net loss is cooling minus heating and depends on radiation spectrum, intensity, shielding and gas density. A universal density-independent function of temperature alone is not generally sufficient for irradiated gas.

###### Optically thin gas cooling time

↑ **Parent:** [Astrophysical cooling function](#astrophysical-cooling-function)

For a nonrelativistic ideal gas with $n_{\rm tot}$ thermal particles per volume, divide its thermal energy $3n_{\rm tot}k_BT/2$ by the optically thin volume radiation loss. In the $n_H^2$ cooling convention this becomes $3\chi k_BT/(2n_H\Lambda)$, where $\chi=n_{\rm tot}/n_H$. Density scaling and ionization-dependent particle count must be kept consistent.

###### Cooling-to-free-fall equality curve

↑ **Parent:** [Optically thin gas cooling time](#optically-thin-gas-cooling-time)

Equating the optically thin cooling time to the uniform-sphere free-fall time gives a critical gas density proportional to $T^2/\Lambda^2$. With [hydrogen mass fraction](stellar-astrophysics.md#hydrogen-mass-fraction) $X$, particle ratio $\chi$ and gravitating gas fraction $f_g$, it is $[32Gm_p/(3\pi Xf_g)][3\chi k_BT/(2\Lambda)]^2$. At fixed temperature, gas above this density cools faster than free fall. A smaller gravitating gas fraction moves the boundary upward because gravity is faster at a fixed gas density.

###### Primordial atomic cooling curve

↑ **Parent:** [Astrophysical cooling function](#astrophysical-cooling-function)

The [primordial atomic cooling curve](#primordial-atomic-cooling-curve) describes hydrogen-helium gas without heavy elements. Near the [hydrogen](chemistry.md#hydrogen) excitation threshold it rises sharply, then shows [hydrogen](chemistry.md#hydrogen) and [helium](chemistry.md#helium) excitation/[ionization](physics.md#ionization) features. Bound-state losses weaken when both elements become highly ionized. At sufficiently high temperatures [thermal bremsstrahlung](astrophysics.md#thermal-bremsstrahlung) gives a slowly rising tail. Composition, density convention and [ionization](physics.md#ionization) assumptions fix the numerical normalization.

###### Atomic line cooling

↑ **Parent:** [Astrophysical cooling function](#astrophysical-cooling-function)

[Atomic line cooling](#atomic-line-cooling) removes gas kinetic energy by [collisional excitation](physics.md#collisional-excitation) followed by photon escape. It is strongest where atoms or ions have bound [Electrons](physics.md#electron) and thermally accessible transitions. If photons are trapped, or if the relevant atoms are fully ionized, the simple optically thin line-cooling rate no longer gives the same loss.

###### Metal-line cooling

↑ **Parent:** [Atomic line cooling](#atomic-line-cooling)

Heavy elements provide many ionic transitions at temperatures where [hydrogen](chemistry.md#hydrogen) and [helium](chemistry.md#helium) have lost their most effective line emitters. [Metal-line cooling](#metal-line-cooling) can therefore increase the plasma cooling function substantially and broaden its temperature features. Low-energy fine-structure transitions also permit cooling below the [hydrogen](chemistry.md#hydrogen) atomic threshold when the relevant ions and [Electrons](physics.md#electron) are present.

### Heat flux density

↑ **Parent:** [Heat](#heat)

Heat flux density is the rate of [heat](#heat) transfer through unit area. Its SI unit is watts per square metre, and [Fourier's law](#fourier-s-law) gives its conductive contribution.

### Thermal conduction

↑ **Parent:** [Heat](#heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_conduction)

Thermal conduction transfers [heat](#heat) down a [temperature](#temperature) gradient through microscopic interactions, without bulk transport of matter.

#### Temperature dipole around an insulating sphere

↑ **Parent:** [Thermal conduction](#thermal-conduction)

In the absence of heat advection, an insulating [sphere](geometry-and-topology.md#sphere) of radius $a$ in a uniform remote [temperature](#temperature) gradient $\mathbf H$ has the displayed exterior [harmonic function](partial-differential-equation.md#harmonic-function) as its temperature field. The reflected dipole term makes $\partial_rT=0$ at $r=a$. The surface temperature is $T_0+(3/2)a\mathbf H\cdot\mathbf n$, so the tangential gradient is amplified by $3/2$. If the sphere has [thermal conductivity](#thermal-conductivity) ratio $K$ relative to its surroundings, temperature and heat-flux continuity instead give surface gradient factor $3/(2+K)$.

#### Isobaric conductive cooling in mass coordinates

↑ **Parent:** [Thermal conduction](#thermal-conduction)

With fixed [pressure](#pressure) $p$, let $A=\mu p/\mathcal R$, so $\rho=A/T$. A material mass coordinate has $\partial_x=\rho\partial_m$ and the material time derivative becomes $\partial_t|_m$. The energy and continuity equations then give the displayed equation with $\tau=Ct$ and $C=(\gamma-1)(\mu/\mathcal R)^2p/\gamma$. A mass integral from a fixed origin is material only when the [mass flux](physics.md#mass-flux) there vanishes; otherwise subtract its time-integrated flux to label parcels. Uniform [pressure](#pressure) is a low-Mach approximation when sound crossing is faster than thermal evolution.

##### Error-function isobaric cooling front

↑ **Parent:** [Isobaric conductive cooling in mass coordinates](#isobaric-conductive-cooling-in-mass-coordinates)

For conductivity $\lambda=\lambda_0T$, no cooling in the hot phase and a zero-[temperature](#temperature) boundary at $m=0$, the mass-coordinate equation is linear diffusion. Its similarity profile solves $f''+\xi f'/2=0$, $f(0)=0$, $f(\infty)=1$, giving the displayed [error function](calculus.md#error-function). The thermal layer broadens as the square root of time. Conducted energy enters the cold radiating reservoir at rate per area $L=\lambda_0A T_m(0)=A T_0\sqrt{\lambda_0}/\sqrt{\pi\tau}$, hence $L\propto t^{-1/2}$.

#### Temperature gradient

↑ **Parent:** [Thermal conduction](#thermal-conduction)

The temperature gradient is the [gradient](calculus.md#gradient) $\nabla T$ of the [temperature](#temperature) field. It points in the direction of fastest temperature increase.

<h4 id="fourier-s-law">Fourier's law</h4>

↑ **Parent:** [Thermal conduction](#thermal-conduction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fourier's_law)

Fourier's law relates the conductive heat-flux density $\mathbf q$ to the [temperature gradient](#temperature-gradient) by $\mathbf q=-k\nabla T$.

##### Thermal conductivity

↑ **Parent:** [Fourier's law](#fourier-s-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_conductivity)

Thermal conductivity is the positive material coefficient $k$ in [Fourier's law](#fourier-s-law). It may depend on [temperature](#temperature), composition, and direction.

###### Thermal conductivity tensor

↑ **Parent:** [Thermal conductivity](#thermal-conductivity)

The thermal conductivity tensor maps a temperature gradient to the negative heat-flux density. In passive reciprocal conduction it is symmetric positive definite. This permits direction-dependent transport while ensuring positive dissipated energy.

###### Thermal diffusivity

↑ **Parent:** [Thermal conductivity](#thermal-conductivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_diffusivity)

Thermal diffusivity is $\kappa=k/(\rho c_p)$, the ratio of [thermal conductivity](#thermal-conductivity) to volumetric [heat capacity](#heat-capacity). It sets the diffusion length $\sqrt{\kappa t}$ over time $t$.

###### Prandtl number

↑ **Parent:** [Thermal diffusivity](#thermal-diffusivity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prandtl_number)

The [Prandtl number](#prandtl-number) is the ratio of [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) to [thermal diffusivity](#thermal-diffusivity). It compares the rates at which momentum and [temperature](#temperature) variations diffuse. In thermal-diffusion units the [Boussinesq equations](geophysical-fluid-dynamics.md#boussinesq-equations) have momentum inertia multiplied by $\operatorname{Pr}^{-1}$; large, rather than small, [Prandtl number](#prandtl-number) supplies the usual instantaneous [Stokes flow](stokes-flow.md) limit.

###### Thermal diffusion time

↑ **Parent:** [Thermal diffusivity](#thermal-diffusivity)

The thermal diffusion time across a distance $L$ is $L^2/\kappa$, where $\kappa$ is the [thermal diffusivity](#thermal-diffusivity). It is the time required for a temperature disturbance to spread over that distance by [thermal conduction](#thermal-conduction).

###### Thermal diffusion rate of a Fourier mode

↑ **Parent:** [Thermal diffusion time](#thermal-diffusion-time)

With [thermal diffusivity](#thermal-diffusivity) $\xi$, a [Fourier mode](fourier-analysis.md#fourier-mode) of [wavenumber](wave-equation.md#wavenumber) $k$ decays by diffusion at this rate.

<h3 id="stefan-boltzmann-law">Stefan–Boltzmann law</h3>

↑ **Parent:** [Heat](#heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stefan–Boltzmann_law)

The Stefan–Boltzmann law gives the thermal-radiation flux emitted by a surface as $F=\epsilon\sigma T^4$, where $\epsilon$ is its [emissivity](#emissivity) and $\sigma$ is the Stefan–Boltzmann constant.

#### Stefan-Boltzmann constant

↑ **Parent:** [Stefan–Boltzmann law](#stefan-boltzmann-law)

The [Stefan-Boltzmann constant](#stefan-boltzmann-constant) $\sigma$ is the proportionality constant in the blackbody flux $F=\sigma T^4$. The blackbody [radiation pressure](#radiation-pressure) is $p_{\rm rad}=4\sigma T^4/(3c)$.

#### Emissivity

↑ **Parent:** [Stefan–Boltzmann law](#stefan-boltzmann-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Emissivity)

Emissivity is the ratio of the thermal radiation emitted by a surface to that emitted by an ideal black body at the same [temperature](#temperature).

#### Radiative equilibrium

↑ **Parent:** [Stefan–Boltzmann law](#stefan-boltzmann-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiative_equilibrium)

A body is in radiative equilibrium when absorbed radiative power equals emitted radiative power. A surface absorbing flux $F$ and emitting as a grey body has equilibrium temperature $T=(F/(\epsilon\sigma))^{1/4}$.

### Heat capacity

↑ **Parent:** [Heat](#heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_capacity)

Heat capacity is the heat required per unit temperature change under a specified constraint.

#### Entropy from heat capacity

↑ **Parent:** [Heat capacity](#heat-capacity)

Along a reversible path at fixed volume, $dS=C_V(T)dT/T$. Hence entropy differences can be measured macroscopically from

$$
S(T_2)-S(T_1)=\int_{T_1}^{T_2}\frac{C_V(T)}T\,dT,
$$

with an additional $L/T_c$ across a first-order transition of [latent heat](#latent-heat) $L$ at $T_c$.

#### Entropy concavity and positive heat capacity

↑ **Parent:** [Heat capacity](#heat-capacity)

For a thermodynamically stable system, the [entropy](#entropy) is concave in energy, so

$$
\frac{\partial^2S}{\partial E^2}
=-\frac1{T^2}\frac{\partial T}{\partial E}<0.
$$

Consequently $\partial E/\partial T>0$: energy increases with [temperature](#temperature), and the corresponding [heat capacity](#heat-capacity) is positive.

#### Specific heat capacity

↑ **Parent:** [Heat capacity](#heat-capacity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Specific_heat_capacity)

Specific heat capacity is [heat capacity](#heat-capacity) per unit mass. The volumetric heat capacity is $\rho c_p$, and $k/(\rho c_p)$ is the [thermal diffusivity](#thermal-diffusivity) when $k$ is the [thermal conductivity](#thermal-conductivity).

##### Specific heat capacity at constant volume

↑ **Parent:** [Specific heat capacity](#specific-heat-capacity)

The specific heat capacity at constant volume is the temperature derivative of [specific internal energy](#specific-internal-energy) at fixed density and composition: $c_V=(\partial u/\partial T)_\rho$. It is the corresponding extensive [heat capacity at constant volume](#heat-capacity-at-constant-volume) divided by material mass.

##### Specific heat capacity at constant pressure

↑ **Parent:** [Specific heat capacity](#specific-heat-capacity)

The specific heat capacity at constant pressure is $c_P=(\partial h/\partial T)_P$, where $h$ is specific enthalpy. It includes expansion work as well as the change in internal energy.

###### Pure-radiation constant-pressure heat-capacity singularity

↑ **Parent:** [Specific heat capacity at constant pressure](#specific-heat-capacity-at-constant-pressure)

For pure [blackbody radiation](statistical-physics.md#black-body-radiation), $P=aT^4/3$ depends only on [temperature](#temperature). Constant pressure therefore fixes temperature, so a usual finite constant-pressure temperature derivative is unavailable. In the material gas-radiation limit the [specific-heat ratio](#heat-capacity-ratio) diverges, although all three [stellar adiabatic exponents](stellar-structure.md#stellar-adiabatic-exponent) approach $4/3$. The radiation index $4/3$ is an adiabatic pressure-volume response, not a finite heat-capacity ratio.

#### Heat capacity at constant volume

↑ **Parent:** [Heat capacity](#heat-capacity)

The heat capacity at constant volume is $C_V=(\partial E/\partial T)_V$ when particle number and other conserved quantities are also fixed.

##### Dulong-Petit law

↑ **Parent:** [Heat capacity at constant volume](#heat-capacity-at-constant-volume)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dulong–Petit_law)

In the classical high-temperature limit, each independent harmonic mode contributes $k_B$ to the constant-volume heat capacity.

A classical crystalline solid has three vibrational modes per atom, giving $C_V\simeq3Nk_B$, or $3R$ per mole.

#### Heat capacity at constant area

↑ **Parent:** [Heat capacity](#heat-capacity)

For a two-dimensional system of fixed area $A$, the heat capacity at constant area is $C_A=(\partial E/\partial T)_{N,A}$ when the particle number and other conserved quantities are also fixed. It is the two-dimensional analogue of [heat capacity at constant volume](#heat-capacity-at-constant-volume).

## Third law of thermodynamics

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Third_law_of_thermodynamics)

The third law implies that the entropy of a system with a nondegenerate ground state approaches zero as its temperature approaches absolute zero. In particular, ordinary equilibrium heat capacities approach zero.

## Pressure

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pressure)

Pressure is normal force per unit area and is thermodynamically conjugate to volume.

### Kinematic pressure

↑ **Parent:** [Pressure](#pressure)

Dividing a [pressure](#pressure) disturbance by the constant reference [mass density](fluid-mechanics.md#density) $\rho_0$ gives a quantity whose [gradient](calculus.md#gradient) enters the [Boussinesq equations](geophysical-fluid-dynamics.md#boussinesq-equations) directly as an [acceleration](classical-mechanics.md#acceleration). Its units are squared [velocity](classical-mechanics.md#velocity). Distinguish this convention from physical [pressure](#pressure) when calculating [energy flux](physics.md#energy-flux) or comparing [wave polarization](physics.md#polarization-waves) formulae.

### Pressure tensor

↑ **Parent:** [Pressure](#pressure)

In the local rest frame of a gas, the [pressure tensor](#pressure-tensor) is the directional [momentum flux](physics.md#momentum-flux) $P_{ij}=\int p_iv_jf(\mathbf p)\,d^3p$, where $f$ is the [phase-space distribution function](statistical-physics.md#phase-space-distribution-function) per unit [momentum](classical-mechanics.md#momentum) volume and $\mathbf v$ is particle velocity. For an isotropic distribution, $P_{ij}=P\delta_{ij}$, recovering the [kinetic pressure of an isotropic gas](statistical-physics.md#kinetic-pressure-of-an-isotropic-gas). An anisotropic distribution can exert different normal [pressures](#pressure) along different directions.

### Gas pressure

↑ **Parent:** [Pressure](#pressure)

Gas pressure is the mechanical pressure contributed by material particles. For a classical ideal gas, $p_{\rm gas}=nk_BT$.

### Radiation pressure

↑ **Parent:** [Pressure](#pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radiation_pressure)

Radiation pressure is momentum flux carried by electromagnetic radiation. Isotropic blackbody radiation has $p_{\rm rad}=a_{\rm rad}T^4/3$.

### Equation of state

↑ **Parent:** [Pressure](#pressure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equation_of_state)

An equation of state is a relation among thermodynamic state variables such as pressure, volume, temperature, energy, and particle number.

#### Barotropic stellar equation of state

↑ **Parent:** [Equation of state](#equation-of-state)

A [perfect fluid in general relativity](general-relativity.md#perfect-fluid-in-general-relativity) stellar model in which pressure depends only on energy density, $p=p(\rho)$. A positive derivative makes this relation locally invertible and turns outward-decreasing pressure into outward-decreasing density. This general relation need not have the constant ratio $p/\rho$ used for a constant cosmological fluid parameter.

#### Clausius gas

↑ **Parent:** [Equation of state](#equation-of-state)

A Clausius gas with covolume parameter $b$ obeys $P(V-Nb)=Nk_BT$. It is the repulsive-volume part of a [Van der Waals equation](#van-der-waals-equation) without the attractive term.

#### Van der Waals equation

↑ **Parent:** [Equation of state](#equation-of-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Van_der_Waals_equation)

The van der Waals equation $(P+aN^2/V^2)(V-Nb)=Nk_BT$ augments excluded volume $b$ with a mean attractive interaction $a$.

##### Van der Waals law of corresponding states

↑ **Parent:** [Van der Waals equation](#van-der-waals-equation)

The [Van der Waals equation](#van-der-waals-equation) becomes independent of its material parameters when [pressure](#pressure), [temperature](#temperature) and molecular [volume](geometry-and-topology.md#volume) are divided by their critical values: $\bar p=8\bar T/(3\bar v-1)-3/\bar v^2$. This explains the common reduced isotherms within this model, without claiming exact agreement for all real fluids.

#### Equation of state of an ideal ultrarelativistic gas

↑ **Parent:** [Equation of state](#equation-of-state)

An isotropic ideal gas whose particles obey the ultrarelativistic dispersion $\varepsilon=pc$ satisfies

$$
pV=\frac E3.
$$

#### Adiabatic equation of state

↑ **Parent:** [Equation of state](#equation-of-state)

An adiabatic equation of state relates pressure and volume along a process with no heat transfer. It commonly has the form $pV^\gamma=\text{constant}$.

## Volume (thermodynamics)

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Volume_(thermodynamics))

Thermodynamic volume is the [volume](geometry-and-topology.md#volume) occupied by a thermodynamic system, treated as an [extensive variable](#extensive-quantity).

## Internal energy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Internal_energy)

Internal energy is the energy stored in the microscopic degrees of freedom of a system.

### Specific internal energy

↑ **Parent:** [Internal energy](#internal-energy)

Specific [internal energy](#internal-energy) is [internal energy](#internal-energy) per unit mass. For a [perfect gas](#ideal-gas) with constant [specific-heat ratio](#heat-capacity-ratio), $e=p/[(\gamma-1)\rho]$. Its material balance is $\rho De/Dt=-p\nabla\cdot\mathbf u+Q$, where $Q$ is [heat](#heat) supplied per unit volume per unit time.

## Thermodynamic free energy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermodynamic_free_energy)

A free energy is a thermodynamic potential whose decrease governs equilibrium under specified environmental constraints.

### Free-energy functional

↑ **Parent:** [Thermodynamic free energy](#thermodynamic-free-energy)

A [free-energy functional](#free-energy-functional) assigns a [free energy](#thermodynamic-free-energy) to an entire spatial [order parameter](critical-phenomenon.md#order-parameter) configuration rather than only to one uniform value. In [Landau-Ginzburg theory](critical-phenomenon.md#landau-ginzburg-theory), a [local derivative expansion](critical-phenomenon.md#local-derivative-expansion) gives $\mathcal A[m]=\int d^Dx\{\kappa(\nabla m)^2/2+V(m)\}$, with appropriate boundary terms and regular backgrounds. The [Landau approximation](critical-phenomenon.md#landau-approximation) minimizes this functional; a fluctuating [statistical field theory](statistical-physics.md#statistical-field-theory) instead integrates its [Boltzmann weight](statistical-physics.md#boltzmann-factor) over configurations. These procedures need not give identical [critical exponents](critical-phenomenon.md#critical-exponent).

### Helmholtz free energy

↑ **Parent:** [Thermodynamic free energy](#thermodynamic-free-energy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helmholtz_free_energy)

At fixed temperature and volume, the Helmholtz free energy is $F=E-TS=-k_BT\log Z$ in the [canonical ensemble](statistical-physics.md#canonical-ensemble).

## Chemical potential

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_potential)

The chemical potential $\mu=(\partial E/\partial N)_{S,V}$ is the energy cost of adding a particle under fixed entropy and volume.

### Chemical potential of a composition field

↑ **Parent:** [Chemical potential](#chemical-potential)

For a composition [free energy](#thermodynamic-free-energy) $F=\int[f(\phi)+\kappa|\nabla\phi|^2/2]$, the local chemical potential is the [functional derivative](calculus-of-variations.md#functional-derivative)

$$
\mu=f'(\phi)-\kappa\nabla^2\phi.
$$

At [phase coexistence](critical-phenomenon.md#phase-coexistence), exchanges between the bulk phases require equal [chemical potentials](#chemical-potential). Mechanical equilibrium additionally requires equal [pressure](#pressure) for a flat interface, or a [Young–Laplace equation](fluid-mechanics.md#young-laplace-equation) pressure jump for a curved interface.

### Chemical equilibrium

↑ **Parent:** [Chemical potential](#chemical-potential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chemical_equilibrium)

At chemical equilibrium, the sum of chemical potentials weighted by each reaction's stoichiometric coefficients vanishes.

#### Chemical disequilibrium

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

A chemical system is out of local [chemical equilibrium](#chemical-equilibrium) when reaction adjustment cannot keep pace with transport, imposed changes or external driving. Comparing the [chemical relaxation time](#chemical-relaxation-time) with transport and irradiation times identifies plausible departures. [Disequilibrium chemistry in an exoplanet atmosphere](exoplanet.md#disequilibrium-chemistry-in-an-exoplanet-atmosphere) combines this principle with mixing, horizontal advection and [atmospheric photochemistry](exoplanet.md#atmospheric-photochemistry).

#### Zero chemical potential from number-changing reactions

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

For one particle species in [chemical equilibrium](#chemical-equilibrium) under $2\phi\leftrightarrow3\phi$, chemical balance gives $2\mu_\phi=3\mu_\phi$, hence $\mu_\phi=0$. Elastic $2\phi\leftrightarrow2\phi$ imposes no such constraint. In an expanding universe the number-changing reaction must remain fast compared with the [Hubble parameter](cosmology.md#hubble-parameter); after chemical freeze-out a nonzero [chemical potential](#chemical-potential) can develop even if elastic collisions maintain [kinetic equilibrium](#kinetic-equilibrium).

#### Chemical relaxation time

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The chemical relaxation time estimates how rapidly a perturbed abundance returns toward [chemical equilibrium](#chemical-equilibrium). Comparing it with the [eddy mixing time](exoplanet.md#eddy-mixing-time) identifies a [chemical quench level](exoplanet.md#chemical-quench-level).

#### Equilibrium constant

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equilibrium_constant)

#### Photon chemical potential

↑ **Parent:** [Chemical equilibrium](#chemical-equilibrium)

The chemical potential of photons in thermal equilibrium is zero because their number is not conserved.

## Ideal gas

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_gas)

An ideal gas obeys $pV=Nk_BT$ and neglects intermolecular interactions except during elastic collisions.

### Ideal gas law

↑ **Parent:** [Ideal gas](#ideal-gas)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ideal_gas_law)

The [ideal gas](#ideal-gas) equation of state relates [pressure](#pressure), volume, particle number and [temperature](#temperature). For a stellar mixture with fixed [mean molecular weight](#mean-molecular-weight) it can be written $P=\mathcal R\rho T/\mu$. It assumes negligible interaction corrections and nondegenerate particles; excitation or ionization can change the particle count and thermodynamic response.

### Monatomic gas

↑ **Parent:** [Ideal gas](#ideal-gas)

A monatomic gas consists of individual atoms or ions rather than molecules. In the classical dilute ideal-gas regime, its three translational degrees of freedom give $U=3Nk_BT/2$ by [equipartition theorem](statistical-physics.md#equipartition-theorem). Thus $C_V=3Nk_B/2$, while $C_P-C_V=Nk_B$ follows by differentiating the ideal-gas enthalpy $H=U+PV=5Nk_BT/2$. Consequently the [adiabatic index](#heat-capacity-ratio) is $\gamma=C_P/C_V=5/3$ and the [specific internal energy](#specific-internal-energy) is $e=3P/(2\rho)$. The same translational result applies to a fully ionized mixture when the particle numbers are fixed. This excludes additional excitation, ionization and radiation contributions to the heat capacity.

### Mean free path

↑ **Parent:** [Ideal gas](#ideal-gas)

The mean free path is the average distance travelled between [collisions](classical-mechanics.md#collision). For dilute targets with [number density](statistical-physics.md#number-density) $n$ and effective [collision cross-section](classical-mechanics.md#collision-cross-section) $\sigma_c$, $\ell\sim1/(n\sigma_c)$; identical-particle conventions introduce factors such as $\sqrt2$.

#### Mean free path through randomly oriented disc absorbers

↑ **Parent:** [Mean free path](#mean-free-path)

For an unclustered population of fully covering circular disc absorbers, the inverse [mean free path](#mean-free-path) is proper number density times mean projected area. A comoving number density must first be multiplied by $(1+z)^3$. The incidence then constrains the proper radius; covering factor and multiplicity of detectable lines can change the inference.

### Mean molecular weight

↑ **Parent:** [Ideal gas](#ideal-gas)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mean_molecular_weight)

The mean molecular weight is the average mass per freely moving gas particle in units of the atomic mass unit. A fully ionized hydrogen-helium gas with mass fractions $X,Y$ has $\mu^{-1}=2X+3Y/4$.

#### Stellar gas constant

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

In stellar [ideal gas](#ideal-gas) equations, the [stellar gas constant](#stellar-gas-constant) $\mathcal R=k_B/m_u$ converts a dimensionless [mean molecular weight](#mean-molecular-weight) $\mu$ into the specific thermal relation $P=\mathcal R\rho T/\mu$. Here $m_u$ is the reference atomic mass unit, commonly approximated by the proton mass in simplified hydrogen-helium models. It has units of energy per mass per temperature. It is the molar gas constant divided by the molar mass corresponding to $m_u$, rather than the molar gas constant used with a dimensional molar molecular weight.

#### Mean molecular weight per ion

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

The [mean molecular weight](#mean-molecular-weight) per ion counts nuclei rather than nuclei plus free electrons: $\rho/(\mu_i m_u)$ is the ion number density. For species with mass fractions $X_j$ and mass numbers $A_j$, $\mu_i^{-1}=\sum_jX_j/A_j$. It is useful when ions provide a thermal [ideal gas](#ideal-gas) pressure but [electron degeneracy pressure](statistical-physics.md#electron-degeneracy-pressure) supplies a separate contribution.

#### Mean molecular weight per electron

↑ **Parent:** [Mean molecular weight](#mean-molecular-weight)

The mean molecular weight per electron is the mass carried per free electron in units of atomic mass $m_u$. Fully ionized hydrogen has $\mu_e=1$, while helium, carbon, and oxygen have approximately $\mu_e=2$. It converts [electron number density](statistical-physics.md#electron-number-density) to bulk [mass density](fluid-mechanics.md#density) in the [equation of state of a cold electron gas](statistical-physics.md#equation-of-state-of-a-cold-electron-gas).

### Heat capacity ratio

↑ **Parent:** [Ideal gas](#ideal-gas)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heat_capacity_ratio)

The specific-heat ratio of an ideal gas is $\gamma=C_p/C_V>1$.

### Nondegenerate gas

↑ **Parent:** [Ideal gas](#ideal-gas)

A gas is nondegenerate when its occupation numbers are low enough that [quantum statistics](statistical-physics.md#quantum-ideal-gas-statistics) reduce to the [Maxwell-Boltzmann distribution](statistical-physics.md#maxwell-boltzmann-distribution). A common criterion is $n\lambda_{\rm th}^3\ll1$, where $\lambda_{\rm th}$ is the thermal de Broglie wavelength.

For an [ideal gas](#ideal-gas), this is the classical statistical regime; nondegeneracy alone does not assert the absence of interactions.

### Internal energy of an ideal gas

↑ **Parent:** [Ideal gas](#ideal-gas)

For a fixed amount of ideal gas, internal energy depends only on temperature. If $C_V$ is constant, $dE=C_V\,dT$ and hence $E=C_VT$ after a choice of energy zero.

<h3 id="mayer-s-relation">Mayer's relation</h3>

↑ **Parent:** [Ideal gas](#ideal-gas)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mayer's_relation)

For an ideal gas of $N$ particles,

$$
C_p-C_V=Nk_B.
$$

Thus, with $\gamma=C_p/C_V$, one has $Nk_B/C_V=\gamma-1$.

## Real gas

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Real_gas)

A [real gas](#real-gas) departs from the [ideal gas](#ideal-gas) law because interactions and molecular volume matter. Nonideal [equations of state](#equation-of-state), including the [Dieterici equation](#dieterici-equation), model such departures.

### Dieterici equation

↑ **Parent:** [Real gas](#real-gas)

The Dieterici equation of state

$$
p=\frac{k_BT}{v-b}\exp\left(-\frac{a}{k_BTv}\right)
$$

models excluded volume through $b$ and attraction through $a$. Its critical point has $v_c=2b$ and $T_c=a/(4bk_B)$.

## Intensive and extensive thermodynamic quantities

↑ **Parent:** [Thermodynamics](thermodynamics.md)

An extensive quantity scales in proportion to the amount of material, while an intensive quantity is unchanged when the system is replicated. Energy, entropy, volume, and particle number are extensive; temperature, pressure, and chemical potential are intensive.

### Extensive quantity

↑ **Parent:** [Intensive and extensive thermodynamic quantities](#intensive-and-extensive-thermodynamic-quantities)

An extensive quantity scales in proportion to the size of a thermodynamic system: combining $n$ independent identical copies multiplies it by $n$. [Energy](classical-mechanics.md#energy), [entropy](#entropy) and [volume](geometry-and-topology.md#volume) are examples.

#### Euler relation in thermodynamics

↑ **Parent:** [Extensive quantity](#extensive-quantity)

For a single-component equilibrium system with extensive [internal energy](#internal-energy) $E(S,V,N)$, scaling its [entropy](#entropy), [volume](geometry-and-topology.md#volume) and particle number together gives $E(\lambda S,\lambda V,\lambda N)=\lambda E(S,V,N)$. The [Euler theorem for homogeneous functions](real-analysis.md#euler-theorem-for-homogeneous-functions) therefore gives $E=S\partial_SE+V\partial_VE+N\partial_NE$. The [first law of thermodynamics](#first-law-of-thermodynamics) identifies these derivatives as $T,-P,\mu$, respectively, proving $E=TS-PV+\mu N$. Dividing by volume yields the [entropy density](#entropy-density) formula $s=(\rho+P-\mu n)/T$. This step fixes the entropy normalization rather than merely identifying its differential. Differentiating the Euler relation and subtracting $dE=T\,dS-P\,dV+\mu\,dN$ gives the [Gibbs-Duhem equation](#gibbs-duhem-equation) $S\,dT-V\,dP+N\,d\mu=0$. The argument requires extensivity; it is not an assumption about arbitrary nonadditive systems.

## Gibbs-Duhem equation

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs–Duhem_equation)

The [Euler theorem for homogeneous functions](real-analysis.md#euler-theorem-for-homogeneous-functions) applied to an [extensive quantity](#extensive-quantity), together with $dE=T\,dS-p\,dV+\mu\,dN$ give

$$
E=TS-pV+\mu N,
\qquad
S\,dT-V\,dp+N\,d\mu=0.
$$

## Gibbs free energy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gibbs_free_energy)

The Gibbs free energy is $G=E-TS+pV$. For a simple system of fixed composition,

$$
dG=-S\,dT+V\,dp.
$$

### Gibbs free energy of an ideal-gas mixture

↑ **Parent:** [Gibbs free energy](#gibbs-free-energy)

For a single-phase [ideal gas](#ideal-gas) mixture with molar amounts $N_i$, common [temperature](#temperature) $T$, and [pressure](#pressure) $P$, extensivity and ideal mixing give

$$
G=\sum_iN_i\mu_i=N\sum_i x_i\left[\mu_i^\circ(T)+\mathcal RT\log\left(\frac{x_iP}{P^\circ}\right)\right].
$$

Here $N=\sum_iN_i$, $x_i$ is the [mole fraction](mathematical-biology.md#mole-fraction), $\mathcal R$ is the molar gas constant, and $P^\circ$ is the standard [pressure](#pressure). Integrating $\partial\mu_i/\partial P=\mathcal RT/P$ and including the ideal mixing [entropy](#entropy) proves $\mu_i=\mu_i^\circ+\mathcal RT\log(x_iP/P^\circ)$. Reactions can change $N$, so fractions alone do not set the extensive [Gibbs free energy](#gibbs-free-energy). Its composition Hessian is $\mathcal RT(\delta_{ij}/N_i-1/N)$; it is positive semidefinite by the weighted [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

### Gibbs free-energy Maxwell relation

↑ **Parent:** [Gibbs free energy](#gibbs-free-energy)

Equality of mixed derivatives of $dG=-S\,dT+V\,dP$ gives

$$
\left(\frac{\partial S}{\partial P}\right)_T
=-\left(\frac{\partial V}{\partial T}\right)_P.
$$

### Chemical-potential balance for a reaction

↑ **Parent:** [Gibbs free energy](#gibbs-free-energy)

For a reaction with stoichiometric changes $\nu_i$, varying the reaction extent at fixed temperature and pressure gives

$$
dG=\left(\sum_i\nu_i\mu_i\right)d\xi.
$$

Equilibrium requires $\sum_i\nu_i\mu_i=0$.

#### Thermochemical equilibrium

↑ **Parent:** [Chemical-potential balance for a reaction](#chemical-potential-balance-for-a-reaction)

Thermochemical equilibrium requires every chemical reaction to have zero Gibbs free-energy change. For ideal reactants, the equilibrium constant is $K=\exp[-\Delta_rG^\circ/(RT)]$ after standard-state activity factors are included.

##### Constrained Gibbs minimization for chemical equilibrium

↑ **Parent:** [Thermochemical equilibrium](#thermochemical-equilibrium)

At fixed [temperature](#temperature) and [pressure](#pressure), a closed reacting system reaches [thermochemical equilibrium](#thermochemical-equilibrium) by minimizing [Gibbs free energy](#gibbs-free-energy) over nonnegative species amounts subject to conserved elemental abundances. For an allowed [stoichiometric vector](mathematical-biology.md#stoichiometric-vector) $\nu$, an interior minimum has $\sum_i\nu_i\mu_i=0$. More generally the [chemical potential](#chemical-potential) vector lies in the row span of the elemental conservation matrix at positive concentrations, with the appropriate one-sided inequalities for absent species. The [first law of thermodynamics](#first-law-of-thermodynamics) gives the thermodynamic differential, while the [Second law of thermodynamics](#second-law-of-thermodynamics) supplies the minimization direction.

##### Reverse reaction rate from equilibrium thermodynamics

↑ **Parent:** [Thermochemical equilibrium](#thermochemical-equilibrium)

For an elementary reversible reaction, detailed balance gives $k_f\prod_r n_r^{\nu_r}=k_r\prod_p n_p^{\nu_p}$ at equilibrium. Hence the reverse rate coefficient is the forward coefficient divided by the equilibrium constant, with units fixed by the reaction stoichiometry.

### Phase coexistence curve

↑ **Parent:** [Gibbs free energy](#gibbs-free-energy)

Two phases coexist where their molar Gibbs free energies agree. Differentiating that equality along the coexistence curve relates its slope to the entropy and volume jumps.

#### Maxwell construction

↑ **Parent:** [Phase coexistence curve](#phase-coexistence-curve)

At fixed [temperature](#temperature), choose a coexistence [pressure](#pressure) $p_*$ such that the gas and liquid have equal [chemical potentials](#chemical-potential). Because $d\mu=v\,dp$, this gives $\int_{v_l}^{v_g}v\,dp=0$, or equivalently $\int_{v_l}^{v_g}[p(v,T)-p_*]\,dv=0$. The equal areas replace the unstable part of an isotherm by a horizontal coexistence segment.

#### Phase diagram

↑ **Parent:** [Phase coexistence curve](#phase-coexistence-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_diagram)

A phase diagram partitions a space of thermodynamic variables into regions occupied by different equilibrium phases and records the coexistence curves between them.

##### Solidus

↑ **Parent:** [Phase diagram](#phase-diagram)

The solidus bounds the entirely solid equilibrium region of a [phase diagram](#phase-diagram). For a linear [liquidus](#liquidus) $T_L(C_l)=-mC_l$ and a constant [segregation coefficient](geophysics.md#solid-liquid-segregation-coefficient) $C_s=k_D C_l$, the corresponding solidus is $T_S(C_s)=-mC_s/k_D$. The [concentration](physics.md#concentration) argument is the solid [concentration](physics.md#concentration), not the neighboring liquid [concentration](physics.md#concentration).

##### Lever rule

↑ **Parent:** [Phase diagram](#phase-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lever_rule)

The lever rule finds phase fractions from a horizontal tie line on a [phase diagram](#phase-diagram). For solid and liquid [concentrations](physics.md#concentration) $C_s,C_l$ and bulk [concentration](physics.md#concentration) $\overline C$, conservation gives $\overline C=(1-\phi)C_s+\phi C_l$. Thus $\phi=(\overline C-C_s)/(C_l-C_s)$ is the [liquid fraction](geophysics.md#liquid-fraction), provided $C_s\le\overline C\le C_l$. For pure solid, $\phi=\overline C/C_l$.

##### Bicritical point

↑ **Parent:** [Phase diagram](#phase-diagram)

A bicritical point is where two continuous transition lines and a first-order line meet, typically separating a disordered phase from two competing ordered phases.

##### Liquidus

↑ **Parent:** [Phase diagram](#phase-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liquidus)

The liquidus is the locus in a [phase diagram](#phase-diagram) above which the equilibrium state is entirely liquid. In a dilute binary solution it is often approximated locally by a linear relation such as $T_L=T_0-mC$.

###### Freezing-point depression

↑ **Parent:** [Liquidus](#liquidus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freezing-point_depression)

Freezing-point depression is the lowering of a solvent's equilibrium freezing temperature by dissolved solute. In the linear dilute approximation, $T_L=T_0-mC$ with $m>0$.

##### Eutectic system

↑ **Parent:** [Phase diagram](#phase-diagram)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eutectic_system)

An eutectic system has a composition and temperature at which a liquid is in equilibrium with two distinct solid phases. Cooling liquid of that composition through the eutectic temperature produces both solid phases together.

###### Eutectic composition

↑ **Parent:** [Eutectic system](#eutectic-system)

The eutectic composition is the liquid [concentration](physics.md#concentration) at the [eutectic temperature](#eutectic-temperature), where liquid and two solid phases coexist. It is a composition coordinate on a [phase diagram](#phase-diagram), not the overall [concentration](physics.md#concentration) of every sample in an [eutectic system](#eutectic-system).

###### Eutectic temperature

↑ **Parent:** [Eutectic system](#eutectic-system)

The eutectic temperature is the temperature of simultaneous liquid–two-solid [phase coexistence](critical-phenomenon.md#phase-coexistence) in an [eutectic system](#eutectic-system). In directional freezing of a solution away from the eutectic composition, a [mushy layer](geophysics.md#mushy-layer) can end at this temperature, where its remaining liquid solidifies.

#### First-order phase transition

↑ **Parent:** [Phase coexistence curve](#phase-coexistence-curve)

At a first-order phase transition, the Gibbs free energy is continuous while at least one first derivative, such as entropy or volume, jumps. A nonzero entropy jump produces latent heat $L=T\Delta S$.

##### Two-phase scalar coexistence endpoint conditions

↑ **Parent:** [First-order phase transition](#first-order-phase-transition)

A smooth scalar [Landau free energy](critical-phenomenon.md#landau-free-energy) can end a two-phase [phase coexistence curve](#phase-coexistence-curve) by merging two minima and their intervening maximum. At a generic stable endpoint, its first three derivatives vanish and its fourth derivative is positive. A field shift and two mixed control parameters reduce the local form to a quartic [Landau free energy](critical-phenomenon.md#landau-free-energy); the order-parameter jump then vanishes and the [magnetic susceptibility](statistical-physics.md#magnetic-susceptibility) diverges. This conclusion assumes there is no competing third phase and that the endpoint lies inside the control-parameter domain. It is not a general theorem about every first-order line: a sextic potential with fixed negative quartic coefficient has a symmetry-related ordered coexistence line that ends at a triple point with a finite jump.

##### Spin-flop transition

↑ **Parent:** [First-order phase transition](#first-order-phase-transition)

##### Classical nucleation theory

↑ **Parent:** [First-order phase transition](#first-order-phase-transition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classical_nucleation_theory)

Classical nucleation theory balances the positive surface free energy of a droplet against its negative bulk free-energy gain. In three dimensions,

$$
F(R)=4\pi\sigma R^2-\frac{4\pi}{3}\Delta R^3
$$

has critical radius $R^*=2\sigma/\Delta$ and barrier $F^*=16\pi\sigma^3/(3\Delta^2)$.

###### Critical nucleus

↑ **Parent:** [Classical nucleation theory](#classical-nucleation-theory)

A critical nucleus is the unstable droplet at the maximum of the nucleation free energy. Smaller droplets shrink, while larger droplets lower their free energy by growing.

###### Arrhenius nucleation time

↑ **Parent:** [Classical nucleation theory](#classical-nucleation-theory)

Thermal crossing of a nucleation barrier $F^*$ has rate proportional to $e^{-F^*/(k_BT)}$ and mean waiting time proportional to $e^{F^*/(k_BT)}$, up to a kinetic prefactor.

#### Latent heat

↑ **Parent:** [Phase coexistence curve](#phase-coexistence-curve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Latent_heat)

The latent heat from phase $\alpha$ to phase $\beta$ is

$$
L=T(S_\beta-S_\alpha)=H_\beta-H_\alpha
$$

per mole or per particle, according to the normalization used.

##### Stefan number

↑ **Parent:** [Latent heat](#latent-heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stefan_number)

The Stefan number compares sensible heat $c_p\Delta T$ with [latent heat](#latent-heat) $L$ per unit mass. Some solidification literature uses its reciprocal as the Stefan parameter, so the defining formula must accompany the convention.

###### Latent-to-sensible heat ratio

↑ **Parent:** [Stefan number](#stefan-number)

The latent-to-sensible heat ratio is the reciprocal of the [Stefan number](#stefan-number) defined by $\mathrm{Ste}=c_p\Delta T/L$. Large $S$ means that phase change uses much more energy than changing temperature by $\Delta T$.

##### Clausius-Clapeyron relation

↑ **Parent:** [Latent heat](#latent-heat)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clausius–Clapeyron_relation)

Along a first-order coexistence curve,

$$
\frac{dp}{dT}
=\frac{S_\beta-S_\alpha}{V_\beta-V_\alpha}
=\frac{L}{T(V_\beta-V_\alpha)}.
$$

At a critical point the two phases merge, their entropy jump vanishes, and the latent heat tends to zero.

###### Common-pressure melting-point slope

↑ **Parent:** [Clausius-Clapeyron relation](#clausius-clapeyron-relation)

When the solid and liquid have the same [pressure](#pressure), equality of [chemical potentials](#chemical-potential) implies $-(s_l-s_s)dT+(1/\rho_l-1/\rho_s)dp=0$. With [latent heat of fusion](statistical-physics.md#latent-heat-of-fusion) $L=T_m(s_l-s_s)$, this gives the displayed slope. If solid is less dense than liquid, raising the common pressure depresses the [melting](critical-phenomenon.md#melting) temperature. $T_m$ is absolute [temperature](#temperature). This coexistence-curve derivative differs from a thermomolecular pressure difference between equal-density phases.

## Conjugate variables (thermodynamics)

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_variables_(thermodynamics))

Two thermodynamic variables are conjugate when their product has units of energy and they occur as a paired term in a thermodynamic differential, such as pressure and volume or tension and length.

## First law of thermodynamics

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_law_of_thermodynamics)

For a simple compressible system with fixed particle number, $dE=T\,dS-p\,dV$.

### Adiabatic process

↑ **Parent:** [First law of thermodynamics](#first-law-of-thermodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Adiabatic_process)

An adiabatic process exchanges no heat with its surroundings, so $\delta Q=0$. A reversible adiabatic process is isentropic.

#### Adiabatic compression

↑ **Parent:** [Adiabatic process](#adiabatic-process)

#### Adiabatic expansion

↑ **Parent:** [Adiabatic process](#adiabatic-process)

#### Isentropic process

↑ **Parent:** [Adiabatic process](#adiabatic-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isentropic_process)

An isentropic process keeps the [entropy](#entropy) constant. Every reversible [adiabatic process](#adiabatic-process) is isentropic, while an irreversible adiabatic process can increase entropy.

#### Reversible ideal-gas adiabat

↑ **Parent:** [Adiabatic process](#adiabatic-process)

For a fixed amount of ideal gas with constant heat capacities, the first law and $\delta Q=0$ give

$$
TV^{\gamma-1}=\text{constant},
\qquad
pV^\gamma=\text{constant},
$$

where $\gamma=C_p/C_V$.

## Enthalpy

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Enthalpy)

Enthalpy is $H=E+pV$ and satisfies $dH=T\,dS+V\,dp$ for a simple compressible system.

### Joule-Thomson coefficient

↑ **Parent:** [Enthalpy](#enthalpy)

The temperature change per pressure change at fixed enthalpy is $\mu=(\partial T/\partial p)_H=[T(\partial V/\partial T)_p-V]/C_p$. A positive coefficient means cooling under an adiabatic throttle pressure drop.

#### Virial criterion for Joule-Thomson cooling

↑ **Parent:** [Joule-Thomson coefficient](#joule-thomson-coefficient)

For $p=k_BT[n+B_2(T)n^2]$, the coefficient is $\mu=N[TB_2'-B_2]/[C_p(1+2B_2n)]$. On the stable dilute branch it is positive precisely when $d(B_2/T)/dT>0$.

### Specific enthalpy

↑ **Parent:** [Enthalpy](#enthalpy)

Specific enthalpy is [enthalpy](#enthalpy) per unit mass. For a simple compressible fluid of fixed composition, the [first law of thermodynamics](#first-law-of-thermodynamics) gives

$$
dh=T\,ds+\frac{dp}{\rho},
$$

where $T$ is [temperature](#temperature), $s$ is [specific entropy](#specific-entropy), $p$ is [pressure](#pressure), and $\rho$ is [mass density](fluid-mechanics.md#density). Along an [isentropic flow](compressible-flow.md#isentropic-flow), $dh=dp/\rho$. For a [perfect gas](#ideal-gas) with constant [specific-heat ratio](#heat-capacity-ratio) $\gamma$, $h=\gamma p/[(\gamma-1)\rho]$.

#### Polytropic enthalpy

↑ **Parent:** [Specific enthalpy](#specific-enthalpy)

For $p=K\rho^{1+1/n}$ with $K,n>0$, the specific [enthalpy](#enthalpy) relative to vacuum is $Q=(n+1)K\rho^{1/n}=(n+1)p/\rho$. It obeys $\nabla Q=\nabla p/\rho$ and $nD_tQ=-Q\nabla\cdot\mathbf u$. The vacuum reference is fixed when these equations are combined with the [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state).

### Enthalpy Maxwell relation

↑ **Parent:** [Enthalpy](#enthalpy)

Since $T=(\partial H/\partial S)_p$ and $V=(\partial H/\partial p)_S$, equality of mixed derivatives gives $(\partial T/\partial p)_S=(\partial V/\partial S)_p$.

### Heat capacity at constant pressure

↑ **Parent:** [Enthalpy](#enthalpy)

At fixed pressure, supplied heat equals enthalpy change; for constant $C_p$, $Q=C_p\Delta T$.

#### Difference between constant-pressure and constant-volume heat capacities

↑ **Parent:** [Heat capacity at constant pressure](#heat-capacity-at-constant-pressure)

For a simple compressible system,

$$
C_P-C_V
=T\left(\frac{\partial V}{\partial T}\right)_P
\left(\frac{\partial P}{\partial T}\right)_V.
$$

This follows by expressing the entropy as a function of temperature and volume and using a Maxwell relation.

## Diatomic ideal-gas enthalpy

↑ **Parent:** [Thermodynamics](thermodynamics.md)

With translational and rotational modes active but vibration frozen, a diatomic ideal gas has $E=5Nk_BT/2$ and $H=7Nk_BT/2$.

## Irreversible adiabatic piston compression

↑ **Parent:** [Thermodynamics](thermodynamics.md)

After a sudden increase to constant external pressure $p_1$, an insulated gas obeys $\Delta E=p_1(V_0-V_1)$ rather than a reversible adiabatic power law.

## Constant-pressure heating of an ideal gas

↑ **Parent:** [Thermodynamics](thermodynamics.md)

At fixed pressure, $Q=\Delta H$ and the expansion work is $p\Delta V=Nk_B\Delta T$.

## Thermodynamic cycle

↑ **Parent:** [Thermodynamics](thermodynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermodynamic_cycle)

A thermodynamic cycle returns a working substance to its initial state. Its net internal-energy change is zero, so the net work output equals net heat input.

### Thermal efficiency

↑ **Parent:** [Thermodynamic cycle](#thermodynamic-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_efficiency)

The thermal efficiency of a heat engine is the net work output divided by heat input. For a cycle absorbing $Q_{\rm in}$ and rejecting the positive amount $Q_{\rm out}$,

$$
\eta=1-\frac{Q_{\rm out}}{Q_{\rm in}}.
$$

### Otto cycle

↑ **Parent:** [Thermodynamic cycle](#thermodynamic-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Otto_cycle)

The ideal Otto cycle has adiabatic compression, constant-volume heat addition, adiabatic expansion, and constant-volume heat rejection. For an ideal gas with compression ratio $r=V_1/V_2$ and specific-heat ratio $\gamma$,

$$
\eta=1-\frac1{r^{\gamma-1}}.
$$

### Diesel cycle

↑ **Parent:** [Thermodynamic cycle](#thermodynamic-cycle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diesel_cycle)

The ideal Diesel cycle consists of reversible adiabatic compression, constant-pressure heat addition, reversible adiabatic expansion, and constant-volume heat rejection.

## ↑ Ancestors (4)

1. [Statistical physics](statistical-physics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Laws of thermodynamics](#laws-of-thermodynamics)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-58.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-311.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1.md#36c/a/solution)
