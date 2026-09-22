# Gravity wave

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravity_wave)

A gravity wave is a fluid disturbance restored by gravity or [buoyancy](fluid-mechanics.md#buoyancy). A [surface gravity wave](fluid-mechanics.md#surface-gravity-wave) displaces a [free surface](fluid-mechanics.md#free-surface), while an [internal gravity wave](#internal-wave) displaces density surfaces within a stratified fluid. Rotation can additionally contribute to restoration, giving an [inertia-gravity wave](geophysical-fluid-dynamics.md#inertia-gravity-wave).

**Table of contents**

- [Internal wave](#internal-wave)
  - [Internal-wave response of a sharp buoyancy interface](#internal-wave-response-of-a-sharp-buoyancy-interface)
  - [Pressure projection in a displaced stratified blob](#pressure-projection-in-a-displaced-stratified-blob)
  - [Finite-amplitude stationary channel internal waves](#finite-amplitude-stationary-channel-internal-waves)
  - [Internal-wave momentum deposition](#internal-wave-momentum-deposition)
    - [Boundary work and mean-flow energy of an internal wave](#boundary-work-and-mean-flow-energy-of-an-internal-wave)
  - [Energy partition of rotating internal waves](#energy-partition-of-rotating-internal-waves)
  - [Internal-wave breaking](#internal-wave-breaking)
  - [Plane internal gravity wave](#plane-internal-gravity-wave)
    - [Displacement pseudomomentum of an internal gravity wave](#displacement-pseudomomentum-of-an-internal-gravity-wave)
      - [Viscous attenuation of an internal gravity wave](#viscous-attenuation-of-an-internal-gravity-wave)
    - [Internal-wave transmission across a buoyancy-frequency jump](#internal-wave-transmission-across-a-buoyancy-frequency-jump)
      - [Internal-wave cavity response](#internal-wave-cavity-response)
    - [Monochromatic internal-wave overturning criterion](#monochromatic-internal-wave-overturning-criterion)
  - [Dispersion relation for interfacial gravity waves between rigid boundaries](#dispersion-relation-for-interfacial-gravity-waves-between-rigid-boundaries)
  - [Stratified internal-wave guide](#stratified-internal-wave-guide)
  - [Boundary-forced internal gravity wave](#boundary-forced-internal-gravity-wave)
    - [Slowly modulated internal-wave boundary forcing](#slowly-modulated-internal-wave-boundary-forcing)
      - [Internal-wave work in a phase-speed frame](#internal-wave-work-in-a-phase-speed-frame)
    - [Two-beam radiation from a localized oscillating boundary](#two-beam-radiation-from-a-localized-oscillating-boundary)
    - [Stationary topographic internal gravity wave](#stationary-topographic-internal-gravity-wave)
      - [Rigid-lid resonance of stationary topographic internal waves](#rigid-lid-resonance-of-stationary-topographic-internal-waves)
      - [Stationary phase of topographic internal waves](#stationary-phase-of-topographic-internal-waves)
    - [Internal-wave transmission across a stratification step](#internal-wave-transmission-across-a-stratification-step)
  - [Interfacial gravity wave](#interfacial-gravity-wave)
    - [Interfacial gravity-wave dispersion relation](#interfacial-gravity-wave-dispersion-relation)
  - [Atmospheric internal gravity wave](#atmospheric-internal-gravity-wave)
    - [Intrinsic frequency](#intrinsic-frequency)
      - [Critical level of an internal gravity wave](#critical-level-of-an-internal-gravity-wave)
        - [Wave-action criterion for critical-level overturning](#wave-action-criterion-for-critical-level-overturning)
        - [Critical-height approach of a stationary wave in linear shear](#critical-height-approach-of-a-stationary-wave-in-linear-shear)
    - [Radiation condition](#radiation-condition)
      - [Internal-wave envelope radiation condition](#internal-wave-envelope-radiation-condition)
      - [Limiting absorption principle](#limiting-absorption-principle)
    - [Wave momentum flux](#wave-momentum-flux)
    - [Taylor–Goldstein equation](#taylor-goldstein-equation)
      - [Exponential-profile stationary stratified waves](#exponential-profile-stationary-stratified-waves)
      - [Nonlinear exactness test for a stratified streamfunction mode](#nonlinear-exactness-test-for-a-stratified-streamfunction-mode)
      - [Variational group velocity of a Taylor-Goldstein mode](#variational-group-velocity-of-a-taylor-goldstein-mode)
      - [Power-transformed Taylor–Goldstein energy identity](#power-transformed-taylor-goldstein-energy-identity)
        - [Miles–Howard theorem](#miles-howard-theorem)
        - [Phase-speed bound for unstable stratified shear modes](#phase-speed-bound-for-unstable-stratified-shear-modes)
      - [Jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow)
        - [Endpoint derivative map for an evanescent wave layer](#endpoint-derivative-map-for-an-evanescent-wave-layer)
        - [Gravity-vorticity interface wave](#gravity-vorticity-interface-wave)
        - [Internal-wave transmission across a velocity jump](#internal-wave-transmission-across-a-velocity-jump)
          - [Displacement impedance for an internal wave at a velocity jump](#displacement-impedance-for-an-internal-wave-at-a-velocity-jump)
        - [Dispersion relation for two density interfaces in uniform shear](#dispersion-relation-for-two-density-interfaces-in-uniform-shear)
      - [Scorer parameter](#scorer-parameter)
        - [Stationary internal-wave WKB solution](#stationary-internal-wave-wkb-solution)
        - [Vertical trapping of an atmospheric gravity wave](#vertical-trapping-of-an-atmospheric-gravity-wave)
          - [Turning level of a stationary internal wave](#turning-level-of-a-stationary-internal-wave)
          - [Turning height of a stationary wave in linear shear](#turning-height-of-a-stationary-wave-in-linear-shear)
  - [Density stratification](#density-stratification)
    - [Density gradient](#density-gradient)
    - [Halocline](#halocline)
      - [Cold halocline](#cold-halocline)
    - [Ocean mixed layer](#ocean-mixed-layer)
    - [Stable density stratification](#stable-density-stratification)
      - [Ozmidov length](#ozmidov-length)
      - [Potential-energy cost of homogenizing a linear stratification](#potential-energy-cost-of-homogenizing-a-linear-stratification)
      - [Unstable density stratification](#unstable-density-stratification)
  - [Buoyancy frequency](#buoyancy-frequency)
    - [Radial buoyancy frequency](#radial-buoyancy-frequency)
      - [Radial Solberg–Høiland instability criterion](#radial-solberg-hoiland-instability-criterion)
    - [Dry parcel buoyancy in a homogeneous atmosphere](#dry-parcel-buoyancy-in-a-homogeneous-atmosphere)
    - [Richardson number](#richardson-number)
      - [Flux Richardson number](#flux-richardson-number)
        - [Buoyancy fraction of total turbulent sinks](#buoyancy-fraction-of-total-turbulent-sinks)
      - [Interfacial Richardson number](#interfacial-richardson-number)
        - [Entrainment exponent from a local interfacial Richardson closure](#entrainment-exponent-from-a-local-interfacial-richardson-closure)
      - [Bulk Richardson number](#bulk-richardson-number)
      - [Gradient Richardson number](#gradient-richardson-number)
    - [Stellar buoyancy frequency](#stellar-buoyancy-frequency)
  - [Internal-wave phase and group velocity](#internal-wave-phase-and-group-velocity)
    - [Right-triangle geometry of internal-wave velocities](#right-triangle-geometry-of-internal-wave-velocities)
    - [Internal-wave polarization](#internal-wave-polarization)
      - [Buoyancy polarization of a plane internal gravity wave](#buoyancy-polarization-of-a-plane-internal-gravity-wave)
    - [Constant-phase line of an internal gravity wave](#constant-phase-line-of-an-internal-gravity-wave)
  - [Reflection of an internal-wave ray](#reflection-of-an-internal-wave-ray)
    - [Internal-wave slope criticality](#internal-wave-slope-criticality)
      - [Subcritical internal-wave reflection](#subcritical-internal-wave-reflection)
      - [Critical internal-wave reflection](#critical-internal-wave-reflection)
    - [Topographic sideband of an internal gravity wave](#topographic-sideband-of-an-internal-gravity-wave)
    - [Internal-wave ray tracing](#internal-wave-ray-tracing)
      - [Internal-wave ray in uniform vertical shear](#internal-wave-ray-in-uniform-vertical-shear)
        - [Circular mountain-wave ray in linear shear](#circular-mountain-wave-ray-in-linear-shear)
      - [Internal-wave attractor](#internal-wave-attractor)
        - [Internal-wave ray return map](#internal-wave-ray-return-map)
      - [Double-zero internal-wave turning level](#double-zero-internal-wave-turning-level)
      - [Causal envelope of stationary internal waves](#causal-envelope-of-stationary-internal-waves)
        - [Refraction of a stationary internal-wave causal envelope](#refraction-of-a-stationary-internal-wave-causal-envelope)
        - [First arrival of a stationary internal wavefront at a layer boundary](#first-arrival-of-a-stationary-internal-wavefront-at-a-layer-boundary)
    - [Focusing power of internal-wave reflection](#focusing-power-of-internal-wave-reflection)
  - [Viscous attenuation of an internal-wave beam](#viscous-attenuation-of-an-internal-wave-beam)
    - [Oscillatory drift of an attenuated internal-wave beam](#oscillatory-drift-of-an-attenuated-internal-wave-beam)
  - [Vertical trapping of an internal gravity wave by planar strain](#vertical-trapping-of-an-internal-gravity-wave-by-planar-strain)
  - [Mountain-wave cutoff](#mountain-wave-cutoff)

## Internal wave

↑ **Parent:** [Gravity wave](gravity-wave.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Internal_wave)

In a uniformly stratified fluid with buoyancy frequency $N$, a plane wave of horizontal and vertical wavenumbers $k,m$ obeys

$$
\omega^2=\frac{N^2k^2}{k^2+m^2}.
$$

### Internal-wave response of a sharp buoyancy interface

↑ **Parent:** [Internal wave](#internal-wave)

For a lower uniformly stratified half-space and an upper well-mixed half-space, the [vertical velocity](fluid-mechanics.md#vertical-velocity) amplitude is continuous and its derivative jumps by $[W']=-k^2\Delta b\,W/\omega^2$. A wave incident upwards with vertical phase factor $e^{-imz}$ therefore has upper evanescent amplitude $T/W_i=2im/[k(1-S)+im]$, where $m=k\sqrt{N^2/\omega^2-1}$ and $S=\Delta b k/\omega^2$. Its magnitude peaks at $S=1$, with amplitude twice the incident amplitude. Lossless reflection carries all incident [energy](classical-mechanics.md#energy) back down; the evanescent upper field carries no mean outgoing vertical energy flux.

### Pressure projection in a displaced stratified blob

↑ **Parent:** [Internal wave](#internal-wave)

Incompressibility makes pressure adjust throughout the surrounding fluid. Projecting the linear [Boussinesq equations](geophysical-fluid-dynamics.md#boussinesq-equations) perpendicular to a Fourier wavevector gives $w_t=[k_h^2/(k_h^2+m^2)]b$ and $b_t=-N^2w$. A localized spherical disturbance contains many wavevector directions and therefore many [internal gravity wave](#internal-wave) frequencies, rather than one oscillator at $N$. Its shape evolves and energy radiates into the surroundings; a rigid-sphere [added mass](physics.md#added-mass) analogy illustrates extra inertia but does not give an exact coherent frequency for a free material blob.

### Finite-amplitude stationary channel internal waves

↑ **Parent:** [Internal wave](#internal-wave)

In a nonrotating ideal [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) layer with uniform current $U>0$, constant [buoyancy frequency](#buoyancy-frequency) $N$ and rigid walls, any stationary superposition of channel wave modes with $k_n^2+(n\pi/H)^2=N^2/U^2$ obeys the displayed relations. With $(u,w)=(\psi_z,-\psi_x)$, the total streamfunction is $\Psi=Uz+\psi'$ and total buoyancy is $\sigma=(N^2/U)\Psi$. Its material derivative vanishes. The perturbation [vorticity](fluid-mechanics.md#vorticity) is proportional to $\psi'$, so its nonlinear self-advection vanishes as well. The modes are therefore exact finite-amplitude solutions, although large amplitudes may violate physical approximation assumptions or become unstable.

### Internal-wave momentum deposition

↑ **Parent:** [Internal wave](#internal-wave)

A slowly established upward [plane internal gravity wave](#plane-internal-gravity-wave) has $\overline{u'w'}=-m|a|^2/(2k)$. The mean horizontal [conservation of momentum](classical-mechanics.md#momentum-conservation) equation gives $\overline u_t=-\partial_z\overline{u'w'}$. Using envelope transport and an initially vanishing mean gives $\overline u=-m|a|^2/(2kc_{gz})$. Its [energy density](statistical-physics.md#energy-density) per unit mass is $\mathcal E=(k^2+m^2)|a|^2/(2k^2)$, so $\overline u=(k/\omega)\mathcal E$. This is the mean flow left behind the advancing wave envelope, rather than a claim that an established uniform wavetrain has nonzero local stress divergence.

#### Boundary work and mean-flow energy of an internal wave

↑ **Parent:** [Internal-wave momentum deposition](#internal-wave-momentum-deposition)

For a traveling sinusoidal boundary forcing with horizontal phase speed $c_p$, the [pressure](thermodynamics.md#pressure) and horizontal [velocity](classical-mechanics.md#velocity) polarization gives the displayed relation between upward [energy](classical-mechanics.md#energy) input and vertical [wave momentum flux](#wave-momentum-flux). A slowly established outgoing wave envelope deposits horizontal mean [momentum](classical-mechanics.md#momentum) as its front advances. In the frame moving at $c_p$, the order-amplitude-squared change of mean [kinetic energy](classical-mechanics.md#kinetic-energy) is $-\rho_0c_p\int\overline u\,dz$. Its loss rate equals the boundary work in the laboratory frame. The comparison uses a finite perturbation of the infinite uniform background [energy](classical-mechanics.md#energy).

### Energy partition of rotating internal waves

↑ **Parent:** [Internal wave](#internal-wave)

For a plane [inertia-gravity wave](geophysical-fluid-dynamics.md#inertia-gravity-wave) independent of one horizontal coordinate, period-mean kinetic and [available potential energy](classical-mechanics.md#available-potential-energy) obey $\langle K\rangle-\langle A\rangle=2\langle K_y\rangle$. The transverse rotating velocity is in quadrature with the in-plane velocity. The modified oscillator balance is $\langle K_{xz}\rangle=\langle A\rangle+\langle K_y\rangle$; ordinary kinetic/potential equipartition occurs only when the transverse amplitude vanishes.

### Internal-wave breaking

↑ **Parent:** [Internal wave](#internal-wave)

Nonlinear disruption of an [internal gravity wave](#internal-wave), for example when large displacement gradients overturn the stable density arrangement or strong shear becomes unstable. The resulting [turbulence](turbulence.md) dissipates wave energy and mixes the stratification, limiting ideal geometric focusing.

### Plane internal gravity wave

↑ **Parent:** [Internal wave](#internal-wave)

A monochromatic [internal gravity wave](#internal-wave) in uniform stratification has a spatially linear phase. In the nonrotating inviscid [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), its [dispersion relation](wave-equation.md#dispersion-relation) is $\omega^2=N^2|\mathbf k_h|^2/(|\mathbf k_h|^2+m^2)$. The [wave vector](continuum-mechanics.md#wavevector) is normal to its phase planes, while the [group velocity](wave-equation.md#group-velocity) lies along them.

#### Displacement pseudomomentum of an internal gravity wave

↑ **Parent:** [Plane internal gravity wave](#plane-internal-gravity-wave)

The displayed displacement convention is the negative of the usual positive-frequency [wave pseudomomentum](geophysical-fluid-dynamics.md#wave-pseudomomentum) $k\overline E/\omega$ for a rightgoing [internal gravity wave](#internal-wave). Here [energy](classical-mechanics.md#energy) per unit reference [mass density](fluid-mechanics.md#density) is $\overline E=|\widehat\sigma|^2/(2N^2)$. From the [buoyancy polarization of a plane internal gravity wave](#buoyancy-polarization-of-a-plane-internal-gravity-wave), horizontal averaging gives $\overline{\zeta_xp}=km|\widehat\sigma|^2/(2N^2K^2)=c_{gz}P$, where $p$ is [kinematic pressure](thermodynamics.md#kinematic-pressure). The sign convention changes both density and flux and leaves their propagation at the [group velocity](wave-equation.md#group-velocity) unchanged.

##### Viscous attenuation of an internal gravity wave

↑ **Parent:** [Displacement pseudomomentum of an internal gravity wave](#displacement-pseudomomentum-of-an-internal-gravity-wave)

With weak [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$, zero buoyancy diffusion and locally unchanged [plane internal gravity wave](#plane-internal-gravity-wave) polarization, the [displacement pseudomomentum of an internal gravity wave](#displacement-pseudomomentum-of-an-internal-gravity-wave) obeys $P_t+\partial_z(c_{gz}P)=-\nu K^2P$. For constant [wavenumbers](wave-equation.md#wavenumber) and a stationary wave envelope, $P\propto|\widehat\sigma|^2$ proves the displayed amplitude decay. Decay is along the [group velocity](wave-equation.md#group-velocity), so $c_{gz}<0$ describes a source above the receiving level. In a slowly varying [shear flow](fluid-mechanics.md#shear-flow), use [wave action](geophysical-fluid-dynamics.md#wave-action-fluid-dynamics) and the changing [intrinsic frequency](#intrinsic-frequency) rather than treating $P/|\widehat\sigma|^2$ as constant.

#### Internal-wave transmission across a buoyancy-frequency jump

↑ **Parent:** [Plane internal gravity wave](#plane-internal-gravity-wave)

At a jump in [buoyancy frequency](#buoyancy-frequency) with continuous background density, incident, reflected and transmitted [internal gravity waves](#internal-wave) share frequency and horizontal wavenumber. Continuity of pressure and normal velocity determines their amplitudes. If amplitudes multiply unit particle-displacement vectors directed along each ray with positive horizontal component, the reflection coefficient is $[\sin\theta_2/\sin\theta_1-\cos\theta_2/\cos\theta_1]/[\sin\theta_2/\sin\theta_1+\cos\theta_2/\cos\theta_1]$. Using vertical-displacement amplitudes reverses the reflected coefficient's sign because the reflected polarization reverses its vertical component.

##### Internal-wave cavity response

↑ **Parent:** [Internal-wave transmission across a buoyancy-frequency jump](#internal-wave-transmission-across-a-buoyancy-frequency-jump)

A reflecting bottom beneath a jump in [buoyancy frequency](#buoyancy-frequency) creates a standing field from repeated transmitted and reflected [internal gravity waves](#internal-wave). For ray angles $\theta_1=\pi/3$ and $\theta_2=\pi/6$, the downward particle-displacement amplitude has magnitude $\sqrt3|\eta_i|/[1+8\sin^2(m_2H)]^{1/2}$. It reaches $\sqrt3|\eta_i|$ when $m_2H$ is an integer multiple of $\pi$. The upper reflected wave has the same amplitude magnitude as the incident wave because the lossless closed cavity admits no net downward energy flux.

#### Monochromatic internal-wave overturning criterion

↑ **Parent:** [Plane internal gravity wave](#plane-internal-gravity-wave)

For a [plane internal gravity wave](#plane-internal-gravity-wave) with vertical displacement $\zeta$, linear density advection gives $\rho'=-\bar\rho_z\zeta$. In a constant stable gradient, $\rho_z=\bar\rho_z(1-\zeta_z)$, so static overturning begins when the maximum of $\zeta_z$ exceeds one. A monochromatic displacement has maximum $|mA_\zeta|$. The criterion predicts the failure of the small-amplitude field, rather than a valid continuation of linear theory beyond overturning.

### Dispersion relation for interfacial gravity waves between rigid boundaries

↑ **Parent:** [Internal wave](#internal-wave)

For two incompressible inviscid layers at rest between rigid horizontal boundaries, with the heavier fluid below and no surface tension, the displayed [dispersion relation](wave-equation.md#dispersion-relation) follows from [Laplace equation](partial-differential-equation.md#laplace-equation) for the velocity potentials, no normal flow at the walls, equal normal velocities at the interface, and pressure continuity. The positive density contrast supplies the restoring force. In the long-wave limit the squared wave speed is $g(\rho_2-\rho_1)/(\rho_1/h_1+\rho_2/h_2)$.

### Stratified internal-wave guide

↑ **Parent:** [Internal wave](#internal-wave)

A stratified layer between unstratified regions can trap [internal gravity waves](#internal-wave), because the exterior disturbance is an [evanescent wave](continuum-mechanics.md#evanescent-wave). Its discrete [normal modes](wave-equation.md#normal-mode) obey [Robin boundary conditions](differential-equation.md#robin-boundary-condition) representing the exterior layers. Periodic boundary forcing at a trapped [normal mode](wave-equation.md#normal-mode) [frequency](physics.md#frequency) produces [resonance](dynamical-systems.md#resonance) in the ideal undamped model.

### Boundary-forced internal gravity wave

↑ **Parent:** [Internal wave](#internal-wave)

A moving boundary excites an [internal gravity wave](#internal-wave) through its [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition). For [wavenumber](wave-equation.md#wavenumber) $k$ and [angular frequency](classical-mechanics.md#angular-frequency) $\omega$, the vertical [velocity field](fluid-mechanics.md#velocity-field) satisfies $W''+k^2(N^2/\omega^2-1)W=0$. The [radiation condition](#radiation-condition) selects outward [group velocity](wave-equation.md#group-velocity); when $\omega>N$, the bounded response is an [evanescent wave](continuum-mechanics.md#evanescent-wave).

#### Slowly modulated internal-wave boundary forcing

↑ **Parent:** [Boundary-forced internal gravity wave](#boundary-forced-internal-gravity-wave)

For a [plane internal gravity wave](#plane-internal-gravity-wave) in uniform [buoyancy frequency](#buoyancy-frequency), substitute $\zeta=A(\mu t,\mu z)e^{i(kx+mz-\omega t)}$ into the displacement equation. The leading order gives $\omega^2=N^2k^2/(k^2+m^2)$; the next order gives the displayed transport equation with $c_{gz}=-\omega m/(k^2+m^2)$. A boundary amplitude $a(T)$ radiates as $A=a(T-Z/c_{gz})$, choosing the sign of $m$ so the [group velocity](wave-equation.md#group-velocity) points into the fluid. The wavelength-averaged energy is $N^2|A|^2/2$ and its vertical flux is $c_{gz}$ times that energy. A causal ramp therefore creates a translating front, not an instantaneous monochromatic field throughout the half-space.

##### Internal-wave work in a phase-speed frame

↑ **Parent:** [Slowly modulated internal-wave boundary forcing](#slowly-modulated-internal-wave-boundary-forcing)

A right-going, boundary-forced [internal gravity wave](#internal-wave) has horizontal momentum per unit inertial density $P=(k/\omega)\overline E$. Its envelope-induced [Eulerian mean](geophysical-fluid-dynamics.md#eulerian-mean-flow) acceleration is $\overline u_t=P_t$ to leading slow order. In the frame moving at horizontal [phase velocity](wave-equation.md#phase-velocity) $c=\omega/k$, the change of mean kinetic energy relative to the initial current $-c$ is $-\rho_0c\int\overline u\,dz$ at quadratic wave order. Its time derivative is minus the boundary work $\overline W=\rho_0\,d\int\overline E\,dz/dt$. The lab-frame mean kinetic energy alone is fourth order in wave amplitude; retaining the moving-frame cross term is essential.

#### Two-beam radiation from a localized oscillating boundary

↑ **Parent:** [Boundary-forced internal gravity wave](#boundary-forced-internal-gravity-wave)

For a nonrotating uniform-stratification fluid under the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) driven at $0<\omega<N$ by a localized vertical-wall [velocity](classical-mechanics.md#velocity), positive vertical [wavenumbers](wave-equation.md#wavenumber) radiate down and right and negative ones up and right. The real [velocity](classical-mechanics.md#velocity) separates into functions of $Z_+$ and $Z_-$. Its in-phase component is half the imposed boundary profile on each beam; the quadrature component is its [Hilbert transform](analysis.md#hilbert-transform) partner. Thus compact localization at maximum boundary speed does not imply compact localization of all components at every phase. A finite-duration source contains several frequencies and spreads [energy](classical-mechanics.md#energy) over their different ray angles and group speeds.

#### Stationary topographic internal gravity wave

↑ **Parent:** [Boundary-forced internal gravity wave](#boundary-forced-internal-gravity-wave)

A fixed terrain obstacle forces a zero laboratory-frequency [internal gravity wave](#internal-wave) through the [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition) $w=U h_x$. Its [intrinsic frequency](#intrinsic-frequency) is $-kU$. Propagation, radiation and the transient arrival of its permanent component are distinct questions.

##### Rigid-lid resonance of stationary topographic internal waves

↑ **Parent:** [Stationary topographic internal gravity wave](#stationary-topographic-internal-gravity-wave)

For a sinusoidal small-amplitude bed, constant current $U>0$ and [buoyancy frequency](#buoyancy-frequency) $N$, put $m=\sqrt{N^2/U^2-k^2}>0$. The linear vertical [velocity](classical-mechanics.md#velocity) amplitude is $W(z)=ikU\eta_0\sin[m(H-z)]/\sin(mH)$. The upward-wave coefficient is $A_+=-kU\eta_0e^{-imH}/[2\sin(mH)]$. At $mH=n\pi$, the prescribed nonzero bed motion and homogeneous rigid-lid condition are incompatible with a bounded stationary inviscid solution. With angle $\theta$ between intrinsic [group velocity](wave-equation.md#group-velocity) and vertical, $\tan\theta=m/k$, giving $kH\tan\theta=n\pi$.

##### Stationary phase of topographic internal waves

↑ **Parent:** [Stationary topographic internal gravity wave](#stationary-topographic-internal-gravity-wave)

For a localized terrain source in uniform flow, the [stationary phase method](analysis.md#stationary-phase-method) applied to $kx+m(k)z$ gives phase $\Phi=(N/U)\sqrt{x^2+z^2}$ on the downstream branch. Permanent phase lines are circular arcs, whereas an individual monochromatic component has straight phase lines. Reflected arcs use an image source; transmitted phase is continuous across the velocity interface.

#### Internal-wave transmission across a stratification step

↑ **Parent:** [Boundary-forced internal gravity wave](#boundary-forced-internal-gravity-wave)

At a step in [buoyancy frequency](#buoyancy-frequency) without a jump in background [mass density](fluid-mechanics.md#density), vertical [velocity](classical-mechanics.md#velocity) and [fluid pressure](fluid-mechanics.md#fluid-pressure) are continuous. For a fixed horizontal [wavenumber](wave-equation.md#wavenumber) and [angular frequency](classical-mechanics.md#angular-frequency), these are continuity of $W$ and $W'$. They determine reflection and transmission between propagating [internal gravity waves](#internal-wave) and [evanescent waves](continuum-mechanics.md#evanescent-wave).

### Interfacial gravity wave

↑ **Parent:** [Internal wave](#internal-wave)

An interfacial gravity wave is a displacement of an interface between two fluids of different [mass density](fluid-mechanics.md#density), restored by [buoyancy](fluid-mechanics.md#buoyancy) when the denser fluid is below. For two deep layers in the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), density difference $\delta\rho$ and horizontal [wavenumber](wave-equation.md#wavenumber) $k$ give intrinsic squared [phase velocity](wave-equation.md#phase-velocity) $g\delta\rho/(2\rho_0k)$. Background flow shifts the laboratory [phase velocity](wave-equation.md#phase-velocity) by its local speed.

#### Interfacial gravity-wave dispersion relation

↑ **Parent:** [Interfacial gravity wave](#interfacial-gravity-wave)

For two inviscid layers of equal depth $h$ between rigid lids, with lower density $\rho_2$ and upper density $\rho_1$, a horizontal mode of wavenumber $k$ satisfies

$$
\omega^2=\frac{\rho_2-\rho_1}{\rho_1+\rho_2}gk\tanh(kh).
$$

The sign reverses when the heavier fluid is above, producing the [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability).

### Atmospheric internal gravity wave

↑ **Parent:** [Internal wave](#internal-wave)

An atmospheric internal gravity wave is an [internal gravity wave](#internal-wave) propagating through a stably stratified atmosphere. Flow across mountains can generate nearly stationary waves whose vertical propagation is controlled by the wind and buoyancy-frequency profiles.

#### Intrinsic frequency

↑ **Parent:** [Atmospheric internal gravity wave](#atmospheric-internal-gravity-wave)

The intrinsic frequency is the frequency observed in a frame moving with the basic flow. For a wave of frequency $\omega$ and horizontal wavenumber $k$ in a uniform current $U$, it is $\widehat\omega=\omega-kU$.

##### Critical level of an internal gravity wave

↑ **Parent:** [Intrinsic frequency](#intrinsic-frequency)

A critical level is a height at which the [intrinsic frequency](#intrinsic-frequency) of an [internal gravity wave](#internal-wave) vanishes. For finite positive [buoyancy frequency](#buoyancy-frequency), its local vertical [wavenumber](wave-equation.md#wavenumber) diverges as $\widehat\omega\to0$. The inviscid [Taylor–Goldstein equation](#taylor-goldstein-equation) is singular there; viscosity, diffusion or nonlinear wave breaking can regularize the resulting small scales.

###### Wave-action criterion for critical-level overturning

↑ **Parent:** [Critical level of an internal gravity wave](#critical-level-of-an-internal-gravity-wave)

For upward [internal gravity waves](#internal-wave), let $B=c_{gz}N^2A_\zeta^2/\widehat\omega$ be constant. Combining $c_{gz}=(N/k)\sin\theta\cos^2\theta$ with the [monochromatic internal-wave overturning criterion](#monochromatic-internal-wave-overturning-criterion) gives $\cot^4\theta<Bk^3\widehat\omega/(N^3\sin^3\theta)$. Near a [critical level](hydrodynamic-stability.md#critical-level-of-a-shear-flow-wave) the onset balance is $\cot\theta\sim(Bk^3\widehat\omega/N^3)^{1/4}$. This is compatible with $\widehat\omega=N\cos\theta$; it fixes the overturning point rather than redefining the [dispersion relation](wave-equation.md#dispersion-relation).

###### Critical-height approach of a stationary wave in linear shear

↑ **Parent:** [Critical level of an internal gravity wave](#critical-level-of-an-internal-gravity-wave)

For $S<0$ and constant positive [buoyancy frequency](#buoyancy-frequency), the critical height is $U_0/|S|$. A stationary upward ray approaches it with vertical [group velocity](wave-equation.md#group-velocity) proportional to $U^2$, requiring infinite ideal ray travel time. Large [gradient Richardson number](#gradient-richardson-number) can preserve the short-wavelength [WKB approximation](analysis.md#wkb-approximation), but parcel-displacement amplitude grows and eventually invalidates linearity.

#### Radiation condition

↑ **Parent:** [Atmospheric internal gravity wave](#atmospheric-internal-gravity-wave)

A radiation condition selects the wave solution whose energy propagates away from its source. For an [internal gravity wave](#internal-wave), the vertical phase and group velocities have opposite signs, so upward radiation fixes the sign of the vertical wavenumber.

##### Internal-wave envelope radiation condition

↑ **Parent:** [Radiation condition](#radiation-condition)

For a slowly switched-on [plane internal gravity wave](#plane-internal-gravity-wave) in the half-space $z>0$, the [method of multiple scales](differential-equation.md#method-of-multiple-scales) gives transport of its amplitude at the vertical [group velocity](wave-equation.md#group-velocity). For $\omega^2=N^2k^2/(k^2+m^2)$, $c_{gz}=-\omega m/(k^2+m^2)$. Initially undisturbed fluid and forcing at the bottom require $c_{gz}>0$. The outgoing [radiation condition](#radiation-condition) therefore selects $m<0$ when $\omega>0$, although the vertical [phase velocity](wave-equation.md#phase-velocity) is downward.

##### Limiting absorption principle

↑ **Parent:** [Radiation condition](#radiation-condition)

Select outgoing waves as a limit of a problem with weak absorption. With time convention $e^{-i\omega t}$ use $\operatorname{Im}\omega>0$; with $e^{i\omega t}$ use $\operatorname{Im}\omega<0$. The resulting [Green function](analysis.md#green-s-function) and transform-contour prescriptions determine which [poles](isolated-singularity.md#pole) represent incoming or outgoing waves. This is especially useful when real-axis singularities obscure a [Wiener-Hopf factorization](differential-equation.md#wiener-hopf-factorization).

#### Wave momentum flux

↑ **Parent:** [Atmospheric internal gravity wave](#atmospheric-internal-gravity-wave)

The wave momentum flux $\rho_0\overline{u'w'}$ is the vertical transport of horizontal momentum by correlated velocity perturbations. Its vertical convergence exerts the mean-flow force $-\rho_0\partial_z\overline{u'w'}$.

<h4 id="taylor-goldstein-equation">Taylor–Goldstein equation</h4>

↑ **Parent:** [Atmospheric internal gravity wave](#atmospheric-internal-gravity-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Taylor–Goldstein_equation)

The Taylor–Goldstein equation governs linear two-dimensional disturbances of an inviscid, vertically sheared, stably stratified parallel flow. For horizontal [phase velocity](wave-equation.md#phase-velocity) $c$, base velocity $U(z)$, [buoyancy frequency](#buoyancy-frequency) $N(z)$, and horizontal [wavenumber](wave-equation.md#wavenumber) $k$,

$$
\widehat w''+\left[
\frac{N^2}{(U-c)^2}
-\frac{U''}{U-c}-k^2
\right]\widehat w=0.
$$

##### Exponential-profile stationary stratified waves

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)

For positive background velocity $U=U_0e^{Mz}$ and [buoyancy frequency](#buoyancy-frequency) $N=N_0e^{Mz}$, a stationary nonzero-horizontal-wavenumber [Taylor–Goldstein equation](#taylor-goldstein-equation) reduces to the displayed constant-coefficient equation. Its structures are oscillatory, affine or exponential according to the sign of $N_0^2/U_0^2-M^2-k^2$. The disturbance [Laplacian](calculus.md#laplacian) is a constant times its [streamfunction](fluid-mechanics.md#stream-function), but its [buoyancy](fluid-mechanics.md#buoyancy) anomaly is $N_0^2e^{Mz}\phi/U_0$. Therefore vorticity self-advection vanishes while buoyancy self-advection produces a nonzero second harmonic for $M\ne0$. These nontrivial real linear modes are not exact finite-amplitude solutions without additional fields. For $M=0$, both polarizations are constant and these nonlinear self-interactions vanish.

##### Nonlinear exactness test for a stratified streamfunction mode

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)

For two-dimensional flow under the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation) with $u=\psi_z$, $w=-\psi_x$, a linear mode whose [Laplacian](calculus.md#laplacian) is proportional to its [streamfunction](fluid-mechanics.md#stream-function) has zero self-advection of [vorticity](fluid-mechanics.md#vorticity). Its [buoyancy](fluid-mechanics.md#buoyancy) anomaly is $\sigma=a(z)\phi$, with $a=N^2/(U-c)$. Self-advection of [buoyancy](fluid-mechanics.md#buoyancy) vanishes only when the displayed Jacobian is zero. Constant stratification and constant flow make $a$ constant and yield finite-amplitude exact wave solutions. A varying polarization coefficient generally creates a second harmonic, even when the [vorticity](fluid-mechanics.md#vorticity) self-interaction vanishes.

##### Variational group velocity of a Taylor-Goldstein mode

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)

For a regular real mode between rigid boundaries, multiply the [Taylor–Goldstein equation](#taylor-goldstein-equation) by its vertical structure and integrate to get the stationary quotient $k^2=\int(\ell^2\phi^2-\phi_z^2)dz/\int\phi^2dz$. Along a differentiable dispersion branch, stationarity removes the variation of the [eigenfunction](linear-operator-theory.md#eigenfunction), giving $2k=(\partial I/\partial c)dc/dk$. Since $\partial_c\ell^2=N^2/(U-c)^3+\ell^2/(U-c)$, the displayed [group velocity](wave-equation.md#group-velocity) follows from $d(kc)/dk$. Critical levels and vanishing branch derivatives require a separate limiting analysis.

<h5 id="power-transformed-taylor-goldstein-energy-identity">Power-transformed Taylor–Goldstein energy identity</h5>

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)

For a mode with nonreal [phase velocity](wave-equation.md#phase-velocity) $c$, let $V=U-c$, choose a continuous branch of $V^a$, and put $\widehat w=V^aq$. Under impermeable boundary conditions, multiplying the transformed [Taylor–Goldstein equation](#taylor-goldstein-equation) by $V^{2a}\overline q$ and applying [integration by parts](calculus.md#integration-by-parts) gives

$$
\int V^{2a}(|q'|^2+k^2|q|^2)dz=\int\left[\{N^2+a(a-1)(U')^2\}V^{2a-2}+(a-1)U''V^{2a-1}\right]|q|^2dz.
$$

Choosing $a=1/2$ gives the [Miles–Howard theorem](#miles-howard-theorem); choosing $a=1$ makes the real [phase velocity](wave-equation.md#phase-velocity) of an unstable mode a weighted mean of $U$.

<h6 id="miles-howard-theorem">Miles–Howard theorem</h6>

↑ **Parent:** [Power-transformed Taylor–Goldstein energy identity](#power-transformed-taylor-goldstein-energy-identity)

A smooth inviscid stratified parallel flow with [gradient Richardson number](#gradient-richardson-number) at least $1/4$ everywhere has no exponentially growing two-dimensional [normal modes](wave-equation.md#normal-mode). Put $a=1/2$ in the [power-transformed Taylor–Goldstein energy identity](#power-transformed-taylor-goldstein-energy-identity) and take its [imaginary part](complex-analysis.md#imaginary-part):

$$
c_i\int\left[|q'|^2+k^2|q|^2+\frac{N^2-(U')^2/4}{|U-c|^2}|q|^2\right]dz=0.
$$

The integral is positive for a nonzero mode when the numerator is nonnegative, forcing $c_i=0$. This is a modal stability theorem, not a prohibition on [transient growth](linear-operator-theory.md#transient-growth). [Maslowe's review](https://www.imi.kyushu-u.ac.jp/wp-content/uploads/2022/07/Maslowe.pdf) discusses the theorem and the role of critical layers.

###### Phase-speed bound for unstable stratified shear modes

↑ **Parent:** [Power-transformed Taylor–Goldstein energy identity](#power-transformed-taylor-goldstein-energy-identity)

For an unstable [Taylor–Goldstein equation](#taylor-goldstein-equation) mode in a finite channel, take $a=1$ in the [power-transformed Taylor–Goldstein energy identity](#power-transformed-taylor-goldstein-energy-identity). Its [imaginary part](complex-analysis.md#imaginary-part) gives

$$
c_r=\frac{\int U(|q'|^2+k^2|q|^2)dz}{\int(|q'|^2+k^2|q|^2)dz}.
$$

Thus the real [phase velocity](wave-equation.md#phase-velocity) lies strictly between the extremes of a nonconstant smooth shear profile. Equality would force the regular [eigenfunction](linear-operator-theory.md#eigenfunction) to vanish on an interval, hence everywhere by uniqueness for its [ordinary differential equation](differential-equation.md#ordinary-differential-equation).

##### Jump conditions for stratified inviscid shear flow

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)

At a material interface without [surface tension](fluid-mechanics.md#surface-tension), continuity of displacement and of the pressure evaluated on the displaced interface gives

$$
\left[\frac{\widehat w}{U-c}\right]=0,\qquad
\left[(U-c)\widehat w'-U'\widehat w-\frac{g\rho}{\rho_0}\frac{\widehat w}{U-c}\right]=0.
$$

The first follows from the [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition) $ik(U-c)\widehat\eta=\widehat w$. The second uses $\widehat p=\rho_0[(U-c)\widehat w'-U'\widehat w]/(ik)$ and hydrostatic displacement $[\widehat p-g\rho\widehat\eta]=0$. These conditions apply to density, velocity and vorticity jumps within the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation).

###### Endpoint derivative map for an evanescent wave layer

↑ **Parent:** [Jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow)

For $\psi''=\alpha^2\psi$ on $-1<z<1$ with endpoint values $P=\psi(1)$ and $Q=\psi(-1)$, the interior derivatives are $\psi'(1)=\alpha[\coth(2\alpha)P-\operatorname{csch}(2\alpha)Q]$ and $\psi'(-1)=\alpha[\operatorname{csch}(2\alpha)P-\coth(2\alpha)Q]$. Fitting the hyperbolic-function solution proves the map. It turns matching conditions into a finite-dimensional interface system, with exponentially small cross-interface coupling at large $\alpha$.

###### Gravity-vorticity interface wave

↑ **Parent:** [Jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow)

At an isolated interface with continuous base [velocity](classical-mechanics.md#velocity), a stable density drop $\Delta\rho/2$ and a jump $[U']$ of base shear, decaying disturbances $w\propto e^{-k|z-z_i|}$ obey the displayed [dispersion relation](wave-equation.md#dispersion-relation). It follows by inserting their derivative jump $[w']=-2kw$ into the [jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow). Both the density jump and the [vorticity](fluid-mechanics.md#vorticity) jump contribute to the intrinsic [phase velocity](wave-equation.md#phase-velocity) $c-U_i$.

###### Internal-wave transmission across a velocity jump

↑ **Parent:** [Jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow)

Across a horizontal material interface with continuous background [mass density](fluid-mechanics.md#density) but a velocity jump, an [internal gravity wave](#internal-wave) preserves laboratory [frequency](physics.md#frequency) and horizontal [wavenumber](wave-equation.md#wavenumber). The matching conditions are continuity of displacement $w/\widehat\omega$ and [pressure](thermodynamics.md#pressure), not continuity of $w$. For [wave amplitudes](physics.md#wave-amplitude) and upward phase-line angles measured from the vertical $\theta_1,\theta_2$, define $r=\widehat\omega_2/\widehat\omega_1$. Then the transmission coefficient is

$$
\frac{A_t}{A_i}=\frac2{r^{-1}\cos\theta_2/\cos\theta_1+r\sin\theta_2/\sin\theta_1}.
$$

The displacement condition is $A_i+A_r=A_t\cos\theta_2/(r\cos\theta_1)$, while pressure continuity gives $A_i-A_r=rA_t\sin\theta_2/\sin\theta_1$. Adding eliminates the reflected amplitude and gives the coefficient. It assumes nonzero intrinsic frequencies and propagating outgoing branches.

###### Displacement impedance for an internal wave at a velocity jump

↑ **Parent:** [Internal-wave transmission across a velocity jump](#internal-wave-transmission-across-a-velocity-jump)

At a material velocity jump with continuous background [mass density](fluid-mechanics.md#density), vertical displacement $\eta$ and [fluid pressure](fluid-mechanics.md#fluid-pressure) are continuous, while $w=ikU\eta$ need not be. For a stationary component, $p=U^2\eta_z$ and the signed upward-wave impedance is $Z=U^2m$. Reflection and vertical-displacement transmission are $R=(Z_1-Z_2)/(Z_1+Z_2)$ and $T=2Z_1/(Z_1+Z_2)$.

###### Dispersion relation for two density interfaces in uniform shear

↑ **Parent:** [Jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow)

Two equal stable density jumps of size $\Delta\rho/2$ at $z=\pm h/2$ lie in the global [linear shear flow](fluid-mechanics.md#linear-shear-flow) $U=\Delta Uz/h$. Decaying [normal modes](wave-equation.md#normal-mode) have

$$
\widehat w=b_+e^{-k|z-h/2|}+b_-e^{-k|z+h/2|}.
$$

The [jump conditions for stratified inviscid shear flow](#jump-conditions-for-stratified-inviscid-shear-flow) give the determinant equation

$$
[(\Delta U/2-c)^2-d][(-\Delta U/2-c)^2-d]-d^2e^{-2kh}=0,\qquad d=\frac{g\Delta\rho}{4\rho_0k}.
$$

Writing $\alpha=kh/2$, $J=g\Delta\rho h/(\rho_0\Delta U^2)$ and $\widetilde c=2c/\Delta U$, this is

$$
\widetilde c^4-(2+J/\alpha)\widetilde c^2+(1-J/(2\alpha))^2-\left[J/(2\alpha)\right]^2e^{-4\alpha}=0.
$$

The two roots for $\widetilde c^2$ are real; one is negative exactly when $2\alpha/(1+e^{-2\alpha})<J<2\alpha/(1-e^{-2\alpha})$. At large $\alpha$, this narrow band centres on $J=2\alpha$, where the isolated counterpropagating [interfacial gravity waves](#interfacial-gravity-wave) have the same zero laboratory speed. This realizes [counterpropagating wave instability](hydrodynamic-stability.md#counterpropagating-wave-instability).

##### Scorer parameter

↑ **Parent:** [Taylor–Goldstein equation](#taylor-goldstein-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scorer_parameter)

The Scorer parameter is the height-dependent coefficient $l^2$ in the stationary atmospheric-wave equation $\widehat w''+(l^2-k^2)\widehat w=0$. Regions with $l^2>k^2$ support vertically oscillatory disturbances, whereas $l^2<k^2$ makes them vertically evanescent.

###### Stationary internal-wave WKB solution

↑ **Parent:** [Scorer parameter](#scorer-parameter)

For a stationary [internal gravity wave](#internal-wave), the [Taylor–Goldstein equation](#taylor-goldstein-equation) gives $m^2=N^2/U^2-U''/U-k^2$. In a propagating interval with slowly varying $m$, the [WKB approximation](analysis.md#wkb-approximation) has amplitude proportional to $m^{-1/2}$ and phase derivative $m$. The conditions $|m'|\ll m^2$ and $|m''|\ll |m|^3$ fail at a regular turning level. With $U>0$, the upward branch has $m>0$ and negative [intrinsic frequency](#intrinsic-frequency); laboratory [group velocity](wave-equation.md#group-velocity) is $U(k^2,km)/(k^2+m^2)$ when the curvature term is negligible.

###### Vertical trapping of an atmospheric gravity wave

↑ **Parent:** [Scorer parameter](#scorer-parameter)

An [atmospheric internal gravity wave](#atmospheric-internal-gravity-wave) is vertically trapped when its squared vertical wavenumber changes from positive to negative with altitude. A decrease of the [Scorer parameter](#scorer-parameter), caused for example by increasing wind speed or decreasing [buoyancy frequency](#buoyancy-frequency), creates a turning level and an evanescent upper region.

###### Turning level of a stationary internal wave

↑ **Parent:** [Vertical trapping of an atmospheric gravity wave](#vertical-trapping-of-an-atmospheric-gravity-wave)

A vertically propagating [stationary topographic internal gravity wave](#stationary-topographic-internal-gravity-wave) meets a turning level when its squared vertical [wavenumber](wave-equation.md#wavenumber) changes from positive to negative. The [stationary internal-wave WKB solution](#stationary-internal-wave-wkb-solution) then fails locally. A simple zero is resolved by an [Airy function](differential-equation.md#airy-function) transition connecting incident and reflected waves below to a decaying [evanescent wave](continuum-mechanics.md#evanescent-wave) above. For negligible wind curvature the condition is $|kU(z_t)|=N(z_t)$, distinct from the zero-intrinsic-frequency [critical layer in a shear flow](hydrodynamic-stability.md#critical-layer-in-a-shear-flow).

###### Turning height of a stationary wave in linear shear

↑ **Parent:** [Vertical trapping of an atmospheric gravity wave](#vertical-trapping-of-an-atmospheric-gravity-wave)

For constant [buoyancy frequency](#buoyancy-frequency) $N$ and $U=U_0+Sz$ with $S>0$, a stationary component of horizontal [wavenumber](wave-equation.md#wavenumber) $k$ turns at $z_t=(N/k-U_0)/S$ if it propagates at the source. Its vertical [wavenumber](wave-equation.md#wavenumber) vanishes there; [WKB approximation](analysis.md#wkb-approximation) fails and an [Airy function](differential-equation.md#airy-function) transition connects reflection to an upper [evanescent wave](continuum-mechanics.md#evanescent-wave).

### Density stratification

↑ **Parent:** [Internal wave](#internal-wave)

Density stratification is variation of a fluid's [mass density](fluid-mechanics.md#density) with height. Its stable or unstable character depends on whether the [buoyancy](fluid-mechanics.md#buoyancy) force restores or amplifies a displaced parcel.

#### Density gradient

↑ **Parent:** [Density stratification](#density-stratification)

The density gradient is the [gradient](calculus.md#gradient) of a spatial [mass density](fluid-mechanics.md#density) field. With an upward vertical coordinate in the [Boussinesq approximation](geophysical-fluid-dynamics.md#boussinesq-approximation), the squared [buoyancy frequency](#buoyancy-frequency) is $N^2=-(g/\rho_*)\partial_z\rho_0$. A negative vertical density gradient therefore gives [stable density stratification](#stable-density-stratification).

#### Halocline

↑ **Parent:** [Density stratification](#density-stratification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Halocline)

A layer with a pronounced vertical change in [salinity](physics.md#salinity) is a halocline. When relatively fresh surface water lies over saltier water, its contribution to [density stratification](#density-stratification) inhibits vertical exchange. A cold Arctic halocline can separate [sea ice](geophysics.md#sea-ice) from warmer Atlantic water; increased heat at depth does not imply an equally increased [ocean heat flux](geophysics.md#ocean-heat-flux) at the ice unless the intervening exchange also changes.

##### Cold halocline

↑ **Parent:** [Halocline](#halocline)

The Arctic cold halocline is a near-freezing layer in which [salinity](physics.md#salinity) increases downward and produces [stable density stratification](#stable-density-stratification), helping isolate [sea ice](geophysics.md#sea-ice) from warmer water below. It can be maintained through shelf-water input, cooling and limited winter convection of inflowing waters, followed by freshwater capping and advection. Its formation cannot be inferred from shelf area alone: water-mass volumes, salt budgets and residence times matter.

#### Ocean mixed layer

↑ **Parent:** [Density stratification](#density-stratification)

The ocean mixed layer is a near-surface layer with relatively weak vertical variations of [temperature](thermodynamics.md#temperature) and [mass density](fluid-mechanics.md#density), maintained by mixing. Beneath it, [stable density stratification](#stable-density-stratification) can isolate colder water from recent surface heating. The mixed-layer depth is not necessarily the full local water depth.

#### Stable density stratification

↑ **Parent:** [Density stratification](#density-stratification)

A fluid has stable density stratification when a small vertical displacement produces a restoring [buoyancy](fluid-mechanics.md#buoyancy) force. In a gravitational field this normally means that [mass density](fluid-mechanics.md#density) increases downward.

##### Ozmidov length

↑ **Parent:** [Stable density stratification](#stable-density-stratification)

Equating an inertial eddy turnover time to the inverse [buoyancy frequency](#buoyancy-frequency) gives the scale separating buoyancy-affected motions from a smaller approximately isotropic cascade. It is distinct from the viscous [Kolmogorov microscales](turbulence.md#kolmogorov-microscales). In very stable local surface-layer scaling it is proportional to the [Obukhov length](continuum-mechanics.md#monin-obukhov-length), up to closure constants.

##### Potential-energy cost of homogenizing a linear stratification

↑ **Parent:** [Stable density stratification](#stable-density-stratification)

Homogenizing the top depth $h$ of a constant-gradient stable stratification over horizontal area $\mathcal A$ creates mean density $\rho_t+\rho_0N^2h/(2g)$. Comparing gravitational potential energies before and after gives $\Delta P=\rho_0\mathcal A N^2h^3/12$. The density jump at the base has [reduced gravity](reduced-gravity.md) $N^2h/2$. The cubic energy cost leads to a quadratic-in-depth coefficient multiplying the deepening rate.

##### Unstable density stratification

↑ **Parent:** [Stable density stratification](#stable-density-stratification)

A fluid has unstable density stratification when a vertical displacement amplifies itself. Denser fluid above lighter fluid can overturn by [Rayleigh-Taylor instability](continuum-mechanics.md#rayleigh-taylor-instability) or develop [thermal convection](fluid-mechanics.md#thermal-convection) when the density difference is thermal.

### Buoyancy frequency

↑ **Parent:** [Internal wave](#internal-wave)

The buoyancy frequency is the natural angular frequency of small vertical oscillations in a stably stratified fluid.

#### Radial buoyancy frequency

↑ **Parent:** [Buoyancy frequency](#buoyancy-frequency)

The radial buoyancy frequency describes restoration of a radially displaced parcel in a stratified [astrophysical disk](astrophysics.md#astrophysical-disk). With a dimensionless [specific entropy](thermodynamics.md#specific-entropy) $S$, its square is proportional to $-\rho^{-1}(dP/dr)(dS/dr)$. Negative $N_r^2$ means an adverse entropy stratification, but [epicyclic motion](astrophysics.md#epicyclic-motion) can still stabilize the parcel. For smooth [thin disk](astrophysics.md#thin-disk) profiles, $|N_r^2|$ is usually of order $(H/r)^2\Omega^2$.

<h5 id="radial-solberg-hoiland-instability-criterion">Radial Solberg–Høiland instability criterion</h5>

↑ **Parent:** [Radial buoyancy frequency](#radial-buoyancy-frequency)

For ideal axisymmetric radial displacements in a [Keplerian shearing sheet](gravitational-instability-of-an-astrophysical-disk.md#keplerian-shearing-sheet), the hydrodynamic squared oscillation frequency is $N_r^2+\kappa^2$, with [radial epicyclic frequency](astrophysics.md#radial-epicyclic-frequency) $\kappa=\Omega$. Exponential instability occurs when $N_r^2+\kappa^2<0$. This is the radial special case of rotating-fluid convective stability, rather than the complete set of three-dimensional Solberg–Høiland criteria.

#### Dry parcel buoyancy in a homogeneous atmosphere

↑ **Parent:** [Buoyancy frequency](#buoyancy-frequency)

For a dry, homogeneous [ideal gas](thermodynamics.md#ideal-gas) in [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium), a displaced parcel undergoing an [adiabatic process](thermodynamics.md#adiabatic-process) follows $dT/dz=-g/C_p$, where $C_p$ is [specific heat capacity at constant pressure](thermodynamics.md#specific-heat-capacity-at-constant-pressure). At a common pressure its buoyancy depends on its temperature difference from the environment, giving $N^2=(g/T)(dT/dz+g/C_p)$. Negative $N^2$ means growing displacements; zero $N^2$ means neutral stability. This is the homogeneous dry limit of the [Schwarzschild criterion](stellar-structure.md#schwarzschild-criterion).

#### Richardson number

↑ **Parent:** [Buoyancy frequency](#buoyancy-frequency)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Richardson_number)

A Richardson number compares gravitational stratification with inertial or shear effects. Its precise form depends on the characteristic scales or local gradients being compared.

##### Flux Richardson number

↑ **Parent:** [Richardson number](#richardson-number)

The ratio of stable buoyancy destruction to shear production of turbulent kinetic energy. With down-gradient transport and [turbulent Prandtl number](turbulence.md#turbulent-prandtl-number) $\mathrm{Pr}_t$, it obeys $\mathrm{Ri}_f=\mathrm{Ri}_g/\mathrm{Pr}_t$, rather than automatically equaling the [gradient Richardson number](#gradient-richardson-number). Unstable buoyancy production gives a negative value in this convention.

###### Buoyancy fraction of total turbulent sinks

↑ **Parent:** [Flux Richardson number](#flux-richardson-number)

With positive stable buoyancy destruction $B$ and positive dissipation $\epsilon$, this normalized sink fraction need not equal the [Flux Richardson number](#flux-richardson-number) $B/P$ away from equilibrium. If $R=(B+\epsilon)/P$, then $J=\mathrm{Ri}_f/R$. In the [fixed-correlation equilibrium model for stratified turbulence](turbulence.md#fixed-correlation-equilibrium-model-for-stratified-turbulence), a minimum of $R=a/q+bq$ has $B=\epsilon$, hence $J=1/2$. The actual flux Richardson number there is $R_{\min}/2$ and equals $1/2$ only when that minimum also satisfies the equilibrium condition $R=1$.

##### Interfacial Richardson number

↑ **Parent:** [Richardson number](#richardson-number)

A local ratio of stabilizing buoyancy to shear across an interface of thickness $\delta$, using [reduced gravity](reduced-gravity.md) jump $g'$ and characteristic velocity $u$. The dimensionless value is $\mathrm{Ri}_i=g'\delta/u^2$. It is distinct from a whole-layer bulk [Richardson number](#richardson-number) based on the total mixed depth. Local [entrainment](fluid-mechanics.md#fluid-entrainment) laws use this ratio when the transition thickness and velocity characterize the turbulence-producing region.

###### Entrainment exponent from a local interfacial Richardson closure

↑ **Parent:** [Interfacial Richardson number](#interfacial-richardson-number)

Combine a fixed-energy mixed-layer relation $u^2h=A\Omega^2R^3$, jump $g'=N^2h/2$, and stress power proportional to $u^3$ with an energy-transfer factor $(\Omega/N)^\alpha(\delta/R)^\beta$. Eliminating depth in favor of the [interfacial Richardson number](#interfacial-richardson-number) gives $E\propto(\Omega/N)^{\alpha-1}(\delta/R)^{\beta+3/2}\mathrm{Ri}_i^{-3/2}$. A local-only [entrainment](fluid-mechanics.md#fluid-entrainment) closure requires $\alpha=1$, $\beta=-3/2$ and exponent $3/2$ on the [Richardson number](#richardson-number).

##### Bulk Richardson number

↑ **Parent:** [Richardson number](#richardson-number)

A [bulk Richardson number](#bulk-richardson-number) compares a characteristic buoyancy difference across a layer with the squared characteristic flow speed. It uses large-scale differences rather than the pointwise [gradient Richardson number](#gradient-richardson-number). Its normalization depends on the chosen velocity, density and length scales.

##### Gradient Richardson number

↑ **Parent:** [Richardson number](#richardson-number)

For a stratified parallel [shear flow](fluid-mechanics.md#shear-flow), the gradient Richardson number compares the squared [buoyancy frequency](#buoyancy-frequency) with squared vertical shear. The [Miles–Howard theorem](#miles-howard-theorem) excludes exponentially growing inviscid [normal modes](wave-equation.md#normal-mode) when this ratio is at least $1/4$ everywhere. Where $U'=0$, the equivalent criterion is written directly as $N^2\geq(U')^2/4$.

#### Stellar buoyancy frequency

↑ **Parent:** [Buoyancy frequency](#buoyancy-frequency)

In a spherically symmetric stellar model with inward gravity magnitude $g$, the squared buoyancy frequency is

$$
N^2=g\left(\frac1{\gamma p}\frac{dp}{dr}-\frac1\rho\frac{d\rho}{dr}\right).
$$

Positive $N^2$ gives stable stratification. Regular central profiles have $g=O(r)$ and logarithmic pressure and density gradients of order $r$, so $N^2=O(r^2)$ near the center.

### Internal-wave phase and group velocity

↑ **Parent:** [Internal wave](#internal-wave)

For a uniformly stratified fluid, internal-wave phase velocity is parallel to the wavevector while group velocity is perpendicular to it. Energy from a localized monochromatic source propagates along four beams forming a St Andrew's cross.

#### Right-triangle geometry of internal-wave velocities

↑ **Parent:** [Internal-wave phase and group velocity](#internal-wave-phase-and-group-velocity)

Choose $k,m>0$, $K=(k^2+m^2)^{1/2}$ and the positive [angular frequency](classical-mechanics.md#angular-frequency) $\omega=Nk/K$. Then the [phase velocity](wave-equation.md#phase-velocity) is $Nk(k,m)/K^3$ and the [group velocity](wave-equation.md#group-velocity) is $N(m^2,-km)/K^3$. Their [dot product](linear-algebra.md#dot-product) vanishes and their sum is horizontal with magnitude $N/K$. Draw the [group velocity](wave-equation.md#group-velocity) from the tip of the [phase velocity](wave-equation.md#phase-velocity): the two form the perpendicular sides of a [right triangle](geometry-and-topology.md#right-triangle). The horizontal hypotenuse is their sum, not the [horizontal phase velocity](wave-equation.md#horizontal-phase-velocity) $\omega/k$.

#### Internal-wave polarization

↑ **Parent:** [Internal-wave phase and group velocity](#internal-wave-phase-and-group-velocity)

For a propagating, non-cutoff two-dimensional [internal gravity wave](#internal-wave) proportional to $e^{i(kx+mz-\omega t)}$, [incompressibility](fluid-mechanics.md#incompressible-flow) gives $U=-mW/k$. Thus the oscillatory [velocity field](fluid-mechanics.md#velocity-field) is perpendicular to the [wavevector](continuum-mechanics.md#wavevector) and parallel to the [group velocity](wave-equation.md#group-velocity), whereas the [phase velocity](wave-equation.md#phase-velocity) is parallel to the [wavevector](continuum-mechanics.md#wavevector).

##### Buoyancy polarization of a plane internal gravity wave

↑ **Parent:** [Internal-wave polarization](#internal-wave-polarization)

For a nonrotating [plane internal gravity wave](#plane-internal-gravity-wave) with phase $kx+mz-\omega t$, let $K^2=k^2+m^2$, $k\ne0$, and use [kinematic pressure](thermodynamics.md#kinematic-pressure). The [Linearized Boussinesq equations](geophysical-fluid-dynamics.md#linearized-boussinesq-equations) and $\mathbf u=\partial_t\boldsymbol\xi$ give $\widehat u=-im\omega\widehat\sigma/(kN^2)$, $\widehat\xi=m\widehat\sigma/(kN^2)$ and $\widehat p=-im\widehat\sigma/K^2$, together with the displayed vertical relations. [Buoyancy](fluid-mechanics.md#buoyancy) and [displacement field](continuum-mechanics.md#displacement-field-mechanics) are in phase or opposite phase; [velocity](classical-mechanics.md#velocity) and [pressure](thermodynamics.md#pressure) are in [quadrature](physics.md#phase-quadrature) with them. [Incompressibility](fluid-mechanics.md#incompressible-flow) makes both the oscillating [velocity](classical-mechanics.md#velocity) and [displacement field](continuum-mechanics.md#displacement-field-mechanics) perpendicular to the [wavevector](continuum-mechanics.md#wavevector).

#### Constant-phase line of an internal gravity wave

↑ **Parent:** [Internal-wave phase and group velocity](#internal-wave-phase-and-group-velocity)

For a two-dimensional [internal gravity wave](#internal-wave) with phase $kx+\int m(z)\,dz-\omega t$, a constant-phase line at fixed time has slope $dz/dx=-k/m(z)$. Its normal spacing from the next crest is $2\pi/(k^2+m^2)^{1/2}$; the [wavevector](continuum-mechanics.md#wavevector) $(k,m)$ is normal to the line. The intrinsic energy ray is tangent to these phase lines, while mean-flow [advection](fluid-mechanics.md#advection) changes the laboratory ray direction.

### Reflection of an internal-wave ray

↑ **Parent:** [Internal wave](#internal-wave)

At a stationary slope, an internal wave preserves frequency and tangential wavenumber. Unlike specular reflection, the reflected energy ray preserves its angle to the vertical; a supercritical slope can reverse its horizontal propagation direction.

#### Internal-wave slope criticality

↑ **Parent:** [Reflection of an internal-wave ray](#reflection-of-an-internal-wave-ray)

Let an [internal gravity wave](#internal-wave) energy ray make angle $\theta$ with the horizontal, so that $\sin\theta=\omega/N$. A boundary of local slope magnitude $s$ is subcritical, critical, or supercritical according as $s$ is smaller than, equal to, or larger than $\tan\theta$. At criticality the inviscid reflected wavelength tends to zero.

##### Subcritical internal-wave reflection

↑ **Parent:** [Internal-wave slope criticality](#internal-wave-slope-criticality)

In subcritical internal-wave reflection, the boundary is everywhere less steep than the energy ray. The reflected ray leaves the boundary without the singular shortening associated with a critical slope.

##### Critical internal-wave reflection

↑ **Parent:** [Internal-wave slope criticality](#internal-wave-slope-criticality)

At critical internal-wave reflection, the reflected group velocity is tangent to the boundary and the inviscid reflected wavenumber diverges. [Kinematic viscosity](fluid-mechanics.md#kinematic-viscosity), [mass diffusivity](fluid-mechanics.md#mass-diffusivity), nonlinear steepening, and wave breaking regularize the ideal singularity.

#### Topographic sideband of an internal gravity wave

↑ **Parent:** [Reflection of an internal-wave ray](#reflection-of-an-internal-wave-ray)

Reflection from periodic topography couples an incident horizontal wavenumber $k$ to sidebands $k+jk_T$. Expanding the impermeability condition on a boundary of small amplitude $h_0$ produces the $j=\pm1$ sidebands at order $h_0$ and the $j=0,\pm2$ corrections at order $h_0^2$.

#### Internal-wave ray tracing

↑ **Parent:** [Reflection of an internal-wave ray](#reflection-of-an-internal-wave-ray)

Internal-wave ray tracing follows the [group velocity](wave-equation.md#group-velocity) while preserving the wave frequency. In a uniformly stratified fluid, each straight ray keeps the angle $\sin^{-1}(\omega/N)$ to the horizontal until reflection or a change in the medium.

##### Internal-wave ray in uniform vertical shear

↑ **Parent:** [Internal-wave ray tracing](#internal-wave-ray-tracing)

For $U=sz$, $N>0$, $k>0$ and the rising branch $m_0<0$, the Hamiltonian is $\omega=ksz+Nk/\sqrt{k^2+m^2}$. It gives constant $\omega,k$ and $m=m_0-kst$. The height approaches $z_c=\omega/(ks)$ as time tends to infinity. With $\theta=\arctan(|m|/k)$, the ray slope is $dx/dz=\tan\theta+ksz/(N\sin\theta\cos^2\theta)$. The intrinsic and absolute frequencies must not be confused.

###### Circular mountain-wave ray in linear shear

↑ **Parent:** [Internal-wave ray in uniform vertical shear](#internal-wave-ray-in-uniform-vertical-shear)

For a stationary [internal gravity wave](#internal-wave) in constant [buoyancy frequency](#buoyancy-frequency) $N$ and wind $U=U_0(1+z/H)$, set $q_0=kU_0/N<1$. Its upward [group velocity](wave-equation.md#group-velocity) has ratio $dx/dz=k/m=q/\sqrt{1-q^2}$, where $q=q_0(1+z/H)$. Integrating from the origin gives a circular ray with center $(H\sqrt{1-q_0^2}/q_0,-H)$ and radius $H/q_0$. The ascending ray becomes horizontal at the [turning level of a stationary internal wave](#turning-level-of-a-stationary-internal-wave); its reflected branch continues downwind along the same circle.

##### Internal-wave attractor

↑ **Parent:** [Internal-wave ray tracing](#internal-wave-ray-tracing)

A periodic spatial [internal-wave ray](#internal-wave-ray-tracing) toward which neighbouring ray paths converge after reflection in a confined stratified basin. A fixed point of an [internal-wave ray return map](#internal-wave-ray-return-map) is attracting when its derivative has magnitude below one. [Viscous attenuation of an internal-wave beam](#viscous-attenuation-of-an-internal-wave-beam) and [internal-wave breaking](#internal-wave-breaking) regularize the ideal [concentration](physics.md#concentration) of energy. A spatial ray construction does not remove turning-level limitations of the [WKB approximation](analysis.md#wkb-approximation).

###### Internal-wave ray return map

↑ **Parent:** [Internal-wave attractor](#internal-wave-attractor)

Map one boundary intersection of an [internal-wave ray](#internal-wave-ray-tracing) to the next intersection with the same boundary after a specified reflection itinerary. A periodic ray is a fixed point. Linear contraction, $|R'|<1$, gives an [internal-wave attractor](#internal-wave-attractor); the reversed itinerary, when invertible, has reciprocal multiplier and is locally repelling.

##### Double-zero internal-wave turning level

↑ **Parent:** [Internal-wave ray tracing](#internal-wave-ray-tracing)

A level where the squared vertical [wavenumber](wave-equation.md#wavenumber) of an [internal gravity wave](#internal-wave) touches zero quadratically without changing sign. The ordinary [WKB approximation](analysis.md#wkb-approximation) fails there; unlike a simple sign-changing turning point, this does not itself provide an evanescent region on one side. Finite-wavelength analysis determines how solutions connect across or meet a boundary at the level.

##### Causal envelope of stationary internal waves

↑ **Parent:** [Internal-wave ray tracing](#internal-wave-ray-tracing)

In uniform positive flow $U$, upward stationary [internal gravity waves](#internal-wave) have laboratory [group velocity](wave-equation.md#group-velocity) $U(\cos^2\theta,\sin\theta\cos\theta)$. Packets emitted by a localized source at startup lie on $(x-Ut/2)^2+z^2=(Ut/2)^2$, with later emissions inside. This envelope belongs to the permanent stationary component, not every possible startup transient.

###### Refraction of a stationary internal-wave causal envelope

↑ **Parent:** [Causal envelope of stationary internal waves](#causal-envelope-of-stationary-internal-waves)

A lower ray reaches $H$ after $\tau_1=H/[U_1\sin\theta_1\cos\theta_1]$, at $x_H=H\cot\theta_1$. Conserved horizontal [wavenumber](wave-equation.md#wavenumber) gives $\cos\theta_2=(U_2N_1/U_1N_2)\cos\theta_1$. The transmitted front is $(x_H,H)+(t-\tau_1)\mathbf c_{g2}$ on propagating branches; reflection reverses the vertical [group velocity](wave-equation.md#group-velocity).

###### First arrival of a stationary internal wavefront at a layer boundary

↑ **Parent:** [Causal envelope of stationary internal waves](#causal-envelope-of-stationary-internal-waves)

A broad-spectrum stationary source below height $H$ first sends an upward packet there after $2H/U$, at $x=H$. This uses the maximum vertical [group velocity](wave-equation.md#group-velocity) $U/2$ at $\theta=\pi/4$. A source lacking the corresponding [wavenumber](wave-equation.md#wavenumber) has a later actual arrival.

#### Focusing power of internal-wave reflection

↑ **Parent:** [Reflection of an internal-wave ray](#reflection-of-an-internal-wave-ray)

For an [internal gravity wave](#internal-wave) ray at angle $\theta$ to the horizontal reflecting from a slope at angle $\alpha$, conservation of tangential [wavenumber](wave-equation.md#wavenumber) gives

$$
\gamma=\frac{k_{\rm reflected}}{k_{\rm incident}}
=\frac{\sin(\theta+\alpha)}{\sin(\theta-\alpha)}.
$$

At a [subcritical internal-wave reflection](#subcritical-internal-wave-reflection), $\gamma>1$: the reflected wavelength shortens and its wavelength-averaged [energy density](statistical-physics.md#energy-density) increases by $\gamma^2$.

### Viscous attenuation of an internal-wave beam

↑ **Parent:** [Internal wave](#internal-wave)

When [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) and [mass diffusivity](fluid-mechanics.md#mass-diffusivity) are equal to $\epsilon$, a monochromatic internal-wave beam with [wavenumber](wave-equation.md#wavenumber) $k$ and ray angle $\theta$ has leading stream-function amplitude

$$
A(\zeta)=A(0)\exp\left(-\frac{\epsilon k^3\zeta}{N\cos\theta}\right)
=A(0)e^{-k\zeta/\operatorname{Re}},
\qquad
\operatorname{Re}=\frac{N\cos\theta}{\epsilon k^2}.
$$

The cubic dependence on $k$ makes slope-focused, short internal waves dissipate especially rapidly.

#### Oscillatory drift of an attenuated internal-wave beam

↑ **Parent:** [Viscous attenuation of an internal-wave beam](#viscous-attenuation-of-an-internal-wave-beam)

In the prescribed along-beam scalar model $U=A(\xi)\cos\omega t$ with $A=U_0e^{-\lambda\xi}$, the first-order [fluid displacement](fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) is $A\sin\omega t/\omega$. Its leading sampled-velocity correction is $-\lambda A^2\sin(2\omega t)/(2\omega)$, whose [period average](function.md#period-average) vanishes. This result concerns the supplied component model and does not determine an Eulerian mean streaming flow.

### Vertical trapping of an internal gravity wave by planar strain

↑ **Parent:** [Internal wave](#internal-wave)

For the planar strain $\mathbf U=\gamma(x,0,-z)$, an internal-wave ray has

$$
k=k_0e^{-\gamma t},
\qquad
m=m_0e^{\gamma t}.
$$

If it initially propagates upward with $m_0<0$, its height remains positive at finite time but decays to zero exponentially as $t\to\infty$.

### Mountain-wave cutoff

↑ **Parent:** [Internal wave](#internal-wave)

A steady hill pattern seen by a uniform flow of speed $U$ has intrinsic frequency magnitude $Uk$. It radiates a propagating internal wave only for $k\leq N/U$; above this cutoff the vertical wavenumber is imaginary and the disturbance is evanescent.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Equatorial wave velocity polarization](geophysical-fluid-dynamics.md#equatorial-wave-velocity-polarization)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-333.md#4/solution)
- [Potential-vorticity inversion](geophysical-fluid-dynamics.md#potential-vorticity-inversion)
