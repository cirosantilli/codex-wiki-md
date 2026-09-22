# Porous-media flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Porous-media_flow)

Porous-media flow is fluid motion through an interconnected pore space. At small pore-scale [Reynolds number](fluid-mechanics.md#reynolds-number), its volume-averaged velocity is commonly governed by [Darcy's law](#darcy-law).

**Table of contents**

- [Aquifer](#aquifer)
  - [Unconfined aquifer](#unconfined-aquifer)
    - [Boussinesq equation for an unconfined aquifer](#boussinesq-equation-for-an-unconfined-aquifer)
      - [Conserved first moment of a draining porous current](#conserved-first-moment-of-a-draining-porous-current)
        - [Dipole similarity solution of a draining porous current](#dipole-similarity-solution-of-a-draining-porous-current)
          - [Drainage volume decay in a dipole porous current](#drainage-volume-decay-in-a-dipole-porous-current)
      - [Separable aquifer drawdown](#separable-aquifer-drawdown)
    - [Dupuit approximation](#dupuit-approximation)
      - [Dupuit flow in a channel with cubic wetted area](#dupuit-flow-in-a-channel-with-cubic-wetted-area)
    - [Unconfined aquifer with depth-dependent permeability](#unconfined-aquifer-with-depth-dependent-permeability)
      - [Outlet layer in a deep unconfined aquifer](#outlet-layer-in-a-deep-unconfined-aquifer)
    - [Poroelastic aquifer](#poroelastic-aquifer)
      - [Poroelastic compaction length](#poroelastic-compaction-length)
- [Delayed polymer diversion in parallel porous layers](#delayed-polymer-diversion-in-parallel-porous-layers)
- [Thermal front in a porous medium](#thermal-front-in-a-porous-medium)
- [Porous medium](#porous-medium)
- [Resident-weighted transit time in a layered flow](#resident-weighted-transit-time-in-a-layered-flow)
- [Capillary imbibition](#capillary-imbibition)
  - [Hemispherical capillary imbibition](#hemispherical-capillary-imbibition)
    - [Evaporation-limited hemispherical imbibition](#evaporation-limited-hemispherical-imbibition)
- [Two-phase porous-media flow](#two-phase-porous-media-flow)
  - [Capillary residual trapping](#capillary-residual-trapping)
    - [Residual-trapping attenuation of a porous current](#residual-trapping-attenuation-of-a-porous-current)
      - [Mobile-volume peak of an exponentially forced porous current](#mobile-volume-peak-of-an-exponentially-forced-porous-current)
    - [Triangular current with capillary retention](#triangular-current-with-capillary-retention)
      - [Maximum-invasion envelope of a retained current](#maximum-invasion-envelope-of-a-retained-current)
  - [Waterflooding](#waterflooding)
  - [Buckley-Leverett equation](#buckley-leverett-equation)
    - [Capillary diffusion](#capillary-diffusion)
    - [Fractional-flow tangent construction](#fractional-flow-tangent-construction)
  - [Fractional flow](#fractional-flow)
  - [Fluid saturation](#fluid-saturation)
- [Flux-weighted residence time in a porous layer](#flux-weighted-residence-time-in-a-porous-layer)
- [Vertical imbibition under a draining liquid layer](#vertical-imbibition-under-a-draining-liquid-layer)
- [Darcy law](#darcy-law)
  - [Darcy flow](#darcy-flow)
    - [Lubrication boundary condition for a crack in a Darcy medium](#lubrication-boundary-condition-for-a-crack-in-a-darcy-medium)
      - [Crack pressure in elliptic coordinates](#crack-pressure-in-elliptic-coordinates)
        - [Elliptic crack pressure dipole](#elliptic-crack-pressure-dipole)
          - [Fixed-throughflow dissipation reduction of a conductive crack](#fixed-throughflow-dissipation-reduction-of-a-conductive-crack)
  - [Uniformly heated vertical plate in a porous medium](#uniformly-heated-vertical-plate-in-a-porous-medium)
    - [Integral exponential profile for porous wall convection](#integral-exponential-profile-for-porous-wall-convection)
  - [Fixed-pressure planar Darcy displacement](#fixed-pressure-planar-darcy-displacement)
    - [Thermal-front retardation in Darcy flow](#thermal-front-retardation-in-darcy-flow)
  - [Porous thermal plume](#porous-thermal-plume)
    - [Conserved momentum flux of a porous thermal plume](#conserved-momentum-flux-of-a-porous-thermal-plume)
    - [Hyperbolic-secant porous plume profile](#hyperbolic-secant-porous-plume-profile)
      - [Heat-weighted head speed of a porous plume](#heat-weighted-head-speed-of-a-porous-plume)
  - [Darcy dissipation](#darcy-dissipation)
  - [Darcy velocity](#darcy-velocity)
    - [Pore velocity](#pore-velocity)
  - [Darcy-Bénard convection](#darcy-benard-convection)
    - [Insulated square-column Darcy convection onset](#insulated-square-column-darcy-convection-onset)
    - [Conducting-square Darcy convection](#conducting-square-darcy-convection)
      - [Growth-rate solvability for conducting-square Darcy convection](#growth-rate-solvability-for-conducting-square-darcy-convection)
      - [Gauge transformation for conducting-square Darcy onset](#gauge-transformation-for-conducting-square-darcy-onset)
    - [Darcy thermal-time Rayleigh number](#darcy-thermal-time-rayleigh-number)
    - [Onset of convection in a horizontal Darcy layer](#onset-of-convection-in-a-horizontal-darcy-layer)
      - [Supercritical saturation of Darcy convection rolls](#supercritical-saturation-of-darcy-convection-rolls)
        - [Mean-temperature correction in weakly nonlinear Darcy convection](#mean-temperature-correction-in-weakly-nonlinear-darcy-convection)
  - [Saffman–Taylor instability](#saffman-taylor-instability)
    - [Planar viscous-fingering dispersion relation](#planar-viscous-fingering-dispersion-relation)
      - [Thermal-front viscous-fingering dispersion relation](#thermal-front-viscous-fingering-dispersion-relation)
      - [Buoyancy-modified Darcy fingering dispersion relation](#buoyancy-modified-darcy-fingering-dispersion-relation)
      - [Surface-tension-gradient stabilization of viscous fingering](#surface-tension-gradient-stabilization-of-viscous-fingering)
  - [Permeability of a porous medium](#permeability-of-a-porous-medium)
    - [Relative permeability](#relative-permeability)
      - [Phase mobility](#phase-mobility)
    - [Effective permeability](#effective-permeability)
      - [Dilute permeability enhancement by aligned cracks](#dilute-permeability-enhancement-by-aligned-cracks)
      - [Effective permeability of complementary wedges](#effective-permeability-of-complementary-wedges)
    - [Porosity](#porosity)
  - [Pressure-dependent Darcy drainage](#pressure-dependent-darcy-drainage)
- [Reactive infiltration instability](#reactive-infiltration-instability)
  - [Melting-front instability due to permeability contrast](#melting-front-instability-due-to-permeability-contrast)
- [Porous gravity current](#porous-gravity-current)
  - [Inclined porous gravity current](#inclined-porous-gravity-current)
    - [Volume Jacobian for downslope stretched coordinates](#volume-jacobian-for-downslope-stretched-coordinates)
    - [Depth-dependent inclined porous-current equation](#depth-dependent-inclined-porous-current-equation)
      - [Far-downslope width of a constant-flux porous current](#far-downslope-width-of-a-constant-flux-porous-current)
    - [Advection limit of an inclined porous current](#advection-limit-of-an-inclined-porous-current)
  - [One-sided constant-volume porous gravity current](#one-sided-constant-volume-porous-gravity-current)
  - [Slope-driven porous gravity current](#slope-driven-porous-gravity-current)
    - [Caprock leakage threshold](#caprock-leakage-threshold)
    - [Moving thermal front in a porous current](#moving-thermal-front-in-a-porous-current)
  - [Porous gravity current with background flow](#porous-gravity-current-with-background-flow)
    - [Advected constant-volume porous gravity current](#advected-constant-volume-porous-gravity-current)
    - [Constant-flux porous gravity current](#constant-flux-porous-gravity-current)
      - [Diffusive nose of an advected porous gravity current](#diffusive-nose-of-an-advected-porous-gravity-current)
  - [Leaky porous gravity current](#leaky-porous-gravity-current)
    - [Hydrostatic leakage through a basal seal](#hydrostatic-leakage-through-a-basal-seal)
    - [Exponential drainage transform for porous-medium diffusion](#exponential-drainage-transform-for-porous-medium-diffusion)
      - [Invasion envelope of an exponentially draining porous current](#invasion-envelope-of-an-exponentially-draining-porous-current)

## Aquifer

↑ **Parent:** [Porous-media flow](porous-media-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Aquifer)

An aquifer is a permeable geological formation containing and transmitting groundwater. A confined aquifer lies beneath a confining layer; an [unconfined aquifer](#unconfined-aquifer) instead has a free water table.

### Unconfined aquifer

↑ **Parent:** [Aquifer](#aquifer)

An unconfined aquifer has a free groundwater table. In a shallow aquifer of thickness $h(x,t)$, hydrostatic pressure and [Darcy's law](#darcy-law) give horizontal flux proportional to $-hh_x$.

#### Boussinesq equation for an unconfined aquifer

↑ **Parent:** [Unconfined aquifer](#unconfined-aquifer)

For pore fraction $n$, permeability $k$, liquid density $\rho$, viscosity $\mu$, rainfall recharge $R$, and a shallow groundwater thickness $h$,

$$
n h_t=\frac{k\rho g}{\mu}(hh_x)_x+R.
$$

This is a nonlinear diffusion equation with diffusivity proportional to the local thickness.

##### Conserved first moment of a draining porous current

↑ **Parent:** [Boussinesq equation for an unconfined aquifer](#boussinesq-equation-for-an-unconfined-aquifer)

For $h_t=\kappa(hh_x)_x$ with a drained boundary $h(0,t)=0$ and a finite current vanishing at its nose, [integration by parts](calculus.md#integration-by-parts) gives $\dot D=-\kappa[h^2]_0^\infty/2=0$. The outlet can have finite [volume flux](fluid-mechanics.md#volumetric-flow-rate) because its contribution to the first-moment flux is multiplied by $x=0$. A positive prescribed boundary height instead gives $\dot D=\kappa h(0,t)^2/2$, so drainage is essential to this invariant.

###### Dipole similarity solution of a draining porous current

↑ **Parent:** [Conserved first moment of a draining porous current](#conserved-first-moment-of-a-draining-porous-current)

The [conserved first moment of a draining porous current](#conserved-first-moment-of-a-draining-porous-current) fixes $\alpha+2\beta=0$ in a [self-similar solution](partial-differential-equation.md#similarity-solution) $h=a t^\alpha f(x/(dt^\beta))$. The [Boussinesq equation for an unconfined aquifer](#boussinesq-equation-for-an-unconfined-aquifer) supplies $\alpha=2\beta-1$, giving $\alpha=-1/2$, $\beta=1/4$. Normalize $\kappa a=d^2$ and the nose at $\eta=1$. Then $-f/2-\eta f'/4=(ff')'$ is solved by

$$
f(\eta)=\frac{\sqrt\eta-\eta^2}{6}\quad(0<\eta<1),\qquad
D=\frac{ad^2}{40},\quad d=(40\kappa D)^{1/4},\quad a=d^2/\kappa.
$$

The square-root outlet has finite drainage flux and the nose has zero flux. This is a particular similarity solution and its scaling family, not an exact description of arbitrary initial data.

###### Drainage volume decay in a dipole porous current

↑ **Parent:** [Dipole similarity solution of a draining porous current](#dipole-similarity-solution-of-a-draining-porous-current)

For the [dipole similarity solution of a draining porous current](#dipole-similarity-solution-of-a-draining-porous-current), $V=\phi\int h\,dx=\phi ad\,t^{-1/4}/18$. Thus $\dot V/V=-1/(4t)$. A shifted similarity origin replaces $t$ by $t+t_0$. Neither a positive rate nor a rate $-1/(2t)$ is compatible with this two-dimensional first-moment-conserving profile.

##### Separable aquifer drawdown

↑ **Parent:** [Boussinesq equation for an unconfined aquifer](#boussinesq-equation-for-an-unconfined-aquifer)

After recharge stops on a finite aquifer connected to a river, the late solution of the [Boussinesq equation for an unconfined aquifer](#boussinesq-equation-for-an-unconfined-aquifer) has the form $h\sim t^{-1}F(x/L)$. The profile solves a nonlinear eigenvalue problem, and river discharge decays as $t^{-2}$.

#### Dupuit approximation

↑ **Parent:** [Unconfined aquifer](#unconfined-aquifer)

The Dupuit approximation treats flow in a shallow [unconfined aquifer](#unconfined-aquifer) as predominantly horizontal, with [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) $p=\rho g(h-z)$ and horizontal pressure gradient independent of depth. Integrating [Darcy's law](#darcy-law) over the saturated depth then gives a [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) depending only on the groundwater height and its slope.

##### Dupuit flow in a channel with cubic wetted area

↑ **Parent:** [Dupuit approximation](#dupuit-approximation)

For saturated [Darcy flow](#darcy-flow) through a long dam occupying a channel of width $\alpha z^2$, let hydraulic conductivity be $K=k\rho g/\mu$ and free-surface height $h(x)$. The [Dupuit approximation](#dupuit-approximation) gives $Q=-K\alpha h^3h_x/3$. Fixed heads $h(0)=H$ and $h(L)=\eta$ give $h^4=H^4-(H^4-\eta^4)x/L$ and the displayed steady discharge. [Porosity](#porosity) relates pore velocity to superficial [Darcy velocity](#darcy-velocity) but does not independently multiply this discharge when $k$ is intrinsic permeability. For depth-dependent permeability, integrate the horizontal conductivity over the saturated cross-section first.

#### Unconfined aquifer with depth-dependent permeability

↑ **Parent:** [Unconfined aquifer](#unconfined-aquifer)

With [permeability of a porous medium](#permeability-of-a-porous-medium) $k(z)=k_0(1+\beta z)$, the [Dupuit approximation](#dupuit-approximation) gives

$$
q=-u_b\left(h+\frac\beta2h^2\right)h_x,\qquad \phi h_t+q_x=R,\qquad u_b=\frac{k_0\rho g}{\mu}.
$$

Here $\phi$ is [porosity](#porosity) and $R$ is recharge. The low-height limit has mobility proportional to $h$, whereas large heights have mobility proportional to $h^2$. This changes both the [forced filling similarity for power-law diffusion](diffusion-equation.md#forced-filling-similarity-for-power-law-diffusion) and the [separable draining profile for power-law diffusion](diffusion-equation.md#separable-draining-profile-for-power-law-diffusion).

##### Outlet layer in a deep unconfined aquifer

↑ **Parent:** [Unconfined aquifer with depth-dependent permeability](#unconfined-aquifer-with-depth-dependent-permeability)

Even when most of an [unconfined aquifer with depth-dependent permeability](#unconfined-aquifer-with-depth-dependent-permeability) is deep, its height vanishes at an absorbing outlet. Near that outlet, finite outward [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) $Q$ gives $u_bhh_x\simeq Q$ and hence $h\simeq(2Qx/u_b)^{1/2}$. The high-depth outer approximation instead has $h\simeq[6Qx/(u_b\beta)]^{1/3}$. Their crossover lies at height of order $1/\beta$ and distance of order $u_b/(\beta^2Q)$; the thin inner [boundary layer](continuum-mechanics.md#boundary-layer) transmits the same leading discharge.

#### Poroelastic aquifer

↑ **Parent:** [Unconfined aquifer](#unconfined-aquifer)

A poroelastic aquifer couples pore-fluid storage and flow to elastic compaction of its solid skeleton. Changes in gravity, surface loading, or pore pressure can therefore change groundwater discharge even without changing rainfall.

##### Poroelastic compaction length

↑ **Parent:** [Poroelastic aquifer](#poroelastic-aquifer)

For a skeleton with Young modulus $E$, undeformed solid fraction $\phi_0$, grain-fluid density difference $\rho_s-\rho$, and reference gravity $g_0$, the hydrostatic poroelastic compaction length is

$$
\ell_c=\frac{E}{\phi_0(\rho_s-\rho)g_0}.
$$

It is the depth over which self-weight changes the solid fraction appreciably.

## Delayed polymer diversion in parallel porous layers

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

For a fixed pressure difference across two noncommunicating layers, an activated viscous polymer segment of length $\ell_i$ adds hydraulic resistance in series with the remaining fluid. The [Darcy flux](#darcy-velocity) is the displayed expression when polymer raises [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity) by a factor $\lambda$. Tracking particle entry time determines activation and exit, while $\dot X_i=q_i/\phi$ gives each displacement front. Preferentially occupying the more permeable layer shifts the relative inflow toward the other layer, but cannot increase that layer's absolute flux at fixed pressure. It can delay its breakthrough and leave original reservoir fluid flowing after the unmodified reservoir would be fully swept.

## Thermal front in a porous medium

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

A sharp advected temperature transition in a fluid-filled [porous medium](#porous-medium). If fluid and solid equilibrate locally in temperature, their effective heat capacity per total volume is $C_{\rm eff}=\phi C_f+(1-\phi)C_s$, while the advected heat flux is $C_fUT$ with $U$ the [Darcy velocity](#darcy-velocity). Neglecting conduction gives $C_{\rm eff}T_t+C_fUT_x=0$, so the thermal front speed is $\Gamma U$ with $\Gamma=C_f/C_{\rm eff}$. The material [pore velocity](#pore-velocity) is $U/\phi$, so thermal retardation relative to that speed is $\Gamma\phi$. Temperature-dependent viscosity couples thermal-front perturbations back to the [Darcy flux](#darcy-velocity).

## Porous medium

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

A porous medium is a solid framework containing connected voids in which a [fluid](fluid-mechanics.md#fluid) can reside and flow. Its [porosity](#porosity) is the void fraction; its [permeability of a porous medium](#permeability-of-a-porous-medium) measures the ease of pressure-driven flow through the connected pores. The averaged [Darcy flux](#darcy-velocity) is measured per total cross-sectional area, whereas the pore velocity is that flux divided by porosity. Not every material with voids has connected permeable pores.

## Resident-weighted transit time in a layered flow

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

Without transverse exchange, a particle chosen uniformly from pore volume samples each streamline's transit time with resident-volume weight. This differs from the [flux-weighted residence time in a porous layer](#flux-weighted-residence-time-in-a-porous-layer), which samples at the inlet proportionally to $v$. For constant [porosity](#porosity) and a linear positive [velocity](classical-mechanics.md#velocity) $v=v_0+(v_1-v_0)y/H$, the two means are $L\log(v_1/v_0)/(v_1-v_0)$ and $2L/(v_0+v_1)$, respectively. Their limits agree for uniform [velocity](classical-mechanics.md#velocity).

## Capillary imbibition

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

A wetting liquid penetrates pore space under a pressure difference that includes capillary suction. With a planar front, fixed pressure drop and negligible gravity/inertia, [Darcy's law](#darcy-law) and pore-volume storage give $z\propto t^{1/2}$. The front pressure must be defined relative to the gas phase consistently; adding a positive suction to the inlet pressure is different from prescribing a positive liquid front pressure.

### Hemispherical capillary imbibition

↑ **Parent:** [Capillary imbibition](#capillary-imbibition)

Radial [capillary imbibition](#capillary-imbibition) into a half-space has hemispherical flow area $2\pi r^2$. Its radial hydraulic resistance is proportional to $1/R_s-1/R$, so its inlet [volume flux](fluid-mechanics.md#volumetric-flow-rate) approaches $2\pi k\Delta P R_s/\mu$. The growing front area gives late-time $R\propto t^{1/3}$, unlike the planar $t^{1/2}$ law. Both results assume capillary-dominated geometry with negligible directional gravity effects.

#### Evaporation-limited hemispherical imbibition

↑ **Parent:** [Hemispherical capillary imbibition](#hemispherical-capillary-imbibition)

When a hemispherical wetted front loses liquid at fixed volumetric flux per unit area $F_e$, equilibrium balances inlet flow with $2\pi R^2F_e$. The displayed radius exceeds $R_s$ and is stable because inlet flow decreases while evaporating area increases with radius. [Porosity](#porosity) affects the adjustment time but cancels from the equilibrium radius.

## Two-phase porous-media flow

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

Immiscible fluids share pore space, with each phase's [Darcy flux](#darcy-velocity) determined by its pressure, viscosity and [relative permeability](#relative-permeability). [Fluid saturation](#fluid-saturation) specifies how much pore space each phase occupies. A [capillary pressure](fluid-mechanics.md#capillary-pressure) couples their pressures, while their individual [mass conservation](continuum-mechanics.md#mass-conservation) laws determine displacement and saturation evolution.

### Capillary residual trapping

↑ **Parent:** [Two-phase porous-media flow](#two-phase-porous-media-flow)

When a nonwetting phase recedes from pores, [surface tension](fluid-mechanics.md#surface-tension) and pore geometry can retain a residual saturation $s$. If $h$ is the mobile invaded thickness and $M$ its maximum past value, stored phase volume per plan area is $\phi[(1-s)h+sM]$. Newly invading pores have $M=h$; during recession $M$ remains fixed. With mobile [Darcy velocity](#darcy-velocity) $u$, conservation gives advance speed $u/\phi$ and recession speed $u/[\phi(1-s)]$. The latter is faster for $0<s<1$.

#### Residual-trapping attenuation of a porous current

↑ **Parent:** [Capillary residual trapping](#capillary-residual-trapping)

When a thinning [porous gravity current](#porous-gravity-current) leaves fraction $s$ behind, receding storage changes by only $\phi(1-s)\,dh$ after accounting for immobile fluid. Thus its advective thinning equation is $\phi(1-s)h_t+uh_x=0$. Advancing into previously unwetted pores still requires the full storage $\phi h$, so the nose moves at $u/\phi$. With exponentially decreasing injection the mobile volume per unit well length is $V=Q\tau(e^{-st/\tau}-e^{-t/\tau})/(1-s)$. It obeys $V'=Qe^{-t/\tau}-sV/\tau$; the second term becomes immobile retained volume.

##### Mobile-volume peak of an exponentially forced porous current

↑ **Parent:** [Residual-trapping attenuation of a porous current](#residual-trapping-attenuation-of-a-porous-current)

For residual fraction $0<s<1$, differentiation of $V=Q\tau(e^{-st/\tau}-e^{-t/\tau})/(1-s)$ gives its unique positive maximum at the displayed time. The maximum volume is $Q\tau s^{s/(1-s)}$. When $s=0$ the mobile volume approaches $Q\tau$ monotonically, with no finite maximum. The limiting $s\to1$ expression is $V=Qt e^{-t/\tau}$ with peak at $t=\tau$.

#### Triangular current with capillary retention

↑ **Parent:** [Capillary residual trapping](#capillary-residual-trapping)

For [capillary residual trapping](#capillary-residual-trapping) of an initial triangular current, the [method of characteristics](partial-differential-equation.md#method-of-characteristics) translates its leading and trailing faces at $v_A=u/\phi$ and $v_R=u/[\phi(1-s)]$. Their intersection has height $a[L-(v_R-v_A)t/2]$. Extinction occurs at $t_*=2L/(v_R-v_A)$ and position $x_*=2L/s$. These formulas require $0<s<1$; at zero residual saturation the triangle translates indefinitely.

##### Maximum-invasion envelope of a retained current

↑ **Parent:** [Triangular current with capillary retention](#triangular-current-with-capillary-retention)

For the [triangular current with capillary retention](#triangular-current-with-capillary-retention), the initial trailing face is already the maximum for $0<x<L$. Further upslope, the maximum occurs when the moving crest passes. Hence

$$
M_\infty(x)=\begin{cases}ax,&0<x<L,\\a(2L-sx)/(2-s),&L<x<2L/s,\\0,&\text{otherwise}.\end{cases}
$$

The final trapped phase has saturation $s$ below this envelope. Its volume is $\phi s\int M_\infty\,dx=\phi aL^2$, exactly the initial mobile volume. Maximum invaded thickness is distinct from residual saturation: $s$ multiplies occupied pore volume rather than shrinking the geometrical envelope.

### Waterflooding

↑ **Parent:** [Two-phase porous-media flow](#two-phase-porous-media-flow)

Injecting [water](chemistry.md#water) to displace oil through a porous reservoir. Spatial permeability contrasts cause preferential flow and early water breakthrough, while unswept slower regions retain oil. The recovery also depends on [fractional flow](#fractional-flow), [capillary pressure](fluid-mechanics.md#capillary-pressure) and phase mixing; a passive streamline model alone does not capture all two-phase effects.

### Buckley-Leverett equation

↑ **Parent:** [Two-phase porous-media flow](#two-phase-porous-media-flow)

The one-dimensional [mass conservation](continuum-mechanics.md#mass-conservation) equation for saturation when total [Darcy flux](#darcy-velocity) is constant and capillary pressure and gravity are neglected. It is a [scalar conservation law](partial-differential-equation.md#scalar-conservation-law) with dimensional characteristic speed $(Q/\phi)F'(s)$. Shock speeds obey a [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions); physically admissible solutions satisfy an entropy selection. [Capillary diffusion](#capillary-diffusion) regularizes the saturation transition.

#### Capillary diffusion

↑ **Parent:** [Buckley-Leverett equation](#buckley-leverett-equation)

Eliminating phase pressures with $p_c=p_n-p_w$ gives $\phi s_t+QF(s)_x=(D_cs_x)_x$. For decreasing [capillary pressure](fluid-mechanics.md#capillary-pressure), $D_c\geq0$. This nonlinear diffusion broadens a saturation shock; it can degenerate where a [phase mobility](#phase-mobility) vanishes. Endpoint conservation retains the limiting [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions).

#### Fractional-flow tangent construction

↑ **Parent:** [Buckley-Leverett equation](#buckley-leverett-equation)

When a [rarefaction wave](partial-differential-equation.md#rarefaction-wave) attaches to a saturation shock, its terminal [characteristic speed](partial-differential-equation.md#characteristic-speed) must match the [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions) speed. This gives a tangent from the initial state $(s_0,F(s_0))$ to the fractional-flow curve at $s_s$. It selects the upstream shock saturation; the actual dimensional shock speed still includes total flux divided by [porosity](#porosity).

### Fractional flow

↑ **Parent:** [Two-phase porous-media flow](#two-phase-porous-media-flow)

The fraction of total advective [Darcy flux](#darcy-velocity) carried by one phase when capillary and gravity corrections are omitted. For two phases it is $\lambda_w/(\lambda_w+\lambda_n)$. This quantity lies between zero and one for nonnegative [phase mobilities](#phase-mobility). Its nonlinear dependence on [fluid saturation](#fluid-saturation) determines [characteristic speeds](partial-differential-equation.md#characteristic-speed) and shocks in the [Buckley-Leverett equation](#buckley-leverett-equation).

### Fluid saturation

↑ **Parent:** [Two-phase porous-media flow](#two-phase-porous-media-flow)

The fraction of pore volume occupied by a fluid phase. For a completely fluid-filled two-phase pore space the saturations sum to one. Residual saturation refers to fluid remaining immobile under the modeled displacement; it can impose zero relative mobility at the endpoint.

## Flux-weighted residence time in a porous layer

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

For steady incompressible flow with no stagnant volume, partition the layer into streamtubes of [volume flux](fluid-mechanics.md#volumetric-flow-rate) $dQ$. The pore volume in a streamtube is $\tau\,dQ$, so $\int\tau\,dQ=V_{\rm pore}$. This gives the mean residence time $V_{\rm pore}/Q$ even when individual path times vary widely. [Streamfunction](fluid-mechanics.md#stream-function) labels measure flux in two-dimensional flow, so they supply the correct weighting.

## Vertical imbibition under a draining liquid layer

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

A liquid layer of depth $h$ above a dry deep porous substrate drives a [Darcy flux](#darcy-velocity) $w=(gk/\nu)(1+h/l)$ through its saturated depth $l$, assuming negligible [capillary pressure](fluid-mechanics.md#capillary-pressure) and negligible resistance from the displaced phase. The pressure head contributes $h/l$ and gravity contributes one. [Volume conservation](physics.md#volume-conservation) gives $\phi\dot l=w$. For a finite column, $h+\phi l=h_0$ and initially

$$
l(t)\sim\left(\frac{2gkh_0t}{\phi\nu}\right)^{1/2}.
$$

The singular initial flux is an idealization; the continuum model requires penetration beyond the pore scale.

## Darcy law

↑ **Parent:** [Porous-media flow](porous-media-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Darcy_law)

Darcy's law relates the [Darcy velocity](#darcy-velocity), the fluid flux per unit total cross-sectional area relative to a solid skeleton, to the driving pressure gradient. With no body force, $\mathbf u=-(k/\mu)\nabla p$, where $k$ is [permeability of a porous medium](#permeability-of-a-porous-medium) and $\mu$ is [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity). With gravity, the pressure gradient is replaced by $\nabla p-\rho\mathbf g$.

### Darcy flow

↑ **Parent:** [Darcy law](#darcy-law)

Darcy flow is slow flow through a [porous medium](#porous-medium) whose averaged flux obeys the [Darcy law](#darcy-law). The [Darcy velocity](#darcy-velocity) is the fluid volume flux per total cross-sectional area; it differs from the velocity averaged only over pore space.

#### Lubrication boundary condition for a crack in a Darcy medium

↑ **Parent:** [Darcy flow](#darcy-flow)

In a thin fluid-filled crack, [lubrication theory](viscous-fluid-flow.md#lubrication-theory) gives flux per unit depth $q=-h^3p_x/(12\mu)$. The surrounding [Darcy flow](#darcy-flow) has normal velocity $-kp_y/\mu$. Conservation in the crack gives $q_x=-[u_y]^+_-$, yielding the displayed condition. Pressure is continuous across the crack. This reduced model neglects transverse pressure variation and assumes wall slip lengths are small compared with $h$.

##### Crack pressure in elliptic coordinates

↑ **Parent:** [Lubrication boundary condition for a crack in a Darcy medium](#lubrication-boundary-condition-for-a-crack-in-a-darcy-medium)

For $h=H_0(1-x^2/a^2)^{1/6}$, [elliptic coordinates](geometry-and-topology.md#elliptic-coordinates) make $h^3/\sin\eta$ constant on the upper crack face. Pressure continuity and harmonicity reduce the boundary condition to $F'(0)=\alpha F(0)$ for the cosine mode, while uniform far flow gives $F\sim-e^\xi/2$. Solving $F''=F$ yields the displayed pressure. The midpoint crack flux is $2aU\alpha/(1+\alpha)$; small $\alpha$ leaves the background pressure gradient nearly unchanged, while large $\alpha$ makes the crack nearly equipotential.

###### Elliptic crack pressure dipole

↑ **Parent:** [Crack pressure in elliptic coordinates](#crack-pressure-in-elliptic-coordinates)

Subtracting the uniform-flow pressure $-\mu Ux/k$ leaves $(\mu Ua/k)\alpha e^{-\xi}\cos\eta/(1+\alpha)$. The coordinate map has $r\sim ae^\xi/2$, so $e^{-\xi}\sim a/(2r)$, giving the displayed dipole coefficient. The one-half is essential. In the perfect-conductor limit the independent expression $p=-(\mu U/k)\operatorname{Re}\sqrt{z^2-a^2}$ has the same far-field expansion.

###### Fixed-throughflow dissipation reduction of a conductive crack

↑ **Parent:** [Elliptic crack pressure dipole](#elliptic-crack-pressure-dipole)

For dipole pressure $\delta p\sim Cx/(x^2+y^2)$, choose a rectangular [control volume](fluid-mechanics.md#control-volume) whose transverse size tends to infinity faster than its streamwise size. Each end face contributes $\pi C$ to $\int\delta p\,n_xds$, so fixed-throughflow boundary work gives $\Delta\mathcal D=-2\pi UC$, the displayed result. This control-surface choice removes the integrated far-field velocity correction. A circular cutoff of the pressure-only functional gives $-\pi UC$ instead and does not implement the same throughflow normalization.

### Uniformly heated vertical plate in a porous medium

↑ **Parent:** [Darcy law](#darcy-law)

For constant wall heat-flux density $F>0$, effective [thermal conductivity](thermodynamics.md#thermal-conductivity) $k_e$, buoyancy mobility $B=\rho_0g\alpha K/\mu$ and thermal transport coefficient $\kappa=k_e/(\rho_0c_f)$, a slender [Darcy flow](#darcy-flow) boundary layer has width $\delta=(\kappa k_e z/(BF))^{1/3}$. Writing $\eta=y/\delta$, $\psi=\kappa zf(\eta)/\delta$ and $T-T_a=(F\delta/k_e)f'(\eta)$ gives the displayed equation with $f(0)=0$, $f''(0)=-1$ and $f'(\infty)=0$. The exact integral is $\int_0^\infty(f')^2d\eta=1$. Consequently its kinematic Darcy momentum flux is $\int w^2dy=B\kappa Fz/k_e$ and its buoyancy flux is $g\alpha\kappa Fz/k_e$. These are per span on one heated face.

#### Integral exponential profile for porous wall convection

↑ **Parent:** [Uniformly heated vertical plate in a porous medium](#uniformly-heated-vertical-plate-in-a-porous-medium)

Assume an exponentially decreasing [temperature](thermodynamics.md#temperature) profile while imposing wall heat flux, impermeability and the exact integrated heat budget. For $f=C(1-e^{-\eta/d})$, the wall condition gives $C=d^2$ and $\int(f')^2d\eta=1$ gives $d^3=2$. This yields the displayed integral approximation and discharge $\int wdy\simeq2^{2/3}\kappa z/\delta$. It satisfies the boundary conditions and exact flux budget, but not the differential equation pointwise; its mass-flux coefficient is approximate.

### Fixed-pressure planar Darcy displacement

↑ **Parent:** [Darcy law](#darcy-law)

For two incompressible fluids separated by a planar material front $X(t)$, the [Darcy flux](#darcy-velocity) is uniform and the pressure drop sums the resistances of the two layers: $U=k\Delta P/[\mu X+\mu_h(L-X)]$. The front moves at the [pore velocity](#pore-velocity) $X'=U/\phi$. Integrating from $X(0)=0$ yields the displayed relation. The formula holds up to breakthrough $X=L$, with either sign of the viscosity difference; equal viscosities give constant speed.

#### Thermal-front retardation in Darcy flow

↑ **Parent:** [Fixed-pressure planar Darcy displacement](#fixed-pressure-planar-darcy-displacement)

If a thermal front has speed $Y'=\Gamma U$ with $U$ the [Darcy velocity](#darcy-velocity), while a material front has speed $X'=U/\phi$, their position ratio from coincident initial locations is $Y/X=\Gamma\phi$. Calling a retardation factor the ratio to pore velocity instead would give $Y/X=\Gamma$; these conventions must not be mixed. With cold viscosity $\mu$ and heated viscosity $b\mu$, the displacement's effective viscosity is $\mu_{\rm eff}=\mu[b-(b-1)\Gamma\phi]$. In the pressure resistance the cold layer has length $Y$, the hot injected layer has length $X-Y$, and the displaced layer has length $L-X$.

### Porous thermal plume

↑ **Parent:** [Darcy law](#darcy-law)

A slender planar plume in a saturated porous medium has buoyancy velocity $w=\beta(T-T_0)$, with $\beta=\rho_0g\alpha\Pi/\mu$. The leading heat equation retains both [advection](fluid-mechanics.md#advection) components and lateral [thermal conduction](thermodynamics.md#thermal-conduction): $uT_x+wT_z=\kappa T_{xx}$. Its convective heat input per span is conserved, $F_h=C_h\int w(T-T_0)dx$. Defining $Q=\beta F_h/C_h$ gives width proportional to $z^{2/3}$ and vertical speed/temperature excess proportional to $z^{-1/3}$.

#### Conserved momentum flux of a porous thermal plume

↑ **Parent:** [Porous thermal plume](#porous-thermal-plume)

For a slender [porous thermal plume](#porous-thermal-plume), [Darcy law](#darcy-law) gives $w=\beta(T-T_0)$, with $\beta=Kg\alpha/\nu$. If $C_h=\rho_0c_p$ and $F_h=C_h\int w(T-T_0)dx$ is the conserved excess convective [heat flux](thermodynamics.md#heat-flux-density) per span, then the kinematic [momentum flux](physics.md#momentum-flux) is $M=\int w^2dx=\beta F_h/C_h$, and the [buoyancy flux](turbulent-plume.md#buoyancy-flux) is $B=\int g\alpha(T-T_0)w dx=g\alpha F_h/C_h$. The [hyperbolic-secant porous plume profile](#hyperbolic-secant-porous-plume-profile) has $Q=(36\kappa Mz)^{1/3}$. Multiplication of $Q$ and $M$ by $\rho_0$ gives physical [mass flux](physics.md#mass-flux) and the density-weighted Darcy second moment. Intrinsic pore-velocity momentum flux instead has an additional inverse-porosity factor. Momentum conservation here follows from the heat/velocity proportionality, not from an inertia balance: porous drag balances buoyancy locally.

#### Hyperbolic-secant porous plume profile

↑ **Parent:** [Porous thermal plume](#porous-thermal-plume)

The symmetric steady [porous thermal plume](#porous-thermal-plume) has $w=W\operatorname{sech}^2(x/b)$, $T-T_0=w/\beta$ and $\psi=-Wb\tanh(x/b)$. Its exact normalizations are $Wb^2=6\kappa z$ and $(4/3)W^2b=Q$, so $b=(48\kappa^2z^2/Q)^{1/3}$ and $W=(3Q^2/(32\kappa z))^{1/3}$. The [streamfunction](fluid-mechanics.md#stream-function) supplies lateral entrainment required by continuity.

##### Heat-weighted head speed of a porous plume

↑ **Parent:** [Hyperbolic-secant porous plume profile](#hyperbolic-secant-porous-plume-profile)

Truncating the steady [porous thermal plume](#porous-thermal-plume) profile below a head height and conserving supplied heat gives $\dot Z_h\simeq\int w^2dx/\int wdx=(2/3)W(Z_h)$. Thus $Z_h\propto t^{3/4}$. This is an integral bulk-head estimate, while fastest centreline parcels have characteristic speed $W$; the approximation does not resolve the transient nose.

### Darcy dissipation

↑ **Parent:** [Darcy law](#darcy-law)

A [Darcy velocity](#darcy-velocity) $\mathbf u$ driven by pressure in a stationary porous skeleton dissipates mechanical power $\mu|\mathbf u|^2/\Pi$ per bulk volume. It follows by dotting [Darcy law](#darcy-law) with the discharge: $-\mathbf u\cdot\nabla p=\mu|\mathbf u|^2/\Pi$. Its contribution to a [heat equation](diffusion-equation.md#heat-equation) can be neglected only when it is small relative to the relevant thermal-energy transfer.

### Darcy velocity

↑ **Parent:** [Darcy law](#darcy-law)

The Darcy velocity is liquid [volume flux](fluid-mechanics.md#volumetric-flow-rate) relative to the solid skeleton, divided by total cross-sectional area. If [porosity](#porosity) is $\epsilon$, liquid velocity is $\mathbf v_l$, and skeleton velocity is $\mathbf v_s$, then $\mathbf u=\epsilon(\mathbf v_l-\mathbf v_s)$. Thus pore-fluid speed relative to the skeleton is $\mathbf u/\epsilon$, rather than $\mathbf u$.

#### Pore velocity

↑ **Parent:** [Darcy velocity](#darcy-velocity)

The mean advective fluid speed within the connected pore volume, distinct from [Darcy velocity](#darcy-velocity) defined per bulk cross-sectional area. For uniform [porosity](#porosity) $\phi$ and saturated flow, $v=q/\phi$. Parcel travel times and solute [advection](fluid-mechanics.md#advection) use this velocity, while pressure-flow relations normally use the bulk-area [Darcy flux](#darcy-velocity).

<h3 id="darcy-benard-convection">Darcy-Bénard convection</h3>

↑ **Parent:** [Darcy law](#darcy-law)

Darcy-Bénard convection is [thermal convection](fluid-mechanics.md#thermal-convection) in a porous layer heated from below, with velocity governed by [Darcy's law](#darcy-law). With fixed temperatures and impermeable boundaries, a normalized two-dimensional model uses [streamfunction](fluid-mechanics.md#stream-function) $\psi$ and temperature $\theta$:

$$
\nabla^2\psi=-R\theta_x,\qquad \theta_t+\psi_z\theta_x-\psi_x\theta_z=\nabla^2\theta.
$$

The control parameter is a porous-medium [Rayleigh number](geophysics.md#rayleigh-number). On $0<z<1$ with temperature values $0,-1$, the conductive state is $\psi=0$, $\theta=-z$.

#### Insulated square-column Darcy convection onset

↑ **Parent:** [Darcy-Bénard convection](#darcy-benard-convection)

A tall porous column with square width $a$, insulated impermeable sidewalls and a maintained upward temperature decrease $\Gamma$ admits nearly vertical, zero-net-flux overturning modes. Let $B=\rho_0g\alpha K/\mu$ be buoyancy mobility and $\kappa=k_e/(\rho_0c_f)$ the thermal transport coefficient accompanying [Darcy flux](#darcy-velocity). Neumann transverse modes have $k_\perp^2=\pi^2(m^2+n^2)/a^2$. In the long-column limit the lowest nonconstant modes have growth rate proportional to $B\Gamma-\kappa\pi^2/a^2$. They are warm ascending and cold descending columns with return flow at distant ends. The two lowest modes, varying along either side direction, are degenerate; linear theory alone does not select their nonlinear superposition.

#### Conducting-square Darcy convection

↑ **Parent:** [Darcy-Bénard convection](#darcy-benard-convection)

In a unit square with prescribed conductive boundary [temperatures](thermodynamics.md#temperature) and impermeable boundaries, the [stream function](fluid-mechanics.md#stream-function) convention $\mathbf u=(-\psi_z,0,\psi_x)$ gives linear equations $\Delta\psi=R\theta_x$, $\theta_t=\psi_x+\Delta\theta$, with $\psi=\theta=0$ on all sides. The [velocity](classical-mechanics.md#velocity) equation follows by taking the vertical-plane [curl](calculus.md#curl) of [Darcy law](#darcy-law), and the [temperature](thermodynamics.md#temperature) equation by linearizing the [heat equation](diffusion-equation.md#heat-equation) about $1-z$. Unlike a laterally unbounded Darcy layer, the conducting side boundaries produce a two-dimensional real marginal [eigenspace](linear-operator-theory.md#eigenspace) at $R_c=8\pi^2$.

##### Growth-rate solvability for conducting-square Darcy convection

↑ **Parent:** [Conducting-square Darcy convection](#conducting-square-darcy-convection)

For $q=q_c+\epsilon q_1$, $\theta_t=\epsilon\lambda\theta$, the first-order equations are $\Delta\psi_1-q_c^2\theta_{1x}=2q_cq_1\theta_{0x}$ and $\psi_{1x}+\Delta\theta_1=\lambda\theta_0$. Multiply them by $\psi_0,q_c^2\theta_0$ and integrate. [Integration by parts](calculus.md#integration-by-parts) and the leading equations cancel the homogeneous correction terms, giving $2q_cq_1\langle\psi_0\theta_{0x}\rangle+q_c^2\lambda\langle\theta_0^2\rangle=0$. Since $\langle\psi_0\theta_{0x}\rangle=-\langle|\nabla\theta_0|^2\rangle$, the displayed title formula follows. The reciprocal norm ratio is incompatible with this [solvability condition](linear-operator-theory.md#solvability-condition). Reflection parity diagonalizes the first-order splitting of the two marginal modes.

##### Gauge transformation for conducting-square Darcy onset

↑ **Parent:** [Conducting-square Darcy convection](#conducting-square-darcy-convection)

At zero growth rate put $P=\psi+iq\theta$, $q=\sqrt R$. The coupled Darcy equations become $\Delta P+iqP_x=0$. Substituting $P=e^{-iq(x-1/2)/2}F$ gives $\Delta F+(q^2/4)F=0$ with homogeneous [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition). The square [Dirichlet Laplacian eigenvalues](partial-differential-equation.md#dirichlet-laplacian-eigenvalue) give $q^2=4\pi^2(m^2+n^2)$, $m,n\geq1$, whose minimum is $8\pi^2$. For $S=\sin\pi x\sin\pi z$, $a=q_c/2$, the complex multiples $F=S,iS$ give real pairs $(S\cos(a\xi),-S\sin(a\xi)/q_c)$ and $(S\sin(a\xi),S\cos(a\xi)/q_c)$, $\xi=x-1/2$. Their reflection parities are opposite, yielding two independent physical modes.

#### Darcy thermal-time Rayleigh number

↑ **Parent:** [Darcy-Bénard convection](#darcy-benard-convection)

With permeability $K$, depth $d$, [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) $\nu$ and the relevant effective [thermal diffusivity](thermodynamics.md#thermal-diffusivity) $\kappa_T$, the Darcy [Rayleigh number](geophysics.md#rayleigh-number) compares [buoyancy](fluid-mechanics.md#buoyancy)-driven Darcy [advection](fluid-mechanics.md#advection) to thermal diffusion. It differs from the clear-fluid [Rayleigh number](geophysics.md#rayleigh-number) by replacing $d^3$ with $Kd$. Effective heat capacity and porosity factors may be absorbed into the definition of $\kappa_T$ and the thermal-time scale, and must be kept consistent with the chosen [Darcy law](#darcy-law) convention.

#### Onset of convection in a horizontal Darcy layer

↑ **Parent:** [Darcy-Bénard convection](#darcy-benard-convection)

A perturbation proportional to $\sin(n\pi z)e^{st+ikx}$ has [growth rate](wave-equation.md#growth-rate)

$$
s=\frac{Rk^2}{k^2+n^2\pi^2}-(k^2+n^2\pi^2).
$$

Minimizing the neutral curve $(k^2+n^2\pi^2)^2/k^2$ gives $n=1$, $k=\pi$ and $R_c=4\pi^2$. Thus the first convection rolls have horizontal wavelength twice the layer depth.

##### Supercritical saturation of Darcy convection rolls

↑ **Parent:** [Onset of convection in a horizontal Darcy layer](#onset-of-convection-in-a-horizontal-darcy-layer)

For $R=4\pi^2+\epsilon^2$, fixed roll phase, $T=\epsilon^2t$ and normalization $\psi=\epsilon A(T)\cos(\pi x)\sin(\pi z)+\cdots$, the [Landau amplitude equation](dynamical-systems.md#landau-amplitude-equation) is

$$
A_T=\frac12A-\frac{\pi^2}{8}A^3.
$$

The [mean-temperature correction in weakly nonlinear Darcy convection](#mean-temperature-correction-in-weakly-nonlinear-darcy-convection) supplies the cubic negative feedback. Projection of the third-order equations onto the critical [eigenfunction](linear-operator-theory.md#eigenfunction) via the [Fredholm solvability condition for a self-adjoint operator](linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator) fixes both coefficients. The stable nonzero amplitudes are $\pm2/\pi$ within the chosen phase, giving a supercritical [pitchfork bifurcation](dynamical-systems.md#pitchfork-bifurcation-normal-form) in this real-amplitude reduction.

###### Mean-temperature correction in weakly nonlinear Darcy convection

↑ **Parent:** [Supercritical saturation of Darcy convection rolls](#supercritical-saturation-of-darcy-convection-rolls)

For $\psi_1=\cos(\pi x)\sin(\pi z)$, the first temperature mode is $\theta_1=(2\pi)^{-1}\sin(\pi x)\sin(\pi z)$. The [streamfunction advection bracket](fluid-mechanics.md#streamfunction-advection-bracket) is $J(\psi_1,\theta_1)=(\pi/4)\sin(2\pi z)$, independent of $x$. The second-order equations therefore have $\psi_2=0$ and

$$
\theta_2=-\frac1{16\pi}\sin(2\pi z).
$$

This modifies the vertical temperature gradient. Its interaction with the critical roll produces the cubic term in the [amplitude equation](dynamical-systems.md#amplitude-equation).

<h3 id="saffman-taylor-instability">Saffman–Taylor instability</h3>

↑ **Parent:** [Darcy law](#darcy-law)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Saffman–Taylor_instability)

The Saffman–Taylor instability occurs when a more mobile fluid displaces a less mobile fluid in a porous medium or Hele–Shaw cell. Viscosity contrast amplifies interface corrugations, while [surface tension](fluid-mechanics.md#surface-tension) suppresses sufficiently short wavelengths.

#### Planar viscous-fingering dispersion relation

↑ **Parent:** [Saffman–Taylor instability](#saffman-taylor-instability)

For two fluids with [dynamic viscosities](fluid-mechanics.md#dynamic-viscosity) $\mu_1<\mu_2$, uniform [permeability of a porous medium](#permeability-of-a-porous-medium) $k$, [porosity](#porosity) $\phi$, and imposed [Darcy velocity](#darcy-velocity) $U$, the [Saffman–Taylor instability](#saffman-taylor-instability) of a planar interface has growth rate $\sigma=\alpha U(\mu_2-\mu_1)/[\phi(\mu_2+\mu_1)]$ without capillarity. With constant interfacial tension $\gamma$ and the stabilizing pressure-jump convention, a perturbation of transverse [wavenumber](wave-equation.md#wavenumber) $\alpha>0$ instead has

$$
\sigma=\frac{\alpha}{\phi(\mu_1+\mu_2)}[(\mu_2-\mu_1)U-k\gamma\alpha^2].
$$

The fastest-growing mode satisfies $\alpha_m^2=(\mu_2-\mu_1)U/(3k\gamma)$.

##### Thermal-front viscous-fingering dispersion relation

↑ **Parent:** [Planar viscous-fingering dispersion relation](#planar-viscous-fingering-dispersion-relation)

For a sharp thermal front moving at fraction $\Gamma$ of the [Darcy velocity](#darcy-velocity) $U$, a cold fluid of viscosity $\mu$ displacing its hot counterpart of viscosity $b\mu$ has the displayed growth rate in the local, unbounded planar approximation without [thermal conduction](thermodynamics.md#thermal-conduction). The harmonic pressure perturbations decay on either side. [Pressure continuity](fluid-mechanics.md#pressure-continuity) and continuity of perturbed [Darcy flux](#darcy-velocity) give the velocity response $\delta U=U|a|(b-1)\eta/(b+1)$; the thermal front's kinematic law is $\eta_t=\Gamma\delta U$. The prefactor is the thermal-front speed, not the material [pore velocity](#pore-velocity). Increasing viscosity with heating therefore makes the trailing thermal interface unstable even when the leading displacement of the original fluid is stable.

##### Buoyancy-modified Darcy fingering dispersion relation

↑ **Parent:** [Planar viscous-fingering dispersion relation](#planar-viscous-fingering-dispersion-relation)

Let fluid 1 lie above fluid 2, with [mass densities](fluid-mechanics.md#density) $\rho_1<\rho_2$ and [dynamic viscosities](fluid-mechanics.md#dynamic-viscosity) $\mu_1<\mu_2$. Define $\Delta\rho=\rho_2-\rho_1>0$, $\Delta\mu=\mu_2-\mu_1>0$, [porosity](#porosity) $\phi$, [permeability of a porous medium](#permeability-of-a-porous-medium) $k$, and downward interface speed $W$. With [Darcy flux](#darcy-velocity) $\phi W$, no capillarity, and two unbounded layers, [Darcy's law](#darcy-law) gives

$$
\sigma(\alpha)=\frac{|\alpha|[\phi W\Delta\mu-kg\Delta\rho]}{\phi(\mu_1+\mu_2)}.
$$

For a [Fourier mode](fourier-analysis.md#fourier-mode) of interface displacement, the two perturbation [pressures](thermodynamics.md#pressure) decay exponentially into the respective layers. The [kinematic boundary condition](fluid-mechanics.md#kinematic-boundary-condition) makes their amplitudes proportional to $\phi\mu_1\sigma/(k|\alpha|)$ and $-\phi\mu_2\sigma/(k|\alpha|)$. Linearized [pressure continuity](fluid-mechanics.md#pressure-continuity) adds the base-gradient difference $\phi W\Delta\mu/k-g\Delta\rho$. Eliminating the amplitudes proves the formula. The critical interface speed is $kg\Delta\rho/(\phi\Delta\mu)$; the critical [Darcy velocity](#darcy-velocity) is $kg\Delta\rho/\Delta\mu$. Without [surface tension](fluid-mechanics.md#surface-tension) this model has unbounded short-wave [growth rate](wave-equation.md#growth-rate) on its unstable side.

##### Surface-tension-gradient stabilization of viscous fingering

↑ **Parent:** [Planar viscous-fingering dispersion relation](#planar-viscous-fingering-dispersion-relation)

Suppose the apparent [capillary pressure](fluid-mechanics.md#capillary-pressure) is $p_1-p_2=\gamma(1+\beta x)(\kappa_0+\nabla\cdot\mathbf n)$, with normal towards the displaced fluid and positive apparent tension at the flat front $x=X$. Linearizing the [Darcy law](#darcy-law) interface problem gives the local growth rate

$$
\sigma(\alpha;X)=\frac{\alpha}{\phi(\mu_1+\mu_2)}[(\mu_2-\mu_1)U-k\gamma\kappa_0\beta-k\gamma(1+\beta X)\alpha^2].
$$

The pressure increase experienced by a forward protrusion is stabilizing when $\kappa_0\beta>0$. It suppresses every positive [wavenumber](wave-equation.md#wavenumber) when $U\le k\gamma\kappa_0\beta/(\mu_2-\mu_1)$. For a fixed spatial gradient, $X=Ut/\phi$ makes the rate time dependent; constant exponential growth is a frozen-position approximation.

### Permeability of a porous medium

↑ **Parent:** [Darcy law](#darcy-law)

The permeability of a porous medium measures its ability to transmit fluid. In [Darcy's law](#darcy-law), $k$ has dimensions of area and depends on the geometry and connectivity of the pore space.

#### Relative permeability

↑ **Parent:** [Permeability of a porous medium](#permeability-of-a-porous-medium)

A dimensionless reduction of a porous formation's intrinsic [permeability of a porous medium](#permeability-of-a-porous-medium) for one fluid phase in multiphase flow. Its effective phase permeability is $Kk_{ri}$, and its [phase mobility](#phase-mobility) is $k_{ri}/\mu_i$. It depends on saturation and pore-scale phase configuration; it is not the magnetic use of relative permeability.

##### Phase mobility

↑ **Parent:** [Relative permeability](#relative-permeability)

Relative permeability divided by the phase's [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity). In the phase [Darcy law](#darcy-law), $q_i=-K\lambda_i\nabla p_i$ without body forces. Ratios of mobilities determine [fractional flow](#fractional-flow) when the phases have a common pressure gradient.

#### Effective permeability

↑ **Parent:** [Permeability of a porous medium](#permeability-of-a-porous-medium)

An equivalent large-scale [permeability of a porous medium](#permeability-of-a-porous-medium) relating imposed pressure drop to total [Darcy flux](#darcy-velocity) through a heterogeneous sample. Parallel flow paths add conductances, whereas successive resistive segments add pressure drops. It depends on direction and boundary conditions; it need not be the arithmetic mean of the local permeabilities.

##### Dilute permeability enhancement by aligned cracks

↑ **Parent:** [Effective permeability](#effective-permeability)

At small areal number density $\phi$, identical aligned cracks contribute independently the [fixed-throughflow dissipation reduction of a conductive crack](#fixed-throughflow-dissipation-reduction-of-a-conductive-crack). Equating the mean dissipation density to $\mu U^2/k_{xx}^*$ gives the displayed first-order enhancement. Writing $k/[1-\pi\phi a^2\alpha/(1+\alpha)]$ is an algebraic noninteraction estimate, not a claim of accuracy at higher density. The enhancement saturates as crack conductance becomes large compared with transport through the surrounding porous matrix.

##### Effective permeability of complementary wedges

↑ **Parent:** [Effective permeability](#effective-permeability)

In a slender layer, two parallel sublayers of fractions $x/L$ and $1-x/L$ have local effective permeability $K(x)=k_1x/L+k_2(1-x/L)$. Integrating their successive hydraulic resistance gives the logarithmic mean displayed above. A leading [pressure gradient](fluid-mechanics.md#pressure-gradient) uniform across the thickness does not make parcel paths horizontal; a small transverse velocity preserves [mass conservation](continuum-mechanics.md#mass-conservation) as the cross-sectional conductance changes.

#### Porosity

↑ **Parent:** [Permeability of a porous medium](#permeability-of-a-porous-medium)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Porosity)

Porosity is the fraction of a representative material volume occupied by pore space. In a saturated medium, it is also the liquid volume fraction; it relates [Darcy velocity](#darcy-velocity) to the mean pore-fluid velocity.

### Pressure-dependent Darcy drainage

↑ **Parent:** [Darcy law](#darcy-law)

Suppose a porous layer has thickness $h(p)$ and [permeability of a porous medium](#permeability-of-a-porous-medium) $k(p)$, and the pressure drop $p$ acts across its thickness. [Darcy's law](#darcy-law) gives the drainage [volume flux](fluid-mechanics.md#volumetric-flow-rate)

$$
w=\frac{k(p)}{\mu h(p)}p.
$$

If $k/h=Kp^{-\beta}$, then $w=(K/\mu)p^{1-\beta}$.

## Reactive infiltration instability

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

Reactive infiltration instability is the positive feedback in which reaction or melting increases [permeability of a porous medium](#permeability-of-a-porous-medium), focuses more reacting fluid into that region, and further increases permeability. Finite reaction-zone thickness, transport, and pore geometry can change the short-wave behavior; [Interacting length scales in the reactive-infiltration instability](https://arxiv.org/abs/1306.5034) analyzes transport and reaction length scales in a dissolution model.

### Melting-front instability due to permeability contrast

↑ **Parent:** [Reactive infiltration instability](#reactive-infiltration-instability)

A planar [advection-driven melting front in a porous matrix](geophysics.md#advection-driven-melting-front-in-a-porous-matrix) with permeabilities $k$ ahead and $k+\Delta k$ behind has the ideal sharp-front [growth rate](wave-equation.md#growth-rate)

$$
\sigma=|\alpha|V\frac{\Delta k}{2k+\Delta k}.
$$

This follows by matching [harmonic](partial-differential-equation.md#harmonic-function) pressure perturbations and normal [Darcy flux](#darcy-velocity), then converting flux to front speed by the [enthalpy](thermodynamics.md#enthalpy) balance. It predicts no finite fastest-growing wavelength when $\Delta k>0$.

## Porous gravity current

↑ **Parent:** [Porous-media flow](porous-media-flow.md)

A porous gravity current spreads because a density difference creates a lateral hydrostatic-pressure gradient. For a two-dimensional current of thickness $h$, density deficit $\Delta\rho$, permeability $k$, viscosity $\mu$, and porosity $\phi$,

$$
\phi h_t=\frac{k\Delta\rho g}{\mu}(h h_x)_x.
$$

### Inclined porous gravity current

↑ **Parent:** [Porous gravity current](#porous-gravity-current)

For a thin buoyant layer beneath an inclined impermeable roof, the [hydrostatic approximation](fluid-mechanics.md#hydrostatic-approximation) and [Darcy's law](#darcy-law) give $u=k g\Delta\rho\sin\theta/\mu$ and the [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) $F=uh-u\cot\theta\,hh_x$. The first term transports fluid upslope; the second spreads the layer through its hydrostatic pressure gradient. The [porosity](#porosity) multiplies the stored fluid volume, so the advection speed is $u/\phi$, not the [Darcy velocity](#darcy-velocity) $u$.

#### Volume Jacobian for downslope stretched coordinates

↑ **Parent:** [Inclined porous gravity current](#inclined-porous-gravity-current)

With constant [porosity](#porosity) $P$ and $X=x\tan\theta$, $Y=y\tan\theta$, a translating frame $\xi=X-T$, $\eta=Y$ has area [Jacobian determinant](calculus.md#jacobian-determinant) $dx\,dy=\cot^2\theta\,d\xi\,d\eta$. Actual fluid volume is $P\iint h\,dx\,dy$, proving the displayed normalization. Replacing the cotangent factor by a tangent factor is incompatible with these coordinates except at a slope of $\pi/4$.

#### Depth-dependent inclined porous-current equation

↑ **Parent:** [Inclined porous gravity current](#inclined-porous-gravity-current)

For [porosity](#porosity) $Pz^{\alpha-1}$ and [permeability of a porous medium](#permeability-of-a-porous-medium) $Kz^{\beta-1}$ above an inclined impermeable plane, stored liquid volume per area is $Ph^\alpha/\alpha$. The depth-integrated [Darcy flux](#darcy-velocity) is $\rho gKh^\beta(\sin\theta-\cos\theta\,h_x,-\cos\theta\,h_y)/(\beta\mu)$. [Conservation of mass](continuum-mechanics.md#mass-conservation) yields the displayed equation with $X=x\tan\theta$, $Y=y\tan\theta$ and $T=t\alpha\rho gK\sin\theta\tan\theta/(\beta\mu P)$.

##### Far-downslope width of a constant-flux porous current

↑ **Parent:** [Depth-dependent inclined porous-current equation](#depth-dependent-inclined-porous-current-equation)

In a slender steady [porous gravity current](#porous-gravity-current), the dominant balance is $(h^\beta)_X=(h^\beta h_Y)_Y$. If its width and height scales are $W,H$, fixed downslope [volume flux](fluid-mechanics.md#volumetric-flow-rate) gives $H^\beta W=\text{constant}$, and transverse spreading gives $W^2\sim HX$. Eliminating $H$ yields the displayed width exponent. The porosity exponent affects transient storage but not this steady balance.

#### Advection limit of an inclined porous current

↑ **Parent:** [Inclined porous gravity current](#inclined-porous-gravity-current)

With exponentially decreasing injection, the advective approximation $\phi h_t+uh_x=0$ and inlet condition $uh(0,t)=Qe^{-t/\tau}$ give $h_0=Q/u$ and the displayed solution along [characteristic curves](partial-differential-equation.md#characteristic-curve). It applies behind the advective nose $X=ut/\phi$. The relative size of the discarded nonlinear spreading term for this profile is $2\phi h\cot\theta/(u\tau)$. Smallness of that quantity, and matching through a narrow leading layer, are necessary qualifications: elapsed time alone does not make the approximation uniform at the nose. In a translating frame the full equation remains a [porous medium equation](diffusion-equation.md#porous-medium-equation) with coefficient $u\cot\theta/\phi$.

### One-sided constant-volume porous gravity current

↑ **Parent:** [Porous gravity current](#porous-gravity-current)

A localized release of actual fluid volume $V$ per unit width on a reflecting half-line $x\geq0$ has the [Barenblatt solution](diffusion-equation.md#barenblatt-solution) $h=[L^2-x^2]_+/(6\lambda t)$, where $L^3=9\lambda Vt/\phi$ and $\lambda=k\Delta\rho g/(\phi\mu)$. The [mass conservation](continuum-mechanics.md#mass-conservation) normalization is $\phi\int_0^Lh\,dx=V$. Zero slope at the reflecting boundary gives zero [Darcy flux](#darcy-velocity). For symmetric spreading on the full line, the same formula has $L^3=9\lambda Vt/(2\phi)$ when $V$ denotes the total released volume. A finite initial patch is not determined by volume alone; this exact source profile has a concentrated initial release.

### Slope-driven porous gravity current

↑ **Parent:** [Porous gravity current](#porous-gravity-current)

A buoyant phase beneath a sloping impermeable cap has a slope-driven [Darcy velocity](#darcy-velocity) proportional to density deficit and slope. Far from thickness-adjustment regions, its uniform plateau speed is $K\Delta\rho g\sin\theta/\mu$. With thickness measured normal to the slope, buoyant cap overpressure is $\Delta\rho g h\cos\theta$. A complete depth model also includes the along-current gradient of thickness.

#### Caprock leakage threshold

↑ **Parent:** [Slope-driven porous gravity current](#slope-driven-porous-gravity-current)

A buoyant current beneath an overlying low-permeability cap can enter it when current overpressure exceeds the capillary entry threshold. The plateau criterion compares $\Delta\rho g h\cos\theta$ to that threshold. Cold and warm portions can have different depths and mobilities, giving distinct onset injection rates. These onset criteria do not determine the depleted current after leakage begins.

#### Moving thermal front in a porous current

↑ **Parent:** [Slope-driven porous gravity current](#slope-driven-porous-gravity-current)

A localized temperature adjustment separates regions with different fluid density, viscosity and Darcy speed. [Mass conservation](continuum-mechanics.md#mass-conservation) in the moving frame gives the displayed plateau-depth relation. A speed stated as $V_T=\Gamma u_c$ with $u_c$ a [Darcy velocity](#darcy-velocity) has effective retardation parameter $\phi\Gamma$. Setting both laboratory-frame mass fluxes equal neglects storage associated with passage of the temperature front.

### Porous gravity current with background flow

↑ **Parent:** [Porous gravity current](#porous-gravity-current)

A shallow buoyant [porous gravity current](#porous-gravity-current) in a deep aquifer with uniform imposed [Darcy velocity](#darcy-velocity) $U$ obeys $\phi h_t+(Uh-K_bhh_x)_x=0$ away from sources, where $K_b=k\Delta\rho g/\mu$. Here $k$ is [permeability of a porous medium](#permeability-of-a-porous-medium), $\phi$ is [porosity](#porosity), and $\mu$ is [dynamic viscosity](fluid-mechanics.md#dynamic-viscosity). The pore-fluid drift speed is $u=U/\phi$, and the gravity [diffusion](thermodynamics.md#diffusion) coefficient multiplying $(hh_x)_x$ is $a=K_b/\phi$. The sharp-interface model neglects capillary trapping and dissolution.

#### Advected constant-volume porous gravity current

↑ **Parent:** [Porous gravity current with background flow](#porous-gravity-current-with-background-flow)

An instantaneous point release of actual volume $V$ per unit width in a [porous gravity current with background flow](#porous-gravity-current-with-background-flow) has the [Barenblatt solution](diffusion-equation.md#barenblatt-solution) $h=[R(t)^2-(x-ut)^2]_+/(6at)$, where $R^3=9aVt/(2\phi)$. Its centre translates at pore speed $u=U/\phi$ and its radius grows as $t^{1/3}$. The conserved physical volume is $\phi\int h\,dx=V$.

#### Constant-flux porous gravity current

↑ **Parent:** [Porous gravity current with background flow](#porous-gravity-current-with-background-flow)

Constant actual volume input $Q$ into a [porous gravity current with background flow](#porous-gravity-current-with-background-flow) gives early symmetric scales $h\sim[(Q/\phi)^2t/a]^{1/3}$ and $x\sim[a(Q/\phi)t^2]^{1/3}$. For $U>0$, drift dominates after $t_c=\phi K_bQ/U^3$. The late interior depth is $Q/U$ and the steady upstream edge is $x_-=-K_bQ/U^2$, with upstream linear profile $h=U(x-x_-)/K_b$. Upstream [volume flux](fluid-mechanics.md#volumetric-flow-rate) is zero because background drift balances gravity spreading.

##### Diffusive nose of an advected porous gravity current

↑ **Parent:** [Constant-flux porous gravity current](#constant-flux-porous-gravity-current)

The downstream edge of a continuously fed [porous gravity current with background flow](#porous-gravity-current-with-background-flow) has a transition width proportional to $\sqrt{a h_{\mathrm{int}}t}$ around drift position $ut$. Its [similarity solution](partial-differential-equation.md#similarity-solution) satisfies $(FF\prime)\prime+\eta F\prime/2=0$, $F(-\infty)=1$, and $F(\eta_N)=0$. A finite front has $F\sim(\eta_N/2)(\eta_N-\eta)$. A clipped linear ramp is a useful mass-preserving approximation, but not an exact solution of this nonlinear transition equation.

### Leaky porous gravity current

↑ **Parent:** [Porous gravity current](#porous-gravity-current)

A leaky porous gravity current loses flux through a localized fracture or a distributed permeable boundary. At a point fracture, [mass conservation](continuum-mechanics.md#mass-conservation) makes the horizontal Darcy flux discontinuous by exactly the leakage rate.

#### Hydrostatic leakage through a basal seal

↑ **Parent:** [Leaky porous gravity current](#leaky-porous-gravity-current)

A dense [porous gravity current](#porous-gravity-current) of height $h$ places excess [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) $\Delta\rho gh$ on a basal seal. For seal [permeability of a porous medium](#permeability-of-a-porous-medium) $\lambda$ and thickness $b$, [Darcy law](#darcy-law) gives downward flux $\lambda\Delta\rho gh/(\mu b)$. Dividing the stored height-volume balance by [porosity](#porosity) $\phi$ gives a linear drainage term $-\Omega h$. The coefficient has inverse-time units and does not contain an extra factor of the aquifer permeability.

#### Exponential drainage transform for porous-medium diffusion

↑ **Parent:** [Leaky porous gravity current](#leaky-porous-gravity-current)

The [porous medium equation](diffusion-equation.md#porous-medium-equation) $h_t=\lambda(hh_x)_x-\Gamma h$ with constant $\Gamma>0$ becomes $H_\tau=\lambda(HH_x)_x$ under the displayed transformation. Substitution gives $h_t+\Gamma h=e^{-\Gamma t}\tau'H_\tau$ and $\lambda(hh_x)_x=\lambda e^{-2\Gamma t}(HH_x)_x$, so $\tau'=e^{-\Gamma t}$. This transformation applies to every solution with appropriately transformed initial and boundary conditions, not just a [similarity solution](partial-differential-equation.md#similarity-solution). A [one-sided constant-volume porous gravity current](#one-sided-constant-volume-porous-gravity-current) therefore has remaining physical volume $Ve^{-\Gamma t}$ and a limiting front $[9\lambda V/(\phi\Gamma)]^{1/3}$. The finite transformed time $\tau\to1/\Gamma$ means that arbitrary initial profiles need not reach the universal large-time source shape before drainage removes them.

##### Invasion envelope of an exponentially draining porous current

↑ **Parent:** [Exponential drainage transform for porous-medium diffusion](#exponential-drainage-transform-for-porous-medium-diffusion)

For an impulsive [leaky porous gravity current](#leaky-porous-gravity-current), write $s=(1-e^{-\Omega t})/\Omega$ and $h=(1-\Omega s)[R^2-x^2]_+/(6Ds)$, where $R=C s^{1/3}$. At a fixed lateral location, $h_t=0$ when $x^2=R^2(1+2\Omega s)/3$. The maximum invaded thickness is the envelope $x_*(s)=C s^{1/3}\sqrt{(1+2\Omega s)/3}$, $h_*(s)=C^2(1-\Omega s)^2/(9D s^{1/3})$. The source solution is singular at the initial line release; finite source size and aquifer depth limit its near-source validity.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Mushy layer](geophysics.md#mushy-layer)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-332.md#1/solution)
