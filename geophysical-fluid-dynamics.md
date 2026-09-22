# Geophysical fluid dynamics

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geophysical_fluid_dynamics)

Geophysical fluid dynamics studies fluid motion on rotating, stratified planets, including oceans, atmospheres, cores, and planetary interiors.

**Table of contents**

- [Ekman number](#ekman-number)
- [Deacon cell](#deacon-cell)
  - [Eddy-induced overturning](#eddy-induced-overturning)
  - [Meridional overturning streamfunction](#meridional-overturning-streamfunction)
- [Deformation radius](#deformation-radius)
  - [Two-layer internal deformation radius](#two-layer-internal-deformation-radius)
- [Burger number](#burger-number)
- [General circulation model](#general-circulation-model)
- [Eulerian mean flow](#eulerian-mean-flow)
- [Thermal wind](#thermal-wind)
  - [Geostrophic thermal wind with separable buoyancy](#geostrophic-thermal-wind-with-separable-buoyancy)
- [Log-pressure coordinate](#log-pressure-coordinate)
- [Rossby number](#rossby-number)
  - [Stellar activity Rossby number](#stellar-activity-rossby-number)
- [Burgers number](#burgers-number)
- [Boussinesq approximation](#boussinesq-approximation)
  - [Strong Boussinesq approximation](#strong-boussinesq-approximation)
  - [Stratification–rotation analogy](#stratification-rotation-analogy)
    - [Causal pressure adjustment by internal waves](#causal-pressure-adjustment-by-internal-waves)
      - [Hydrostatic response to a localized horizontal force](#hydrostatic-response-to-a-localized-horizontal-force)
  - [Boussinesq up-down symmetry](#boussinesq-up-down-symmetry)
  - [Boussinesq equations](#boussinesq-equations)
    - [Linearized Boussinesq equations](#linearized-boussinesq-equations)
  - [Inertial wave](#inertial-wave)
    - [Inertial modes in a rigid rotating sphere](#inertial-modes-in-a-rigid-rotating-sphere)
      - [Cubic axisymmetric inertial mode of a rigid sphere](#cubic-axisymmetric-inertial-mode-of-a-rigid-sphere)
- [Rotating fluid](#rotating-fluid)
  - [Taylor–Proudman theorem](#taylor-proudman-theorem)
    - [Geostrophic contour](#geostrophic-contour)
  - [Taylor number](#taylor-number)
  - [Traditional approximation (geophysical fluid dynamics)](#traditional-approximation-geophysical-fluid-dynamics)
  - [Coriolis parameter](#coriolis-parameter)
    - [f-plane](#f-plane)
    - [beta plane](#beta-plane)
    - [Inertial oscillation](#inertial-oscillation)
      - [Beta drift of an inertial oscillation](#beta-drift-of-an-inertial-oscillation)
- [Potential vorticity](#potential-vorticity)
  - [Potential-vorticity inversion](#potential-vorticity-inversion)
    - [Two-dimensional potential-vorticity inversion](#two-dimensional-potential-vorticity-inversion)
    - [Shallow-water quasi-geostrophic inversion](#shallow-water-quasi-geostrophic-inversion)
    - [Stratified quasi-geostrophic inversion](#stratified-quasi-geostrophic-inversion)
      - [Prandtl ratio of scales](#prandtl-ratio-of-scales)
      - [Stretched coordinates for quasi-geostrophic inversion](#stretched-coordinates-for-quasi-geostrophic-inversion)
        - [Spherical potential-vorticity anomaly](#spherical-potential-vorticity-anomaly)
  - [Potential-vorticity gradient](#potential-vorticity-gradient)
  - [Potential-vorticity evolution equation](#potential-vorticity-evolution-equation)
    - [Potential-vorticity conservation](#potential-vorticity-conservation)
      - [Momentum loss from uniform potential-vorticity mixing](#momentum-loss-from-uniform-potential-vorticity-mixing)
        - [Rossby-wave PV mixing and zonal momentum](#rossby-wave-pv-mixing-and-zonal-momentum)
  - [Ertel potential vorticity](#ertel-potential-vorticity)
    - [Ertel's theorem](#ertel-s-theorem)
  - [Shallow-water potential vorticity](#shallow-water-potential-vorticity)
    - [Circular topographic anticyclone](#circular-topographic-anticyclone)
      - [Closed-streamline threshold for a circular topographic anticyclone](#closed-streamline-threshold-for-a-circular-topographic-anticyclone)
    - [Zero-potential-vorticity rotating channel flow](#zero-potential-vorticity-rotating-channel-flow)
      - [Hydraulic control of a zero-PV rotating channel](#hydraulic-control-of-a-zero-pv-rotating-channel)
    - [Linearized shallow-water potential-vorticity anomaly](#linearized-shallow-water-potential-vorticity-anomaly)
    - [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)
      - [Cosine-ridge shallow-water geostrophic response](#cosine-ridge-shallow-water-geostrophic-response)
      - [Uniform-current obstruction to constant shallow-water QG potential vorticity](#uniform-current-obstruction-to-constant-shallow-water-qg-potential-vorticity)
        - [Gaussian topographic response with compensated uniform potential vorticity](#gaussian-topographic-response-with-compensated-uniform-potential-vorticity)
          - [Closed-streamline threshold for a Gaussian disturbance in uniform flow](#closed-streamline-threshold-for-a-gaussian-disturbance-in-uniform-flow)
      - [Potential-vorticity mixing over a finite bottom slope](#potential-vorticity-mixing-over-a-finite-bottom-slope)
      - [Potential-vorticity step edge wave](#potential-vorticity-step-edge-wave)
      - [Barotropic deformation radius](#barotropic-deformation-radius)
- [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)
  - [Two-layer quasi-geostrophic potential vorticity](#two-layer-quasi-geostrophic-potential-vorticity)
    - [Two-layer quasi-geostrophic energy conservation](#two-layer-quasi-geostrophic-energy-conservation)
      - [Baroclinic energy ratio and deformation scale](#baroclinic-energy-ratio-and-deformation-scale)
    - [Vortex stretching in layered quasi-geostrophic flow](#vortex-stretching-in-layered-quasi-geostrophic-flow)
  - [Quasi-geostrophic omega equation](#quasi-geostrophic-omega-equation)
  - [Quasi-geostrophic streamfunction](#quasi-geostrophic-streamfunction)
  - [Geostrophic flow](#geostrophic-flow)
    - [Strict geostrophic balance](#strict-geostrophic-balance)
  - [Ageostrophic flow](#ageostrophic-flow)
  - [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)
    - [Reference-buoyancy convention in quasi-geostrophic potential vorticity](#reference-buoyancy-convention-in-quasi-geostrophic-potential-vorticity)
    - [Quasi-geostrophic vertical mode](#quasi-geostrophic-vertical-mode)
      - [Barotropic mode](#barotropic-mode)
      - [Baroclinic mode](#baroclinic-mode)
    - [Quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation)
      - [Topographic buoyancy boundary condition for quasi-geostrophic flow](#topographic-buoyancy-boundary-condition-for-quasi-geostrophic-flow)
      - [Rigid-boundary buoyancy condition for quasi-geostrophic waves](#rigid-boundary-buoyancy-condition-for-quasi-geostrophic-waves)
      - [Diabatically forced quasi-geostrophic potential vorticity](#diabatically-forced-quasi-geostrophic-potential-vorticity)
        - [Harmonic heating response of quasi-geostrophic flow](#harmonic-heating-response-of-quasi-geostrophic-flow)
        - [Steady quasi-geostrophic response to localized heating](#steady-quasi-geostrophic-response-to-localized-heating)
    - [Log-pressure quasi-geostrophic potential vorticity](#log-pressure-quasi-geostrophic-potential-vorticity)
      - [Vertical-advection consistency criterion for log-pressure quasi-geostrophy](#vertical-advection-consistency-criterion-for-log-pressure-quasi-geostrophy)
    - [Isopycnal displacement](#isopycnal-displacement)
    - [Quasi-geostrophic mountain wave](#quasi-geostrophic-mountain-wave)
      - [Resonant topographic quasi-geostrophic wave](#resonant-topographic-quasi-geostrophic-wave)
        - [Phase of a resonantly forced topographic edge wave](#phase-of-a-resonantly-forced-topographic-edge-wave)
      - [Thermally damped quasi-geostrophic mountain wave](#thermally-damped-quasi-geostrophic-mountain-wave)
- [Geostrophic adjustment](#geostrophic-adjustment)
  - [Geostrophic adjustment of a Gaussian height ridge](#geostrophic-adjustment-of-a-gaussian-height-ridge)
  - [Geostrophic adjustment of a finite-width height ramp](#geostrophic-adjustment-of-a-finite-width-height-ramp)
  - [Coastal adjustment of an elevated strip](#coastal-adjustment-of-an-elevated-strip)
  - [Balanced shallow-water energy as a signed potential-vorticity pairing](#balanced-shallow-water-energy-as-a-signed-potential-vorticity-pairing)
  - [Geostrophic adjustment of a finite-width current](#geostrophic-adjustment-of-a-finite-width-current)
    - [Energy retention in finite-width geostrophic adjustment](#energy-retention-in-finite-width-geostrophic-adjustment)
  - [Geostrophic adjustment of a surface-height jump](#geostrophic-adjustment-of-a-surface-height-jump)
  - [Inertia-gravity wave](#inertia-gravity-wave)
    - [Linear pressure equation for rotating stratified flow](#linear-pressure-equation-for-rotating-stratified-flow)
    - [Particle ellipses for rotating shallow-water waves](#particle-ellipses-for-rotating-shallow-water-waves)
    - [External gravity wave](#external-gravity-wave)
    - [Linear rotating shallow-water dispersion relation](#linear-rotating-shallow-water-dispersion-relation)
  - [Kelvin wave](#kelvin-wave)
    - [Kelvin-wave channel invariant](#kelvin-wave-channel-invariant)
- [Ocean circulation](#ocean-circulation)
  - [Antarctic Convergence](#antarctic-convergence)
  - [Antarctic Coastal Current](#antarctic-coastal-current)
  - [Antarctic Circumpolar Current](#antarctic-circumpolar-current)
  - [Antarctic bottom water](#antarctic-bottom-water)
  - [Wind stress](#wind-stress)
    - [Wind stress curl](#wind-stress-curl)
    - [Ekman layer](#ekman-layer)
      - [Laminar Ekman boundary stress](#laminar-ekman-boundary-stress)
      - [Surface Ekman layer](#surface-ekman-layer)
      - [Bottom Ekman layer](#bottom-ekman-layer)
    - [Ekman transport](#ekman-transport)
      - [Ekman pumping](#ekman-pumping)
        - [Ekman spin-down in a shallow-water layer](#ekman-spin-down-in-a-shallow-water-layer)
        - [Quasi-geostrophic Ekman spin-down](#quasi-geostrophic-ekman-spin-down)
    - [Ocean gyre](#ocean-gyre)
      - [Sverdrup balance](#sverdrup-balance)
        - [Ocean basin equation with bottom drag and lateral viscosity](#ocean-basin-equation-with-bottom-drag-and-lateral-viscosity)
          - [Drag-dominated basin solution with no-slip layers](#drag-dominated-basin-solution-with-no-slip-layers)
        - [Two-layer Sverdrup interior](#two-layer-sverdrup-interior)
          - [Linear stability of a meridional two-layer current](#linear-stability-of-a-meridional-two-layer-current)
            - [Meridional-wave instability of a two-layer Sverdrup flow](#meridional-wave-instability-of-a-two-layer-sverdrup-flow)
          - [Potential-vorticity gradients in a meridional two-layer current](#potential-vorticity-gradients-in-a-meridional-two-layer-current)
        - [Point-forced Sverdrup–drag Green function](#point-forced-sverdrup-drag-green-function)
        - [Ocean transport streamfunction](#ocean-transport-streamfunction)
          - [Relative vorticity from a variable-depth transport streamfunction](#relative-vorticity-from-a-variable-depth-transport-streamfunction)
        - [Godfrey island rule](#godfrey-island-rule)
        - [Topographic Sverdrup balance](#topographic-sverdrup-balance)
          - [Wind-driven circulation over parabolic basin topography](#wind-driven-circulation-over-parabolic-basin-topography)
          - [Topographic potential-vorticity pseudovelocity](#topographic-potential-vorticity-pseudovelocity)
          - [Topographic potential-vorticity steering](#topographic-potential-vorticity-steering)
      - [Western boundary current](#western-boundary-current)
        - [Stommel boundary layer](#stommel-boundary-layer)
        - [Munk boundary layer](#munk-boundary-layer)
- [Rossby wave](#rossby-wave)
  - [Rossby-wave equation for a sheared zonal current](#rossby-wave-equation-for-a-sheared-zonal-current)
    - [Local Rossby-wave dispersion relation in a zonal jet](#local-rossby-wave-dispersion-relation-in-a-zonal-jet)
      - [Stationary Rossby waves in a sinusoidal zonal jet](#stationary-rossby-waves-in-a-sinusoidal-zonal-jet)
  - [Linear Rossby-wave equation](#linear-rossby-wave-equation)
    - [Shallow-water Rossby-wave dispersion relation](#shallow-water-rossby-wave-dispersion-relation)
      - [Reflection of a Rossby wave at a meridional wall](#reflection-of-a-rossby-wave-at-a-meridional-wall)
      - [Rossby-wave isofrequency circle](#rossby-wave-isofrequency-circle)
  - [Topographic Rossby-wave dispersion relation](#topographic-rossby-wave-dispersion-relation)
    - [Square-basin topographic Rossby mode](#square-basin-topographic-rossby-mode)
    - [Step-trapped topographic Rossby wave](#step-trapped-topographic-rossby-wave)
      - [Double Kelvin-wave adjustment at a depth step](#double-kelvin-wave-adjustment-at-a-depth-step)
      - [Long-wave transport along a depth step](#long-wave-transport-along-a-depth-step)
  - [Barotropic Rossby wave](#barotropic-rossby-wave)
    - [Stationary Rossby-wave ray envelope](#stationary-rossby-wave-ray-envelope)
  - [Baroclinic Rossby wave](#baroclinic-rossby-wave)
    - [Rossby wave in a log-pressure atmosphere](#rossby-wave-in-a-log-pressure-atmosphere)
- [Wave activity](#wave-activity)
  - [Wave action (fluid dynamics)](#wave-action-fluid-dynamics)
    - [Wave pseudomomentum](#wave-pseudomomentum)
  - [Quasi-geostrophic wave pseudomomentum](#quasi-geostrophic-wave-pseudomomentum)
- [Equatorial wave](#equatorial-wave)
  - [Equivalent depth](#equivalent-depth)
  - [Equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation)
    - [Equatorial wave velocity polarization](#equatorial-wave-velocity-polarization)
    - [Frequency gap for higher equatorial wave modes](#frequency-gap-for-higher-equatorial-wave-modes)
  - [Equatorial Kelvin wave](#equatorial-kelvin-wave)
  - [Equatorial Rossby wave](#equatorial-rossby-wave)
    - [Equatorial Rossby-wave dispersion relation](#equatorial-rossby-wave-dispersion-relation)
  - [Equatorial inertia--gravity wave](#equatorial-inertia-gravity-wave)
  - [Rossby-gravity waves](#rossby-gravity-waves)
    - [Exceptional root of the mixed Rossby-gravity mode](#exceptional-root-of-the-mixed-rossby-gravity-mode)
  - [Damped equatorial Kelvin and Rossby response](#damped-equatorial-kelvin-and-rossby-response)
- [Transformed Eulerian mean](#transformed-eulerian-mean)
  - [Eddy buoyancy flux](#eddy-buoyancy-flux)
  - [Eliassen–Palm flux](#eliassen-palm-flux)
    - [Taylor identity for quasi-geostrophic flux](#taylor-identity-for-quasi-geostrophic-flux)
    - [Non-acceleration theorem for quasi-geostrophic waves](#non-acceleration-theorem-for-quasi-geostrophic-waves)
    - [Wave-activity deposition](#wave-activity-deposition)
    - [Quasi-geostrophic wave-activity conservation law](#quasi-geostrophic-wave-activity-conservation-law)
  - [Residual mean circulation](#residual-mean-circulation)
    - [Eliassen equation for residual circulation](#eliassen-equation-for-residual-circulation)
      - [Step-flux residual circulation in a stratified channel](#step-flux-residual-circulation-in-a-stratified-channel)
      - [Localized wave-drag response in a stratified channel](#localized-wave-drag-response-in-a-stratified-channel)
        - [Vertically integrated wave-drag acceleration](#vertically-integrated-wave-drag-acceleration)

## Ekman number

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ekman_number)

The ratio of viscous force to [Coriolis force](physics.md#coriolis-force) in a rotating fluid at length scale $L$. This convention uses rotation frequency $2\Omega$; conventions omitting the factor two are also common. For small $E$, bulk viscosity is weak but no-slip boundaries can form [Ekman layers](#ekman-layer) of thickness of order $L\sqrt E$, with relatively larger boundary shear stress.

## Deacon cell

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)

A zonal-mean meridional overturning circulation associated with Southern Ocean wind forcing. In a southern-hemisphere channel with eastward wind stress, the mean circulation has northward surface transport and a southward deep return. Its Eulerian strength need not equal the residual water-mass transport because [eddy-induced overturning](#eddy-induced-overturning) can oppose it.

### Eddy-induced overturning

↑ **Parent:** [Deacon cell](#deacon-cell)

The effective meridional circulation associated with eddy buoyancy transport. In a stratified Southern Ocean, mesoscale eddies tend to flatten the isopycnals tilted by the wind-driven mean circulation, so their contribution can largely oppose the mean Deacon circulation. The residual combines mean and eddy contributions with the diabatic water-mass budget.

### Meridional overturning streamfunction

↑ **Parent:** [Deacon cell](#deacon-cell)

A streamfunction for an incompressible zonal-mean flow in the meridional-vertical plane. Its derivatives give meridional and vertical velocity, and differences in its values measure volume transport per zonal span. Constant values on closed impermeable boundaries encode zero net normal flow.

## Deformation radius

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)

A horizontal scale comparing gravitational or buoyancy restoring forces with rotation. For a shallow-water gravity mode with propagation speed $c$, the [deformation radius](#deformation-radius) is $c/|f|$. The [barotropic deformation radius](#barotropic-deformation-radius) uses $c=\sqrt{gH}$; internal layered modes use a speed set by [reduced gravity](reduced-gravity.md) and layer depths.

### Two-layer internal deformation radius

↑ **Parent:** [Deformation radius](#deformation-radius)

The [two-layer quasi-geostrophic potential vorticity](#two-layer-quasi-geostrophic-potential-vorticity) coupling defines $R_d^{-2}=F_1+F_2$. With $F_i=f_0^2/(g\prime H_i)$ this gives the stated radius. The [baroclinic energy ratio and deformation scale](#baroclinic-energy-ratio-and-deformation-scale) depends on $(l/R_d)^2$, so the thinner layer matters when the depths are strongly unequal.

## Burger number

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)

The [Burger number](#burger-number) compares the square of a relevant [deformation radius](#deformation-radius) with the square of the horizontal flow scale: $\mathrm{Bu}=R_d^2/l^2$. In a two-layer geostrophic model $R_d^2=g\prime H_1H_2/[f_0^2(H_1+H_2)]$. Its inverse measures the scale ratio of baroclinic [available potential energy](classical-mechanics.md#available-potential-energy) to [kinetic energy](classical-mechanics.md#kinetic-energy). Keeping it of order unity retains both interface and relative-vorticity contributions in QG scaling.

## General circulation model

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/General_circulation_model)

A general circulation model evolves rotating fluid dynamics together with heating/cooling and suitable transport parameterizations. Atmospheric applications can couple [radiative transfer](astrophysics.md#radiative-transfer), clouds and chemistry to resolve longitudinal and latitudinal structure. For an [exoplanet atmosphere](exoplanet.md#exoplanet-atmosphere), it can predict winds and an [exoplanet thermal phase curve](exoplanet.md#exoplanet-thermal-phase-curve). Unresolved turbulence and cloud microphysics still require approximate closures.

## Eulerian mean flow

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)

An Eulerian mean flow is obtained by averaging the [velocity field](fluid-mechanics.md#velocity-field) at fixed spatial positions, for example over longitude or over an ensemble. It differs from a parcel-following average. In the [transformed Eulerian mean](#transformed-eulerian-mean), its meridional circulation is corrected by an eddy-induced contribution to form the [residual mean circulation](#residual-mean-circulation).

## Thermal wind

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thermal_wind)

Thermal-wind balance relates vertical shear of geostrophic flow to horizontal density or temperature gradients. With constant Coriolis parameter $f_0$ and reference density $\rho_0$,

$$
f_0u_z=\frac g{\rho_0}\rho_y
$$

for the sign conventions used here.

### Geostrophic thermal wind with separable buoyancy

↑ **Parent:** [Thermal wind](#thermal-wind)

For $b=A(y)+B(z)$, constant nonzero $f_0$, and zero basic velocity at $z=0$, [thermal-wind balance](#thermal-wind) gives

$$
\bar u=-\frac{zA'(y)}{f_0},\qquad \bar v=0.
$$

With full buoyancy represented by $f_0\bar\psi_z$, the constant-coefficient [three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) is $\bar q=f_0+zA''/f_0+f_0B'/N^2$. The [reference-buoyancy convention in quasi-geostrophic potential vorticity](#reference-buoyancy-convention-in-quasi-geostrophic-potential-vorticity) changes only the uniform reference contribution.

## Log-pressure coordinate

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)

A log-pressure coordinate uses atmospheric pressure to define an effective height. Its density weight is proportional to $e^{-z/H}$, and its continuity equation has vertical divergence $e^{z/H}\partial_z(e^{-z/H}w)$. Here $H$ is the chosen pressure scale height; the coordinate is not generally identical to geometric altitude.

## Rossby number

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rossby_number)

The Rossby number compares inertial acceleration with [Coriolis acceleration](physics.md#coriolis-acceleration). For speed $U$, horizontal length $L$, and [Coriolis parameter](#coriolis-parameter) $f$, it is $\operatorname{Ro}=U/(|f|L)$. Small Rossby number supports [geostrophic balance](physics.md#geostrophic-balance) and the [quasi-geostrophic approximation](#quasi-geostrophic-approximation).

### Stellar activity Rossby number

↑ **Parent:** [Rossby number](#rossby-number)

For a convective star, the activity convention compares its rotation period with a convective turnover time. It differs by fixed factors from the fluid [Rossby number](#rossby-number) estimated from speed, length and angular velocity. Small $\operatorname{Ro}_*$ denotes strong rotational influence on [convection](fluid-mechanics.md#convection). Magnetic activity usually rises as this ratio decreases in the unsaturated regime, but levels off in a saturated rapid-rotation regime.

## Burgers number

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burgers_number)

The Burgers number compares stratification with rotational effects. In shallow-water and stratified flows it is commonly the squared ratio of deformation radius to horizontal length scale.

## Boussinesq approximation

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boussinesq_approximation)

The Boussinesq approximation treats density as constant except where a small density variation multiplies gravity to produce buoyancy. The velocity remains incompressible.

### Strong Boussinesq approximation

↑ **Parent:** [Boussinesq approximation](#boussinesq-approximation)

In the constant-property convection convention, the strong [Boussinesq approximation](#boussinesq-approximation) supplements small relative [mass density](fluid-mechanics.md#density) changes with constant [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity), [thermal diffusivity](thermodynamics.md#thermal-diffusivity), [specific heat capacity](thermodynamics.md#specific-heat-capacity) and [thermal expansion coefficient](thermodynamics.md#thermal-expansion-coefficient) throughout the modeled temperature interval. A uniform reference density replaces density in inertia and [mass conservation](continuum-mechanics.md#mass-conservation), while a linear density anomaly is retained in gravitational [buoyancy](fluid-mechanics.md#buoyancy). The temperature obeys an [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) with constant coefficients. The term “strong” is not uniform across all fluid-mechanics literature: some stratified-flow treatments instead emphasize the use of a globally constant reference density. The constant-property convection usage is explained in [https://courses.physics.ucsd.edu/2021/Spring/physics218c/Spiegel%20Convection.pdf](https://courses.physics.ucsd.edu/2021/Spring/physics218c/Spiegel%20Convection.pdf) .

<h3 id="stratification-rotation-analogy">Stratification–rotation analogy</h3>

↑ **Parent:** [Boussinesq approximation](#boussinesq-approximation)

Uniformly stratified, nonrotating, two-dimensional ideal [Boussinesq equations](#boussinesq-equations) in coordinates $(x,z)$ are equivalent to unstratified rotating equations independent of $Y$, with $(X,Y,Z)=(z,y,-x)$, rotation $2\boldsymbol\Omega=N\mathbf e_Z$, velocity $(U,V,W)=(w,\sigma/N,-u)$, and the same reduced pressure. The transverse rotating velocity represents [buoyancy perturbation](fluid-mechanics.md#buoyancy-perturbation), while the rotation-axis velocity represents the stratified horizontal velocity. Matching prescribed forces may have components in the invariant plane, but no transverse component. Physical [free surface](fluid-mechanics.md#free-surface) conditions are not preserved: the physical vertical direction and its normal velocity are different under the mapping.

#### Causal pressure adjustment by internal waves

↑ **Parent:** [Stratification–rotation analogy](#stratification-rotation-analogy)

A weak horizontal force $f'(x)e^{imz}$, with $m>0$ and $\int f'(x)\,dx=\varepsilon$, admits many steady pressures differing by an arbitrary function of height. Switching the force on in initially motionless, unbounded, uniformly stratified fluid selects $p_\infty=[f(x)-\varepsilon/2]e^{imz}$, up to a spatially constant pressure gauge. For horizontal [wavenumber](wave-equation.md#wavenumber) $q$, the transient frequency is $\Omega(q)=Nq/\sqrt{q^2+m^2}$. Its long-wave [group velocity](wave-equation.md#group-velocity) is $N/m$, and oppositely propagating outgoing fronts leave pressure limits $-\varepsilon/2$ and $+\varepsilon/2$. The limit is at fixed $x$ after the fronts have passed; dispersive tails need not vanish at any finite time.

##### Hydrostatic response to a localized horizontal force

↑ **Parent:** [Causal pressure adjustment by internal waves](#causal-pressure-adjustment-by-internal-waves)

For a weak horizontal forcing proportional to $e^{imz}$ in an ideal uniformly stratified nonrotating fluid, the low-frequency [hydrostatic approximation](fluid-mechanics.md#hydrostatic-approximation) gives the displayed one-dimensional [wave equation](wave-equation.md) for the [streamfunction](fluid-mechanics.md#stream-function) amplitude. Two oppositely propagating characteristic integrals determine the response. A source confined to $|x|\leq a$ and switched on at time zero produces no response beyond $|x|\leq ct+a$ in this reduced equation. The bound on mixed forcing derivative $|f_{xt}|\ll |mNf_{\max}|$ controls the neglected vertical acceleration in characteristic magnitude.

### Boussinesq up-down symmetry

↑ **Parent:** [Boussinesq approximation](#boussinesq-approximation)

With mechanically and thermally equivalent upper and lower boundaries, the [Boussinesq approximation](#boussinesq-approximation) permits reflection through the layer midplane together with reversal of the temperature perturbation and vertical velocity. In a reduced [convection](fluid-mechanics.md#convection) temperature equation this induces temperature inversion. A quadratic term which changes differently from the linear terms breaks this symmetry; a cubic term can preserve it. The [Boussinesq approximation](#boussinesq-approximation) alone does not impose symmetry on unequal boundary conditions.

### Boussinesq equations

↑ **Parent:** [Boussinesq approximation](#boussinesq-approximation)

The inviscid Boussinesq equations for velocity $\mathbf u$, buoyancy $b$, and reference density $\rho_0$ are

$$
\frac{D\mathbf u}{Dt}
=-\rho_0^{-1}\nabla p+b\widehat{\mathbf z},
\qquad
\nabla\cdot\mathbf u=0,
$$

together with an advection or advection–diffusion equation for $b$.

#### Linearized Boussinesq equations

↑ **Parent:** [Boussinesq equations](#boussinesq-equations)

The linearized Boussinesq equations describe small velocity, pressure, and buoyancy perturbations about a motionless, stably stratified reference state. With [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$, [mass diffusivity](fluid-mechanics.md#mass-diffusivity) $\kappa$, and [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, they are

$$
(\partial_t-\nu\nabla^2)\mathbf u=-\frac1{\rho_0}\nabla p+b\mathbf e_z,
\qquad
(\partial_t-\kappa\nabla^2)b=-N^2w,
\qquad
\nabla\mathbin\cdot\mathbf u=0.
$$

### Inertial wave

↑ **Parent:** [Boussinesq approximation](#boussinesq-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertial_wave)

An inertial wave is a rotating-fluid wave restored by the Coriolis force. Its frequency depends on the angle between its wavevector and the rotation axis.

#### Inertial modes in a rigid rotating sphere

↑ **Parent:** [Inertial wave](#inertial-wave)

In a uniform-density [incompressible flow](fluid-mechanics.md#incompressible-flow) inside a smooth rigid sphere rotating at angular speed $\Omega$, a [normal mode](wave-equation.md#normal-mode) with phase $e^{i\sigma t+im\phi}$ has intrinsic frequency $s=\sigma+m\Omega$. For $s\ne0,\pm2\Omega$, eliminating [velocity](classical-mechanics.md#velocity) from the [linearized Euler equations](fluid-mechanics.md#linearized-euler-equations) gives the displayed pressure equation, with $W=p'/\rho$. Impermeability gives $R W_R+(2m\Omega/s)W+(1-4\Omega^2/s^2)zW_z=0$ on the sphere. There is no condition $W=0$: the rigid wall supplies variable normal [pressure](thermodynamics.md#pressure). These [inertial waves](#inertial-wave) are restored by [Coriolis acceleration](physics.md#coriolis-acceleration), and their pressure equation is hyperbolic for $|s|<2|\Omega|$.

##### Cubic axisymmetric inertial mode of a rigid sphere

↑ **Parent:** [Inertial modes in a rigid rotating sphere](#inertial-modes-in-a-rigid-rotating-sphere)

For an axisymmetric [normal mode](wave-equation.md#normal-mode) in a rigid rotating sphere, substitute $W=z(AR^2+Bz^2+C)$ into the pressure equation and its impermeability condition. With $\beta=1-4\Omega^2/\sigma^2$, the interior equation gives $2A+3\beta B=0$. The boundary polynomial gives $3\beta B=(2+\beta)A$ and $\beta C=-(2+\beta)Ar_0^2$. A nontrivial oscillatory solution has $\beta=-4$, hence the displayed frequency and $B=A/6$, $C=-Ar_0^2/2$. It satisfies both equations identically.

## Rotating fluid

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotating_fluid)

A rotating fluid is described in a rotating reference frame, where the [Coriolis acceleration](physics.md#coriolis-acceleration) and centrifugal acceleration supplement the physical forces.

<h3 id="taylor-proudman-theorem">Taylor–Proudman theorem</h3>

↑ **Parent:** [Rotating fluid](#rotating-fluid)

For homogeneous, incompressible, inviscid flow with constant rotation vector and negligible inertia, taking the [curl](calculus.md#curl) of $2\boldsymbol\Omega\times\mathbf u=-\nabla p$ gives $(\boldsymbol\Omega\cdot\nabla)\mathbf u=0$. Thus a [geostrophic flow](#geostrophic-flow) is independent of distance along the rotation axis. Body forces modify the relation by their [curl](calculus.md#curl); it applies unchanged in unforced exterior regions. A nontrivial exterior column cannot both obey this leading balance and decay along the rotation axis.

#### Geostrophic contour

↑ **Parent:** [Taylor–Proudman theorem](#taylor-proudman-theorem)

In nearly columnar flow between rigid boundaries, a geostrophic contour is a contour of column height divided by the [Coriolis parameter](#coriolis-parameter). If relative [vorticity](fluid-mechanics.md#vorticity) is negligible, conservation of [shallow-water potential vorticity](#shallow-water-potential-vorticity) constrains leading [geostrophic flow](#geostrophic-flow) to these contours. Motion across them stretches or squashes columns, generating relative [vorticity](fluid-mechanics.md#vorticity); for constant $f$, the contours are simply contours of $H$.

### Taylor number

↑ **Parent:** [Rotating fluid](#rotating-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor_number)

For a layer rotating at angular speed $\Omega$, of depth $d$ and [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$, the [Taylor number](#taylor-number) compares the [Coriolis force](physics.md#coriolis-force) to viscous damping through the squared ratio $(2\Omega d^2/\nu)^2$. Definitions in other geometries may include different geometric factors; this is the plane-layer convention.

### Traditional approximation (geophysical fluid dynamics)

↑ **Parent:** [Rotating fluid](#rotating-fluid)

The traditional approximation retains only the locally vertical component of planetary rotation in the Coriolis force. It gives the horizontal acceleration $f\widehat{\mathbf z}\times\mathbf u_h$ and neglects terms involving the horizontal component of the rotation vector and vertical velocity.

### Coriolis parameter

↑ **Parent:** [Rotating fluid](#rotating-fluid)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coriolis_parameter)

The Coriolis parameter is $f=2\Omega\sin\varphi$ for planetary rotation rate $\Omega$ and latitude $\varphi$. It controls the vertical component of the Coriolis acceleration acting on horizontal flow.

#### f-plane

↑ **Parent:** [Coriolis parameter](#coriolis-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/f-plane)

An f-plane approximates the [Coriolis parameter](#coriolis-parameter) by a constant $f_0$ over a limited horizontal region.

#### beta plane

↑ **Parent:** [Coriolis parameter](#coriolis-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/beta_plane)

A beta plane retains the leading meridional variation $f=f_0+\beta y$ of the [Coriolis parameter](#coriolis-parameter).

#### Inertial oscillation

↑ **Parent:** [Coriolis parameter](#coriolis-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertial_oscillation)

An inertial oscillation is the horizontal circular motion of an unforced parcel in a rotating fluid. On an [f-plane](#f-plane), $\dot u-fv=0$ and $\dot v+fu=0$, so the speed is constant and the angular frequency is $|f|$.

##### Beta drift of an inertial oscillation

↑ **Parent:** [Inertial oscillation](#inertial-oscillation)

On a [beta plane](#beta-plane), the turning rate of an [inertial oscillation](#inertial-oscillation) is larger on the poleward side of its orbit than on the equatorward side. For initial speed $V$ and $\beta V/f_0^2\ll1$, this asymmetry produces westward mean drift of magnitude $\beta V^2/(2f_0^2)$.

## Potential vorticity

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Potential_vorticity)

Potential vorticity combines [vorticity](fluid-mechanics.md#vorticity) with [vortex stretching](physics.md#vortex-stretching) and [density stratification](gravity-wave.md#density-stratification). It also applies to nonrotating stratified flow through [Ertel potential vorticity](#ertel-potential-vorticity). In the inviscid [shallow water equations](physics.md#shallow-water-equations),

$$
q=\frac{f+\zeta}{h},
$$

where $\zeta$ is [relative vorticity](fluid-mechanics.md#relative-vorticity) and $h$ is layer thickness.

### Potential-vorticity inversion

↑ **Parent:** [Potential vorticity](#potential-vorticity)

Potential-vorticity inversion recovers a balanced [velocity field](fluid-mechanics.md#velocity-field) from [potential vorticity](#potential-vorticity) and specified boundary and global data. In [two-dimensional vortex dynamics](fluid-mechanics.md#two-dimensional-vortex-dynamics) this is a [Poisson equation](partial-differential-equation.md#poisson-equation); [shallow-water quasi-geostrophic inversion](#shallow-water-quasi-geostrophic-inversion) and [stratified quasi-geostrophic inversion](#stratified-quasi-geostrophic-inversion) use different [elliptic boundary value problems](elliptic-boundary-value-problem.md). Advance the materially conserved scalar, then invert again to recover the evolving flow. Boundary [buoyancy](fluid-mechanics.md#buoyancy) can induce flow with zero interior anomaly. The balance relation and [boundary conditions](differential-equation.md#boundary-condition) are essential: unrestricted [gravity waves](gravity-wave.md) are additional degrees of freedom. [McIntyre's potential-vorticity account](https://pordlabs.ucsd.edu/wryoung/theorySeminar/pdf14/McIntyrePV.pdf) explains the general invertibility principle.

#### Two-dimensional potential-vorticity inversion

↑ **Parent:** [Potential-vorticity inversion](#potential-vorticity-inversion)

In [two-dimensional vortex dynamics](fluid-mechanics.md#two-dimensional-vortex-dynamics), solve the [Poisson equation](partial-differential-equation.md#poisson-equation) for the [streamfunction](fluid-mechanics.md#stream-function) with the prescribed [boundary conditions](differential-equation.md#boundary-condition). On the plane its fundamental solution is $(2\pi)^{-1}\log|\mathbf x|$, so differentiating the displayed inverse gives the [planar Biot-Savart kernel](fluid-mechanics.md#planar-vorticity-velocity-kernel). The [harmonic function](partial-differential-equation.md#harmonic-function) $\psi_h$ represents boundary and global-flow data. An additive constant changes no [velocity](classical-mechanics.md#velocity); circulation around holes and a uniform flow are additional degrees of freedom if their boundary or far-field values are not prescribed. The same inverse acts independently on each level in [nonrotating layerwise-two-dimensional vortex dynamics](fluid-mechanics.md#nonrotating-layerwise-two-dimensional-vortex-dynamics).

#### Shallow-water quasi-geostrophic inversion

↑ **Parent:** [Potential-vorticity inversion](#potential-vorticity-inversion)

The [shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity) relation is a [modified Helmholtz equation](partial-differential-equation.md#modified-helmholtz-equation) for the [quasi-geostrophic streamfunction](#quasi-geostrophic-streamfunction). Its inverse with specified [boundary conditions](differential-equation.md#boundary-condition) recovers horizontal [geostrophic flow](#geostrophic-flow) and surface elevation $\eta=f_0\psi/g$. The [Rossby deformation radius](physics.md#rossby-deformation-radius) $L_D=\sqrt{gH}/|f_0|$ is the range of the balanced response: for a horizontal Fourier component, $\widehat\psi=-\widehat q/(|\mathbf k_h|^2+L_D^{-2})$, after subtracting background [potential vorticity](#potential-vorticity).

#### Stratified quasi-geostrophic inversion

↑ **Parent:** [Potential-vorticity inversion](#potential-vorticity-inversion)

The [three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) relation defines an anisotropic [elliptic boundary value problem](elliptic-boundary-value-problem.md). Interior [potential vorticity](#potential-vorticity) and boundary [buoyancy perturbation](fluid-mechanics.md#buoyancy-perturbation) $b=f_0\psi_z$, together with lateral and global conditions, determine the [quasi-geostrophic streamfunction](#quasi-geostrophic-streamfunction) up to its allowed constant. If two solutions have the same data, their difference has zero elliptic source and homogeneous boundary data. [Integration by parts](calculus.md#integration-by-parts) gives zero integral of $|\nabla_h\psi|^2+(f_0^2/N^2)|\psi_z|^2$, proving uniqueness modulo a constant in a connected domain when the boundary terms vanish. [Eady edge waves](hydrodynamic-stability.md#eady-edge-wave) show that zero interior source alone is insufficient.

##### Prandtl ratio of scales

↑ **Parent:** [Stratified quasi-geostrophic inversion](#stratified-quasi-geostrophic-inversion)

The Prandtl ratio compares horizontal and vertical scales in rotating [density stratification](gravity-wave.md#density-stratification). In the [three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) operator, horizontal curvature scales as $\psi/L^2$ and vertical stretching as $(f_0^2/N^2)\psi/H^2$. Comparable terms therefore require $H/L\sim |f_0|/N$. For constant $N$, the stretched coordinate $Z=(N/|f_0|)z$ makes the operator isotropic. This aspect ratio concerns rotational and stratification effects, not the viscous-to-thermal diffusivity [Prandtl number](thermodynamics.md#prandtl-number).

##### Stretched coordinates for quasi-geostrophic inversion

↑ **Parent:** [Stratified quasi-geostrophic inversion](#stratified-quasi-geostrophic-inversion)

For constant nonzero [Coriolis parameter](#coriolis-parameter) and positive constant [buoyancy](fluid-mechanics.md#buoyancy) [frequency](physics.md#frequency), the anisotropic [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) operator becomes the ordinary three-dimensional [Laplacian](calculus.md#laplacian) in the displayed coordinates. Its decaying whole-space inverse is $\psi(\mathbf X)=-\int[Q(\mathbf X')-f]/(4\pi|\mathbf X-\mathbf X'|)\,d^3X'$. Boundary or far-field data are needed to exclude arbitrary harmonic additions.

###### Spherical potential-vorticity anomaly

↑ **Parent:** [Stretched coordinates for quasi-geostrophic inversion](#stretched-coordinates-for-quasi-geostrophic-inversion)

A uniform positive [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) anomaly in a sphere of stretched radius $R$ has the displayed regular, decaying [streamfunction](fluid-mechanics.md#stream-function). Both it and its radial derivative match at the sphere. In its equatorial plane the horizontal [relative vorticity](fluid-mechanics.md#relative-vorticity) is $2Q_0/3$ inside and $-Q_0R^3/(3r^3)$ outside. The exterior potential-vorticity anomaly remains zero because its vertical stretching contribution compensates that [relative vorticity](fluid-mechanics.md#relative-vorticity). A stretched sphere corresponds to a flattened ellipsoid in physical coordinates when $N\gg|f|$.

### Potential-vorticity gradient

↑ **Parent:** [Potential vorticity](#potential-vorticity)

The spatial [gradient](calculus.md#gradient) of [potential vorticity](#potential-vorticity) controls the anomaly created when a parcel is displaced. The linear [potential-vorticity equation](#potential-vorticity-evolution-equation) contains $\mathbf u'\cdot\nabla\bar q$. A gradient of the [Coriolis parameter](#coriolis-parameter) contributes [planetary vorticity](fluid-mechanics.md#planetary-vorticity), but gradients of relative [vorticity](fluid-mechanics.md#vorticity) and layer stretching can be equally important.

### Potential-vorticity evolution equation

↑ **Parent:** [Potential vorticity](#potential-vorticity)

A [potential vorticity](#potential-vorticity) budget has the form

$$
\frac{Dq}{Dt}=S_q.
$$

The [material derivative](continuum-mechanics.md#material-derivative) follows the fluid motion and $S_q$ collects forcing or dissipation. With $S_q=0$ it becomes [potential-vorticity conservation](#potential-vorticity-conservation). For a [quasi-geostrophic streamfunction](#quasi-geostrophic-streamfunction), horizontal advection is $J(\psi,q)=\psi_xq_y-\psi_yq_x$.

#### Potential-vorticity conservation

↑ **Parent:** [Potential-vorticity evolution equation](#potential-vorticity-evolution-equation)

In unforced adiabatic inviscid motion, [potential vorticity](#potential-vorticity) is conserved following a parcel:

$$
Dq/Dt=0.
$$

The linearization about a basic state is $(\partial_t+\bar{\mathbf u}\cdot\nabla)q'+\mathbf u'\cdot\nabla\bar q=0$. This separates advection of a disturbance from its generation by displacement across a basic [potential-vorticity gradient](#potential-vorticity-gradient).

##### Momentum loss from uniform potential-vorticity mixing

↑ **Parent:** [Potential-vorticity conservation](#potential-vorticity-conservation)

If [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) initially has gradient $\beta$ across a channel of width $W$ and is homogenized, a height-independent change of zonal velocity obeys $\delta Q=-\delta U_y$. Requiring $\delta U(0)=\delta U(W)=0$ gives uniform final potential vorticity equal to its original channel mean, $\delta U=\beta y(y-W)/2$, and channel-mean momentum change $-\beta W^2/12$. The negative change for $\beta>0$ is wave drag associated with mixing, not a loss of total momentum in an isolated unforced system.

###### Rossby-wave PV mixing and zonal momentum

↑ **Parent:** [Momentum loss from uniform potential-vorticity mixing](#momentum-loss-from-uniform-potential-vorticity-mixing)

In zonally averaged barotropic [quasi-geostrophic approximation](#quasi-geostrophic-approximation) flow with zero mean meridional transport, the [Taylor identity for quasi-geostrophic flux](#taylor-identity-for-quasi-geostrophic-flux) relates the meridional [potential vorticity](#potential-vorticity) flux to the convergence of [Reynolds stress](turbulence.md#reynolds-stress). A local downgradient closure $\overline{v'q'}=-\kappa\overline Q_y$, with $\kappa\ge0$, therefore gives westward mean acceleration where the background gradient is positive. [Rossby wave](#rossby-wave) breaking can stir PV into fine filaments; coarse-graining or weak diffusion produces the inferred mixing. Globally the momentum-flux convergence integrates to boundary stresses, so localized westward changes need compensating transport or momentum changes elsewhere in an isolated system.

### Ertel potential vorticity

↑ **Parent:** [Potential vorticity](#potential-vorticity)

Ertel potential vorticity is the scalar product of [absolute vorticity](fluid-mechanics.md#absolute-vorticity) with the gradient of a materially conserved stratifying scalar. In [Boussinesq flow](#boussinesq-approximation) with buoyancy $b$,

$$
Q=\boldsymbol\omega_a\mathbin{\cdot}\nabla b.
$$

It is materially conserved by inviscid, adiabatic motion.

<h4 id="ertel-s-theorem">Ertel's theorem</h4>

↑ **Parent:** [Ertel potential vorticity](#ertel-potential-vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ertel's_theorem)

An inviscid fluid with conservative body force, a materially conserved stratifying scalar $\alpha$, and an [equation of state](thermodynamics.md#equation-of-state) making $\nabla\rho,\nabla p,\nabla\alpha$ coplanar conserves its [Ertel potential vorticity](#ertel-potential-vorticity). The stretching of [absolute vorticity](fluid-mechanics.md#absolute-vorticity) per unit [density](fluid-mechanics.md#density) cancels the deformation of the scalar [gradient](calculus.md#gradient); the remaining baroclinic triple product vanishes. In an incompressible density-stratified ideal fluid, choosing the advected [density](fluid-mechanics.md#density) as $\alpha$ gives that cancellation directly.

### Shallow-water potential vorticity

↑ **Parent:** [Potential vorticity](#potential-vorticity)

Shallow-water potential vorticity is materially conserved by inviscid, unforced [shallow water equations](physics.md#shallow-water-equations). Linearizing about rest with depth $H_0$ gives an anomaly proportional to

$$
\zeta-\frac{f\eta}{H_0}.
$$

#### Circular topographic anticyclone

↑ **Parent:** [Shallow-water potential vorticity](#shallow-water-potential-vorticity)

For an upstream irrotational current on an [f-plane](#f-plane) in a rigid layer of height $h$, a circular region of height $h(1-\epsilon)$ has the displayed relative [vorticity](fluid-mechanics.md#vorticity) if its fluid retains upstream [potential vorticity](#potential-vorticity) $f/h$. To leading order in the height contrast, take $u=-\Psi_y$, $v=\Psi_x$ and $\Psi=-Uy+\psi$. Solving the [Poisson equation](partial-differential-equation.md#poisson-equation) for $\psi$ gives $\psi=-Cr^2/2$ inside and $\psi=Ca^2[\log(a/r)-1/2]$ outside, where $C=f\epsilon/2$. The disturbance is clockwise for positive $f\epsilon$. Variable-depth transport and the transition across the rim introduce higher-order corrections to this leading columnar inversion.

##### Closed-streamline threshold for a circular topographic anticyclone

↑ **Parent:** [Circular topographic anticyclone](#circular-topographic-anticyclone)

For the [circular topographic anticyclone](#circular-topographic-anticyclone) in a positive uniform current $U$, the opposing disturbance speed is at most $Ca=f\epsilon a/2$. Below the displayed threshold $u$ remains positive everywhere, so no [streamline](fluid-mechanics.md#streamline) can close. Above it an interior [stagnation point](fluid-mechanics.md#stagnation-point) at $(0,-U/C)$ is a center, while the exterior point $(0,-Ca^2/U)$ is a saddle. At equality the two meet at the rim. This is the onset criterion; once closed contours form, the [potential vorticity](#potential-vorticity) of trapped fluid is not determined solely by its present upstream conditions.

#### Zero-potential-vorticity rotating channel flow

↑ **Parent:** [Shallow-water potential vorticity](#shallow-water-potential-vorticity)

For a steady, slowly varying rotating channel, negligible transverse velocity and zero [shallow-water potential vorticity](#shallow-water-potential-vorticity) give $u_y=f$. Cross-channel [geostrophic balance](physics.md#geostrophic-balance) gives $gh_y=-fu$, producing the displayed profiles. The specific energy $E=h+u^2/(2g)$ is constant across the channel, and $E+H$ is constant along it. Zero potential vorticity is not the value in an ordinary finite-depth reservoir at rest in the rotating frame; it requires vanishing absolute vorticity or a deep-reservoir approximation.

##### Hydraulic control of a zero-PV rotating channel

↑ **Parent:** [Zero-potential-vorticity rotating channel flow](#zero-potential-vorticity-rotating-channel-flow)

At a hydraulic control, the specific-energy function of a [zero-potential-vorticity rotating channel flow](#zero-potential-vorticity-rotating-channel-flow) is stationary with respect to wall depth at fixed discharge and width. Writing $v=u_1+fb/2$ gives $v(v+fb/2)=gh_1$ and $Q_c=bv^3/g$, hence the displayed discharge. The fully wetted positive-flow solution requires $fb<\sqrt{2gh_1}$; at equality the other wall dries and the first wall velocity vanishes. Beyond that limit the assumed two-wet-wall profile must be replaced.

#### Linearized shallow-water potential-vorticity anomaly

↑ **Parent:** [Shallow-water potential vorticity](#shallow-water-potential-vorticity)

For a constant-depth resting layer on an [f-plane](#f-plane), the depth-scaled linear [potential vorticity](#potential-vorticity) anomaly is

$$
q=\zeta-\frac fH\eta,\qquad \zeta=v_x-u_y.
$$

It satisfies $q_t=0$ under the [linearized shallow water equations](physics.md#linearized-shallow-water-equations). The physical perturbation of $(f+\zeta)/(H+\eta)$ is $q/H$. The signed scalar $q$, not its absolute value, is used in [potential-vorticity inversion](#potential-vorticity-inversion) and balanced energy pairings.

#### Shallow-water quasi-geostrophic potential vorticity

↑ **Parent:** [Shallow-water potential vorticity](#shallow-water-potential-vorticity)

For small Rossby number and small free-surface displacement, shallow-water potential vorticity reduces, up to a constant factor and additive constant, to relative vorticity plus background PV gradients and the stretching term $-\psi/L_D^2$.

##### Cosine-ridge shallow-water geostrophic response

↑ **Parent:** [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)

For a uniform upstream current whose free-surface and bottom slopes compensate, steady [quasi-geostrophic approximation](#quasi-geostrophic-approximation) flow with uniform incoming [potential vorticity](#potential-vorticity) obeys the displayed inversion equation. Let $\widehat b=\epsilon\cos(x/L)$ on $|x|<a=\pi L/2$ and zero outside. With $C=(f\epsilon/h_0)/(L^{-2}+L_R^{-2})$, the decaying even response is $\phi=C[\cos(x/L)+(L_R/L)e^{-a/L_R}\cosh(x/L_R)]$ inside and $\phi=C(L_R/L)e^{-a/L_R}\cosh(a/L_R)e^{-(|x|-a)/L_R}$ outside. Continuity of $\phi$ and $\phi'$ fixes the coefficients. Its streamlines satisfy $y=y_\infty+\phi(x)/U$, so the response extends beyond the compact ridge through exponentially decaying balanced tails.

##### Uniform-current obstruction to constant shallow-water QG potential vorticity

↑ **Parent:** [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)

On a constant [f-plane](#f-plane) with finite [Rossby deformation radius](physics.md#rossby-deformation-radius), a geostrophic uniform current $(U,0)$ has streamfunction $-Uy$ and a sloping free surface. The full [shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity) is $Q=f+\nabla^2\Psi-\Psi/L_R^2+fb/H$, so a flat-bottom background has the displayed nonconstant value. Omitting its gradient is not a harmless streamfunction gauge choice. A uniform-current, constant-PV inversion must explicitly supply a compensating background, external balance, or a rigid-lid limit.

###### Gaussian topographic response with compensated uniform potential vorticity

↑ **Parent:** [Uniform-current obstruction to constant shallow-water QG potential vorticity](#uniform-current-obstruction-to-constant-shallow-water-qg-potential-vorticity)

In a shallow-water [potential-vorticity inversion](#potential-vorticity-inversion) with the background gradient explicitly compensated, uniform PV gives $(\nabla^2-L_R^{-2})\psi'=-fb/H$. The displayed [Gaussian function](calculus.md#gaussian-function) solves it for $b=\epsilon[4(1-r^2/a^2)+a^2/L_R^2]e^{-r^2/a^2}$. This is not, without that compensation, a steady solution of the standard finite-depth constant-f current problem: its residual is $U\psi'_x/L_R^2$. Closed streamlines can occur while [Rossby number](#rossby-number) and surface displacement remain small.

###### Closed-streamline threshold for a Gaussian disturbance in uniform flow

↑ **Parent:** [Gaussian topographic response with compensated uniform potential vorticity](#gaussian-topographic-response-with-compensated-uniform-potential-vorticity)

For total [streamfunction](fluid-mechanics.md#stream-function) $\Psi=-Uy+Ae^{-(x^2+y^2)/a^2}$, the maximum opposing zonal disturbance speed is $\sqrt{2/e}|A|/a$. Below the displayed threshold the zonal velocity never changes sign and streamlines cannot close. Above it two stagnation points appear on the symmetry axis: one has definite Hessian and is a center, the other has indefinite Hessian and is a saddle. Closed contours surround the center. Equality is a degenerate onset, not a finite-area closed-cell regime.

##### Potential-vorticity mixing over a finite bottom slope

↑ **Parent:** [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)

Homogenizing the [potential vorticity](#potential-vorticity) over a finite constant bottom slope creates the odd anomaly displayed here while leaving the exterior unchanged. Inverting $(\partial_y^2-L_R^{-2})\psi=\Delta Q$ with decay at both infinities and matching $\psi,\psi_y$ gives a central return current and flanking jets. The [deformation radius](#deformation-radius) sets the smoothing length. For $L_R\ll a$, the central surface follows the bottom slope to leading order, but edge corrections and decaying exterior flow are essential.

##### Potential-vorticity step edge wave

↑ **Parent:** [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)

A positive jump $\Delta Q$ of shallow-water [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) supports a current $U=U_0e^{-|y|/L_R}$ with $U_0=L_R\Delta Q/2$. A disturbance has structure $\phi=Ae^{-\sqrt{k^2+L_R^{-2}}|y|}$. Integrating the linear [potential-vorticity conservation](#potential-vorticity-conservation) equation across the interface gives $(U_0-c)[\phi_y]+\Delta Q\phi(0)=0$, hence the displayed [dispersion relation](wave-equation.md#dispersion-relation). The wave propagates intrinsically against the mean current because the displaced PV interface induces the [velocity](classical-mechanics.md#velocity) that advects it; no planetary beta is required.

##### Barotropic deformation radius

↑ **Parent:** [Shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity)

The barotropic deformation radius is the horizontal scale at which free-surface gravity and rotation balance. It contributes $L_D^{-2}$ to the denominator of the one-layer Rossby-wave dispersion relation.

## Quasi-geostrophic approximation

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasi-geostrophic_approximation)

The quasi-geostrophic approximation describes slowly evolving, nearly geostrophic flow with small Rossby number. Its dynamics are governed by advection and forcing of [potential vorticity](#potential-vorticity).

### Two-layer quasi-geostrophic potential vorticity

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

For equal-depth layers coupled by an interface,

$$
q_1=f+\nabla_h^2\psi_1-F(\psi_1-\psi_2),\qquad q_2=f+\nabla_h^2\psi_2-F(\psi_2-\psi_1),\qquad F=k_I^2.
$$

The [Laplacian](calculus.md#laplacian) terms are relative [vorticity](fluid-mechanics.md#vorticity); the streamfunction differences encode opposite layer-thickness changes. Each [material derivative](continuum-mechanics.md#material-derivative) follows that layer's own velocity. The sum has a [barotropic mode](#barotropic-mode) without interface displacement, while the difference contains a [baroclinic mode](#baroclinic-mode).

#### Two-layer quasi-geostrophic energy conservation

↑ **Parent:** [Two-layer quasi-geostrophic potential vorticity](#two-layer-quasi-geostrophic-potential-vorticity)

For inviscid unforced two-layer QG dynamics, $H_1F_1=H_2F_2=f_0^2/g\prime$ makes the coupling symmetric in the layer-depth inner product. Multiplication by $H_i\psi_i$ gives the positive energy $E=\tfrac12[\sum_iH_i|\nabla\psi_i|^2+(f_0^2/g\prime)(\psi_1-\psi_2)^2]$. It is conserved after integration when the lateral energy flux vanishes. The interface term is [available potential energy](classical-mechanics.md#available-potential-energy); the gradient terms are [kinetic energy](classical-mechanics.md#kinetic-energy).

##### Baroclinic energy ratio and deformation scale

↑ **Parent:** [Two-layer quasi-geostrophic energy conservation](#two-layer-quasi-geostrophic-energy-conservation)

Depth-weighted decomposition gives reduced depth $H_r=H_1H_2/(H_1+H_2)$ and internal radius $R_d^2=g\prime H_r/f_0^2$. On scale $l$, the ratio of interface [available potential energy](classical-mechanics.md#available-potential-energy) to baroclinic [kinetic energy](classical-mechanics.md#kinetic-energy) is of order $(l/R_d)^2$. Comparable depths recover $l^2f_0^2/(g\prime H_i)$; for strongly unequal depths the thinner layer sets the scale.

#### Vortex stretching in layered quasi-geostrophic flow

↑ **Parent:** [Two-layer quasi-geostrophic potential vorticity](#two-layer-quasi-geostrophic-potential-vorticity)

The stretching contribution to upper-layer [potential vorticity](#potential-vorticity) is $-F(\psi_1-\psi_2)$, with the opposite sign below. An interface displacement thickens one layer and thins the other. In a parcel's [potential-vorticity equation](#potential-vorticity-evolution-equation), its material change balances changes of relative and [planetary vorticity](fluid-mechanics.md#planetary-vorticity) and any forcing. The two layer derivatives cannot in general be replaced by one common advection operator.

### Quasi-geostrophic omega equation

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

Define $J(a,b)=a_xb_y-a_yb_x$ and $\zeta=\nabla_h^2\psi$. Combining [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) dynamics with buoyancy evolution eliminates the pressure tendency and gives

$$
N^2\nabla_h^2w+f_0^2w_{zz}=\nabla_h^2R+f_0\beta\psi_{xz}+f_0\left[\partial_zJ(\psi,\zeta)-\nabla_h^2J(\psi,\psi_z)\right].
$$

The beta term remains when the nonlinear terms are omitted. For a steady weak response to heating about rest, $w=R/N^2$ solves this equation using $\beta\psi_x=f_0R_z/N^2$ and suitable no-through-flow and decay conditions.

### Quasi-geostrophic streamfunction

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

The quasi-geostrophic streamfunction defines horizontal velocity by $u=-\psi_y$ and $v=\psi_x$. For a one-layer free-surface model, geostrophic balance gives $\psi=g\eta/f_0$.

### Geostrophic flow

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

A geostrophic flow is a horizontal flow in leading [geostrophic balance](physics.md#geostrophic-balance). Its velocity follows pressure contours rather than pointing directly down the pressure gradient.

#### Strict geostrophic balance

↑ **Parent:** [Geostrophic flow](#geostrophic-flow)

For a homogeneous [incompressible flow](fluid-mechanics.md#incompressible-flow), strict [geostrophic balance](physics.md#geostrophic-balance) means that the [Coriolis acceleration](physics.md#coriolis-acceleration) is exactly balanced by the [pressure gradient](fluid-mechanics.md#pressure-gradient), after conservative body-force potentials have been absorbed into the pressure per unit density $\pi$. It neglects [material acceleration](continuum-mechanics.md#material-acceleration) rather than merely assuming that its size is small. With constant vertical rotation, $\pi_z=0$ and taking the [curl](calculus.md#curl) gives $\mathbf u_z=0$, the [Taylor–Proudman theorem](#taylor-proudman-theorem). Nonzero cross-contour motion over sloping rigid boundaries requires small departures from this strict limit.

### Ageostrophic flow

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

Ageostrophic flow is the part of velocity beyond leading [geostrophic flow](#geostrophic-flow). Its small horizontal divergence supplies vertical motion and the stretching term in the [quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation).

### Three-dimensional quasi-geostrophic potential vorticity

↑ **Parent:** [Quasi-geostrophic approximation](#quasi-geostrophic-approximation)

For constant buoyancy frequency $N$ on a beta plane, three-dimensional quasi-geostrophic potential vorticity can be written

$$
q=\psi_{xx}+\psi_{yy}
+\frac{\partial}{\partial z}
\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y.
$$

#### Reference-buoyancy convention in quasi-geostrophic potential vorticity

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)

The hydrostatic convention $b=f_0\psi_z$ may refer to full [buoyancy](fluid-mechanics.md#buoyancy) or to its anomaly relative to $N^2z$. Subtracting the uniform reference profile changes $\psi$ by $-N^2z^2/(2f_0)$ and changes $q=f_0+\nabla_h^2\psi+(f_0^2/N^2)\psi_{zz}$ by the uniform constant $-f_0$. Horizontal velocity and [potential-vorticity gradients](#potential-vorticity-gradient) are unchanged, so the advection and stability dynamics are identical. Stating the convention avoids mistaking this reference constant for a dynamical gradient.

#### Quasi-geostrophic vertical mode

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)

A quasi-geostrophic vertical mode separates horizontal and vertical dependence of the streamfunction. With rigid horizontal boundaries and constant stratification, the vertical eigenfunctions are $\cos(n\pi z/H)$.

##### Barotropic mode

↑ **Parent:** [Quasi-geostrophic vertical mode](#quasi-geostrophic-vertical-mode)

A barotropic mode has horizontal velocity independent of depth. It is the zeroth [quasi-geostrophic vertical mode](#quasi-geostrophic-vertical-mode) and usually has the largest gravity-wave speed and [Rossby deformation radius](physics.md#rossby-deformation-radius).

##### Baroclinic mode

↑ **Parent:** [Quasi-geostrophic vertical mode](#quasi-geostrophic-vertical-mode)

A baroclinic mode has nontrivial vertical shear and at least one change of vertical structure through the fluid depth. Higher [quasi-geostrophic vertical modes](#quasi-geostrophic-vertical-mode) have smaller gravity-wave speeds and [Rossby deformation radii](physics.md#rossby-deformation-radius).

#### Quasi-geostrophic potential-vorticity equation

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)

The quasi-geostrophic potential-vorticity equation states that [three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) is materially conserved in inviscid, adiabatic flow. On a [beta plane](#beta-plane) with constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency),

$$
\frac{D_g}{Dt}\left(
\nabla_h^2\psi+\frac{f_0^2}{N^2}\psi_{zz}
\right)+\beta\psi_x=0.
$$

##### Topographic buoyancy boundary condition for quasi-geostrophic flow

↑ **Parent:** [Quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation)

For a small steady lower-boundary height $b(x,y)$, impermeability gives $w=\mathbf u_g\cdot\nabla b$ at the reference plane. Substitution in the [buoyancy](fluid-mechanics.md#buoyancy) equation $D_g(f_0\psi_z)+N^2w=0$ yields the displayed [boundary condition](differential-equation.md#boundary-condition). For nonzero Fourier modes in a uniform crossing current, this fixes $\psi_z(0)=-N^2b/f_0$. An upper [radiation condition](gravity-wave.md#radiation-condition) or decay condition is still needed to select the physical response.

##### Rigid-boundary buoyancy condition for quasi-geostrophic waves

↑ **Parent:** [Quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation)

With basic zonal velocity $U(z)$, basic horizontal [buoyancy](fluid-mechanics.md#buoyancy) gradient $b_y=-f_0U_z$, and $b'=f_0\psi'_z$, adiabatic buoyancy evolution at a flat impermeable wall gives

$$
(\partial_t+U\partial_x)\psi'_z-U_z\psi'_x=0.
$$

A [normal mode](wave-equation.md#normal-mode) thus obeys $(U-c)\widehat\psi'-U_z\widehat\psi=0$ at the wall. This dynamical condition, rather than vanishing streamfunction, sets the frequency of an [Eady edge wave](hydrodynamic-stability.md#eady-edge-wave).

##### Diabatically forced quasi-geostrophic potential vorticity

↑ **Parent:** [Quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation)

For a [Boussinesq approximation](#boussinesq-approximation), constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, and [buoyancy](fluid-mechanics.md#buoyancy) heating rate $R$, the [quasi-geostrophic potential-vorticity equation](#quasi-geostrophic-potential-vorticity-equation) becomes $D_gq/Dt=(f_0/N^2)R_z$, where $q=\nabla_h^2\psi+(f_0^2/N^2)\psi_{zz}+\beta y$. Heating changes the vertical gradient of buoyancy and therefore produces a potential-vorticity tendency proportional to its height derivative.

###### Harmonic heating response of quasi-geostrophic flow

↑ **Parent:** [Diabatically forced quasi-geostrophic potential vorticity](#diabatically-forced-quasi-geostrophic-potential-vorticity)

For constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency), [density](fluid-mechanics.md#density) forcing $r_0e^{-\mu z}\cos kx\cos\omega_0t$ gives two frequencies $\omega=\pm\omega_0$. The [quasi-geostrophic streamfunction](#quasi-geostrophic-streamfunction) satisfies $\lambda_\omega^2=(N^2/f_0^2)(k^2+\beta k/\omega)$ and $C_\omega=ig\mu r_0/(2\rho_0f_0\omega)$. With zero [streamfunction](fluid-mechanics.md#stream-function) at the bottom, a positive $\lambda_\omega^2$ selects the decaying solution $C_\omega(e^{-\mu z}-e^{-\lambda_\omega z})/(\mu^2-\lambda_\omega^2)$. For $\beta,k>0$, the westward branch propagates vertically when $\omega_0<\beta/k$; a [radiation condition](gravity-wave.md#radiation-condition) selects positive vertical [group velocity](wave-equation.md#group-velocity), not merely bounded amplitude. Coincident exponential exponents are handled by the finite limit $-C_\omega z e^{-\mu z}/(2\mu)$.

###### Steady quasi-geostrophic response to localized heating

↑ **Parent:** [Diabatically forced quasi-geostrophic potential vorticity](#diabatically-forced-quasi-geostrophic-potential-vorticity)

In the weak-forcing steady response about rest, [diabatically forced quasi-geostrophic potential vorticity](#diabatically-forced-quasi-geostrophic-potential-vorticity) gives $\beta\psi_x=(f_0/N^2)R_z$. For $\beta\ne0$, an eastern zero-flow condition fixes the horizontal circulation through $\psi=-(f_0/\beta N^2)\int_x^\infty R_z\,dX$, up to a horizontally uniform pressure gauge. The thermodynamic equation gives $w=R/N^2$. A western zonal wake can remain even though the heating and vertical velocity vanish there. This is a formal steady interior solution: specified initial boundary buoyancy can prevent it from being the attained steady state. For example, under a rigid lid where the heating vanishes, initially uniform boundary buoyancy remains uniform at linear order.

#### Log-pressure quasi-geostrophic potential vorticity

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)

In a [log-pressure coordinate](#log-pressure-coordinate), [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity) uses density-weighted vertical stretching. For stratification $N^2=RS/H$ and [geostrophic flow](#geostrophic-flow) $\mathbf u_g=(-\psi_y,\psi_x,0)$, the inviscid equation is $D_gq/Dt=0$. Combining horizontal [vorticity](fluid-mechanics.md#vorticity) balance with the thermal equation eliminates [ageostrophic flow](#ageostrophic-flow) and gives this conservation law.

##### Vertical-advection consistency criterion for log-pressure quasi-geostrophy

↑ **Parent:** [Log-pressure quasi-geostrophic potential vorticity](#log-pressure-quasi-geostrophic-potential-vorticity)

For scales $U,L,D$, thermal balance estimates $w\sim f_0U^2/(N^2D)$. Density-weighted continuity gives horizontal [ageostrophic flow](#ageostrophic-flow) of order $Lw/\min(D,H)$. It is small relative to $U$ only if

$$
\epsilon_a=\frac{f_0^2L^2}{N^2D\min(D,H)}\frac{U}{|f_0|L}\ll1.
$$

This condition supplements small [Rossby number](#rossby-number) and small relative variation $\beta L/|f_0|$ of the [Coriolis parameter](#coriolis-parameter).

#### Isopycnal displacement

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isopycnal_displacement)

An isopycnal displacement is the vertical displacement $\xi$ of a constant-density surface. In linear stratified quasi-geostrophic flow,

$$
\xi=-\frac{f_0}{N^2}\psi_z.
$$

#### Quasi-geostrophic mountain wave

↑ **Parent:** [Three-dimensional quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity)

A quasi-geostrophic mountain wave is a stationary [Rossby wave](#rossby-wave) forced when a geostrophic basic flow crosses topography. Its vertical wavenumber is real only when the intrinsic Rossby-wave phase speed permits vertical propagation.

##### Resonant topographic quasi-geostrophic wave

↑ **Parent:** [Quasi-geostrophic mountain wave](#quasi-geostrophic-mountain-wave)

A stationary boundary corrugation can resonate with a [Rossby wave](#rossby-wave) whose intrinsic propagation cancels the background current. For constant $N$, rigid upper height $H$, and $m=\pi/H$, define $\kappa^2=k^2+\ell^2+f_0^2m^2/N^2$. When $U=\beta/\kappa^2$, a lower corrugation proportional to $e^{ikx}\sin(\ell y)$ admits a disturbance proportional to $e^{ikx}\sin(\ell y)[Bt\cos(mz)+C(z-H)\sin(mz)]$, with $B=2ikf_0U^2/\beta$ and $C=N^2/(f_0m)$. Its [wave activity](#wave-activity) grows quadratically with time while the upward [Eliassen–Palm flux](#eliassen-palm-flux) grows linearly. The linear prediction applies only while the disturbance remains small.

###### Phase of a resonantly forced topographic edge wave

↑ **Parent:** [Resonant topographic quasi-geostrophic wave](#resonant-topographic-quasi-geostrophic-wave)

For constant stratification and $U=U_0+\Lambda z$, a decaying zero-interior-PV mode has vertical structure $e^{-Kz}$. Its topographic [boundary condition](differential-equation.md#boundary-condition) gives $A'+ik(U_0+\Lambda/K)A=ik\epsilon N^2U_0/(Kf)$. Resonance requires $KU_0+\Lambda=0$ and nonzero forcing $k\epsilon U_0$. With zero initial disturbance, $A$ grows linearly and is imaginary relative to cosine topography. Its meridional [velocity](classical-mechanics.md#velocity) is therefore opposite in phase to the relief for positive $f,U_0,\epsilon$. A zero zonal [wavenumber](wave-equation.md#wavenumber) or zero boundary current removes the forcing and invalidates an unconditional claim of secular growth.

##### Thermally damped quasi-geostrophic mountain wave

↑ **Parent:** [Quasi-geostrophic mountain wave](#quasi-geostrophic-mountain-wave)

Thermal damping makes the vertical wavenumber of a stationary topographic [Rossby wave](#rossby-wave) complex. A vertically propagating wave then decays while oscillating, whereas an inviscidly evanescent disturbance acquires both decay and phase tilt; both can exert wave drag.

## Geostrophic adjustment

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geostrophic_adjustment)

Geostrophic adjustment is the radiation of inertia-gravity waves from an unbalanced disturbance, leaving a slower flow in [geostrophic balance](physics.md#geostrophic-balance) while conserving linearized [potential vorticity](#potential-vorticity).

### Geostrophic adjustment of a Gaussian height ridge

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

An initially resting, along-ridge-uniform [shallow water](physics.md#shallow-water-approximation) layer with height disturbance $\zeta_0(x)$ conserves $q-f\zeta/h=-f\zeta_0/h$. Its balanced remainder satisfies the displayed [modified Helmholtz equation](partial-differential-equation.md#modified-helmholtz-equation), with $R_D=\sqrt{gh}/f$. On the infinite line,

$$
\zeta_s(x)=\frac1{2R_D}\int_{\mathbb R}e^{-|x-x'|/R_D}\zeta_0(x')\,dx',\qquad u_s=0,\quad v_s=\frac gf\zeta_s'.
$$

For each [Fourier transform](analysis.md#fourier-transform) component, $\widehat\zeta(t)=\widehat\zeta_s+(\widehat\zeta_0-\widehat\zeta_s)\cos(\sqrt{f^2+ghk^2}\,t)$. The oscillatory part is [inertia-gravity waves](#inertia-gravity-wave). For a localized [Gaussian function](calculus.md#gaussian-function) on the infinite line those waves spread away, leaving the steady component locally; a reflecting finite basin generally retains oscillations.

### Geostrophic adjustment of a finite-width height ramp

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

For an initially resting [shallow water](physics.md#shallow-water-approximation) layer whose height rises linearly from $-h$ to $h$ across $(-L,L)$, let $R_d=\sqrt{gH}/|f|$ and $\alpha=L/R_d$. Conserved linear [shallow-water potential vorticity](#shallow-water-potential-vorticity) gives $R_d^2\eta_s''-\eta_s=-\eta_0$. Boundedness, oddness, and continuity of height and slope give $\eta_s/h=x/L-e^{-\alpha}\sinh(x/R_d)/\alpha$ inside the ramp, and $\eta_s/h=\operatorname{sgn}(x)[1-(\sinh\alpha/\alpha)e^{-|x|/R_d}]$ outside. The balanced [velocity](classical-mechanics.md#velocity) is $u_s=0$, $v_s=g\eta_s'/f$. Narrow ramps spread over the [Rossby deformation radius](physics.md#rossby-deformation-radius); wide ramps retain their initial height except for narrow matching layers.

### Coastal adjustment of an elevated strip

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

For a resting shallow-water strip $-L<x<0$ adjacent to an impermeable coast, conserved linear [potential vorticity](#potential-vorticity) gives $a^2\eta_{xx}-\eta=-\eta_{\rm initial}$. Decay offshore, matching and conserved volume give $\eta=\eta_0e^{x/a}\sinh(L/a)$ outside the strip and $\eta=\eta_0[1-e^{-L/a}\cosh(x/a)]$ inside it. The adjusted velocity is $v=g\eta_x/f$, with zero tangential wall velocity inherited from initial rest and alongshore uniformity.

### Balanced shallow-water energy as a signed potential-vorticity pairing

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

With constant density divided out, a decaying or periodic [geostrophic balance](physics.md#geostrophic-balance) on an [f-plane](#f-plane) has

$$
E_b=\frac12\int(H|\mathbf u_g|^2+g\eta^2)\,dA=-\frac{gH}{2f}\int\eta q\,dA,
$$

where $q=\zeta-f\eta/H$ is the signed [linearized shallow-water potential-vorticity anomaly](#linearized-shallow-water-potential-vorticity-anomaly). The stationary height equation and [integration by parts](calculus.md#integration-by-parts) prove the identity. Replacing $q$ by $|q|$ destroys it: an odd height paired with symmetric opposite-sign sheets would then misleadingly give zero.

### Geostrophic adjustment of a finite-width current

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

An initial current $U\mathbf1_{|y|<a}$ with flat surface has two oppositely signed [vortex sheets](fluid-mechanics.md#vortex-sheet). On an [f-plane](#f-plane), its local final [geostrophic balance](physics.md#geostrophic-balance) has

$$
\frac{\eta_f}H=-\frac{U}{2c}\left(e^{-|y-a|/\lambda}-e^{-|y+a|/\lambda}\right),\qquad \lambda=\frac cf,\quad c^2=gH.
$$

The [Rossby deformation radius](physics.md#rossby-deformation-radius) controls the edge layers. The height is continuous and odd; the along-strip velocity is $-g\eta_f'/f$ and has the sheet jumps. Outgoing [inertia-gravity waves](#inertia-gravity-wave) carry the energy not retained in this balanced component.

#### Energy retention in finite-width geostrophic adjustment

↑ **Parent:** [Geostrophic adjustment of a finite-width current](#geostrophic-adjustment-of-a-finite-width-current)

For an initially uniform strip current of half-width $a$, the final balanced energy fraction is

$$
\frac{E_b}{E_i}=\frac{1-e^{-2r}}{2r},\qquad r=\frac a\lambda.
$$

The fraction tends to $1-r+O(r^2)$ for a narrow strip and to $1/(2r)$ for a wide strip. The difference is outgoing [inertia-gravity wave](#inertia-gravity-wave) energy, consistent with [conservation of energy](physics.md#conservation-of-energy); the infinite-strip energies are interpreted per unit along-strip length.

### Geostrophic adjustment of a surface-height jump

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)

A constant-depth layer initially at rest with a step in its [free surface](fluid-mechanics.md#free-surface) adjusts by radiating [inertia-gravity waves](#inertia-gravity-wave). Conservation of linearized [shallow-water potential vorticity](#shallow-water-potential-vorticity) leaves the bounded balanced profile $\eta_s=\eta_0\operatorname{sgn}(x)(1-e^{-|x|/R_D})$, where $R_D=\sqrt{gH}/|f|$ is the [Rossby deformation radius](physics.md#rossby-deformation-radius). The released [potential energy](classical-mechanics.md#potential-energy) per unit transverse length is $3\rho g\eta_0^2R_D/2$; the final [kinetic energy](classical-mechanics.md#kinetic-energy) is $\rho g\eta_0^2R_D/2$, leaving $\rho g\eta_0^2R_D$ in radiated waves.

### Inertia-gravity wave

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inertia-gravity_wave)

An inertia-gravity wave is restored jointly by buoyancy or free-surface gravity and the Coriolis force.

#### Linear pressure equation for rotating stratified flow

↑ **Parent:** [Inertia-gravity wave](#inertia-gravity-wave)

With downward buoyancy $b=g\rho\prime/\rho_0$ in a uniform rotating [Boussinesq approximation](#boussinesq-approximation), $q=\zeta-fb_z/N^2$ is time-independent. The linear pressure obeys $\nabla^2p_{tt}+f^2p_{zz}+N^2\nabla_H^2p=\rho_0fN^2q$. The initial [potential vorticity](#potential-vorticity) supplies the steady pressure source; nonzero-frequency [inertia-gravity waves](#inertia-gravity-wave) have zero perturbation PV.

#### Particle ellipses for rotating shallow-water waves

↑ **Parent:** [Inertia-gravity wave](#inertia-gravity-wave)

For a plane [inertia-gravity wave](#inertia-gravity-wave) on a resting layer, $\eta=\eta_0\cos(kx-\omega t)$, the horizontal velocities are $u=U\cos\theta$ and $v=V\sin\theta$, where $U=\omega\eta_0/(kh_0)$ and $V=f\eta_0/(kh_0)$. First-order integration at a fixed equilibrium coordinate gives $\xi=-U\sin\theta/\omega$, $\upsilon=V\cos\theta/\omega$. The particle trajectory is an [ellipse](geometry-and-topology.md#ellipse) with axis ratio $|f|/\omega$. For positive $f$, the orbit is clockwise in the $(x,y)$ plane.

#### External gravity wave

↑ **Parent:** [Inertia-gravity wave](#inertia-gravity-wave)

An external gravity wave displaces a fluid's [free surface](fluid-mechanics.md#free-surface) and moves nearly uniformly through the depth in the long-wave limit. In a layer of depth $H$, its leading [shallow-water approximation](physics.md#shallow-water-approximation) speed is $\sqrt{gH}$.

#### Linear rotating shallow-water dispersion relation

↑ **Parent:** [Inertia-gravity wave](#inertia-gravity-wave)

On an [f-plane](#f-plane), linear shallow-water plane waves have one zero-frequency geostrophic mode and two inertia-gravity modes with $\omega^2=f^2+c^2(k^2+l^2)$. The crossover scale $c/|f|$ is the [barotropic deformation radius](#barotropic-deformation-radius).

### Kelvin wave

↑ **Parent:** [Geostrophic adjustment](#geostrophic-adjustment)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kelvin_wave)

A coastal Kelvin wave is trapped within a [Rossby deformation radius](physics.md#rossby-deformation-radius) of a boundary. It propagates with the boundary on its right in the Northern Hemisphere and on its left in the Southern Hemisphere, and its linear shallow-water potential-vorticity anomaly vanishes.

#### Kelvin-wave channel invariant

↑ **Parent:** [Kelvin wave](#kelvin-wave)

Exponentially weighted cross-channel integrals of velocity and pressure isolate the two oppositely propagating boundary Kelvin waves. Their conserved characteristic amplitudes supply the two integral constraints missing from a channel geostrophic-adjustment problem.

## Ocean circulation

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ocean_circulation)

Ocean circulation comprises wind-driven, buoyancy-driven, and tidal motions of the ocean over a wide range of spatial and temporal scales.

### Antarctic Convergence

↑ **Parent:** [Ocean circulation](#ocean-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antarctic_Convergence)

### Antarctic Coastal Current

↑ **Parent:** [Ocean circulation](#ocean-circulation)

The Antarctic Coastal Current is a mainly westward flow near the Antarctic coast. It can transport [icebergs](geophysics.md#iceberg) along the continental margin; coastal geometry, winds and regional circulation make trajectories variable.

### Antarctic Circumpolar Current

↑ **Parent:** [Ocean circulation](#ocean-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antarctic_Circumpolar_Current)

### Antarctic bottom water

↑ **Parent:** [Ocean circulation](#ocean-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antarctic_bottom_water)

Antarctic bottom water is a dense southern-origin water mass that ventilates much of the abyssal ocean. Cooling and [brine rejection](geophysics.md#brine-rejection) form dense shelf water; its descent and mixing with adjacent waters contribute to Antarctic bottom water production. Shelf production is geographically concentrated and does not mean that every [polynya](geophysics.md#polynya) exports water to the abyss.

### Wind stress

↑ **Parent:** [Ocean circulation](#ocean-circulation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wind_stress)

Wind stress is the tangential traction exerted by the atmosphere on the ocean surface. Its curl injects vorticity into the ocean.

#### Wind stress curl

↑ **Parent:** [Wind stress](#wind-stress)

The vertical [curl](calculus.md#curl) of surface [wind stress](#wind-stress) is $(\nabla_h\times\boldsymbol\tau)_z=\tau_{y,x}-\tau_{x,y}$. In a layer of density $\rho_0$ and depth $h$, its normalized [potential vorticity](#potential-vorticity) source is $W=(\nabla_h\times\boldsymbol\tau)_z/(\rho_0h)$. It drives [Sverdrup balance](#sverdrup-balance) in the weakly nonlinear steady ocean interior.

#### Ekman layer

↑ **Parent:** [Wind stress](#wind-stress)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ekman_layer)

An Ekman layer is a viscous boundary layer in a rotating fluid. For constant [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$ and [Coriolis parameter](#coriolis-parameter) $f$, its characteristic thickness is $\delta_E=\sqrt{2\nu/|f|}$, and its velocity turns with distance from the boundary.

##### Laminar Ekman boundary stress

↑ **Parent:** [Ekman layer](#ekman-layer)

For $f>0$, a stationary lower [no-slip boundary condition](viscous-fluid-flow.md#no-slip-boundary-condition) below uniform exterior [geostrophic flow](#geostrophic-flow) $W_g$ produces $W_E=-W_g e^{-(1+i)z/\delta_E}$. The upward shear component at the bottom is $T_b=\rho\nu W_E^{\prime}(0)=\rho\sqrt{f\nu/2}(1+i)W_g$; the bottom traction on the fluid is $-T_b$. This law cannot be assigned to an arbitrary prescribed surface [wind stress](#wind-stress) without an additional boundary condition.

##### Surface Ekman layer

↑ **Parent:** [Ekman layer](#ekman-layer)

A surface [Ekman layer](#ekman-layer) is the stress-driven boundary correction below a rotating fluid’s upper boundary. For upward $z\le0$, $f>0$, constant [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) and imposed complex [wind stress](#wind-stress) $T$, its steady velocity is $W_E=T e^{\lambda z}/(\rho\nu\lambda)$, $\lambda=(1+i)/\delta_E$. The underlying [geostrophic flow](#geostrophic-flow) is independent of $T$ unless an additional boundary velocity condition couples them.

##### Bottom Ekman layer

↑ **Parent:** [Ekman layer](#ekman-layer)

A viscous no-slip boundary below a geostrophic current creates a bottom Ekman layer of thickness $\delta=(2\nu/|f|)^{1/2}$. Its depth-integrated ageostrophic transport has a component opposite the geostrophic current and a transverse component set by the sign of $f$.

#### Ekman transport

↑ **Parent:** [Wind stress](#wind-stress)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ekman_transport)

Ekman transport is the depth-integrated ageostrophic flow in a frictional rotating boundary layer. Beneath a surface stress $\boldsymbol\tau$,

$$
\mathbf M_E=\frac{\boldsymbol\tau\times\widehat{\mathbf z}}{\rho f}
$$

with the stated orientation convention.

##### Ekman pumping

↑ **Parent:** [Ekman transport](#ekman-transport)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ekman_pumping)

Spatial convergence or divergence of [Ekman transport](#ekman-transport) drives vertical motion at the base of the Ekman layer. With upward vertical coordinate,

$$
w_E=\widehat{\mathbf z}\mathbin\cdot
\nabla\times\left(\frac{\boldsymbol\tau}{\rho f}\right).
$$

###### Ekman spin-down in a shallow-water layer

↑ **Parent:** [Ekman pumping](#ekman-pumping)

In a thin [Bottom Ekman layer](#bottom-ekman-layer), slowly evolving [geostrophic flow](#geostrophic-flow) drives upward [Ekman pumping](#ekman-pumping) into a uniform-depth exterior layer. With $f>0$, $\alpha=\sqrt{f\nu/2}$ and $R_D=\sqrt{gH}/f$, its balanced height satisfies $(\nabla_h^2-R_D^{-2})\eta_t=-(\alpha/H)\nabla_h^2\eta$. Small-scale [Fourier modes](fourier-analysis.md#fourier-mode) decay on $H/\alpha$; large-scale modes obey a [diffusion equation](diffusion-equation.md) with diffusivity $g\alpha/f^2$. The balanced approximation requires $|f|\tau\gg1$.

###### Quasi-geostrophic Ekman spin-down

↑ **Parent:** [Ekman pumping](#ekman-pumping)

Bottom [Ekman pumping](#ekman-pumping) damps a horizontal quasi-geostrophic Fourier mode while its influence penetrates vertically only over $|f|/(Nk)$. For a half-space with a vertically uniform initial mode, the boundary amplitude decays exponentially while the remote interior remains unchanged.

#### Ocean gyre

↑ **Parent:** [Wind stress](#wind-stress)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ocean_gyre)

An ocean gyre is a basin-scale rotating circulation driven principally by wind stress and shaped by planetary rotation and boundaries.

##### Sverdrup balance

↑ **Parent:** [Ocean gyre](#ocean-gyre)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sverdrup_balance)

Sverdrup balance equates meridional advection of planetary vorticity to wind-stress curl in the weakly frictional ocean interior.

###### Ocean basin equation with bottom drag and lateral viscosity

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

With depth transport $(-\psi_y,\psi_x)$ and a depth-mean bottom-drag closure, the wind-driven equation is $\beta\psi_x=S-r\nabla^2\psi+\nu\nabla^4\psi$, where $S$ is wind-stress curl divided by density and $r=\gamma/(\rho_0H)$ is the drag rate. Its zonal boundary modes solve $\nu\lambda^3-r\lambda-\beta=0$. The [Munk boundary layer](#munk-boundary-layer) and [Stommel boundary layer](#stommel-boundary-layer) are different limits of this combined equation.

###### Drag-dominated basin solution with no-slip layers

↑ **Parent:** [Ocean basin equation with bottom drag and lateral viscosity](#ocean-basin-equation-with-bottom-drag-and-lateral-viscosity)

If $r^3\gg\beta^2\nu$, the broad western [Stommel boundary layer](#stommel-boundary-layer) has thickness $r/\beta$, but small viscosity supplies no-slip skins of thickness $(\nu/r)^{1/2}$ at both east and west walls. The western solution therefore contains two decaying exponentials, while the east has the rapidly decaying skin. Setting viscosity identically to zero removes the modes needed to satisfy all four lateral no-slip conditions.

###### Two-layer Sverdrup interior

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

For a uniform normalized upper-layer [wind stress curl](#wind-stress-curl) $W$ and no lower-layer forcing, a uniform local [Sverdrup balance](#sverdrup-balance) is

$$
\bar\psi_1=Vx,\quad\bar\psi_2=0,\quad V=W/\beta.
$$

The upper layer flows meridionally and the lower layer rests. Although the relative [vorticity](fluid-mechanics.md#vorticity) vanishes, the [potential vorticity](#potential-vorticity) has the zonal gradients $\bar q_{1,x}=-FV$, $\bar q_{2,x}=FV$. These are essential for the perturbation stability and do not vanish merely because the background velocity is uniform.

###### Linear stability of a meridional two-layer current

↑ **Parent:** [Two-layer Sverdrup interior](#two-layer-sverdrup-interior)

Let $K^2=k^2+l^2$, $A=K^2+F$, $\mathcal B=K^2(K^2+2F)$ and use $e^{i(kx+ly-\sigma t)}$. The uniform upper-layer flow $V$ over a resting lower layer has the [dispersion relation](wave-equation.md#dispersion-relation)

$$
\mathcal B\sigma^2+[2A\beta k-\mathcal B lV]\sigma+\beta^2k^2-A\beta klV+FK^2l^2V^2=0.
$$

Its discriminant is $4F^2\beta^2k^2+\mathcal B K^2(K^2-2F)l^2V^2$. A negative value gives exponential [baroclinic instability](hydrodynamic-stability.md#baroclinic-instability). This model includes advection across the interface-induced [potential-vorticity gradients in a meridional two-layer current](#potential-vorticity-gradients-in-a-meridional-two-layer-current).

###### Meridional-wave instability of a two-layer Sverdrup flow

↑ **Parent:** [Linear stability of a meridional two-layer current](#linear-stability-of-a-meridional-two-layer-current)

For purely meridional [wavevectors](continuum-mechanics.md#wavevector), $k=0$, $l\ne0$, the growth rate of a uniform meridional upper-layer flow $V$ over a resting lower layer is

$$
\gamma=\frac{|lV|}{2}\sqrt{\frac{2F-l^2}{l^2+2F}}.
$$

Growth requires $V\ne0$ and $0<l^2<2F$. The perturbation has no northward velocity, so [planetary vorticity](fluid-mechanics.md#planetary-vorticity) advection does not explicitly stabilize it. At fixed normalized [wind stress curl](#wind-stress-curl), $V=W/\beta$ means stronger $|\beta|$ nevertheless reduces the shear and growth rate.

###### Potential-vorticity gradients in a meridional two-layer current

↑ **Parent:** [Two-layer Sverdrup interior](#two-layer-sverdrup-interior)

For $\bar\psi_1=Vx$ and $\bar\psi_2=0$, the [two-layer quasi-geostrophic potential vorticity](#two-layer-quasi-geostrophic-potential-vorticity) is $\bar q_1=f_0+\beta y-FVx$, $\bar q_2=f_0+\beta y+FVx$. A perturbation therefore feels both the northward gradient $\beta$ and opposite zonal gradients $\mp FV$. Dropping the zonal gradients removes the instability mechanism from the linearization.

<h6 id="point-forced-sverdrup-drag-green-function">Point-forced Sverdrup–drag Green function</h6>

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

The unbounded constant-depth steady transport response to a unit point wind-curl source solves $r\nabla_h^2\psi+\beta\psi_x=H\delta(x)\delta(y)$ for $r,\beta>0$. An exponential substitution reduces it to a modified Helmholtz equation, yielding the expression shown in terms of the [Modified Bessel function of the second kind](analysis.md#modified-bessel-function-of-the-second-kind). Its finite-level [streamfunction](fluid-mechanics.md#stream-function) contours are nearly circular near the source and stretched into a western wake far away. The wake width is of order $\sqrt{(r/\beta)|x|}$.

###### Ocean transport streamfunction

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

An ocean transport streamfunction defines depth-integrated horizontal transport. For constant depth $H$, it is $H$ times the velocity [streamfunction](fluid-mechanics.md#stream-function). Its difference between two boundaries gives signed transport across a connecting line.

###### Relative vorticity from a variable-depth transport streamfunction

↑ **Parent:** [Ocean transport streamfunction](#ocean-transport-streamfunction)

The [ocean transport streamfunction](#ocean-transport-streamfunction) convention $Hu=-\psi_y$, $Hv=\psi_x$ gives [relative vorticity](fluid-mechanics.md#relative-vorticity) $\zeta=H^{-1}\nabla^2\psi-H^{-2}\nabla H\cdot\nabla\psi$. This identity is exact for variable positive depth and does not assume that depth variations are small.

###### Godfrey island rule

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

For an island in a constant-depth ocean with [Sverdrup balance](#sverdrup-balance), choose a counterclockwise contour running from the island's southern tip east to the basin wall, north along that wall, west to the northern tip, and south along the island's western coast. If that contour avoids dissipative boundary layers, the [ocean transport streamfunction](#ocean-transport-streamfunction) on the island is

$$
\psi_I=-\frac H{f(y_N)-f(y_S)}\oint_C\mathbf W\cdot d\mathbf l.
$$

Here $\mathbf W$ is the wind acceleration appearing in the depth-averaged momentum equation. The basin-boundary streamfunction is zero. This integral fixes the otherwise undetermined constant on the island without requiring a friction law, as in [Godfrey's original island-circulation model](https://doi.org/10.1080/03091928908208894).

###### Topographic Sverdrup balance

↑ **Parent:** [Sverdrup balance](#sverdrup-balance)

When depth varies but the [Coriolis parameter](#coriolis-parameter) is constant, forcing can balance advection of $f/H$ rather than advection of planetary vorticity. This topographic potential-vorticity gradient plays the role normally played by the beta effect.

###### Wind-driven circulation over parabolic basin topography

↑ **Parent:** [Topographic Sverdrup balance](#topographic-sverdrup-balance)

With $f=f_0+\beta y$ and parabolic depth, the [topographic potential-vorticity pseudovelocity](#topographic-potential-vorticity-pseudovelocity) is $(-\beta/H,-fH_x/H^2)$. For positive $f,\beta$, it points west and turns south on the western slope, north on the eastern slope. Its characteristics are the parabolas $y=Qa x(L_x-x)/\beta-f_0/\beta$, where $Q=f/H$. Wind-driven [ocean gyres](#ocean-gyre) are steered by these depth gradients; drag and boundary data determine the actual [ocean transport streamfunction](#ocean-transport-streamfunction). The zero-depth shoreline is a singular limit that requires a separate physical regularization.

###### Topographic potential-vorticity pseudovelocity

↑ **Parent:** [Topographic Sverdrup balance](#topographic-sverdrup-balance)

In the steady small-[Rossby number](#rossby-number) transport equation, this coefficient field advects the [ocean transport streamfunction](#ocean-transport-streamfunction) along contours of background [shallow-water potential vorticity](#shallow-water-potential-vorticity) $f/H$. It is not a physical velocity: when $\psi$ has units of volume transport, its units are inverse length squared per time. For uniform depth on a [beta plane](#beta-plane) it points westward, $\widetilde{\mathbf u}=(-\beta/H,0)$. With no forcing or drag, $\psi$ is constant on each connected characteristic; locally $\psi=\Phi(f/H)$ at regular points.

###### Topographic potential-vorticity steering

↑ **Parent:** [Topographic Sverdrup balance](#topographic-sverdrup-balance)

In a slowly varying inviscid layer, parcels tend to follow contours of $f/H$. If depth increases in the direction of motion, conservation of [potential vorticity](#potential-vorticity) requires a poleward displacement or a compensating change of relative vorticity. Ekman pumping permits streamlines to cross those contours.

##### Western boundary current

↑ **Parent:** [Ocean gyre](#ocean-gyre)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Western_boundary_current)

A western boundary current is a narrow, intense return flow that closes a broad wind-driven interior circulation. The beta effect selects the western side for this frictional boundary layer.

###### Stommel boundary layer

↑ **Parent:** [Western boundary current](#western-boundary-current)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stommel_boundary_layer)

The Stommel boundary layer closes a Sverdrup interior using linear drag. Balancing beta-effect advection against drag gives width

$$
\delta=\frac{\gamma f_0}{\beta}
$$

for the normalization in which quasi-geostrophic drag is $-\gamma\nabla^2\psi$.

###### Munk boundary layer

↑ **Parent:** [Western boundary current](#western-boundary-current)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Munk_boundary_layer)

A Munk boundary layer closes a [Sverdrup balance](#sverdrup-balance) interior using lateral viscosity. At a zonal wall, balancing $\beta\psi_x$ with $\nu\nabla^4\psi$ gives the width $(\nu/\beta)^{1/3}$.

## Rossby wave

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rossby_wave)

A Rossby wave is a low-frequency wave restored by the spatial variation of planetary or background potential vorticity. On a beta plane its phase commonly propagates westward.

### Rossby-wave equation for a sheared zonal current

↑ **Parent:** [Rossby wave](#rossby-wave)

Linearizing [shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity) about a zonal current $U(y)$ gives $Q_y=\beta-U^{\prime\prime}+U/R_D^2$. A normal mode $\widehat\phi(y)e^{i(kx-\omega t)}$ obeys $(U-\omega/k)[\widehat\phi^{\prime\prime}-(k^2+R_D^{-2})\widehat\phi]+Q_y\widehat\phi=0$. A global transverse [plane wave](quantum-mechanics.md#plane-wave) is generally unavailable for an arbitrary nonuniform jet; boundary conditions or a local short-wavelength approximation are required.

#### Local Rossby-wave dispersion relation in a zonal jet

↑ **Parent:** [Rossby-wave equation for a sheared zonal current](#rossby-wave-equation-for-a-sheared-zonal-current)

When a zonal current varies slowly compared with the wavelength, freeze its velocity and background [potential vorticity](#potential-vorticity) gradient locally in the [Rossby-wave equation for a sheared zonal current](#rossby-wave-equation-for-a-sheared-zonal-current). The resulting local [dispersion relation](wave-equation.md#dispersion-relation) includes curvature $U^{\prime\prime}$ and, for a free surface, the basic surface-slope contribution $U/R_D^2$. In the nondivergent limit it becomes $\omega=kU-k(\beta-U^{\prime\prime})/(k^2+l^2)$.

##### Stationary Rossby waves in a sinusoidal zonal jet

↑ **Parent:** [Local Rossby-wave dispersion relation in a zonal jet](#local-rossby-wave-dispersion-relation-in-a-zonal-jet)

For a sinusoidal mean jet on an $f$ plane, its QG potential-vorticity gradient is $(\pi^2/L^2+k_d^2)U$. Ground-stationary modes satisfy the displayed circle and can solve the full stationary shear equation even though their scale does not meet a local short-wave assumption. The local stationary group vector is $2Uk(k,l)/(k^2+l^2+k_d^2)$, reducing to a zonal scalar formula only for $l=0$.

### Linear Rossby-wave equation

↑ **Parent:** [Rossby wave](#rossby-wave)

For a mode with streamfunction $\phi$, deformation radius $L_D$, and constant planetary-vorticity gradient $\beta$, the linear Rossby-wave equation is

$$
\partial_t(\nabla_h^2\phi-L_D^{-2}\phi)+\beta\phi_x=F.
$$

In the long-wave limit it becomes a first-order westward transport equation.

#### Shallow-water Rossby-wave dispersion relation

↑ **Parent:** [Linear Rossby-wave equation](#linear-rossby-wave-equation)

For a resting midlatitude layer, the slow [Rossby wave](#rossby-wave) equation is $(\nabla_h^2-a^2)\eta_t=-\beta\eta_x$, where $a=f_0/\sqrt{gH}$. With the [plane wave](quantum-mechanics.md#plane-wave) convention $e^{i(kx+ly-\omega t)}$,

$$
\omega=-\frac{\beta k}{k^2+l^2+a^2}.
$$

The zonal [phase velocity](wave-equation.md#phase-velocity) is westward for $\beta>0$, but the zonal [group velocity](wave-equation.md#group-velocity) changes sign at $k^2=l^2+a^2$.

##### Reflection of a Rossby wave at a meridional wall

↑ **Parent:** [Shallow-water Rossby-wave dispersion relation](#shallow-water-rossby-wave-dispersion-relation)

A stationary straight meridional wall preserves frequency and tangential wavenumber $l$. The two normal wavenumbers obey

$$
k_i k_r=l^2+a^2,\qquad k_i+k_r=-\frac\beta\omega.
$$

Incidence and reflection are distinguished by the normal [group velocity](wave-equation.md#group-velocity). In the leading [quasi-geostrophic approximation](#quasi-geostrophic-approximation), a nonzero $l$ and the [impermeability condition](viscous-fluid-flow.md#no-penetration-boundary-condition) give reflected height amplitude $A_r=-A_i$. The $l=0$ no-normal-flow condition is degenerate in that reduced model; exact ageostrophic transport generally changes the amplitude ratio.

##### Rossby-wave isofrequency circle

↑ **Parent:** [Shallow-water Rossby-wave dispersion relation](#shallow-water-rossby-wave-dispersion-relation)

The [wavevectors](continuum-mechanics.md#wavevector) of a nonzero-frequency [Rossby wave](#rossby-wave) in a resting shallow layer satisfy

$$
\left(k+\frac\beta{2\omega}\right)^2+l^2=\frac{\beta^2}{4\omega^2}-a^2.
$$

This follows by completing the square in the [shallow-water Rossby-wave dispersion relation](#shallow-water-rossby-wave-dispersion-relation). A real circle requires $|\omega|\leq|\beta|/(2|a|)$. Its two intersections with a given tangential wavenumber provide the incident and reflected normal wavenumbers at a meridional wall.

### Topographic Rossby-wave dispersion relation

↑ **Parent:** [Rossby wave](#rossby-wave)

In a one-layer quasi-geostrophic fluid with effective meridional PV gradient $\beta_{\rm eff}$,

$$
\omega=-\frac{\beta_{\rm eff}k}{k^2+l^2+L_D^{-2}}.
$$

Bottom slope contributes to $\beta_{\rm eff}$ through vortex stretching.

#### Square-basin topographic Rossby mode

↑ **Parent:** [Topographic Rossby-wave dispersion relation](#topographic-rossby-wave-dispersion-relation)

In a square with impermeable walls and background topographic [potential-vorticity gradient](#potential-vorticity-gradient) $\beta$, the linear [shallow-water quasi-geostrophic potential vorticity](#shallow-water-quasi-geostrophic-potential-vorticity) equation is $\partial_t(\nabla^2-L_D^{-2})\psi+\beta\psi_x=0$. For a nonzero-frequency [normal mode](wave-equation.md#normal-mode), setting $\widehat\psi=\psi e^{i\beta x/(2\omega)}$ gives a [Helmholtz equation](partial-differential-equation.md#helmholtz-equation) with homogeneous wall data. The [eigenfunctions](linear-operator-theory.md#eigenfunction) are $\widehat\psi=\sin(m\pi x/L)\sin(n\pi y/L)$, with $m,n\geq1$, and the displayed frequencies. The positive and negative frequency representations are complex conjugates for a real wave.

#### Step-trapped topographic Rossby wave

↑ **Parent:** [Topographic Rossby-wave dispersion relation](#topographic-rossby-wave-dispersion-relation)

A depth discontinuity between two constant-depth rotating layers supports an exponentially trapped [Rossby wave](#rossby-wave). Continuity of surface height and cross-step volume flux gives $\omega(H_+\kappa_++H_-\kappa_-)=fk(H_+-H_-)$, where $\kappa_\pm^2=k^2+(f^2-\omega^2)/(gH_\pm)$ and positive roots give decay. For $H_\pm=H_0\pm d$ with $|d|\ll H_0$, the low-frequency branch has $\omega\simeq (fd/H_0)k/\sqrt{k^2+R_D^{-2}}$. In the Northern Hemisphere it propagates with the shallow side on its right.

##### Double Kelvin-wave adjustment at a depth step

↑ **Parent:** [Step-trapped topographic Rossby wave](#step-trapped-topographic-rossby-wave)

A long disturbance trapped on a depth step is sometimes called a double [Kelvin wave](#kelvin-wave). With $H_+>H_-$, $f>0$ and $c_\pm=\sqrt{gH_\pm}$, cross-step [geostrophic balance](physics.md#geostrophic-balance) and the along-step acceleration yield the transport equation shown for a background height jump $\eta_0\operatorname{sgn}(x)$. Its zero-initial-amplitude solution is $A=\eta_0[\operatorname{sgn}(x)-\operatorname{sgn}(x-(c_+-c_-)t)]$. The adjusted region diverts cross-step [volume flux](fluid-mechanics.md#volumetric-flow-rate) along the step; the propagating front still carries flux. This outer approximation does not resolve fast adjustment at the fronts.

##### Long-wave transport along a depth step

↑ **Parent:** [Step-trapped topographic Rossby wave](#step-trapped-topographic-rossby-wave)

The long [step-trapped topographic Rossby wave](#step-trapped-topographic-rossby-wave) has equal [phase velocity](wave-equation.md#phase-velocity) and [group velocity](wave-equation.md#group-velocity), $c_T=fdR_D/H_0$. For an outer surface profile $\eta=\eta_0\operatorname{sgn}(x)-A(x,t)e^{-|y|/R_D}$, cross-step matching gives $A_t+c_TA_x=2c_T\eta_0\delta(x)$. With $A(x,0)=0$, its weak solution is $A=\eta_0[\operatorname{sgn}(x)-\operatorname{sgn}(x-c_Tt)]$. This describes the slowly varying outer response; the fast adjustment region at the origin is unresolved.

### Barotropic Rossby wave

↑ **Parent:** [Rossby wave](#rossby-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Barotropic_Rossby_wave)

A barotropic Rossby wave has no vertical shear. For horizontal wavenumbers $k,l$, its quasi-geostrophic frequency is $\omega=-\beta k/(k^2+l^2)$.

#### Stationary Rossby-wave ray envelope

↑ **Parent:** [Barotropic Rossby wave](#barotropic-rossby-wave)

For a uniform eastward current $U>0$ on a [beta plane](#beta-plane) with $\beta>0$, stationary nondivergent [Rossby waves](#rossby-wave) have $k^2+l^2=\beta/U$. Their ground-frame [group velocity](wave-equation.md#group-velocity) is $2U(k^2,kl)/(k^2+l^2)$, tracing a circle centered at $(U,0)$ with radius $U$. Packets emitted by a localized source throughout $0<s<t$ occupy the disk shown in geometrical ray theory. This envelope is distinct from the full balanced near field. A westward current has no nontrivial stationary propagating branch in this model.

### Baroclinic Rossby wave

↑ **Parent:** [Rossby wave](#rossby-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baroclinic_Rossby_wave)

A baroclinic Rossby wave has nontrivial vertical structure. Constant stratification and rigid boundaries add a positive vertical-mode contribution to the denominator of its dispersion relation.

#### Rossby wave in a log-pressure atmosphere

↑ **Parent:** [Baroclinic Rossby wave](#baroclinic-rossby-wave)

For constant [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, the [log-pressure quasi-geostrophic potential vorticity](#log-pressure-quasi-geostrophic-potential-vorticity) equation has modes $\psi=e^{z/(2H)}e^{i(kx+mz-\omega t)}$ with

$$
\omega=-\frac{\beta k}{k^2+(f_0^2/N^2)[m^2+1/(4H^2)]}.
$$

The prefactor compensates the density decrease in the energy weight. For $\beta,k>0$, vertical propagation occurs for $-\beta k/[k^2+f_0^2/(4N^2H^2)]<\omega<0$. An outgoing [radiation condition](gravity-wave.md#radiation-condition) selects the root with positive vertical [group velocity](wave-equation.md#group-velocity); bounded weighted amplitude alone does not select between two propagating roots.

## Wave activity

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wave_activity)

Wave activity is a conserved quadratic measure of a small disturbance when the basic state has a continuous symmetry. Its flux divergence gives the exchange of pseudomomentum between waves and the mean flow.

### Wave action (fluid dynamics)

↑ **Parent:** [Wave activity](#wave-activity)

For a small-amplitude conservative wave packet in a slowly varying [fluid flow](fluid-mechanics.md#fluid-flow), its intrinsic [energy](classical-mechanics.md#energy) divided by [intrinsic frequency](gravity-wave.md#intrinsic-frequency) is transported along its [group velocity](wave-equation.md#group-velocity), with the basic [advection](fluid-mechanics.md#advection) added in the laboratory frame. A stationary background conserves laboratory [angular frequency](classical-mechanics.md#angular-frequency), but a changing mean [velocity](classical-mechanics.md#velocity) changes the intrinsic one through the [Doppler effect](physics.md#doppler-effect); intrinsic [energy](classical-mechanics.md#energy) alone need not be conserved. Geometrical spreading and dissipation enter the action-flux balance.

#### Wave pseudomomentum

↑ **Parent:** [Wave action (fluid dynamics)](#wave-action-fluid-dynamics)

The [wavevector](continuum-mechanics.md#wavevector) times [wave action](#wave-action-fluid-dynamics) gives the canonical momentum associated with translations of a wave's [phase](physics.md#phase-waves). It describes momentum exchange with a slowly varying mean [fluid flow](fluid-mechanics.md#fluid-flow), rather than simply the spatial average of oscillating fluid momentum. For horizontal [wavenumber](wave-equation.md#wavenumber) $k$, its horizontal component is $kE/\widehat\omega$. A convention using [displacement pseudomomentum of an internal gravity wave](gravity-wave.md#displacement-pseudomomentum-of-an-internal-gravity-wave) instead has the opposite sign.

### Quasi-geostrophic wave pseudomomentum

↑ **Parent:** [Wave activity](#wave-activity)

For small [quasi-geostrophic approximation](#quasi-geostrophic-approximation) waves on a locally uniform basic zonal flow with nonzero meridional [potential-vorticity gradient](#potential-vorticity-gradient) $Q_y$, this signed quadratic [wave activity](#wave-activity) obeys $\mathcal A_t+\nabla\cdot\mathbf F=\overline{q'\mathcal D}/Q_y$, where $\mathbf F$ is the [Eliassen–Palm flux](#eliassen-palm-flux) and $\mathcal D$ is a PV source. Multiply the linear PV equation by $q'/Q_y$ and use the [Taylor identity for quasi-geostrophic flux](#taylor-identity-for-quasi-geostrophic-flux) to obtain it. In a locally uniform conservative wave packet, $\mathbf F=\mathcal A\mathbf c_g$, so the flux follows the [group velocity](wave-equation.md#group-velocity), with its sign determined by $Q_y$.

## Equatorial wave

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equatorial_wave)

An equatorial wave is trapped near the equator by the sign change of the [Coriolis parameter](#coriolis-parameter). Its meridional structures are Gaussian-weighted [Hermite polynomials](numerical-analysis.md#hermite-polynomial).

### Equivalent depth

↑ **Parent:** [Equatorial wave](#equatorial-wave)

An equivalent depth is the shallow-water depth whose gravity-wave speed matches one vertical mode of a continuously stratified fluid. Each vertical mode then obeys its own horizontal shallow-water wave equations.

### Equatorial shallow-water dispersion relation

↑ **Parent:** [Equatorial wave](#equatorial-wave)

With $c=\sqrt{gH}$, [beta plane](#beta-plane) parameter $\beta>0$, and [Hermite polynomial](numerical-analysis.md#hermite-polynomial) index $n\geq0$, meridional trapping of the nonzero meridional-velocity branch requires

$$
\omega^2-c^2k^2-\frac{\beta kc^2}{\omega}=(2n+1)\beta c.
$$

Its meridional velocity is proportional to $H_n(Y)e^{-Y^2/2}$, with $Y=y\sqrt{\beta/c}$. Exceptional roots with $\omega^2=c^2k^2$ must be checked in the original equations, since eliminating velocity and height divides by this factor.

#### Equatorial wave velocity polarization

↑ **Parent:** [Equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation)

In dimensionless [equatorial wave](#equatorial-wave) units with [gravity wave](gravity-wave.md) speed and [beta plane](#beta-plane) coefficient one, a Fourier mode $e^{i(kx-\omega t)}$ obeys $\omega u-k\eta=iyv$ and $\omega\eta-ku=-iv'$. Inverting this two-by-two [linear system](linear-algebra.md#system-of-linear-equations) gives the displayed [wave polarization](physics.md#polarization-waves), provided $\omega^2\ne k^2$. Inserting it in the meridional momentum equation gives the [Hermite differential equation](analysis.md#hermite-differential-equation) after a Gaussian factor is removed. At singular values the original equations, rather than these quotient formulae, determine whether a trapped mode exists.

#### Frequency gap for higher equatorial wave modes

↑ **Parent:** [Equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation)

For fixed positive frequency and $n\geq1$, the [equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation) has real zonal [wavenumbers](wave-equation.md#wavenumber) only if

$$
\frac{\omega^2}{\beta c}\leq n+\frac12-\sqrt{n(n+1)}\quad\hbox{or}\quad \frac{\omega^2}{\beta c}\geq n+\frac12+\sqrt{n(n+1)}.
$$

Between these values the zonal roots are complex, giving an evanescent response rather than freely propagating modes.

### Equatorial Kelvin wave

↑ **Parent:** [Equatorial wave](#equatorial-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equatorial_Kelvin_wave)

An equatorial Kelvin wave has zero meridional velocity, eastward phase propagation, and Gaussian meridional trapping.

### Equatorial Rossby wave

↑ **Parent:** [Equatorial wave](#equatorial-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equatorial_Rossby_wave)

An equatorial Rossby wave propagates westward and has a Gaussian-weighted Hermite-polynomial meridional structure.

#### Equatorial Rossby-wave dispersion relation

↑ **Parent:** [Equatorial Rossby wave](#equatorial-rossby-wave)

Under meridional geostrophic balance, the mode with Hermite index $n\geq1$ has $\omega=-kc/(2n+1)$. The full shallow-water equations bend this long-wave line into a dispersive Rossby branch.

<h3 id="equatorial-inertia-gravity-wave">Equatorial inertia--gravity wave</h3>

↑ **Parent:** [Equatorial wave](#equatorial-wave)

An equatorial inertia--gravity wave is a high-frequency equatorially trapped mode restored jointly by [buoyancy](fluid-mechanics.md#buoyancy) and the [Coriolis force](physics.md#coriolis-force). Its dispersion relation has eastward and westward branches lying outside the low-frequency [equatorial Rossby wave](#equatorial-rossby-wave) branch.

### Rossby-gravity waves

↑ **Parent:** [Equatorial wave](#equatorial-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rossby-gravity_waves)

The Yanai wave is the $n=0$ branch of the [equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation) with positive frequency:

$$
k=\frac\omega c-\frac\beta\omega,\qquad v\propto e^{-\beta y^2/(2c)}.
$$

Its [group velocity](wave-equation.md#group-velocity) is $d\omega/dk=c\omega^2/(\omega^2+\beta c)>0$. At low frequency it has westward [phase velocity](wave-equation.md#phase-velocity) but transports energy eastward; at high frequency its phase and group velocities approach $c$.

#### Exceptional root of the mixed Rossby-gravity mode

↑ **Parent:** [Rossby-gravity waves](#rossby-gravity-waves)

For dimensionless Hermite index zero, the [equatorial shallow-water dispersion relation](#equatorial-shallow-water-dispersion-relation) factorizes as $(\omega+k)(\omega^2-k\omega-1)=0$. The root $\omega=-k$ is generally spurious: for $v=Ce^{-y^2/2}$, the original equations require $\delta'-y\delta=i(2k-1/k)v$, where $\delta=u-\eta$. Multiplication by $e^{-y^2/2}$ and integration over the real line shows that decay at both ends requires $C=0$ unless $k^2=1/2$. At that exception the root already belongs to the physical quadratic; $u=\eta=i\omega yv$ is regular and no extra wave branch is created. The assertion concerns nonzero $k$ and [angular frequency](classical-mechanics.md#angular-frequency).

### Damped equatorial Kelvin and Rossby response

↑ **Parent:** [Equatorial wave](#equatorial-wave)

With Rayleigh friction rate $\gamma$ and thermal damping rate $\alpha$, a steady localized equatorial forcing produces an eastward Kelvin tail of zonal scale $c/\sqrt{\alpha\gamma}$ and westward Rossby tails of scales $c/[(2n+1)\sqrt{\alpha\gamma}]$. Their common meridional scale is $[c\sqrt{\gamma/\alpha}/\beta]^{1/2}$.

## Transformed Eulerian mean

↑ **Parent:** [Geophysical fluid dynamics](geophysical-fluid-dynamics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transformed_Eulerian_mean)

The transformed Eulerian mean combines the Eulerian-mean meridional circulation with an eddy-induced circulation. This moves eddy buoyancy transport out of the mean thermodynamic equation and gathers wave forcing into the divergence of an [Eliassen–Palm flux](#eliassen-palm-flux).

### Eddy buoyancy flux

↑ **Parent:** [Transformed Eulerian mean](#transformed-eulerian-mean)

The local meridional eddy [buoyancy](fluid-mechanics.md#buoyancy) flux is the covariance of disturbance meridional [velocity](classical-mechanics.md#velocity) with disturbance [buoyancy](fluid-mechanics.md#buoyancy). In a [Boussinesq approximation](#boussinesq-approximation), $b'=-g\rho'/\rho_0$. This is a local transport [density](fluid-mechanics.md#density), distinct from a plume's cross-section-integrated [buoyancy flux](turbulent-plume.md#buoyancy-flux). In the [transformed Eulerian mean](#transformed-eulerian-mean), division by the background [buoyancy frequency](gravity-wave.md#buoyancy-frequency) squared gives an eddy-induced [meridional overturning streamfunction](#meridional-overturning-streamfunction).

<h3 id="eliassen-palm-flux">Eliassen–Palm flux</h3>

↑ **Parent:** [Transformed Eulerian mean](#transformed-eulerian-mean)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Eliassen–Palm_flux)

The Eliassen–Palm flux is a wave-activity flux whose divergence forces the transformed mean flow. Its vertical component combines vertical eddy momentum flux with a correction from meridional buoyancy transport.

#### Taylor identity for quasi-geostrophic flux

↑ **Parent:** [Eliassen–Palm flux](#eliassen-palm-flux)

For zonal averages, $u'=-\psi'_y$, $v'=\psi'_x$, and $Q'=\nabla_H^2\psi'+\partial_z(S\psi'_z)$, with $S=f_0^2/N^2$ depending only on height, define $F=-\overline{u'v'}$ and $G=S\overline{\psi'_x\psi'_z}$. Integrating zonal derivatives by parts gives $\overline{v'Q'}=\partial_y\overline{\psi'_x\psi'_y}+\partial_z(S\overline{\psi'_x\psi'_z})$. This identity is exact within [quasi-geostrophic potential vorticity](#three-dimensional-quasi-geostrophic-potential-vorticity), without assuming small disturbance amplitudes. Periodicity or appropriate vanishing zonal boundary terms is essential.

#### Non-acceleration theorem for quasi-geostrophic waves

↑ **Parent:** [Eliassen–Palm flux](#eliassen-palm-flux)

Steady conservative small-amplitude waves have divergence-free [Eliassen–Palm flux](#eliassen-palm-flux) by [wave activity](#wave-activity) conservation. In a balanced mean state with homogeneous impermeable boundaries and no independently forced [residual mean circulation](#residual-mean-circulation), this gives zero residual circulation and zero mean acceleration. The [Eulerian mean](#eulerian-mean-flow) circulation can nevertheless be nonzero because the residual circulation includes an eddy-induced correction. Wave dissipation, time-dependent wave activity or boundary forcing can invalidate the conclusion.

#### Wave-activity deposition

↑ **Parent:** [Eliassen–Palm flux](#eliassen-palm-flux)

When waves dissipate or encounter a critical layer, their [Eliassen–Palm flux](#eliassen-palm-flux) changes with position. Its divergence transfers wave pseudomomentum to the mean flow and produces wave drag.

#### Quasi-geostrophic wave-activity conservation law

↑ **Parent:** [Eliassen–Palm flux](#eliassen-palm-flux)

For linear perturbations about a uniform zonal flow, multiplying the forced quasi-geostrophic potential-vorticity equation by the PV anomaly gives a local conservation law for quadratic wave activity. Its flux is the [Eliassen–Palm flux](#eliassen-palm-flux), and forcing or damping appears as a wave-activity source or sink.

### Residual mean circulation

↑ **Parent:** [Transformed Eulerian mean](#transformed-eulerian-mean)

The residual mean circulation is the meridional and vertical circulation used by the [transformed Eulerian mean](#transformed-eulerian-mean). It combines the Eulerian-mean circulation with an eddy-induced contribution so that mean tracer evolution is advected by a single nondivergent flow.

#### Eliassen equation for residual circulation

↑ **Parent:** [Residual mean circulation](#residual-mean-circulation)

For constant Coriolis parameter $f_0$ and [buoyancy frequency](gravity-wave.md#buoyancy-frequency) $N$, thermal-wind balance and transformed mean-flow equations give

$$
f_0^2\chi_{zz}^*+N^2\chi_{yy}^*
=-f_0(\nabla\mathbin\cdot\mathbf F)_z,
$$

where $\chi^*$ is the residual-circulation streamfunction and $\mathbf F$ is the [Eliassen–Palm flux](#eliassen-palm-flux).

##### Step-flux residual circulation in a stratified channel

↑ **Parent:** [Eliassen equation for residual circulation](#eliassen-equation-for-residual-circulation)

Take $v=-\mathcal X_z$, $w=\mathcal X_y$, constant [density](fluid-mechanics.md#density) gradient $S<0$, and meridional eddy [density](fluid-mechanics.md#density) flux $F=\sin(ly)[-\mathbf1_{z<0}]$. If the divergence of the eddy [momentum flux](physics.md#momentum-flux) is zero, bounded Eulerian circulation and decaying [residual mean circulation](#residual-mean-circulation) give $\mathcal X=\sin(ly)\chi(z)$ with $\chi=-A_0(1-e^{\kappa z}/2)$ below zero and $\chi=-A_0e^{-\kappa z}/2$ above, where $A_0=-1/S$ and $\kappa=Nl/|f_0|$. The transformed [streamfunction](fluid-mechanics.md#stream-function) is $\mathcal X^*=\mathcal X+F/S$, yielding the displayed $\chi^*$ and two oppositely rotating cells. Its jump represents a horizontal delta-function transport at the discontinuous flux termination. A smooth flux cutoff replaces that sheet by a thin regular return flow. Density flux alone does not determine either circulation if the momentum-flux divergence is left unspecified.

##### Localized wave-drag response in a stratified channel

↑ **Parent:** [Eliassen equation for residual circulation](#eliassen-equation-for-residual-circulation)

For a sinusoidal [Eliassen–Palm flux](#eliassen-palm-flux) whose vertical divergence is constant in $-D<z<D$ and zero elsewhere, the [residual mean circulation](#residual-mean-circulation) is determined by a forced one-dimensional modified Helmholtz equation. With $v^*=C'(z)\sin(\pi y/L)$ and $w^*=-(\pi/L)C(z)\cos(\pi y/L)$, a forcing proportional to $-G_0\sin(\pi y/L)/(2D)$ gives

$$
C(z)=\frac{G_0}{4f_0Dm}\left[e^{-m|z-D|}-e^{-m|z+D|}\right].
$$

The response is uniquely selected by decay of the residual circulation at both vertical infinities. An [Eulerian mean](#eulerian-mean-flow) vertical flow can persist in the undamped wave region even where this residual response vanishes.

###### Vertically integrated wave-drag acceleration

↑ **Parent:** [Localized wave-drag response in a stratified channel](#localized-wave-drag-response-in-a-stratified-channel)

In the [localized wave-drag response in a stratified channel](#localized-wave-drag-response-in-a-stratified-channel), the full vertical integral of zonal acceleration equals the deposited wave momentum, $-G_0\sin(\pi y/L)$. The fraction inside the directly forced layer is $1-(1-e^{-2s})/(2s)$, where $s=\pi ND/(|f_0|L)$. A small $s$ spreads most acceleration outside the dissipation layer; a large $s$ confines most of it inside.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
