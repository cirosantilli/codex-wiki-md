# Stellar structure

↑ **Parent:** [Stellar astrophysics](stellar-astrophysics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stellar_structure)

Stellar structure follows from mass conservation, hydrostatic equilibrium, energy generation, and energy transport together with an equation of state and opacity law.

**Table of contents**

- [Central stellar temperature](#central-stellar-temperature)
- [Stellar core](#stellar-core)
- [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)
  - [Roche model of a uniformly rotating star](#roche-model-of-a-uniformly-rotating-star)
  - [Radiative gradient in a uniformly rotating star](#radiative-gradient-in-a-uniformly-rotating-star)
  - [Meridional circulation in a star](#meridional-circulation-in-a-star)
    - [Eddington-Sweet circulation](#eddington-sweet-circulation)
    - [Equipotential luminosity conservation with stellar circulation](#equipotential-luminosity-conservation-with-stellar-circulation)
  - [Radiative-equilibrium obstruction in a rotating barotropic star](#radiative-equilibrium-obstruction-in-a-rotating-barotropic-star)
  - [Gravity darkening](#gravity-darkening)
    - [Radiative gravity-darkening law](#radiative-gravity-darkening-law)
- [Uniform-density stellar model](#uniform-density-stellar-model)
- [Linear-density stellar model](#linear-density-stellar-model)
- [Stellar energy balance equation](#stellar-energy-balance-equation)
  - [Stellar neutrino energy loss](#stellar-neutrino-energy-loss)
  - [Gravothermal stellar energy generation](#gravothermal-stellar-energy-generation)
- [Stellar gas-pressure fraction](#stellar-gas-pressure-fraction)
  - [Uniform gas-pressure fraction and constant-luminosity radiative-envelope incompatibility](#uniform-gas-pressure-fraction-and-constant-luminosity-radiative-envelope-incompatibility)
- [Stellar thermal equilibrium](#stellar-thermal-equilibrium)
- [Stellar equation-of-state regime diagram](#stellar-equation-of-state-regime-diagram)
  - [Ionic Coulomb coupling parameter](#ionic-coulomb-coupling-parameter)
  - [Radiation-to-degeneracy pressure boundary](#radiation-to-degeneracy-pressure-boundary)
  - [Radiation-to-gas pressure boundary](#radiation-to-gas-pressure-boundary)
  - [Thermal electron relativistic threshold](#thermal-electron-relativistic-threshold)
- [Stellar composition profile](#stellar-composition-profile)
- [Stellar structure equations](#stellar-structure-equations)
  - [Stellar mass conservation equation](#stellar-mass-conservation-equation)
- [Stellar adiabatic exponent](#stellar-adiabatic-exponent)
  - [Adiabatic exponents of a monatomic gas-radiation mixture](#adiabatic-exponents-of-a-monatomic-gas-radiation-mixture)
    - [Specific heats of a monatomic gas-radiation mixture](#specific-heats-of-a-monatomic-gas-radiation-mixture)
- [Enclosed mass](#enclosed-mass)
- [Hydrostatic pressure support equation](#hydrostatic-pressure-support-equation)
- [Stellar polytrope](#stellar-polytrope)
  - [Polytrope of index five](#polytrope-of-index-five)
    - [Luminosity integral of an index-five polytrope](#luminosity-integral-of-an-index-five-polytrope)
  - [Moment of inertia of a polytropic star](#moment-of-inertia-of-a-polytropic-star)
  - [Polytrope of index zero](#polytrope-of-index-zero)
  - [Low-density polytropic mass divergence](#low-density-polytropic-mass-divergence)
  - [Gravitational energy of a stellar polytrope](#gravitational-energy-of-a-stellar-polytrope)
  - [Lane-Emden variables for a stellar polytrope](#lane-emden-variables-for-a-stellar-polytrope)
  - [Polytrope of index one](#polytrope-of-index-one)
    - [Cubic polytropic interior](#cubic-polytropic-interior)
      - [Cubic polytrope fails isolated gravitational matching](#cubic-polytrope-fails-isolated-gravitational-matching)
        - [Corner-force obstruction for a cubic polytrope](#corner-force-obstruction-for-a-cubic-polytrope)
  - [Eddington standard model](#eddington-standard-model)
  - [Polytropic index](#polytropic-index)
  - [Adiabatic stellar polytrope](#adiabatic-stellar-polytrope)
  - [Polytropic mass-radius relation](#polytropic-mass-radius-relation)
    - [Entropy dependence of a polytropic mass-radius relation](#entropy-dependence-of-a-polytropic-mass-radius-relation)
  - [Lane-Emden mass formula](#lane-emden-mass-formula)
    - [Lane-Emden surface mass constant](#lane-emden-surface-mass-constant)
  - [Eddington quartic relation](#eddington-quartic-relation)
- [Stellar homology](#stellar-homology)
  - [Fully convective homology with tenth-power surface opacity](#fully-convective-homology-with-tenth-power-surface-opacity)
  - [Homologous adiabatic stellar stability](#homologous-adiabatic-stellar-stability)
  - [Constant-opacity homologous contraction to CNO ignition](#constant-opacity-homologous-contraction-to-cno-ignition)
  - [Homology scaling of central stellar pressure](#homology-scaling-of-central-stellar-pressure)
  - [Homologous rotating collapse](#homologous-rotating-collapse)
    - [Critical rotation of a spherical cloud](#critical-rotation-of-a-spherical-cloud)
  - [Homology relations for radiative stars](#homology-relations-for-radiative-stars)
    - [Radiative homology with density-half inverse-five-halves opacity](#radiative-homology-with-density-half-inverse-five-halves-opacity)
    - [Kramers homology with a variable nuclear exponent](#kramers-homology-with-a-variable-nuclear-exponent)
    - [Radiative homology with fifth-power hydrogen burning and inverse-cubic opacity](#radiative-homology-with-fifth-power-hydrogen-burning-and-inverse-cubic-opacity)
    - [Radiative homology with proton-proton burning and inverse-fourth-power opacity](#radiative-homology-with-proton-proton-burning-and-inverse-fourth-power-opacity)
      - [Turnoff mass of a homogeneously mixed proton-proton-burning population](#turnoff-mass-of-a-homogeneously-mixed-proton-proton-burning-population)
    - [CNO homology with density-dependent inverse-cubic opacity](#cno-homology-with-density-dependent-inverse-cubic-opacity)
    - [Homogeneous fuel-depletion luminosity feedback](#homogeneous-fuel-depletion-luminosity-feedback)
    - [Composition-dependent CNO homology](#composition-dependent-cno-homology)
      - [Fully mixed hydrogen-burning evolutionary track](#fully-mixed-hydrogen-burning-evolutionary-track)
    - [Hertzsprung-Russell slope of a stellar homology sequence](#hertzsprung-russell-slope-of-a-stellar-homology-sequence)
    - [Radiative homology with proton-proton burning and Kramers opacity](#radiative-homology-with-proton-proton-burning-and-kramers-opacity)
    - [Radiative homology with CNO burning and electron scattering](#radiative-homology-with-cno-burning-and-electron-scattering)
- [Surface gravity of a star](#surface-gravity-of-a-star)
- [Stellar surface boundary condition](#stellar-surface-boundary-condition)
  - [Photosphere](#photosphere)
    - [Hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth)
      - [Grey-atmosphere convection onset with eighth-power temperature opacity](#grey-atmosphere-convection-onset-with-eighth-power-temperature-opacity)
      - [Grey-atmosphere pressure with power-law opacity](#grey-atmosphere-pressure-with-power-law-opacity)
        - [Surface boundary condition for a power-law-opacity grey atmosphere](#surface-boundary-condition-for-a-power-law-opacity-grey-atmosphere)
        - [Grey-atmosphere convection onset with density-linear opacity](#grey-atmosphere-convection-onset-with-density-linear-opacity)
        - [Grey-atmosphere convection onset with seventeenth-power opacity](#grey-atmosphere-convection-onset-with-seventeenth-power-opacity)
- [Stellar virial theorem](#stellar-virial-theorem)
- [Stellar convective stability](#stellar-convective-stability)
  - [Grey-atmosphere convection onset with thirteenth-power opacity](#grey-atmosphere-convection-onset-with-thirteenth-power-opacity)
  - [Stellar convective instability](#stellar-convective-instability)
    - [Convective instability of a uniform-density star](#convective-instability-of-a-uniform-density-star)
  - [Schwarzschild criterion](#schwarzschild-criterion)
  - [Ledoux criterion](#ledoux-criterion)
  - [Convection onset in a logarithmic-pressure grey atmosphere](#convection-onset-in-a-logarithmic-pressure-grey-atmosphere)
  - [Convective core](#convective-core)
    - [Eddington-model convective-core mass fraction](#eddington-model-convective-core-mass-fraction)
  - [Convective envelope](#convective-envelope)
  - [Radiative envelope](#radiative-envelope)
    - [Kramers radiative-zero envelope around a stellar core](#kramers-radiative-zero-envelope-around-a-stellar-core)
    - [Self-gravitating Kramers power-law envelope](#self-gravitating-kramers-power-law-envelope)
    - [Power-law opacity radiative envelope](#power-law-opacity-radiative-envelope)
      - [Radiative-envelope convection matching](#radiative-envelope-convection-matching)
        - [Deep radiative boundary beneath a power-law-opacity convective envelope](#deep-radiative-boundary-beneath-a-power-law-opacity-convective-envelope)
  - [Fully convective star](#fully-convective-star)
- [Radiative stellar structure](#radiative-stellar-structure)
  - [Radiative core](#radiative-core)
  - [Stellar radiative temperature gradient](#stellar-radiative-temperature-gradient)
  - [Opacity](#opacity)
    - [Negative hydrogen ion opacity](#negative-hydrogen-ion-opacity)
      - [Negative-hydrogen-opacity alpha-disk thickness scaling](#negative-hydrogen-opacity-alpha-disk-thickness-scaling)
    - [Kramers' opacity law](#kramers-opacity-law)
    - [Electron-scattering opacity](#electron-scattering-opacity)
    - [Free-free opacity](#free-free-opacity)
  - [Radiative diffusion in a star](#radiative-diffusion-in-a-star)
    - [Radiative conductivity](#radiative-conductivity)
- [Effective temperature](#effective-temperature)
- [Mass-luminosity relation](#mass-luminosity-relation)
  - [Eddington luminosity](#eddington-luminosity)
    - [Stellar electron-scattering Eddington factor](#stellar-electron-scattering-eddington-factor)
    - [Dust-grain Eddington limit](#dust-grain-eddington-limit)
    - [Radiative force multiplier](#radiative-force-multiplier)

## Central stellar temperature

↑ **Parent:** [Stellar structure](stellar-structure.md)

The [temperature](thermodynamics.md#temperature) at a star's centre. In gas-pressure-supported [stellar homology](#stellar-homology), the [stellar hydrostatic equation](#hydrostatic-pressure-support-equation) and [ideal gas law](thermodynamics.md#ideal-gas-law) give $T_c\propto\mu GM/(\mathcal R R)$, with a coefficient set by the [dimensionless](physics.md#dimensionless-quantity) density and pressure profiles. It controls the strongly temperature-dependent [stellar energy-generation rate](stellar-astrophysics.md#stellar-energy-generation-rate).

## Stellar core

↑ **Parent:** [Stellar structure](stellar-structure.md)

A stellar core is the central region distinguished from the surrounding envelope by its composition, energy generation or thermodynamic state. A core boundary at radius $R_c$ encloses mass $M_c=m(R_c)=4\pi\int_0^{R_c}\rho(r)r^2dr$. In a hydrogen-shell-burning [red giant](stellar-astrophysics.md#red-giant), a helium-rich core can be inert while a narrow surrounding layer supplies the luminosity. Core mass and core radius are separate variables: the relation between them must come from a structural model, such as a [polytropic mass-radius relation](#polytropic-mass-radius-relation), rather than from the word core alone.

## Uniformly rotating stellar hydrostatic equilibrium

↑ **Parent:** [Stellar structure](stellar-structure.md)

Uniform [solid-body rotation](classical-mechanics.md#solid-body-rotation) adds the [centrifugal potential](physics.md#centrifugal-potential) $-\Omega^2\varpi^2/2$ to the gravitational potential. In the corotating frame, [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) becomes $\nabla P=-\rho\nabla\phi$. The [Poisson equation](partial-differential-equation.md#poisson-equation) gives $\nabla^2\phi=4\pi G\rho-2\Omega^2$. On regular connected [equipotential surfaces](classical-mechanics.md#equipotential-surface), $P$ is constant; taking the curl shows that $\rho$ is constant too. Uniform composition and an invertible equation of state then make $T$ constant on each such surface. These statements do not require $|\nabla\phi|$ to be constant there.

### Roche model of a uniformly rotating star

↑ **Parent:** [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)

This approximation represents the [gravitational potential](classical-mechanics.md#newtonian-potential-of-a-point-mass) by a central point mass while retaining the [centrifugal potential](physics.md#centrifugal-potential). A surface through polar radius $R_p$ satisfies $R_p/r+q(r/R_p)^2\sin^2\theta/2=1$, where $q=\Omega^2R_p^3/(GM)$. The inner closed surface is regular below $q=8/27$; at the limiting value its equatorial radius is $3R_p/2$ and equatorial effective gravity vanishes. The approximation is useful for illustrating oblateness and [gravity darkening](#gravity-darkening), rather than modeling the density distribution of every rotating star.

### Radiative gradient in a uniformly rotating star

↑ **Parent:** [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)

The [divergence theorem](calculus.md#divergence-theorem) and [Poisson equation](partial-differential-equation.md#poisson-equation) give $\int_S\nabla\phi\cdot d\mathbf S=4\pi Gm-2\Omega^2V$ on a bounding [equipotential surface](classical-mechanics.md#equipotential-surface). [Equipotential luminosity conservation with stellar circulation](#equipotential-luminosity-conservation-with-stellar-circulation) then fixes $f=L/(4\pi Gm-2\Omega^2V)$. Combining $dT/d\phi=-f/\chi$, $dP/d\phi=-\rho$ and [radiative conductivity](#radiative-conductivity) gives the displayed logarithmic temperature-pressure gradient. Both appearances of mass mean the enclosed mass $m$; only on the outer boundary can both be replaced by the total mass.

### Meridional circulation in a star

↑ **Parent:** [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)

Slow circulation in planes containing the rotation axis can transport entropy through a rotating star while the leading mechanical balance remains nearly [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). Its steady mass flux satisfies the [continuity equation](physics.md#continuity-equation). It is distinct from assuming an exactly motionless radiative interior, and from turbulent [convection](fluid-mechanics.md#convection).

#### Eddington-Sweet circulation

↑ **Parent:** [Meridional circulation in a star](#meridional-circulation-in-a-star)

The thermal imbalance of a slowly rotating radiative [star](stellar-astrophysics.md#star) can drive [stellar meridional circulation](#meridional-circulation-in-a-star). Its fractional centrifugal distortion is $\epsilon_\Omega\sim\Omega^2R^3/(GM)$, so balancing an order-$\epsilon_\Omega$ fraction of the [luminosity](astrophysics.md#luminosity) by thermal advection estimates $t_{\rm ES}\sim t_{\rm KH}/\epsilon_\Omega$, where $t_{\rm KH}\sim GM^2/(RL)$. Stable composition gradients can further impede the circulation. This radiative thermal estimate is different from rapid torque-driven circulation in a convective envelope.

#### Equipotential luminosity conservation with stellar circulation

↑ **Parent:** [Meridional circulation in a star](#meridional-circulation-in-a-star)

For steady [stellar meridional circulation](#meridional-circulation-in-a-star), $T\nabla s=\nabla(h+\phi)$ and $\nabla\cdot(\rho\mathbf v)=0$. Thus $\rho\mathbf v\cdot T\nabla s=\nabla\cdot[\rho\mathbf v(h+\phi)]$. In the leading [uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium), $h+\phi$ is constant on an [equipotential surface](classical-mechanics.md#equipotential-surface); its total advected flux vanishes because the net mass flux vanishes. Integrating the energy equation then identifies the outward [luminosity](astrophysics.md#luminosity) with enclosed nuclear energy generation, even though local heat advection is nonzero.

### Radiative-equilibrium obstruction in a rotating barotropic star

↑ **Parent:** [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)

On a regular [equipotential surface](classical-mechanics.md#equipotential-surface), $f,f',\rho$ and $\nabla^2\phi$ are constant, but $|\nabla\phi|^2$ generally varies. Consequently a flux $\mathbf F=f(\phi)\nabla\phi$ cannot ordinarily satisfy local [radiative equilibrium](thermodynamics.md#radiative-equilibrium) $\nabla\cdot\mathbf F=\rho\epsilon$ at all latitudes. Special cases such as $f'=0$ or spherical symmetry evade this obstruction. [Stellar meridional circulation](#meridional-circulation-in-a-star) supplies heat advection in the leading hydrostatic treatment.

### Gravity darkening

↑ **Parent:** [Uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravity_darkening)

[Gravity darkening](#gravity-darkening) is the variation of surface brightness and [effective temperature](#effective-temperature) with effective gravity over a rotating or tidally distorted star. Lower equatorial gravity generally corresponds to cooler equatorial regions. The [radiative gravity-darkening law](#radiative-gravity-darkening-law) applies to the idealized uniformly rotating, radiatively transporting, composition-uniform case; its exponent is not universal for every stellar envelope.

#### Radiative gravity-darkening law

↑ **Parent:** [Gravity darkening](#gravity-darkening)

In [uniformly rotating stellar hydrostatic equilibrium](#uniformly-rotating-stellar-hydrostatic-equilibrium), composition-uniform thermodynamic quantities are functions of the total potential. [Radiative conductivity](#radiative-conductivity) gives $\mathbf F=f(\phi)\nabla\phi$, with $f=-\chi\,dT/d\phi$. On one surface, $f$ is constant, so the outward flux is $F_n=f g$. The [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) therefore gives $T_e\propto g^{1/4}$. This is a surface-flux law: the material temperature constant on an interior equipotential is not the latitude-dependent emergent [effective temperature](#effective-temperature).

## Uniform-density stellar model

↑ **Parent:** [Stellar structure](stellar-structure.md)

A uniform-density spherical [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) model with zero surface pressure has $P(r)=2\pi G\rho^2(R^2-r^2)/3$, $M=4\pi\rho R^3/3$ and gravitational energy $-3GM^2/(5R)$. A [perfect gas](thermodynamics.md#ideal-gas) can have this mechanical structure with varying [temperature](thermodynamics.md#temperature) and entropy; the imposed equilibrium density does not require incompressible perturbations.

## Linear-density stellar model

↑ **Parent:** [Stellar structure](stellar-structure.md)

An imposed spherical profile $\rho=\rho_c(1-r/R)$ gives $M=\pi\rho_cR^3/3$ in [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). For an [ideal gas](thermodynamics.md#ideal-gas) with zero surface pressure, $P=P_c(1-x)^2(1+2x-9x^2/5)$ and $T=T_c(1-x)(1+2x-9x^2/5)$, where $x=r/R$, $P_c=5GM^2/(4\pi R^4)$ and $T_c=5GM/(12\mathcal RR)$. The density has a central cusp and temperature initially rises outward, so positive outward [radiative diffusion](astrophysics.md#radiative-diffusion) with regular positive nuclear heating cannot satisfy this imposed profile near the centre.

## Stellar energy balance equation

↑ **Parent:** [Stellar structure](stellar-structure.md)

For a slowly evolving spherical star, the Lagrangian energy equation separates nuclear rest-mass release, [stellar neutrino energy loss](#stellar-neutrino-energy-loss), thermal storage and pressure-volume work. Specific internal energy and nuclear energy conventions must avoid counting nuclear mass changes or escaping reaction-neutrino energy twice. At fixed composition the [gravothermal stellar energy generation](#gravothermal-stellar-energy-generation) is $-TDS/Dt$. Energy transport processes redistribute heat rather than creating it.

### Stellar neutrino energy loss

↑ **Parent:** [Stellar energy balance equation](#stellar-energy-balance-equation)

Escaping [neutrinos](standard-model.md#neutrino) remove energy produced by nuclear reactions or drawn from thermal reservoirs. Pair annihilation, plasma excitations, photoneutrino emission and electron-ion bremsstrahlung provide thermal losses. This reduces photon [luminosity](astrophysics.md#luminosity) or increases the required nuclear and gravothermal supply. At sufficiently extreme collapse densities, [neutrino](standard-model.md#neutrino) transport must replace a free-escape loss approximation.

### Gravothermal stellar energy generation

↑ **Parent:** [Stellar energy balance equation](#stellar-energy-balance-equation)

This term accounts for thermal storage and compression or expansion in the [stellar energy balance equation](#stellar-energy-balance-equation). At fixed composition the [first law of thermodynamics](thermodynamics.md#first-law-of-thermodynamics) makes it $-TDS/Dt$. [Kelvin-Helmholtz contraction](stellar-astrophysics.md#kelvin-helmholtz-mechanism) can supply positive [luminosity](astrophysics.md#luminosity), while thermal adjustment may locally absorb energy. It is not simply the full change in gravitational potential energy: the [stellar virial theorem](#stellar-virial-theorem) also requires changes in internal energy.

## Stellar gas-pressure fraction

↑ **Parent:** [Stellar structure](stellar-structure.md)

The gas-pressure fraction describes the relative support by an [ideal gas](thermodynamics.md#ideal-gas) and [radiation pressure](thermodynamics.md#radiation-pressure). For monatomic gas plus equilibrium radiation, it determines the [adiabatic exponents of a monatomic gas-radiation mixture](#adiabatic-exponents-of-a-monatomic-gas-radiation-mixture). Its value at the unperturbed state may be specified, but it generally changes during an isentropic parcel displacement.

### Uniform gas-pressure fraction and constant-luminosity radiative-envelope incompatibility

↑ **Parent:** [Stellar gas-pressure fraction](#stellar-gas-pressure-fraction)

For a radiative envelope, $dP_{\rm rad}/dP=\kappa L_r/(4\pi cGm)$. Exactly uniform [stellar gas-pressure fraction](#stellar-gas-pressure-fraction) instead requires this derivative to be $1-\beta$. Constant opacity therefore requires $L_r$ to increase in proportion to enclosed mass. A positive-density finite-mass envelope with no local energy generation has constant $L_r$ and cannot satisfy all these conditions pointwise. The [Eddington-model convective-core mass fraction](#eddington-model-convective-core-mass-fraction) uses constant $\beta$ as a global approximation, rather than an exact detailed envelope constraint.

## Stellar thermal equilibrium

↑ **Parent:** [Stellar structure](stellar-structure.md)

In [stellar structure](stellar-structure.md), stellar thermal equilibrium means that internal heating balances the surface [luminosity](astrophysics.md#luminosity) and any energy loss through neutrinos, with negligible secular storage of thermal [energy](classical-mechanics.md#energy) on the timescale considered. A star can satisfy this balance while its interior is hotter than its surface and [heat](thermodynamics.md#heat) flows outward. It is therefore different from equal-temperature [thermal equilibrium](thermodynamics.md#thermal-equilibrium) between systems. Neglecting neutrino losses, the balance is $L_{\rm surface}=L_{\rm heat}$. In a slowly mass-losing [donor star](stellar-astrophysics.md#donor-star), a [stellar thermal equilibrium](#stellar-thermal-equilibrium) radius sequence applies only when thermal adjustment is fast compared with the mass-loss timescale; rapid loss instead requires the adiabatic [stellar radius response exponent](stellar-astrophysics.md#stellar-radius-response-exponent).

## Stellar equation-of-state regime diagram

↑ **Parent:** [Stellar structure](stellar-structure.md)

A [temperature](thermodynamics.md#temperature) versus density diagram separates classical, degenerate, nonrelativistic and relativistic stellar-matter limits. The [Electron](physics.md#electron) degeneracy boundary is $T\sim T_F(\rho)$, with slope $2/3$ at low density and $1/3$ at high density. Thermal relativity is controlled by $k_BT\sim m_ec^2$, while relativity of degenerate [Electrons](physics.md#electron) is controlled by $p_F\sim m_ec$. [Photon](quantum-mechanics.md#photon) [pressure](thermodynamics.md#pressure) and thermal electron-positron pairs add further crossovers; all depend on composition and are gradual, not thermodynamic phase boundaries.

### Ionic Coulomb coupling parameter

↑ **Parent:** [Stellar equation-of-state regime diagram](#stellar-equation-of-state-regime-diagram)

For one ionic species of [number density](statistical-physics.md#number-density) $n_i$, the ion-sphere radius is $a_i=(3/(4\pi n_i))^{1/3}$. The ionic Coulomb coupling parameter compares the interaction energy from [Coulomb's law](electromagnetism.md#coulomb-s-law) at that separation with thermal energy $k_BT$. At fixed composition, $\Gamma\propto\rho^{1/3}/T$. Values near one mark significant corrections to the ideal ion gas; strong coupling can lead to an ordered solid. Screening, mixtures and quantum motion modify detailed transitions, so this estimate is not a universal crystallization boundary. It is separate from the electron degeneracy criterion based on the [electron Fermi temperature](statistical-physics.md#electron-fermi-temperature).

### Radiation-to-degeneracy pressure boundary

↑ **Parent:** [Stellar equation-of-state regime diagram](#stellar-equation-of-state-regime-diagram)

Equating [radiation pressure](thermodynamics.md#radiation-pressure) to cold [electron degeneracy pressure](statistical-physics.md#electron-degeneracy-pressure) gives $T=[3P_e(\rho)/a_{\rm rad}]^{1/4}$. Because the two [Electron](physics.md#electron) [pressure](thermodynamics.md#pressure) limits scale as $\rho^{5/3}$ and $\rho^{4/3}$, this boundary has logarithmic slopes $5/12$ and $1/3$, respectively. Above it, [photon](quantum-mechanics.md#photon) [pressure](thermodynamics.md#pressure) can dominate even when the net [Electrons](physics.md#electron) remain degenerate; degeneracy of one component and dominance of the total [pressure](thermodynamics.md#pressure) are different criteria. Thermal pairs modify the high-temperature [pressure](thermodynamics.md#pressure) comparison.

### Radiation-to-gas pressure boundary

↑ **Parent:** [Stellar equation-of-state regime diagram](#stellar-equation-of-state-regime-diagram)

For a nondegenerate fully ionized gas, equating $P_{\rm gas}=\rho k_BT/(\mu_{\rm mol}m_u)$ with $P_\gamma=a_{\rm rad}T^4/3$ gives $T^3=3k_B\rho/(a_{\rm rad}\mu_{\rm mol}m_u)$. Radiation dominates at higher [temperature](thermodynamics.md#temperature) for fixed density. A degenerate [Electron](physics.md#electron) gas requires its degeneracy [pressure](thermodynamics.md#pressure) instead of extrapolating this ideal-gas formula.

### Thermal electron relativistic threshold

↑ **Parent:** [Stellar equation-of-state regime diagram](#stellar-equation-of-state-regime-diagram)

In a dilute [Electron](physics.md#electron) gas, thermal kinetic energies become relativistic near $k_BT=m_ec^2$, corresponding to $T_*\simeq5.93\times10^9\,\mathrm K$. This is a crossover in the momentum distribution, not an abrupt [temperature](thermodynamics.md#temperature) transition. Degenerate [Electrons](physics.md#electron) can instead be relativistic at much lower [temperature](thermodynamics.md#temperature) if their [Fermi momentum](statistical-physics.md#fermi-momentum) exceeds $m_ec$.

## Stellar composition profile

↑ **Parent:** [Stellar structure](stellar-structure.md)

A stellar composition profile gives chemical mass fractions against radius or [enclosed mass](#enclosed-mass). Flat portions can indicate mixing in a [convective core](#convective-core) or [convective envelope](#convective-envelope), while burning shells and moving convective boundaries leave gradients and discontinuities.

## Stellar structure equations

↑ **Parent:** [Stellar structure](stellar-structure.md)

The stellar structure equations describe spherical hydrostatic stars through radial conservation of mass, force balance, energy generation, and energy transport. An equation of state, opacity, energy-generation law, and boundary conditions close the system.

### Stellar mass conservation equation

↑ **Parent:** [Stellar structure equations](#stellar-structure-equations)

In spherical [stellar structure](stellar-structure.md), a shell of [radius](topology.md#radius) $r$, thickness $dr$ and [mass density](fluid-mechanics.md#density) $\rho$ has [mass](classical-mechanics.md#mass) $dm=4\pi r^2\rho\,dr$. Integrating outward gives the [enclosed mass](#enclosed-mass), $m(r)=4\pi\int_0^r\rho(s)s^2ds$.

## Stellar adiabatic exponent

↑ **Parent:** [Stellar structure](stellar-structure.md)

The stellar adiabatic exponents describe pressure and temperature responses to an isentropic density change:

$$
\Gamma_1=\left(\frac{\partial\log P}{\partial\log\rho}\right)_s,
\qquad
\Gamma_3-1=\left(\frac{\partial\log T}{\partial\log\rho}\right)_s,
\qquad
\frac{\Gamma_2}{\Gamma_2-1}
=\left(\frac{\partial\log P}{\partial\log T}\right)_s.
$$

### Adiabatic exponents of a monatomic gas-radiation mixture

↑ **Parent:** [Stellar adiabatic exponent](#stellar-adiabatic-exponent)

For fixed-composition monatomic [ideal gas](thermodynamics.md#ideal-gas) plus equilibrium [radiation pressure](thermodynamics.md#radiation-pressure), specific internal energy is $u=3\mathcal RT/2+a_{\rm r}T^4/\rho$. An [isentropic process](thermodynamics.md#isentropic-process) satisfies $du=P\,d\rho/\rho^2$, giving $\Gamma_3-1=(8-6\beta)/(24-21\beta)$ and

$$
\Gamma_2=\frac{32-24\beta-3\beta^2}{24-18\beta-3\beta^2},\qquad
\nabla_{\rm ad}=\frac{8-6\beta}{32-24\beta-3\beta^2}.
$$

The [stellar gas-pressure fraction](#stellar-gas-pressure-fraction) must be allowed to change along the adiabat. The pure-radiation and pure-gas limits give $\Gamma_1=\Gamma_2=4/3$ and $5/3$, respectively. Partial ionization or different gas heat capacities change these formulas.

#### Specific heats of a monatomic gas-radiation mixture

↑ **Parent:** [Adiabatic exponents of a monatomic gas-radiation mixture](#adiabatic-exponents-of-a-monatomic-gas-radiation-mixture)

For fixed-composition monatomic [ideal gas](thermodynamics.md#ideal-gas) plus equilibrium [blackbody radiation](statistical-physics.md#black-body-radiation), let $\mathcal R=k/(\mu H)$ and $\beta=P_g/P$. The mass-specific heats are $c_P=\mathcal R(32-24\beta-3\beta^2)/(2\beta^2)$ and $c_V=\mathcal R(24-21\beta)/(2\beta)$. The [specific-heat ratio](thermodynamics.md#heat-capacity-ratio) is $\Gamma_1/\beta$, not generally any one of the [stellar adiabatic exponents](#stellar-adiabatic-exponent). Differentiate at constant total pressure rather than at constant $\beta$.

## Enclosed mass

↑ **Parent:** [Stellar structure](stellar-structure.md)

For a spherically symmetric density $\rho(r)$, the mass enclosed inside radius $r$ is

$$
m(r)=4\pi\int_0^r\rho(s)s^2\,ds,
\qquad
\frac{dm}{dr}=4\pi r^2\rho(r).
$$

## Hydrostatic pressure support equation

↑ **Parent:** [Stellar structure](stellar-structure.md)

For a static spherically symmetric Newtonian star, balancing the inward gravitational force against the pressure gradient gives

$$
\frac{dP}{dr}=-\frac{Gm(r)\rho(r)}{r^2},
\qquad
\frac{dm}{dr}=4\pi r^2\rho(r).
$$

## Stellar polytrope

↑ **Parent:** [Stellar structure](stellar-structure.md)

A stellar polytrope obeys $P=K\rho^{1+1/n}$ for constant $K$ and polytropic index $n$. Its dimensionless density profile satisfies the [Lane-Emden equation](nonlinear-analysis.md#lane-emden-equation).

### Polytrope of index five

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

The regular $n=5$ [Lane-Emden equation](nonlinear-analysis.md#lane-emden-equation) solution has no finite first zero. Its [Lane-Emden mass formula](#lane-emden-mass-formula) gives $m(\xi)=4\pi\rho_c\alpha^3\xi^3/[3(1+\xi^2/3)^{3/2}]$, so its infinite-radius total [mass](classical-mechanics.md#mass) is $4\pi\sqrt3\rho_c\alpha^3$. Its enclosed mean [mass density](fluid-mechanics.md#density) is $\rho_c(1+\xi^2/3)^{-3/2}$ and tends to zero. A finite externally confined core instead requires a specified truncation pressure.

#### Luminosity integral of an index-five polytrope

↑ **Parent:** [Polytrope of index five](#polytrope-of-index-five)

For a gas-pressure-supported [polytrope of index five](#polytrope-of-index-five) with uniform [mean molecular weight](thermodynamics.md#mean-molecular-weight), $T/T_c=\theta$. A specific [stellar energy-generation rate](stellar-astrophysics.md#stellar-energy-generation-rate) $\epsilon=\epsilon_0\rho T^q$ therefore integrates to $4\pi\epsilon_0\alpha^3\rho_c^2T_c^q\int_0^\infty\xi^2\theta^{10+q}d\xi$. Substituting $u=\xi/\sqrt{3+\xi^2}$ gives the displayed formula, convergent for $q>-7$. At $q=11$ its dimensionless coefficient is approximately $1.02942$. The scale factor is a volume, $\alpha^3$, rather than an area.

### Moment of inertia of a polytropic star

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

For a spherical [stellar polytrope](#stellar-polytrope), the axial [moment of inertia](classical-mechanics.md#moment-of-inertia) is $I=(8\pi/3)\int_0^R\rho(r)r^4\,dr$. With [Lane-Emden variables for a stellar polytrope](#lane-emden-variables-for-a-stellar-polytrope), first zero $\xi_1$ and [Lane-Emden surface mass constant](#lane-emden-surface-mass-constant) $\omega_n$, its dimensionless form is

$$
\frac{I}{MR^2}=\frac{2}{3\omega_n\xi_1^2}\int_0^{\xi_1}\xi^4\theta(\xi)^n\,d\xi.
$$

A [polytrope of index zero](#polytrope-of-index-zero) gives $2/5$, while a [polytrope of index one](#polytrope-of-index-one) gives $(2/3)(1-6/\pi^2)$. The latter is smaller because more of the mass lies near the center. The scalar second mass moment $\int r^2dm$ is $3I/2$, not the axial [moment of inertia](classical-mechanics.md#moment-of-inertia).

### Polytrope of index zero

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

The regular $n=0$ solution of the [Lane-Emden equation](nonlinear-analysis.md#lane-emden-equation) is $\theta=1-\xi^2/6$, with first zero $\sqrt6$. Its interior density is constant and its pressure varies as $\theta$. This is the structural incompressible limit; $P=K\rho^{1+1/n}$ itself is singular at $n=0$, and does not assign the perturbative [stellar adiabatic exponent](#stellar-adiabatic-exponent) of a thermally stratified ideal-gas model.

### Low-density polytropic mass divergence

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

For $p=K\rho^{1+1/n}$, the [Lane-Emden mass formula](#lane-emden-mass-formula) gives $M\propto\rho_c^{(3-n)/(2n)}$ at fixed $K$, while $M/R\propto\rho_c^{1/n}$. For $3<n<5$, the [Lane-Emden equation](nonlinear-analysis.md#lane-emden-equation) has a finite-radius solution, yet $M\to\infty$ as $\rho_c\to0$. The relativistic [Tolman–Oppenheimer–Volkoff equation](general-relativity.md#tolman-oppenheimer-volkoff-equation) approaches this limit since $p_c/\rho_c\to0$. Monotone pressure and density alone therefore do not impose a finite stellar maximum mass.

### Gravitational energy of a stellar polytrope

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

For a spherical [stellar polytrope](#stellar-polytrope) of finite radius and zero surface pressure, the [specific enthalpy](thermodynamics.md#specific-enthalpy) is $(n+1)P/\rho$. [Hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) gives $h+\Phi=-GM/R$, hence $(n+1)\int P\,dV=-GM^2/R-2\Omega$. Eliminating the pressure integral with the [stellar virial theorem](#stellar-virial-theorem) proves the displayed formula. For a gas [adiabatic stellar polytrope](#adiabatic-stellar-polytrope), $n=1/(\gamma-1)$ and $U=GM^2/[(5\gamma-6)R]$; a general [polytropic index](#polytropic-index) need not have this relation to the [specific-heat ratio](thermodynamics.md#heat-capacity-ratio).

### Lane-Emden variables for a stellar polytrope

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

Writing

$$
\rho=\rho_c\theta^n,\qquad r=\alpha\xi,\qquad
\alpha^2=\frac{(n+1)K}{4\pi G}\rho_c^{(1-n)/n}
$$

reduces Newtonian hydrostatic balance to

$$
\frac1{\xi^2}\frac d{d\xi}\left(\xi^2\theta'\right)=-\theta^n,
\qquad \theta(0)=1,\quad\theta'(0)=0.
$$

The stellar surface is the first zero $\xi_1$ of $\theta$, and $R=\alpha\xi_1$.

### Polytrope of index one

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

A [stellar polytrope](#stellar-polytrope) with [polytropic index](#polytropic-index) one has $\nabla\Phi=-2K\nabla\rho$ in [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium). Combining this with the [Poisson equation for Newtonian gravity](classical-mechanics.md#poisson-equation-for-newtonian-gravity) gives the [Helmholtz equation](partial-differential-equation.md#helmholtz-equation)

$$
\nabla^2\rho+k^2\rho=0,\qquad k^2=\frac{2\pi G}{K}.
$$

The spherical solution regular at the origin is $\rho(r)=\rho_c\sin(kr)/(kr)$. Its first zero gives $R=\pi/k=\sqrt{\pi K/(2G)}$, independent of central [mass density](fluid-mechanics.md#density), and $\bar\rho/\rho_c=3/\pi^2$.

#### Cubic polytropic interior

↑ **Parent:** [Polytrope of index one](#polytrope-of-index-one)

The interior [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) for a [polytrope of index one](#polytrope-of-index-one) also admits a positive solution vanishing on the faces of a cube:

$$
\rho(x,y,z)=\rho_c\sin\frac{\pi x}{L}\sin\frac{\pi y}{L}\sin\frac{\pi z}{L},
\qquad L^2=\frac{3\pi K}{2G}.
$$

Its central value is $\rho_c$ and its average is $\bar\rho=8\rho_c/\pi^3$. Together with $\Phi=C-2K\rho$, it solves the interior [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) and [Poisson equation for Newtonian gravity](classical-mechanics.md#poisson-equation-for-newtonian-gravity). A local interior solution need not match the external field of its own mass.

##### Cubic polytrope fails isolated gravitational matching

↑ **Parent:** [Cubic polytropic interior](#cubic-polytropic-interior)

For the [cubic polytropic interior](#cubic-polytropic-interior), $\nabla\rho$ vanishes at each vertex, so the locally defined potential $\Phi=C-2K\rho$ predicts zero gravitational acceleration there. But at the vertex $(0,0,0)$, the actual self-gravitational acceleration of the positive mass distribution is

$$
\mathbf g(0)=G\int_{[0,L]^3}\rho(\mathbf r')\frac{\mathbf r'}{|\mathbf r'|^3}\,d^3r',
$$

whose three components are strictly positive. The fields cannot match continuously. Thus the interior [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) and zero density on the faces do not construct an isolated static cubic star. External stresses or an external gravitational field would be needed to realize such a boundary-value construction.

###### Corner-force obstruction for a cubic polytrope

↑ **Parent:** [Cubic polytrope fails isolated gravitational matching](#cubic-polytrope-fails-isolated-gravitational-matching)

The sine-product [cubic polytropic interior](#cubic-polytropic-interior) has zero [mass density](fluid-mechanics.md#density) gradient at every corner. Its hydrostatic potential $C-2K\rho$ therefore has zero gradient there. In contrast, at a corner of a cube containing a positive [mass density](fluid-mechanics.md#density), every interior mass element contributes a gravitational-potential gradient pointing into the same coordinate octant. Each component of the gradient is strictly nonzero. This directly proves failure of global isolated gravitational matching, even though the interior hydrostatic and Poisson equations hold.

### Eddington standard model

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eddington_standard_model)

The Eddington standard model is a chemically homogeneous $n=3$ stellar polytrope with constant gas-pressure fraction $\beta$. It approximates massive radiative stars in which gas and radiation both contribute appreciably to pressure.

### Polytropic index

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

The polytropic index $n$ is defined by $P=K\rho^{1+1/n}$. A monatomic convective ideal gas has $n=3/2$, while a radiation-supported Eddington model has $n=3$.

### Adiabatic stellar polytrope

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

An adiabatic stellar polytrope has $P=K\rho^\gamma$ with constant specific entropy, so $n=1/(\gamma-1)$. For a monatomic perfect gas, $\gamma=5/3$ and $n=3/2$.

### Polytropic mass-radius relation

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

Eliminating central density from the Lane-Emden scalings gives

$$
R\propto K^{n/(3-n)}M^{(1-n)/(3-n)}
$$

for $n\ne3$. In particular, $R\propto KM^{-1/3}$ for $n=3/2$.

With $Y_n=-\xi_1^2\theta'(\xi_1)$, the exact rearranged relation is

$$
M=A_nK^{n/(n-1)}R^{(3-n)/(1-n)},
$$

where

$$
A_n=4\pi Y_n
\left(\frac{n+1}{4\pi G}\right)^{n/(n-1)}
\xi_1^{(3-n)/(n-1)}.
$$

For $n=3$, the radius dependence disappears and the mass is proportional to $K^{3/2}$.

#### Entropy dependence of a polytropic mass-radius relation

↑ **Parent:** [Polytropic mass-radius relation](#polytropic-mass-radius-relation)

For a finite regular [polytrope](astrophysical-fluid-dynamics.md#polytrope) with fixed index, the scale $\alpha^2\propto K\rho_c^{(1-n)/n}$ implies $M^{n-1}R^{3-n}\propto K^n$. Thus, for $n\ne3$, $R\propto K^{n/(3-n)}M^{(1-n)/(3-n)}$. For $n=3/2$, $R\propto KM^{-1/3}$. Fixed composition makes the cold [electron degeneracy pressure](statistical-physics.md#electron-degeneracy-pressure) coefficient approximately fixed, but a convective [ideal gas](thermodynamics.md#ideal-gas) has $K$ controlled by [entropy](thermodynamics.md#entropy). A stellar sequence with changing entropy therefore need not follow the fixed-$K$ negative slope.

### Lane-Emden mass formula

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

If $\rho=\rho_c\theta^n$, $r=\alpha\xi$, and $\xi_1$ is the first zero of the Lane-Emden function, then a spherical polytrope has

$$
M=4\pi\alpha^3\rho_c\left[-\xi_1^2\theta'(\xi_1)\right].
$$

#### Lane-Emden surface mass constant

↑ **Parent:** [Lane-Emden mass formula](#lane-emden-mass-formula)

For a Lane-Emden function whose first zero is $\xi_1$,

$$
Y_n=-\xi_1^2\theta'(\xi_1)
=\int_0^{\xi_1}\xi^2\theta(\xi)^n\,d\xi.
$$

### Eddington quartic relation

↑ **Parent:** [Stellar polytrope](#stellar-polytrope)

For a chemically uniform $n=3$ gas-plus-radiation polytrope with constant gas-pressure fraction $\beta$, the mass obeys

$$
\frac{1-\beta}{\beta^4}\propto\mu^4M^2.
$$

It follows from the $n=3$ mass scaling $M\propto K^{3/2}$ and the equation of state.

## Stellar homology

↑ **Parent:** [Stellar structure](stellar-structure.md)

Homologous stellar models have the same dimensionless radial profiles after mass, radius, density, pressure, and temperature are scaled by characteristic values.

### Fully convective homology with tenth-power surface opacity

↑ **Parent:** [Stellar homology](#stellar-homology)

For a monatomic [ideal gas](thermodynamics.md#ideal-gas) [fully convective star](#fully-convective-star), $P=K\rho^{5/3}$ and $K\propto RM^{1/3}$. Matching its adiabat to a photosphere with $P\sim g/\kappa$ and $\kappa\propto\rho T^{10}$ gives $T_{\rm eff}^{14}\propto M^2R$, and hence surface luminosity $L\propto M^{4/7}R^{16/7}$. Specific heating $\epsilon\propto\rho T^5$ gives $L\propto M^7R^{-8}$. Equality yields the displayed laws and $T_{\rm eff}\propto M^{3/16}$, so the theoretical HR slope is $32/3$. Fixed composition, efficient convection and the surface matching approximation are essential.

### Homologous adiabatic stellar stability

↑ **Parent:** [Stellar homology](#stellar-homology)

A mass-preserving [stellar homology](#stellar-homology) with scale $x$ has [mass density](fluid-mechanics.md#density) proportional to $x^{-3}$. For an [adiabatic process](thermodynamics.md#adiabatic-process) with constant [adiabatic index](thermodynamics.md#heat-capacity-ratio) $\gamma$, its [internal energy](thermodynamics.md#internal-energy) scales as $x^{-3(\gamma-1)}$ and its [Newtonian gravitational potential energy](classical-mechanics.md#newtonian-gravitational-potential-energy) as $x^{-1}$. Writing $a=3(\gamma-1)$, stationarity at $x=1$ requires $W_0=-aU_0$, and the second scale derivative is $a(a-1)U_0$. Thus this particular displacement is restoring for $\gamma>4/3$, destabilizing for $1<\gamma<4/3$, and marginal at $\gamma=4/3$. This is a test of homologous radial stability; it does not by itself test every stellar displacement.

### Constant-opacity homologous contraction to CNO ignition

↑ **Parent:** [Stellar homology](#stellar-homology)

For radiative, gas-pressure-supported homologous stars with constant [opacity](#opacity), write $\rho=M b/(4\pi R^3)$, $P=GM^2p/(4\pi R^4)$ and $T=\mu GMp/(\mathcal R Rb)$. The [radiative diffusion in a star](#radiative-diffusion-in-a-star) equation contains the [dimensionless](physics.md#dimensionless-quantity) coefficient $D=3\kappa_0\mathcal R^4L/(64\pi^2ac\mu^4G^4M^3)$. A common fixed profile fixes $D$, so $L\propto M^3$ and the [luminosity](astrophysics.md#luminosity) of a fixed-mass member is constant. [Gravitational energy generation in a homologously contracting ideal-gas star](stellar-astrophysics.md#gravitational-energy-generation-in-a-homologously-contracting-ideal-gas-star) gives $\dot R=-2ELR^2/(3GM^2)$ for a positive profile constant $E$. Thus $R^{-1}=R_0^{-1}+2ELt/(3GM^2)$. For [CNO cycle](stellar-astrophysics.md#cno-cycle) heating $\epsilon\propto\rho T^{16}$, the [stellar nuclear fusion](stellar-astrophysics.md#stellar-nuclear-fusion) [luminosity](astrophysics.md#luminosity) scales as $M^{18}R^{-19}$. Equating this with $M^3$ gives $R_{\rm MS}\propto M^{15/19}$. Neglecting $R_0^{-1}$, the arrival time is $t_{\rm MS}\propto M^{-34/19}$, hence a coeval cluster's newly arriving [mass](classical-mechanics.md#mass) scales as $t^{-19/34}$. All comparisons hold [stellar composition](stellar-astrophysics.md#stellar-chemical-abundance), [opacity](#opacity) normalization and [dimensionless](physics.md#dimensionless-quantity) profiles fixed.

### Homology scaling of central stellar pressure

↑ **Parent:** [Stellar homology](#stellar-homology)

In [stellar homology](#stellar-homology), a fixed dimensionless density profile gives $\rho_c=C_\rho M/R^3$ through the mass integral. Integrating the [stellar hydrostatic equation](#hydrostatic-pressure-support-equation) through the same profile gives $P_c=C_PGM^2/R^4$ when surface pressure is negligible. The constants depend on the shape, rather than the mass and radius. For an [ideal gas](thermodynamics.md#ideal-gas), $T_c=(C_P/C_\rho)\mu GM/(\mathcal R R)$.

### Homologous rotating collapse

↑ **Parent:** [Stellar homology](#stellar-homology)

During a spherical [stellar homology](#stellar-homology) contraction at fixed mass and [angular momentum](classical-mechanics.md#angular-momentum), a constant inertia coefficient gives $I=\alpha MR^2$ and [solid-body rotation](classical-mechanics.md#solid-body-rotation) gives $\Omega=J/I\propto R^{-2}$. A fixed fluid label $s=r/R$ retains its enclosed mass and polar angle, so centrifugal acceleration scales as $R^{-3}$ and gravity as $R^{-2}$. Their ratio increases as $R^{-1}$. This assumes spin conservation, not continuous synchronization to an external orbit.

#### Critical rotation of a spherical cloud

↑ **Parent:** [Homologous rotating collapse](#homologous-rotating-collapse)

In the spherical approximation, equatorial centrifugal acceleration balances surface gravity when $\Omega_c^2R_c=GM/R_c^2$. For $I=\alpha MR^2$ and conserved [angular momentum](classical-mechanics.md#angular-momentum) $J$, this gives the displayed critical radius. Real rotating gas can deform, lose matter and exchange torques before a spherical model remains accurate at this limit.

### Homology relations for radiative stars

↑ **Parent:** [Stellar homology](#stellar-homology)

For chemically uniform, gas-pressure-supported stars with homologous dimensionless profiles, [mass conservation](continuum-mechanics.md#mass-conservation) and [hydrostatic pressure support equation](#hydrostatic-pressure-support-equation) give $\rho_c\propto M/R^3$ and $T_c\propto M/R$. Suppose [opacity](#opacity) scales as $\kappa\propto\rho^aT^b$ and specific nuclear energy generation as $\epsilon\propto\rho^cT^d$. Then

$$
L_{\rm nuc}\propto M^{1+c+d}R^{-3c-d},\qquad
L_{\rm rad}\propto M^{3-a-b}R^{3a+b}.
$$

The second scaling follows from [radiative diffusion in a star](#radiative-diffusion-in-a-star), $L\propto RT_c^4/(\kappa_c\rho_c)$. Equating the two gives

$$
R\propto M^{(a+b+c+d-2)/(3a+b+3c+d)}
$$

when the denominator is nonzero. Fixed composition and self-similar profiles are essential; these are relations between idealized models rather than universal stellar laws.

#### Radiative homology with density-half inverse-five-halves opacity

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For gas-pressure-supported [stellar homology](#stellar-homology) with $\kappa\propto\rho^{1/2}T^{-5/2}$ and specific nuclear heating $\epsilon\propto\rho T^5$, the central scalings give $L_{\rm nuc}\propto M^7R^{-8}$ and [radiative diffusion in a star](#radiative-diffusion-in-a-star) gives $L_{\rm rad}\propto M^5R^{-1}$. Equating them yields the displayed laws. The [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) gives $T_{\rm eff}\propto M^{29/28}$, hence $d\log L/d\log T_{\rm eff}=132/29$. Composition and dimensionless profiles are held fixed.

#### Kramers homology with a variable nuclear exponent

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For a chemically uniform, gas-pressure-supported [stellar homology](#stellar-homology) with [Kramers' opacity law](#kramers-opacity-law) and specific heating $\epsilon=\epsilon_0\rho T^\nu$, [radiative diffusion in a star](#radiative-diffusion-in-a-star) gives $L\propto\kappa_0^{-1}\mu^{15/2}M^{11/2}R^{-1/2}$. Nuclear heating gives $L\propto\epsilon_0\mu^\nu M^{\nu+2}R^{-\nu-3}$. Equating them yields $R^{\nu+5/2}\propto\epsilon_0\kappa_0\mu^{\nu-15/2}M^{\nu-7/2}$. Thus $\nu=7/2$ gives a mass-independent radius, whereas $\nu=23/2$ gives $R\propto M^{4/7}$ and $L\propto M^{73/14}$. The coefficients and dimensionless profiles must be fixed; this is an idealized radiative model rather than a universal stellar law.

#### Radiative homology with fifth-power hydrogen burning and inverse-cubic opacity

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For gas-pressure-supported [stellar homology](#stellar-homology) with [opacity](#opacity) $\kappa=\kappa_0Z\rho T^{-3}$ and [stellar energy-generation rate](stellar-astrophysics.md#stellar-energy-generation-rate) $\epsilon=\epsilon_0X^2\rho T^5$, [radiative diffusion in a star](#radiative-diffusion-in-a-star) gives $L\propto RT_c^7/(Z\rho_c^2)\propto\mu^7M^5/Z$. Integrating the heating rate instead gives $L\propto X^2\mu^5M^7/R^8$. Equality in [stellar thermal equilibrium](#stellar-thermal-equilibrium) yields the displayed [radius](topology.md#radius) law and $T_c\propto\mu^{5/4}M^{3/4}X^{-1/4}Z^{-1/8}$. This fixes the [dimensionless](physics.md#dimensionless-quantity) profiles and coefficients, and neglects [radiation pressure](thermodynamics.md#radiation-pressure); it is a model comparison rather than a universal law for all [main sequence](stellar-astrophysics.md#main-sequence) stars. At fixed [mass](classical-mechanics.md#mass) and [metal mass fraction](stellar-astrophysics.md#metal-mass-fraction), homogeneous [hydrogen burning](stellar-astrophysics.md#hydrogen-burning) gives the [homogeneous fuel-depletion luminosity feedback](#homogeneous-fuel-depletion-luminosity-feedback) through $L\propto\mu^7$.

#### Radiative homology with proton-proton burning and inverse-fourth-power opacity

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For a chemically uniform, ideal-gas-supported [stellar homology](#stellar-homology) sequence with nuclear energy generation $\epsilon=\epsilon_0X^2\rho T^4$ and [opacity](#opacity) $\kappa=\kappa_0Z(1+X)\rho T^{-4}$, [radiative diffusion in a star](#radiative-diffusion-in-a-star) fixes $L R Z(1+X)/(\mu^8M^6)$ and nuclear heating fixes $X^2\mu^4M^6/(R^7L)$. Eliminating $L$ gives $R^6\propto X^2Z(1+X)\mu^{-4}$, hence

$$
R\propto X^{1/3}[Z(1+X)]^{1/6}\mu^{-2/3},\qquad L\propto M^6\mu^{26/3}X^{-1/3}[Z(1+X)]^{-7/6}.
$$

The absence of $M$ in the radius law is a consequence of these particular power laws; it is not a universal relation for real stars. At fixed initial $X$ and $\mu$, the [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) gives $T_e\propto Z^{-1/12}$ at fixed [luminosity](astrophysics.md#luminosity).

##### Turnoff mass of a homogeneously mixed proton-proton-burning population

↑ **Parent:** [Radiative homology with proton-proton burning and inverse-fourth-power opacity](#radiative-homology-with-proton-proton-burning-and-inverse-fourth-power-opacity)

Let a fixed-mass, fully mixed stellar model evolve by [hydrogen burning](stellar-astrophysics.md#hydrogen-burning), with $L=C M^6Z^{-7/6}H(X)$ and $H(X)=\mu(X)^{26/3}X^{-1/3}(1+X)^{-7/6}$. Energy conservation gives $\dot X=-L/(ME_H)$. The time to reach $X=fX_0$ is therefore $t=(E_H/C)M^{-5}Z^{7/6}\int_{fX_0}^{X_0}H(X)^{-1}dX$. If $X_0,f$ and the function $\mu(X)$ are common to the population, the integral is constant and $M_{\mathrm{to}}\propto Z^{7/30}t^{-1/5}$. This includes the change of [luminosity](astrophysics.md#luminosity) during fuel depletion rather than replacing the luminosity by its initial value.

#### CNO homology with density-dependent inverse-cubic opacity

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For gas-pressure-supported [stellar homology](#stellar-homology) with specific nuclear heating $\epsilon=\epsilon_0\rho T^{13}$ and [opacity](#opacity) $\kappa=\kappa_0\rho T^{-3}$, the dimensionless radiative coefficient is proportional to $L\mu^{-7}M^{-5}$. The nuclear coefficient is proportional to $\mu^{13}M^{15}/(LR^{16})$. Holding both and the dimensionless profiles fixed gives the displayed scalings. The [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) then gives $T_e\propto\mu^{25/16}M^{15/16}$ and $L\propto\mu^{-4/3}T_e^{16/3}$. The coefficients, pressure regime and composition assumptions must be held as specified; these relations are not universal laws for massive stars.

#### Homogeneous fuel-depletion luminosity feedback

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For a fixed-mass fully mixed [hydrogen burning](stellar-astrophysics.md#hydrogen-burning) star with $\mu=4/(3+5X)$ whose radiative [stellar homology](#stellar-homology) gives $L\propto\mu^7$, put $s=3+5X$. The [luminosity](astrophysics.md#luminosity) is $L=L_0(s_0/s)^7$ and fuel conservation gives $M E_H\dot X=-L$. Hence $d(s^8)/dt=-40L_0s_0^7/(ME_H)$, producing the displayed feedback law. This applies both to [CNO homology with density-dependent inverse-cubic opacity](#cno-homology-with-density-dependent-inverse-cubic-opacity) and to [radiative homology with fifth-power hydrogen burning and inverse-cubic opacity](#radiative-homology-with-fifth-power-hydrogen-burning-and-inverse-cubic-opacity), at fixed [metal mass fraction](stellar-astrophysics.md#metal-mass-fraction) in the latter. Its physical domain ends at $X=0$, before the formal denominator vanishes. The idealization holds the coefficient normalizations fixed while [stellar composition](stellar-astrophysics.md#stellar-chemical-abundance) changes through the [mean molecular weight](thermodynamics.md#mean-molecular-weight) and fuel abundance.

#### Composition-dependent CNO homology

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For homologous, chemically uniform, gas-pressure-supported radiative stars with specific energy generation $\epsilon\propto X\rho T^{13}$ and composition-dependent constant [opacity](#opacity), [stellar homology](#stellar-homology) gives $L_{\mathrm{nuc}}\propto X\mu^{13}M^{15}R^{-16}$ and $L_{\mathrm{rad}}\propto\mu^4M^3/\kappa$. Equating them gives the displayed scalings. [Hydrogen](chemistry.md#hydrogen) depletion changes both [mean molecular weight](thermodynamics.md#mean-molecular-weight) and [electron-scattering opacity](#electron-scattering-opacity); holding composition fixed gives $R\propto M^{3/4}$ and $L\propto M^3$. The power-law burning approximation applies only while [hydrogen](chemistry.md#hydrogen) fuel remains.

##### Fully mixed hydrogen-burning evolutionary track

↑ **Parent:** [Composition-dependent CNO homology](#composition-dependent-cno-homology)

With negligible heavy-element contribution to the [mean molecular weight](thermodynamics.md#mean-molecular-weight), $\mu=4/(3+5X)$ and $\kappa\propto1+X$. At fixed [mass](classical-mechanics.md#mass), [composition-dependent CNO homology](#composition-dependent-cno-homology) gives $L\propto(1+X)^{-1}(3+5X)^{-4}$ and $R\propto[X(1+X)]^{1/16}(3+5X)^{-9/16}$. The [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) then gives $T_e\propto X^{-1/32}(1+X)^{-9/32}(3+5X)^{-23/32}$. From the formal $X=1$ reference, declining $X$ initially increases [luminosity](astrophysics.md#luminosity) and [effective temperature](#effective-temperature), unlike the usual redward main-sequence turn-off. A trace CNO catalyst abundance is implicit in the burning coefficient; an exactly metal-free pure-hydrogen star cannot burn through that cycle.

#### Hertzsprung-Russell slope of a stellar homology sequence

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

For a [stellar homology](#stellar-homology) sequence with $R\propto M^X$ and $L\propto M^Y$, the [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law) gives $T_{\rm eff}\propto M^{(Y-2X)/4}$. Eliminating mass gives the displayed [Hertzsprung-Russell diagram](stellar-astrophysics.md#hertzsprung-russell-diagram) slope when $Y\ne2X$. The usual horizontal axis decreases in [temperature](thermodynamics.md#temperature) toward the right, reversing the visual left-to-right sign. The relation is between logarithmic variables and depends on the specified structural assumptions.

#### Radiative homology with proton-proton burning and Kramers opacity

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

With [proton–proton chain](stellar-astrophysics.md#proton-proton-chain) energy generation $\epsilon\propto\rho T^4$ and [Kramers' opacity law](#kramers-opacity-law) $\kappa\propto\rho T^{-7/2}$, [homology relations for radiative stars](#homology-relations-for-radiative-stars) give

$$
R\propto M^{1/13},\qquad L\propto M^{71/13},\qquad
T_{\rm eff}\propto L^{69/284}.
$$

The [Hertzsprung-Russell diagram](stellar-astrophysics.md#hertzsprung-russell-diagram) relation has $d\log L/d\log T_{\rm eff}=284/69$, with [effective temperature](#effective-temperature) increasing toward the left in the usual plotting convention.

#### Radiative homology with CNO burning and electron scattering

↑ **Parent:** [Homology relations for radiative stars](#homology-relations-for-radiative-stars)

Using the idealized [CNO cycle](stellar-astrophysics.md#cno-cycle) law $\epsilon\propto\rho T^{16}$ and constant [electron-scattering opacity](#electron-scattering-opacity), [homology relations for radiative stars](#homology-relations-for-radiative-stars) give

$$
R\propto M^{15/19},\qquad L\propto M^3,\qquad T_{\rm eff}\propto L^{9/76}.
$$

These retain ideal-gas pressure support; significant [radiation pressure](thermodynamics.md#radiation-pressure) or convection changes the model.

## Surface gravity of a star

↑ **Parent:** [Stellar structure](stellar-structure.md)

The surface gravity of a spherical star of mass $M$ and radius $R$ is $g=GM/R^2$ in Newtonian gravity.

## Stellar surface boundary condition

↑ **Parent:** [Stellar structure](stellar-structure.md)

A stellar surface boundary condition matches the interior pressure and temperature to an atmospheric solution, commonly near optical depth $\tau=2/3$ where a grey atmosphere has $T=T_{\rm eff}$.

### Photosphere

↑ **Parent:** [Stellar surface boundary condition](#stellar-surface-boundary-condition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Photosphere)

The photosphere is the layer from which most observed stellar radiation escapes; in a grey atmosphere it is represented approximately by optical depth $\tau=2/3$.

#### Hydrostatic equilibrium in optical depth

↑ **Parent:** [Photosphere](#photosphere)

In a plane-parallel atmosphere with $d\tau=-\kappa\rho\,dr$ and $dP/dr=-\rho g$, one has $dP/d\tau=g/\kappa$. If gravity and opacity vary slowly, the pressure at optical depth $\tau$ is approximately $P\simeq g\tau/\kappa$.

##### Grey-atmosphere convection onset with eighth-power temperature opacity

↑ **Parent:** [Hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth)

Take an [ideal gas](thermodynamics.md#ideal-gas) [grey atmosphere](astrophysics.md#grey-atmosphere) with $T^4=T_e^4(3\tau+2)/4$, constant [surface gravity of a star](#surface-gravity-of-a-star) $g$, vanishing external pressure and $\kappa=\kappa_0P^{1/2}T^8$. Integrating [hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth) gives $P^{3/2}=8g[1/2-(3\tau+2)^{-1}]/(\kappa_0T_e^8)$. Its logarithmic temperature-pressure gradient is $9\tau/16$, so the [Schwarzschild criterion](#schwarzschild-criterion) for a monatomic gas is crossed at $\tau_c=32/45$. The radiative continuation beyond that depth is unstable and must be replaced by convective transport.

##### Grey-atmosphere pressure with power-law opacity

↑ **Parent:** [Hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth)

In a [grey atmosphere](astrophysics.md#grey-atmosphere) with $T^4=T_0^4(1+3\tau/2)$ and $\kappa=\kappa_0P^{\alpha-1}T^{4-4\beta}$, [hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth) gives $dP/d\tau=g/\kappa$. With $\alpha,\beta>0$ and $P(0)=0$, integration gives the displayed pressure-temperature relation. At the matching surface $T=T_e$, the [Eddington surface boundary condition](astrophysics.md#eddington-surface-boundary-condition) gives $T_e^4=2T_0^4$, hence $P\kappa/g=4\alpha(1-2^{-\beta})/(3\beta)$.

###### Surface boundary condition for a power-law-opacity grey atmosphere

↑ **Parent:** [Grey-atmosphere pressure with power-law opacity](#grey-atmosphere-pressure-with-power-law-opacity)

For a [plane-parallel atmosphere](astrophysics.md#plane-parallel-atmosphere) in [radiative equilibrium](thermodynamics.md#radiative-equilibrium), constant [surface gravity of a star](#surface-gravity-of-a-star) $g$ and [opacity](#opacity) $\kappa=\kappa_0P^{\alpha-1}T^{4-4\beta}$, match the [stellar structure](stellar-structure.md) interior where the [radiative flux](astrophysics.md#radiative-flux) satisfies $F=\sigma T^4$. The [grey atmosphere](astrophysics.md#grey-atmosphere) law then puts the surface at [optical depth](astrophysics.md#optical-depth) $\tau=2/3$ with $T^4=2T_0^4$. Integrating [hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth) from $P(0)=0$ gives $P^\alpha=2\alpha g(T^{4\beta}-T_0^{4\beta})/(3\beta\kappa_0T_0^4)$. Multiplication by $\kappa_0T^{4-4\beta}/g$ proves the displayed boundary condition for $\alpha>0$, $\beta\ne0$. At $\beta=0$ the integral is logarithmic and the continuous [limit](calculus.md#limit-of-a-function) is $P\kappa/g=4\alpha\log2/3$. The relation assumes negligible [radiation pressure](thermodynamics.md#radiation-pressure) and describes the [Eddington closure approximation](astrophysics.md#eddington-closure-approximation), rather than exact angular transfer.

###### Grey-atmosphere convection onset with density-linear opacity

↑ **Parent:** [Grey-atmosphere pressure with power-law opacity](#grey-atmosphere-pressure-with-power-law-opacity)

Assume an ideal-gas [grey atmosphere](astrophysics.md#grey-atmosphere) with $P(0)=0$, constant [surface gravity of a star](#surface-gravity-of-a-star) $g$, $T^4=T_e^4(1+3\tau/2)/2$ and $\kappa=\kappa_0\rho T^{4\beta+1}$ for $\beta>1$. Using $\rho=\mu P/(\mathcal RT)$ in $dP/d\tau=g/\kappa$ and integrating gives

$$
P^2=\frac{2^{\beta+2}\mathcal Rg}{3\kappa_0(\beta-1)\mu T_e^{4\beta}}\left[1-(1+3\tau/2)^{1-\beta}\right].
$$

Differentiation yields $d\log T/d\log P=[(1+3\tau/2)^{\beta-1}-1]/[2(\beta-1)]$. Applying the [Schwarzschild criterion](#schwarzschild-criterion) with monatomic adiabatic gradient $2/5$ gives $\tau_b=\frac23[((4\beta+1)/5)^{1/(\beta-1)}-1]$. Since $\tau_b$ depends only on $\beta$, matching to $P=K T^{5/2}$ fixes $K\propto g^{1/2}T_e^{-2\beta-5/2}$.

###### Grey-atmosphere convection onset with seventeenth-power opacity

↑ **Parent:** [Grey-atmosphere pressure with power-law opacity](#grey-atmosphere-pressure-with-power-law-opacity)

For a [grey atmosphere](astrophysics.md#grey-atmosphere) with $T^4=T_e^4(2+3\tau)/4$, an [ideal gas](thermodynamics.md#ideal-gas) and $\kappa=\kappa_0\rho T^{17}$, [hydrostatic equilibrium in optical depth](#hydrostatic-equilibrium-in-optical-depth) integrates to $P^2=512\mathcal Rg[1/8-(2+3\tau)^{-3}]/(9\mu\kappa_0T_e^{16})$, taking $P(0)=0$. The logarithmic radiative gradient is $[(2+3\tau)^3-8]/48$. Equating it to the monatomic [adiabatic temperature gradient](exoplanet.md#adiabatic-temperature-gradient) $2/5$ gives $(2+3\tau_b)^3=136/5$ and the displayed onset temperature. Beyond this point the radiative profile must be replaced by convective transport.

## Stellar virial theorem

↑ **Parent:** [Stellar structure](stellar-structure.md)

For a self-gravitating fluid star with surface pressure $P_s$, volume $V$, kinetic energy $T$, gravitational energy $\Omega$, and $I=\int r^2dm$,

$$
\frac12\ddot I=2T+3\int P\,dV-3P_sV+\Omega.
$$

## Stellar convective stability

↑ **Parent:** [Stellar structure](stellar-structure.md)

Stellar convective stability compares the density of an adiabatically displaced fluid element with its new surroundings. Temperature and composition gradients determine whether buoyancy restores the element or amplifies its displacement.

### Grey-atmosphere convection onset with thirteenth-power opacity

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

In a thin ideal-gas [grey atmosphere](astrophysics.md#grey-atmosphere) with $T^4=T_e^4(1/2+3\tau/4)$, constant enclosed [mass](classical-mechanics.md#mass) $M$ and [luminosity](astrophysics.md#luminosity) $L$, and $\kappa=\kappa_0\rho T^{13}$, divide the [stellar hydrostatic equation](#hydrostatic-pressure-support-equation) by [radiative diffusion in a star](#radiative-diffusion-in-a-star). This gives $P\,dP/dT=16\pi acGM\mathcal R\,T^{-9}/(3\kappa_0L\mu)$. Integrating from $P=0$, $T^4=T_e^4/2$, yields

$$
P^2=\frac{4\pi acGM\mathcal R}{3\kappa_0L\mu T_e^8}\left(4-\frac{T_e^8}{T^8}\right).
$$

[Logarithmic derivative](analytic-number-theory.md#logarithmic-derivative) gives $\nabla=T^8/T_e^8-1/4$. For a [monatomic gas](thermodynamics.md#monatomic-gas) gas, the [Schwarzschild criterion](#schwarzschild-criterion) reaches equality at $\nabla=2/5$, hence $T/T_e=(13/20)^{1/8}$. The purely radiative profile cannot be continued past this point as a convectively stable model.

### Stellar convective instability

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

Stellar convective instability occurs when an [adiabatic process](thermodynamics.md#adiabatic-process) displaces a fluid element and [buoyancy](fluid-mechanics.md#buoyancy) amplifies the displacement. For uniform composition the [Schwarzschild criterion](#schwarzschild-criterion) gives instability when the actual [temperature gradient](thermodynamics.md#temperature-gradient) exceeds the [adiabatic temperature gradient](exoplanet.md#adiabatic-temperature-gradient); composition gradients instead require the [Ledoux criterion](#ledoux-criterion).

#### Convective instability of a uniform-density star

↑ **Parent:** [Stellar convective instability](#stellar-convective-instability)

A uniform-density perfect-gas sphere supported by decreasing pressure has [buoyancy frequency](gravity-wave.md#buoyancy-frequency) squared $N^2=-2\omega_d^2r^2/[\gamma(R^2-r^2)]$ in the interior. Its [specific entropy](thermodynamics.md#specific-entropy) decreases outward and adiabatic displacements are buoyantly unstable. For the nonradial polynomial family, the product of the two normalized squared mode frequencies is $-l(l+1)$, displaying one growing branch even when radial compression modes are stable.

### Schwarzschild criterion

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schwarzschild_criterion)

For uniform composition, a stellar layer is convectively stable when $\nabla<\nabla_{\rm ad}$ and unstable when $\nabla>\nabla_{\rm ad}$, where $\nabla=d\log T/d\log P$.

### Ledoux criterion

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ledoux_criterion)

With a composition gradient, stability requires

$$
\nabla<\nabla_{\rm ad}+\frac{\phi}{\delta}\nabla_\mu.
$$

A mean molecular weight increasing inward normally provides an additional stabilizing term.

### Convection onset in a logarithmic-pressure grey atmosphere

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

For a [grey atmosphere](astrophysics.md#grey-atmosphere) with $T^4=\tfrac34T_{\rm eff}^4(\tau+2/3)$ and $P^2=P_0^2\log(1+3\tau/2)$, logarithmic differentiation gives

$$
\nabla_{\rm rad}=\frac{d\log T}{d\log P}=\frac12\log(1+3\tau/2).
$$

A monatomic [perfect gas](thermodynamics.md#ideal-gas) of uniform composition has [adiabatic temperature gradient](exoplanet.md#adiabatic-temperature-gradient) $2/5$. The [Schwarzschild criterion](#schwarzschild-criterion) therefore predicts the first marginally unstable layer at $\tau_c=\tfrac23(e^{4/5}-1)$, and convection for larger [optical depth](astrophysics.md#optical-depth). Beyond that onset, the assumed purely radiative profile is no longer a self-consistent transport solution.

### Convective core

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

A convective core is a central stellar region in which the radiative temperature gradient exceeds the adiabatic threshold. Efficient convection makes its entropy nearly uniform and mixes its composition.

#### Eddington-model convective-core mass fraction

↑ **Parent:** [Convective core](#convective-core)

The global Eddington closure $L=(1-\beta)4\pi cGM/\kappa$, combined with a representative [stellar gas-pressure fraction](#stellar-gas-pressure-fraction), makes the exterior [stellar radiative temperature gradient](#stellar-radiative-temperature-gradient) approximately $M/(4m)$ when the [luminosity](astrophysics.md#luminosity) is constant outside the core. Matching it to the [adiabatic temperature gradient](exoplanet.md#adiabatic-temperature-gradient) estimates the displayed boundary mass. This is a closure estimate: imposing exactly uniform $\beta$ throughout a finite-mass radiative envelope also conflicts with constant [luminosity](astrophysics.md#luminosity), as described by the [constant-beta radiative-envelope obstruction](#uniform-gas-pressure-fraction-and-constant-luminosity-radiative-envelope-incompatibility).

### Convective envelope

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

A convective envelope is an outer stellar region in which [convection](fluid-mechanics.md#convection) carries a substantial fraction of the energy and mixes material. Its nearly adiabatic response to rapid mass loss is important for the [dynamical stability of binary mass transfer](stellar-astrophysics.md#dynamical-stability-of-binary-mass-transfer).

### Radiative envelope

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

A radiative envelope transports most of its energy by [radiative diffusion](astrophysics.md#radiative-diffusion). Its stratified entropy profile gives a different rapid mass-loss response from a [convective envelope](#convective-envelope).

#### Kramers radiative-zero envelope around a stellar core

↑ **Parent:** [Radiative envelope](#radiative-envelope)

For a negligible-mass ideal-gas envelope above a core of [mass](classical-mechanics.md#mass) $M_c$, with constant [luminosity](astrophysics.md#luminosity) $L$ and [Kramers' opacity law](#kramers-opacity-law), division of [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) by radiative diffusion gives $P\,dP/dT=16\pi acGM_c\mathcal R\,T^{15/2}/(3\kappa_0L\mu)$. Taking the outer [pressure](thermodynamics.md#pressure) constant to be negligible yields $P=CT^{17/4}$, where $C^2=64\pi acGM_c\mathcal R/(51\kappa_0L\mu)$, and $\rho=(\mu C/\mathcal R)T^{13/4}$. [Hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) then gives $dT/dr=-4\mu GM_c/(17\mathcal Rr^2)$, so $T=B/r+T_0$ with $B=4\mu GM_c/(17\mathcal R)$. The radiative-zero choice $T_0=0$ is exact for a vanishing-temperature boundary at infinity and a deep-envelope approximation for a very extended finite star. It is not implied by small surface [temperature](thermodynamics.md#temperature) alone at a specified finite [radius](topology.md#radius).

#### Self-gravitating Kramers power-law envelope

↑ **Parent:** [Radiative envelope](#radiative-envelope)

For a constant-luminosity [radiative envelope](#radiative-envelope) with ideal-gas [pressure](thermodynamics.md#pressure) and [Kramers' opacity law](#kramers-opacity-law), impose [power laws](analysis.md#power-law) on [enclosed mass](#enclosed-mass), density, [pressure](thermodynamics.md#pressure) and [temperature](thermodynamics.md#temperature) while retaining $M_r'=4\pi r^2\rho$. If their exponents are $m,b,p,d$, respectively, mass conservation gives $m=b+3$, hydrostatic balance gives $d=m-1$, the gas law gives $d=p-b$, and diffusion gives $d-1=2b-2-13d/2$. Solving gives $(m,b,p,d)=(1,-32,-42,-10)/11$. In particular $R/r_c=(T_c/T_R)^{11/10}$. Neglecting envelope self-gravity instead sets $M_r$ approximately constant and changes the exponents to $d=-1,b=-13/4,p=-17/4$; that approximation is not an exact solution of mass conservation with nonzero density.

#### Power-law opacity radiative envelope

↑ **Parent:** [Radiative envelope](#radiative-envelope)

A thin [radiative envelope](#radiative-envelope) with constant enclosed mass, luminosity and [mean molecular weight](thermodynamics.md#mean-molecular-weight), [ideal gas](thermodynamics.md#ideal-gas) pressure and opacity $\kappa=\kappa_0\rho^nT^{-s}$ has $a=n+1$, $b=n+s+4$, and $C=16\pi a_{\rm rad}cGM/[3\kappa_0(\mu m_u/k_B)^nL]$. Combining [radiative diffusion in a star](#radiative-diffusion-in-a-star) with [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) gives $\nabla_{\rm rad}=P^a/(CT^b)$, so $P^a-P_0^a=(aC/b)(T^b-T_0^b)$ for nonzero exponents. Zero exponents give logarithmic limits. The model must be stopped or modified if the [Schwarzschild criterion](#schwarzschild-criterion) predicts [convection](fluid-mechanics.md#convection).

##### Radiative-envelope convection matching

↑ **Parent:** [Power-law opacity radiative envelope](#power-law-opacity-radiative-envelope)

For $P=C(T^b+K)^{1/p}$ with $p=n+1$ and $b=4+n+m$, the logarithmic radiative [temperature](thermodynamics.md#temperature) gradient is $(p/b)(1+K/T^b)$. At a marginal boundary with an efficient ideal-gas [convective envelope](#convective-envelope), the [Schwarzschild criterion](#schwarzschild-criterion) equates it to $(\gamma-1)/\gamma$. Hence $K=T_b^b[(b/p)(\gamma-1)/\gamma-1]$. The notation $K=T_0^b$ with real positive $T_0$ requires a nonnegative bracket. Vanishing $p$ or $b$ needs the corresponding logarithmic integration instead of this power form.

###### Deep radiative boundary beneath a power-law-opacity convective envelope

↑ **Parent:** [Radiative-envelope convection matching](#radiative-envelope-convection-matching)

In a negligible-mass, non-burning stellar envelope with $P=KT^{5/2}$ and [Kramers' opacity law](#kramers-opacity-law) $\kappa=\kappa_1\rho T^{-7/2}$, the [stellar radiative temperature gradient](#stellar-radiative-temperature-gradient) is $\nabla_{\mathrm{rad}}=3\kappa_1\mu K^2L/(16\pi ac\mathcal RGM T^{7/2})$. It decreases inward as the temperature rises, so the inner edge of efficient [convection](fluid-mechanics.md#convection) is where it equals $2/5$. If outer matching gives $K\propto g^{1/2}T_e^{-2\beta-5/2}$, then $T_b^{7/2}\propto K^2L/M\propto T_e^{-4\beta-1}$, since $g=GM/R^2$ and $L=4\pi R^2\sigma T_e^4$. Hence $T_b\propto T_e^{-(8\beta+2)/7}$.

### Fully convective star

↑ **Parent:** [Stellar convective stability](#stellar-convective-stability)

A fully convective star has [convection](fluid-mechanics.md#convection) throughout nearly its entire interior. Very low-mass [red dwarfs](stellar-astrophysics.md#red-dwarf) are fully convective; the transition to this structure is used in the [disrupted magnetic braking model](stellar-astrophysics.md#disrupted-magnetic-braking-model).

## Radiative stellar structure

↑ **Parent:** [Stellar structure](stellar-structure.md)

In a radiative stellar region, photons carry luminosity down the temperature gradient. Dimensional scaling of the radiative-diffusion equation gives $L\sim RT_c^4/(\kappa_c\rho_c)$.

### Radiative core

↑ **Parent:** [Radiative stellar structure](#radiative-stellar-structure)

A stellar core in which [radiative diffusion in a star](#radiative-diffusion-in-a-star) carries most of the energy, rather than [convection](fluid-mechanics.md#convection). Its formation in a [pre-main-sequence star](stellar-astrophysics.md#pre-main-sequence-star) breaks the fully convective assumption behind an idealized [Hayashi track](stellar-astrophysics.md#hayashi-track).

### Stellar radiative temperature gradient

↑ **Parent:** [Radiative stellar structure](#radiative-stellar-structure)

The [radiative temperature gradient](exoplanet.md#radiative-temperature-gradient) needed to carry a spherical stellar [luminosity](astrophysics.md#luminosity) follows by dividing [radiative diffusion in a star](#radiative-diffusion-in-a-star) by the [hydrostatic pressure support equation](#hydrostatic-pressure-support-equation). It is a logarithmic [pressure](thermodynamics.md#pressure) gradient, not $dT/dr$ itself. Comparing it with the [adiabatic temperature gradient](exoplanet.md#adiabatic-temperature-gradient) by the [Schwarzschild criterion](#schwarzschild-criterion) determines whether purely radiative transport is locally unstable at uniform composition.

### Opacity

↑ **Parent:** [Radiative stellar structure](#radiative-stellar-structure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Opacity)

Opacity is an extinction cross-section per unit mass. It controls the photon mean free path and therefore the radiative temperature gradient in an optically thick star.

#### Negative hydrogen ion opacity

↑ **Parent:** [Opacity](#opacity)

The [negative hydrogen ion](chemistry.md#hydrogen-anion) supplies important continuum [opacity](#opacity) in cool hydrogen-rich stellar atmospheres. A useful local approximate law is $\kappa=\kappa_0\rho^{1/2}T^9$; it is not valid over arbitrary temperatures and compositions. In an [ideal gas](thermodynamics.md#ideal-gas) [power-law opacity radiative envelope](#power-law-opacity-radiative-envelope) matched to $\nabla_{\rm phot}=1/8$, it gives $\nabla_{\rm rad}=-1/3+(11/24)(T/T_{\rm eff})^{9/2}$, rising rapidly toward [convective instability](#stellar-convective-instability).

##### Negative-hydrogen-opacity alpha-disk thickness scaling

↑ **Parent:** [Negative hydrogen ion opacity](#negative-hydrogen-ion-opacity)

Let $\mathcal R=k_B/(\mu_m m_p)$ for constant [mean molecular weight](thermodynamics.md#mean-molecular-weight) $\mu_m$ in proton-mass units, and let $\sigma$ be the Stefan–Boltzmann constant in the [Stefan–Boltzmann law](thermodynamics.md#stefan-boltzmann-law). The gas [sound speed](compressible-flow.md#speed-of-sound) used here satisfies $c_s^2=\mathcal R T$, and $\Omega$ is the local orbital frequency. For the local [opacity](#opacity) approximation $\kappa=\kappa_0\rho^{1/3}T^{10}$, a gas-supported [optically thick](astrophysics.md#optically-thick-medium) [alpha disk](astrophysics.md#alpha-disk) has $\rho\sim\Sigma/H$ and $\mathcal R T\sim\Omega^2H^2$. Integrated viscous heating is $F_+\sim\alpha\Sigma\Omega^3H^2$. [Radiative diffusion](astrophysics.md#radiative-diffusion) gives $F_-\sim(\sigma/\kappa_0)T^{-6}\Sigma^{-4/3}H^{1/3}\sim(\sigma/\kappa_0)\mathcal R^6\Omega^{-12}\Sigma^{-4/3}H^{-35/3}$. Equating the fluxes proves the thickness scaling. At fixed composition and $\alpha$, it gives $H/r\propto r^{53/82}\Sigma^{-7/41}$ and $c_s\propto r^{6/41}\Sigma^{-7/41}$ in [Keplerian rotation](astrophysics.md#keplerian-disk). Radial powers therefore require a surface-density profile; they are not determined by [opacity](#opacity) alone. The formula is local to the stated [opacity](#opacity) regime and small [disk aspect ratio](astrophysics.md#disk-aspect-ratio).

#### Kramers' opacity law

↑ **Parent:** [Opacity](#opacity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kramers'_opacity_law)

The Kramers opacity law has $\kappa=\kappa_0\rho T^{-7/2}$ for bound-free and free-free absorption under its idealized ionized-gas assumptions.

#### Electron-scattering opacity

↑ **Parent:** [Opacity](#opacity)

Electron-scattering opacity is approximately independent of density and temperature in a fully ionized nonrelativistic plasma of fixed composition. For hydrogen mass fraction $X$, $\kappa_{\rm es}\simeq0.2(1+X)\,{\rm cm^2\,g^{-1}}$.

#### Free-free opacity

↑ **Parent:** [Opacity](#opacity)

Free-free opacity is absorption caused when a photon is absorbed during a Coulomb encounter between an electron and an ion. In the Kramers approximation its Rosseland mean scales approximately as $\kappa_{\rm ff}\propto\rho T^{-7/2}$.

### Radiative diffusion in a star

↑ **Parent:** [Radiative stellar structure](#radiative-stellar-structure)

In an optically thick stellar region, radiative diffusion carries luminosity according to

$$
\frac{dT}{dr}=-\frac{3\kappa\rho L_r}{16\pi a_{\rm rad}c r^2T^3}.
$$

#### Radiative conductivity

↑ **Parent:** [Radiative diffusion in a star](#radiative-diffusion-in-a-star)

In the optically thick [radiative diffusion in a star](#radiative-diffusion-in-a-star) approximation, the heat flux is $\mathbf F=-\chi\nabla T$. The conductivity depends on [opacity](#opacity), [mass density](fluid-mechanics.md#density) and [temperature](thermodynamics.md#temperature). It relates a material temperature gradient to energy transport and must not be confused with the emergent [effective temperature](#effective-temperature).

## Effective temperature

↑ **Parent:** [Stellar structure](stellar-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Effective_temperature)

The effective temperature is the temperature of a blackbody with the same radiative flux as a star: $L=4\pi R^2\sigma T_{\rm eff}^4$.

## Mass-luminosity relation

↑ **Parent:** [Stellar structure](stellar-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass-luminosity_relation)

The mass-luminosity relation connects a star's mass to its luminosity. Its slope depends on opacity, nuclear burning, pressure support, composition, and evolutionary state.

### Eddington luminosity

↑ **Parent:** [Mass-luminosity relation](#mass-luminosity-relation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eddington_luminosity)

Balancing outward radiative acceleration against gravity gives

$$
L_{\rm Edd}=\frac{4\pi cGM}{\kappa}.
$$

It is an approximate upper luminosity for a hydrostatic star of opacity $\kappa$.

#### Stellar electron-scattering Eddington factor

↑ **Parent:** [Eddington luminosity](#eddington-luminosity)

This factor is the ratio of acceleration due to [electron-scattering opacity](#electron-scattering-opacity) to gravitational acceleration in a spherical luminous star. The remaining effective gravity is approximately $GM(1-\Gamma_e)/R^2$ when other radiative forces are neglected. Being below the electron-scattering limit does not preclude a line-driven [stellar wind](stellar-astrophysics.md#stellar-wind), because additional [opacity](#opacity) can provide more acceleration.

#### Dust-grain Eddington limit

↑ **Parent:** [Eddington luminosity](#eddington-luminosity)

An isolated compact dust grain of radius $r_d$ and material density $\rho_d$ has opacity per unit dust mass $\kappa_d=3Q_{\rm pr}/(4\rho_dr_d)$, where $Q_{\rm pr}$ is its [radiation-pressure efficiency](planetary-science.md#radiation-pressure-efficiency). Its [Eddington luminosity](#eddington-luminosity) is $4\pi GMc/\kappa_d$. Matching the [electron-scattering opacity](#electron-scattering-opacity) gives $r_{d,\rm crit}=3Q_{\rm pr}/(4\rho_d\kappa_{\rm es})$, approximately $1.9\,\mathrm{cm}$ for $Q_{\rm pr}=1$, $\rho_d=1\,\mathrm{g\,cm^{-3}}$, and $\kappa_{\rm es}=0.4\,\mathrm{cm^2\,g^{-1}}$. At that electron-scattering luminosity, smaller grains feel a net outward force and larger grains remain attracted. This is an isolated-grain force balance, not the opacity of an arbitrary gas-dust mixture.

#### Radiative force multiplier

↑ **Parent:** [Eddington luminosity](#eddington-luminosity)

A radiative force multiplier is the ratio of total radiative acceleration to a reference electron-scattering acceleration. Spectral lines, bound-free absorption, and dust can make $\mathcal M\gg1$, whereas highly ionized gas approaches $\mathcal M=1$.

## ↑ Ancestors (5)

1. [Stellar astrophysics](stellar-astrophysics.md)
2. [Astrophysics](astrophysics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-37.md#4/solution)
- [Stellar atmosphere](stellar-astrophysics.md#stellar-atmosphere)
- [Stellar mass conservation equation](#stellar-mass-conservation-equation)
- [Stellar thermal equilibrium](#stellar-thermal-equilibrium)
- [Surface boundary condition for a power-law-opacity grey atmosphere](#surface-boundary-condition-for-a-power-law-opacity-grey-atmosphere)
