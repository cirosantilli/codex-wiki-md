# Reduced gravity

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_gravity)

For two Boussinesq fluids with density difference $\Delta\rho$ and reference density $\rho_0$, reduced gravity is $g'=g\Delta\rho/\rho_0$.

**Table of contents**

- [Entraining shallow-water layer](#entraining-shallow-water-layer)
- [Gravity current](#gravity-current)
  - [Finite-volume inertial gravity current](#finite-volume-inertial-gravity-current)
  - [Finite-Froude lock-release rarefaction](#finite-froude-lock-release-rarefaction)
    - [Reflected information in a finite lock release](#reflected-information-in-a-finite-lock-release)
  - [Front-regularized triangular-channel dam break](#front-regularized-triangular-channel-dam-break)
  - [Entraining shallow-water current in a triangular channel](#entraining-shallow-water-current-in-a-triangular-channel)
    - [Characteristic compatibility for an entraining triangular-channel current](#characteristic-compatibility-for-an-entraining-triangular-channel-current)
  - [Floating extensional viscous gravity current](#floating-extensional-viscous-gravity-current)
    - [Constant-flux floating extensional gravity current](#constant-flux-floating-extensional-gravity-current)
  - [Axisymmetric viscous gravity current](#axisymmetric-viscous-gravity-current)
  - [V-shaped channel gravity current](#v-shaped-channel-gravity-current)
    - [Shallow V-channel lubrication flux](#shallow-v-channel-lubrication-flux)
      - [Porous-medium transformation of V-channel spreading](#porous-medium-transformation-of-v-channel-spreading)
    - [Constant-volume similarity in a V-shaped channel](#constant-volume-similarity-in-a-v-shaped-channel)
  - [Shear-driven viscous gravity current](#shear-driven-viscous-gravity-current)
    - [Line-source upstream reach under imposed shear](#line-source-upstream-reach-under-imposed-shear)
    - [Downstream similarity of a shear-driven gravity current](#downstream-similarity-of-a-shear-driven-gravity-current)
  - [Subglacial current with constant viscous wall layers](#subglacial-current-with-constant-viscous-wall-layers)
    - [Melting-source gravity-current equation](#melting-source-gravity-current-equation)
      - [Meltwater production over an advancing footprint](#meltwater-production-over-an-advancing-footprint)
  - [Constant-speed entraining gravity current on a slope](#constant-speed-entraining-gravity-current-on-a-slope)
  - [Interfacial viscous gravity current](#interfacial-viscous-gravity-current)
    - [Diffusion-controlled solute gravity current](#diffusion-controlled-solute-gravity-current)
    - [Ambient-controlled interfacial plug current](#ambient-controlled-interfacial-plug-current)
      - [Disc-traction analogy for an interfacial current](#disc-traction-analogy-for-an-interfacial-current)
        - [Interfacial plug-current similarity profile](#interfacial-plug-current-similarity-profile)
      - [Viscosity window for an interfacial plug current](#viscosity-window-for-an-interfacial-plug-current)
    - [Isostatic depth partition of an interfacial current](#isostatic-depth-partition-of-an-interfacial-current)
  - [Froude number](#froude-number)
    - [Critical width of a rectangular open-channel contraction](#critical-width-of-a-rectangular-open-channel-contraction)
    - [Hydraulic control](#hydraulic-control)
      - [Weir](#weir)
        - [Broad-crested weir](#broad-crested-weir)
      - [Hydraulic flow in an inverted channel](#hydraulic-flow-in-an-inverted-channel)
        - [Two successive hydraulic controls](#two-successive-hydraulic-controls)
      - [Hydraulic control with prescribed seepage](#hydraulic-control-with-prescribed-seepage)
      - [Head-loss correction to hydraulic control](#head-loss-correction-to-hydraulic-control)
      - [Hydraulic control in a variable-width channel](#hydraulic-control-in-a-variable-width-channel)
    - [Supercritical flow](#supercritical-flow)
    - [Subcritical flow](#subcritical-flow)
    - [Gravity-current front condition](#gravity-current-front-condition)
      - [Benjamin deep-ambient front condition](#benjamin-deep-ambient-front-condition)
      - [Saint-Venant dry-front condition](#saint-venant-dry-front-condition)
  - [Gravity-current box model](#gravity-current-box-model)
    - [Finite-volume triangular-channel current](#finite-volume-triangular-channel-current)
    - [Hindered-settling runout in a rectangular channel](#hindered-settling-runout-in-a-rectangular-channel)
    - [Inertial dam-break current in a triangular valley](#inertial-dam-break-current-in-a-triangular-valley)
    - [Parabolic-channel sediment-current box model](#parabolic-channel-sediment-current-box-model)
    - [Prismatic triangular-channel gravity-current box model](#prismatic-triangular-channel-gravity-current-box-model)
      - [Finite-volume inertial spreading in a triangular channel](#finite-volume-inertial-spreading-in-a-triangular-channel)
      - [Constant-settling runout in a triangular valley](#constant-settling-runout-in-a-triangular-valley)
        - [Deposit profile of a finite triangular-valley particle current](#deposit-profile-of-a-finite-triangular-valley-particle-current)
      - [Hindered-settling runout invariant in a prismatic triangular channel](#hindered-settling-runout-invariant-in-a-prismatic-triangular-channel)
    - [Detrainment-limited gravity-current runout](#detrainment-limited-gravity-current-runout)
    - [Particle-laden gravity current](#particle-laden-gravity-current)
      - [Particle-laden current with suction](#particle-laden-current-with-suction)
      - [Sedimenting rectangular-channel characteristic compatibility](#sedimenting-rectangular-channel-characteristic-compatibility)
      - [Axisymmetric settling box model](#axisymmetric-settling-box-model)
        - [Settling exposure for a particle size distribution](#settling-exposure-for-a-particle-size-distribution)
        - [Monodisperse circular ash runout](#monodisperse-circular-ash-runout)
          - [Circular ash deposit profile](#circular-ash-deposit-profile)
      - [Prismatic triangular-channel shallow water equations](#prismatic-triangular-channel-shallow-water-equations)
        - [Sedimenting triangular-channel characteristic compatibility](#sedimenting-triangular-channel-characteristic-compatibility)
      - [Buoyancy production in a particle-laden current](#buoyancy-production-in-a-particle-laden-current)
      - [Weak-settling attenuation of a sloping gravity current](#weak-settling-attenuation-of-a-sloping-gravity-current)
        - [Formal sedimentation runout of a sloping gravity current](#formal-sedimentation-runout-of-a-sloping-gravity-current)
      - [Steady depositing gravity current](#steady-depositing-gravity-current)
        - [Bidisperse gravity-current deposition](#bidisperse-gravity-current-deposition)
        - [Depth branches of a steady depositing gravity current](#depth-branches-of-a-steady-depositing-gravity-current)
      - [Heated particle-laden gravity current](#heated-particle-laden-gravity-current)
        - [Heated gravity-current runout](#heated-gravity-current-runout)
      - [Triangular-channel shallow water equations](#triangular-channel-shallow-water-equations)
      - [Triangular-channel gravity-current box model](#triangular-channel-gravity-current-box-model)
      - [Runout length of a gravity current](#runout-length-of-a-gravity-current)
  - [Draining gravity current](#draining-gravity-current)
    - [Deep-substrate drainage of a gravity current](#deep-substrate-drainage-of-a-gravity-current)
      - [Cubic-input similarity for a draining gravity current](#cubic-input-similarity-for-a-draining-gravity-current)
    - [Similarity exponents of a draining gravity current](#similarity-exponents-of-a-draining-gravity-current)
  - [Lock-exchange flow](#lock-exchange-flow)

## Entraining shallow-water layer

↑ **Parent:** [Reduced gravity](reduced-gravity.md)

An entraining shallow-water layer changes depth, density, and momentum as ambient fluid crosses its interface. Entrainment dilutes its reduced gravity and accelerates or decelerates it through the momentum needed to bring new fluid into the layer.

## Gravity current

↑ **Parent:** [Reduced gravity](reduced-gravity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravity_current)

A gravity current is a predominantly horizontal flow driven by a density difference. Its front speed scales as the square root of reduced gravity times current depth.

### Finite-volume inertial gravity current

↑ **Parent:** [Gravity current](#gravity-current)

For a one-sided fixed-volume [gravity current](#gravity-current) in a unit-width channel with a closed rear wall, use front closure $\dot L=F\sqrt{g'h_f}$ with $0<F<2$. An exact late-time [similarity solution](partial-differential-equation.md#similarity-solution) has $u=\dot L x/L$, $h=h_f[1-F^2/4+(F^2/4)(x/L)^2]$ and $h_fL=V/(1-F^2/6)$. Substituting into the [shallow water equations](physics.md#shallow-water-equations) proves the radius law. The [Benjamin deep-ambient front condition](#benjamin-deep-ambient-front-condition) has $F=\sqrt2$. The virtual time origin $t_v$ is fixed by matching to the finite release, not by volume alone.

### Finite-Froude lock-release rarefaction

↑ **Parent:** [Gravity current](#gravity-current)

A semi-infinite resting layer of depth $H$ and constant [reduced gravity](reduced-gravity.md) $b$ released into a deep ambient develops a [rarefaction wave](partial-differential-equation.md#rarefaction-wave) satisfying $u+2\sqrt{bh}=2\sqrt{bH}$. The head closure $u_f=F\sqrt{bh_f}$ gives $h_f=4H/(F+2)^2$ and $u_f=2F\sqrt{bH}/(F+2)$. A constant-depth shelf lies between the rarefaction tail speed $u_f-\sqrt{bh_f}$ and the front speed $u_f$; its width is positive for every finite positive $F$.

#### Reflected information in a finite lock release

↑ **Parent:** [Finite-Froude lock-release rarefaction](#finite-froude-lock-release-rarefaction)

A rectangular lock of length $\ell_0$ and depth $h_0$ has rarefaction head speed $-c_0$, where $c_0=\sqrt{g'h_0}$. It reaches a closed rear wall at $t_r=\ell_0/c_0$. The first reflected positive [characteristic curve](partial-differential-equation.md#characteristic-curve) follows $x=\ell_0+2c_0t-3c_0t_r^{2/3}t^{1/3}$ inside the undisturbed rarefaction, then crosses the uniform shelf and reaches the front at the displayed time. This marks the end of the initial constant-speed front stage in the ideal fixed-front-Froude model.

### Front-regularized triangular-channel dam break

↑ **Parent:** [Gravity current](#gravity-current)

In a prismatic triangular channel with constant [reduced gravity](reduced-gravity.md), the wave speed is $c=\sqrt{g'h/2}$ and the [Riemann invariants](compressible-flow.md#riemann-invariant) are $u\pm4c$. A dam release into a deep ambient produces a simple-wave rarefaction with $u+4c=4c_0$. The imposed [gravity-current front condition](#gravity-current-front-condition) $u_f=F\sqrt{g'h_f}$ gives the displayed uniform nose-adjacent state. The fan has $c=(4c_0-x/t)/5$ and $u=4(c_0+x/t)/5$, extending from $x/t=-c_0$ to $u_f-c_f$; a uniform region then reaches the front $x/t=u_f$. The nose closure supplies physics absent from the one-layer interior equations.

### Entraining shallow-water current in a triangular channel

↑ **Parent:** [Gravity current](#gravity-current)

For a prismatic channel of width $b(z)=z$, a [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) current of depth $h$ occupies area $A=h^2/2$. Ambient fluid at rest enters across the interface at speed $w_e$, supplying volume but no horizontal momentum or excess density. The [volume conservation](physics.md#volume-conservation), momentum and excess-density balances are

$$
A_t+(Au)_x=hw_e,\qquad
(Au)_t+(Au^2+g'h^3/6)_x=0,\qquad
(Ag')_t+(Aug')_x=0.
$$

Here $g'$ is the [reduced gravity](reduced-gravity.md). With $D=\partial_t+u\partial_x$, these give $Dh+(h/2)u_x=w_e$, $Du+g'h_x+(h/3)g'_x=-2uw_e/h$, and $Dg'=-2g'w_e/h$. The momentum source in primitive form describes acceleration of newly entrained fluid, even when bed drag vanishes.

#### Characteristic compatibility for an entraining triangular-channel current

↑ **Parent:** [Entraining shallow-water current in a triangular channel](#entraining-shallow-water-current-in-a-triangular-channel)

For positive depth and [reduced gravity](reduced-gravity.md), the [characteristic speeds](partial-differential-equation.md#characteristic-speed) are $u,u\pm c$. Along the material characteristic, $Dg'=-2g'w_e/h$. Along $D_\pm=\partial_t+(u\pm c)\partial_x$, the left-eigenvector compatibility equations are

$$
D_\pm u\pm\frac{2c}{h}D_\pm h\pm\frac{h}{3c}D_\pm g'
=-\frac{2w_e}{h}\left(u\mp\frac c3\right).
$$

If $w_e=0$ and $g'$ is spatially constant, these reduce to the [Riemann invariants](compressible-flow.md#riemann-invariant) $u\pm4c$. Variable buoyancy or entrainment prevents that simplification.

### Floating extensional viscous gravity current

↑ **Parent:** [Gravity current](#gravity-current)

A thin layer of very viscous liquid floating on an effectively inviscid denser liquid has negligible shear traction on both faces. Its leading horizontal [velocity](classical-mechanics.md#velocity) is a plug, and [incompressibility](fluid-mechanics.md#incompressible-flow) gives vertical strain $w_z=-u_x$. Normal-stress balance shifts the [pressure](thermodynamics.md#pressure) by $-2\mu u_x$, so the longitudinal excess stress is $4\mu u_x$. Combining depth-integrated momentum balance with hydrostatic [reduced gravity](reduced-gravity.md) gives the displayed extensional equations. This is distinct from a no-slip, shear-driven thin-film gravity current.

#### Constant-flux floating extensional gravity current

↑ **Parent:** [Floating extensional viscous gravity current](#floating-extensional-viscous-gravity-current)

With fixed inlet thickness $h_0$ and [velocity](classical-mechanics.md#velocity) $u_0$, and nose tension $4\mu h_Nu_x=\rho g'h_N^2/2$, integrating momentum gives $u_x=\rho g'h/(8\mu)$. For a slice injected at $t_0$, write $\tau=t-t_0$ and $T=8\mu/(\rho g'h_0)$. Its thickness, [velocity](classical-mechanics.md#velocity) and position are $h=h_0/(1+\tau/T)$, $u=u_0(1+\tau/T)$, and $x=u_0[\tau+\tau^2/(2T)]$. Eliminating its age gives the steady profile behind the nose, while the nose is the slice with the earliest injection time.

### Axisymmetric viscous gravity current

↑ **Parent:** [Gravity current](#gravity-current)

A shallow radially spreading viscous drop on a horizontal plane has lubrication flux proportional to $-h^3h_r$. Absorbing the positive dimensional coefficient into time gives the displayed equation. For a finite-volume drop, $M=\int_0^Rrh\,dr$ is constant when the origin and front carry zero volume flux. A similarity form $h=t^{-\beta}f(r/t^\alpha)$ has $2\alpha=\beta$ from volume and $\beta+1=4\beta+2\alpha$ from the equation, giving $\alpha=1/8$ and $\beta=1/4$.

### V-shaped channel gravity current

↑ **Parent:** [Gravity current](#gravity-current)

For a fixed half-angle $0<\alpha<\pi/2$, a slow slender [gravity current](#gravity-current) in a V-shaped channel has an almost horizontal [free surface](fluid-mechanics.md#free-surface) across each section. Its area is $h^2\tan\alpha$, and its axial [volume flux](fluid-mechanics.md#volumetric-flow-rate) is $-gQ(\alpha)h^4h_x/\nu$. Here $Q$ is the integral of the dimensionless cross-sectional [Poisson equation](partial-differential-equation.md#poisson-equation) solution: $\Delta\phi=-1$, with zero velocity on the two rigid slopes and zero normal velocity derivative on the horizontal shear-free surface. [Conservation of mass](continuum-mechanics.md#mass-conservation) gives $C=gQ/(\nu\tan\alpha)$. This treats the full two-dimensional section and does not require a shallow V angle.

#### Shallow V-channel lubrication flux

↑ **Parent:** [V-shaped channel gravity current](#v-shaped-channel-gravity-current)

For a shallow V-channel with floor $z=\alpha|y|$, $0<\alpha\ll1$, let the [free surface](fluid-mechanics.md#free-surface) be $z=h(x,t)$. [Hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) gives $p_x=\rho g h_x$. A vertical strip has thickness $H_y=h-\alpha|y|$ and, with no slip below and zero shear above, flux $-\rho gH_y^3h_x/(3\mu)$. Integrating across $|y|<h/\alpha$ gives

$$
Q=-\frac{\rho g}{6\mu\alpha}h^4h_x,\qquad A=\frac{h^2}{\alpha}.
$$

Conservation of volume is $(h^2)_t=C(h^4h_x)_x$, $C=\rho g/(6\mu)$. Here $\alpha$ is the wall slope to the horizontal, not the opening half-angle measured from the vertical in a general V-section. Vertical shear dominates transverse shear by the shallow-slope approximation.

##### Porous-medium transformation of V-channel spreading

↑ **Parent:** [Shallow V-channel lubrication flux](#shallow-v-channel-lubrication-flux)

The variable $w=h^2$ converts the [shallow V-channel lubrication flux](#shallow-v-channel-lubrication-flux) equation into a [porous medium equation](diffusion-equation.md#porous-medium-equation):

$$
w_t=\frac C5(w^{5/2})_{xx},\qquad C=\frac{\rho g}{6\mu},\qquad\int_{\mathbb R}w\,dx=\alpha V.
$$

Indeed $h^4h_x=w^{3/2}w_x/2=(w^{5/2})_x/5$. Its fixed-mass source-type solution gives $h\propto t^{-1/7}$ and [support](function.md#support) length proportional to $t^{2/7}$. Integrating the similarity equation once gives $Ch^4h_x=-2xh^2/(7t)$, and hence $h=[3(X(t)^2-x^2)/(7Ct)]_+^{1/3}$. The [constant-volume similarity in a V-shaped channel](#constant-volume-similarity-in-a-v-shaped-channel) fixes $X$ from the positive [integral](calculus.md#integral) $J=\int_{-1}^1(1-s^2)^{2/3}ds$: $X=(\alpha V/J)^{3/7}(7Ct/3)^{2/7}$.

#### Constant-volume similarity in a V-shaped channel

↑ **Parent:** [V-shaped channel gravity current](#v-shaped-channel-gravity-current)

The symmetric [similarity solution](partial-differential-equation.md#similarity-solution) for a localized fixed volume $V$ in a [V-shaped channel gravity current](#v-shaped-channel-gravity-current) has $h(x,t)=[3(X^2-x^2)/(7Ct)]_+^{1/3}$. Integrating the similarity [conservation of mass](continuum-mechanics.md#mass-conservation) equation once gives $Ch^4h_x=-2xh^2/(7t)$, and vanishing thickness at the two noses gives the profile. Its volume fixes $X=[V/(I\tan\alpha)]^{3/7}(7Ct/3)^{2/7}$, where $I=\int_{-1}^1(1-s^2)^{2/3}\,ds$. At any fixed nonzero position, the thickness first rises after arrival and then falls; its maximum occurs when $X^2=7x^2/3$.

### Shear-driven viscous gravity current

↑ **Parent:** [Gravity current](#gravity-current)

A thin dense [gravity current](#gravity-current) on a rigid no-slip substrate can be carried downstream by imposed upper [shear stress](viscous-fluid-flow.md#shear-stress) $\tau$. For density contrast $\Delta\rho$, [lubrication theory](viscous-fluid-flow.md#lubrication-theory) gives $\mathbf q=Ah^2\mathbf e_x-Dh^3\nabla h$, where $A=\tau/(2\mu)$ and $D=\Delta\rho g/(3\mu)$. The [continuity equation](physics.md#continuity-equation) gives the displayed equation. Besides small slopes and reduced inertia, the hydrostatic reduction requires $\tau/(\Delta\rho gL)\ll1$ to keep shear-related normal stress small. Finite zero-thickness fronts are formal outer profiles and need a separate local description when their slopes are large.

#### Line-source upstream reach under imposed shear

↑ **Parent:** [Shear-driven viscous gravity current](#shear-driven-viscous-gravity-current)

For a steady line-source [shear-driven viscous gravity current](#shear-driven-viscous-gravity-current) with downstream constant thickness, $h_d^2=2\mu Q_{2d}/\tau$. Zero upstream [volume flux per unit width](fluid-mechanics.md#volume-flux-per-unit-width) gives $h h_x=3\tau/(2\Delta\rho g)$, so $h^2=h_d^2+3\tau x/(\Delta\rho g)$ until it vanishes at $x=-x_N$. Unlike the point-source scaling estimate, this reduced line-source model fixes the exact coefficient $2/3$. The square-root nose has an unresolved steep edge.

#### Downstream similarity of a shear-driven gravity current

↑ **Parent:** [Shear-driven viscous gravity current](#shear-driven-viscous-gravity-current)

For a steady point-source [shear-driven viscous gravity current](#shear-driven-viscous-gravity-current) far downstream, $h\ll y_N\ll x$ permits dropping the downstream gravity flux. With $w=h^2$, the equation is $w_x=D(w^2)_{yy}/(4A)$, a quadratic [porous medium equation](diffusion-equation.md#porous-medium-equation). Conserving $A\int w\,dy=Q$ yields $y_N=(3\mu\Delta\rho gQx/\tau^2)^{1/3}$ and $h^2=\tau(y_N^2-y^2)/(2\Delta\rho gx)$ inside the current. The central height decays as $x^{-1/6}$. Near the source, balancing shear and gravity gives an upstream reach of order $\sqrt{\mu\Delta\rho gQ}/\tau$, whose numerical coefficient is not determined by scaling.

### Subglacial current with constant viscous wall layers

↑ **Parent:** [Gravity current](#gravity-current)

In a water layer confined between horizontal rock and a movable constant-pressure ice roof, [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) and two wall stresses $\mu u/\delta_v$ give $u=-Dh h_x$, $q=-Dh^2h_x$ and $h_t=D(h^2h_x)_x$, with $D=\rho_wg\delta_v/(2\mu)>0$. This closure uses a constant [viscous boundary layer](viscous-fluid-flow.md#viscous-boundary-layer) thickness, not a generic quadratic turbulent drag law.

#### Melting-source gravity-current equation

↑ **Parent:** [Subglacial current with constant viscous wall layers](#subglacial-current-with-constant-viscous-wall-layers)

A shallow current receiving meltwater over its wetted area obeys $h_t+q_x=s_m$, with $q=-Dh^2h_x$. The source is zero ahead of the advancing front. The [Stefan condition](geophysics.md#stefan-condition) determines normal ice-retreat speed $v_m$; the water-volume source is $s_m=(\rho_i/\rho_w)v_m$, or simply $v_m$ in the equal-density approximation. Water volume and geometric excavation must be distinguished if densities differ.

##### Meltwater production over an advancing footprint

↑ **Parent:** [Melting-source gravity-current equation](#melting-source-gravity-current-equation)

For constant water-production rate per wetted area $s_m$, dry zero-flux noses and footprint length $\mathcal L(t)$, the moving-boundary [conservation of mass](continuum-mechanics.md#mass-conservation) gives $\dot{\mathcal V}=s_m\mathcal L$ per out-of-plane span. Consequently $\ddot{\mathcal V}=s_m\dot{\mathcal L}$. Equivalently the melt volume is $s_m\int_0^t\mathcal L(t\prime)dt\prime$; a point begins producing melt only after the front arrives.

### Constant-speed entraining gravity current on a slope

↑ **Parent:** [Gravity current](#gravity-current)

For steady flow with [entrainment coefficient](turbulent-plume.md#entrainment-coefficient) $E$, bottom-drag coefficient $c$ and slope angle $\theta$, a constant [buoyancy flux](turbulent-plume.md#buoyancy-flux) $B$ gives $h=h_0+Ex$, $g^{\prime}=B/(uh)$ and $u^3=B(\sin\theta-E\cos\theta/2)/(c+E)$. The half factor comes from hydrostatic pressure, while the denominator includes both bed drag and acceleration of entrained fluid.

### Interfacial viscous gravity current

↑ **Parent:** [Gravity current](#gravity-current)

A viscous current with density between those of two ambient fluids spreads along their interface. Vertical buoyancy divides its thickness above and below the undisturbed interface. When its internal shear and in-plane extension are both negligible, resistance from the two ambient [Stokes flows](stokes-flow.md) controls its spreading.

#### Diffusion-controlled solute gravity current

↑ **Parent:** [Interfacial viscous gravity current](#interfacial-viscous-gravity-current)

When vertical [diffusion equation](diffusion-equation.md) controls depth, $H\sim\sqrt{Dt}$, while conserved excess solute mass gives $\Delta\rho R^2H\sim\Delta\rho_0V_0$. Ambient viscous resistance then leads to a $t^{1/2}$ spreading law. The enriched-fluid volume grows, so the fixed-volume $t^{1/5}$ law does not apply.

#### Ambient-controlled interfacial plug current

↑ **Parent:** [Interfacial viscous gravity current](#interfacial-viscous-gravity-current)

The gravity force per interfacial area is $\Delta\rho gH^2/R$, while ambient viscous [traction](continuum-mechanics.md#traction) is $\mu u/R$. Their balance gives the radial velocity scale independently of current [viscosity](fluid-mechanics.md#dynamic-viscosity) within the appropriate plug-flow window.

##### Disc-traction analogy for an interfacial current

↑ **Parent:** [Ambient-controlled interfacial plug current](#ambient-controlled-interfacial-plug-current)

[Linearity of Stokes flow](stokes-flow.md#linearity-of-stokes-flow) and [Uniqueness of Stokes flow](stokes-flow.md#uniqueness-of-stokes-flow) identify the ambient resistance to an expanding thin plug with the reversed perturbation around a stationary disc in an axisymmetric straining flow. The imposed straining flow has zero tangential stress on the disc plane. Each face then resists radial velocity $Er$ with [traction](continuum-mechanics.md#traction) $-8\mu Er/[\pi\sqrt{R^2-r^2}]$.

###### Interfacial plug-current similarity profile

↑ **Parent:** [Disc-traction analogy for an interfacial current](#disc-traction-analogy-for-an-interfacial-current)

For fixed volume and equal ambient viscosities, radial volume conservation gives $u=r/(5t)$. Summing both ambient-face tractions gives $H^2=32\mu R/(5\pi\Delta\rho gt)$ and $R^5=125\Delta\rho gV^2t/(512\pi\mu)$. The edge slope is singular, so the profile is a leading bulk thin-current approximation.

##### Viscosity window for an interfacial plug current

↑ **Parent:** [Ambient-controlled interfacial plug current](#ambient-controlled-interfacial-plug-current)

The lower bound makes internal vertical velocity variation negligible; the upper bound makes internal in-plane extensional stress negligible compared with ambient [traction](continuum-mechanics.md#traction). Both are needed for an [ambient-controlled interfacial plug current](#ambient-controlled-interfacial-plug-current).

#### Isostatic depth partition of an interfacial current

↑ **Parent:** [Interfacial viscous gravity current](#interfacial-viscous-gravity-current)

[Hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) continuity across both interfaces fixes the partition of current thickness. The modified current pressure is $\Delta\rho gh$, with $\Delta\rho=(\rho_0-\rho_1)(\rho_2-\rho_0)/(\rho_2-\rho_1)$. The equivalent radial [body force](fluid-mechanics.md#body-force) is $-\Delta\rho g h_r\mathbf e_r$.

### Froude number

↑ **Parent:** [Gravity current](#gravity-current)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Froude_number)

The Froude number compares inertial speed with a gravity-wave speed. For a shallow [gravity current](#gravity-current) of depth $h$ and [reduced gravity](reduced-gravity.md) $g'$, $\operatorname{Fr}=U/\sqrt{g'h}$.

#### Critical width of a rectangular open-channel contraction

↑ **Parent:** [Froude number](#froude-number)

For a steady slowly varying rectangular channel, [mass conservation](continuum-mechanics.md#mass-conservation) and the [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) give $(W/w)^2=((F+2)/F)s^2-(2/F)s^3$, where $s=h/H$. The positive cubic has its maximum at $s=(F+2)/3$, with value $(F+2)^3/(27F)$. This gives the displayed minimum possible width for the prescribed upstream flux and energy. Smooth subcritical and supercritical branches connected to upstream data remain distinct unless the critical width is attained.

#### Hydraulic control

↑ **Parent:** [Froude number](#froude-number)

A [hydraulic control](#hydraulic-control) is a critical section where a [shallow water](physics.md#shallow-water-approximation) flow passes smoothly between [subcritical flow](#subcritical-flow) and [supercritical flow](#supercritical-flow). One long-wave [characteristic speed](partial-differential-equation.md#characteristic-speed) relative to the bed vanishes there. Regularity supplies an extra relation between discharge, depth and channel geometry, allowing the control to set the discharge or upstream state. A critical depth alone is not sufficient for a regular transcritical solution: the channel forcing must also be compatible there.

##### Weir

↑ **Parent:** [Hydraulic control](#hydraulic-control)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weir)

A weir is an obstruction across a channel that can regulate [volume flux](fluid-mechanics.md#volumetric-flow-rate) by creating a hydraulic control. In a [shallow water](physics.md#shallow-water-approximation) model a sufficiently smooth crest has a critical section, with upstream flow subcritical and downstream flow supercritical under free discharge. Losses, submergence and geometry determine whether this ideal control applies.

###### Broad-crested weir

↑ **Parent:** [Weir](#weir)

For reservoir head $\delta$ above a broad crest, negligible approach [velocity](classical-mechanics.md#velocity), constant [reduced gravity](reduced-gravity.md), and no head loss, [hydraulic control](#hydraulic-control) gives $\delta=3h_c/2$ and the displayed discharge. Reflecting the vertical coordinate gives the same result for a light layer escaping beneath a lowered roof. An orifice discharge coefficient is a separate closure and should not be silently inserted into this inviscid weir law.

##### Hydraulic flow in an inverted channel

↑ **Parent:** [Hydraulic control](#hydraulic-control)

A light shallow layer flows below a roof of height $H(x)$ and width $W(x)$ through a deeper approximately motionless ambient. [Hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) and inviscid steady [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) give the displayed specific [energy](classical-mechanics.md#energy) for constant [volume flux](fluid-mechanics.md#volumetric-flow-rate) $Q$ and [reduced gravity](reduced-gravity.md) $g'$. At fixed position, $E_h=g'(1-\mathrm{Fr}^2)$ and $h_c=[Q^2/(g'W^2)]^{1/3}$. A roof depression raises the minimum admissible energy, just as a bed elevation does for a heavy lower layer.

###### Two successive hydraulic controls

↑ **Parent:** [Hydraulic flow in an inverted channel](#hydraulic-flow-in-an-inverted-channel)

For two same-height throats carrying the same light-layer [volume flux](fluid-mechanics.md#volumetric-flow-rate) and [reduced gravity](reduced-gravity.md), the narrower throat has the larger critical minimum [energy](classical-mechanics.md#energy). A narrower downstream throat can back up and submerge an upstream throat. If the first throat is narrower, it can control discharge and feed a supercritical current through the second; a [hydraulic jump](physics.md#hydraulic-jump) followed by a second control is also possible when the available energy drop and intermediate geometry permit it. Equal throat widths are a marginal lossless case. Relative width alone does not fix jump position or mixing in the intervening reservoir.

##### Hydraulic control with prescribed seepage

↑ **Parent:** [Hydraulic control](#hydraulic-control)

For loss of fluid carrying its local axial velocity, the inviscid [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) head stays constant while discharge decreases. On a flat bed a regular control requires a positive local maximum of $q=Q/b$. In the parabolic-width channel $b=b_0(1+x^2/L^2)$, this maximum occurs at $x_c=-SL^2/(Q_0+\sqrt{Q_0^2+S^2L^2})$, with $q_c=(Q_0+\sqrt{Q_0^2+S^2L^2})/(2b_0)$. Its critical depth is $(q_c^2/g)^{1/3}$. A control exists only when the prescribed total head equals the maximum critical-head envelope and the reach includes that point while retaining positive discharge.

##### Head-loss correction to hydraulic control

↑ **Parent:** [Hydraulic control](#hydraulic-control)

For a prescribed positive head-loss rate $\gamma(x)$, the steady energy balance is $(E+H)_x=-\gamma$. The accumulated loss is added to the bed elevation when applying [hydraulic control](#hydraulic-control) compatibility: $H_x+\gamma=h_cb_x/b$. A local loss law alone does not determine the accumulated loss between a remote inlet and the control; that integral must also be specified.

##### Hydraulic control in a variable-width channel

↑ **Parent:** [Hydraulic control](#hydraulic-control)

For a smooth rectangular channel, conservation of discharge and [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) head gives $(1-F^2)h_x=F^2h b_x/b-H_x$. A regular [hydraulic control](#hydraulic-control) has $F=1$ and the displayed geometric compatibility condition. At fixed discharge the critical-head envelope is $T(x)=H(x)+3h_c(x)/2$, with $h_c=(Q^2/(gb^2))^{1/3}$. A simple smooth control requires a local maximum of $T$: $T_x=0$ and $T_{xx}<0$. A local minimum cannot be crossed at the critical head because the real depth branches disappear nearby.

#### Supercritical flow

↑ **Parent:** [Froude number](#froude-number)

A shallow [gravity current](#gravity-current) is supercritical when its [Froude number](#froude-number) exceeds one: both gravity-wave [characteristic curves](partial-differential-equation.md#characteristic-curve) move downstream relative to the bed.

#### Subcritical flow

↑ **Parent:** [Froude number](#froude-number)

A shallow [gravity current](#gravity-current) is subcritical when its [Froude number](#froude-number) is less than one: a gravity disturbance can propagate upstream relative to the bed. This definition uses the characteristic speed $\sqrt{g'h}$ appropriate to the stated model.

#### Gravity-current front condition

↑ **Parent:** [Froude number](#froude-number)

A common high-[Reynolds number](fluid-mechanics.md#reynolds-number) closure for a deep-ambient [gravity current](#gravity-current) is $\dot L=\operatorname{Fr}\sqrt{g'h}$, where $L$ is front position and the order-one [Froude number](#froude-number) depends on the chosen front model.

##### Benjamin deep-ambient front condition

↑ **Parent:** [Gravity-current front condition](#gravity-current-front-condition)

In an ideal [Boussinesq](geophysical-fluid-dynamics.md#boussinesq-approximation) [gravity current](#gravity-current) advancing beneath a much deeper ambient, the local head [Froude number](#froude-number) is $u_f/\sqrt{g'h_f}=\sqrt2$. The ambient must be displaced around the finite-depth head. This differs from the [Saint-Venant dry-front condition](#saint-venant-dry-front-condition), which neglects ambient inertia. The coefficient belongs to the ideal deep-ambient head model; confinement, mixing and drag can change it.

##### Saint-Venant dry-front condition

↑ **Parent:** [Gravity-current front condition](#gravity-current-front-condition)

The [shallow water equations](physics.md#shallow-water-equations) at a dry bed, with negligible ambient [mass density](fluid-mechanics.md#density), end in a vanishing-depth edge, rather than a finite-depth [gravity current](#gravity-current) head. In a prismatic triangular channel the [Riemann invariant](compressible-flow.md#riemann-invariant) $u+4\sqrt{g'h/2}$ gives the speed $2\sqrt{2g'h_0}$ after release of a resting semi-infinite layer of depth $h_0$. In a rectangular channel the corresponding speed is $2\sqrt{g'h_0}$; the channel geometry matters.

### Gravity-current box model

↑ **Parent:** [Gravity current](#gravity-current)

A gravity-current box model replaces the current by a well-mixed region with uniform depth and density. Integral volume, scalar, and front-speed balances then reduce the spreading problem to [ordinary differential equations](differential-equation.md#ordinary-differential-equation).

#### Finite-volume triangular-channel current

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

A [gravity-current box model](#gravity-current-box-model) in a prismatic channel with width equal to height has volume $V_0=Lh^2/2$. Closing the front speed by $\dot L=F\sqrt{g'h}$ gives the displayed law and long-time spreading $L\propto t^{4/5}$. This is an integral approximation with constant volume and [reduced gravity](reduced-gravity.md), not an exact uniform-depth solution of the local [shallow water equations](physics.md#shallow-water-equations).

#### Hindered-settling runout in a rectangular channel

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

For a constant-volume unit-width [particle-laden gravity current](#particle-laden-gravity-current) with $M=Lh$, define the particle-fluid reference [reduced gravity](reduced-gravity.md) $g_0'=g(\rho_p-\rho_0)/\rho_0$, so the current has $g'=g_0'\phi$. A constant front [Froude number](#froude-number) and absorbing-bed [hindered settling](fluid-mechanics.md#hindered-settling) give $\dot L=F\sqrt{g_0'\phi M/L}$ and $\dot\phi=-(V_sL/M)\phi(1-\phi)$. Eliminating time and integrating gives the displayed [runout length of a gravity current](#runout-length-of-a-gravity-current). For large runout and dilute initial concentration, $L_\infty^5\sim25F^2M^3g_0'(\phi_0+2\phi_0^2/3+\cdots)/V_s^2$. This $g_0'$ is buoyancy per unit particle fraction, not the initial current reduced gravity $g_0'\phi_0$.

#### Inertial dam-break current in a triangular valley

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

In a horizontal prismatic V-shaped valley with section area $A=\lambda h^2$, a fixed-volume high-Reynolds-number [gravity-current box model](#gravity-current-box-model) has $h=(W/(\lambda X))^{1/2}$ and front speed $\dot X=\operatorname{Fr}\sqrt{gh}$. Integrating gives $X=[5\operatorname{Fr}\sqrt g(W/\lambda)^{1/4}t/4]^{4/5}$ after the initial release scale is neglected. This is an inertial closure, distinct from the viscous [V-shaped channel gravity current](#v-shaped-channel-gravity-current), whose exponent is different.

#### Parabolic-channel sediment-current box model

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

A well-mixed [particle-laden gravity current](#particle-laden-gravity-current) in a prismatic channel with $b(z)=C\sqrt z$ has volume $V=2Ch^{3/2}L/3$. Negligible entrainment gives fixed $V$. Vertical [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) is $W_s\phi b(h)L$, so $\dot\phi=-3W_s\phi/(2h)$. Close the front by $\dot L=F\sqrt{G\phi h}$, where $G=g(\rho_p-\rho_0)/\rho_0$. Eliminating time gives

$$
\sqrt\phi+\frac{3W_sL^2}{8F\sqrt G\,h_0^{3/2}L_0}
=\sqrt{\phi_0}+\frac{3W_sL_0^2}{8F\sqrt G\,h_0^{3/2}L_0}.
$$

The concentration tends to zero at a finite limiting [runout length of a gravity current](#runout-length-of-a-gravity-current), although reaching that limit takes infinite time in this model.

#### Prismatic triangular-channel gravity-current box model

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

A uniform-depth [particle-laden gravity current](#particle-laden-gravity-current) in fixed triangular cross section has conserved [volume](geometry-and-topology.md#volume) proportional to $h^2X$. A [gravity-current front condition](#gravity-current-front-condition) and absorbing-boundary [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) give $\dot X=\operatorname{Fr}\sqrt{G\phi h}$ and $\dot\phi=-2w(\phi)\phi/h$. The box describes late-time bulk evolution; it does not resolve the nose or immediate dam-break flow.

##### Finite-volume inertial spreading in a triangular channel

↑ **Parent:** [Prismatic triangular-channel gravity-current box model](#prismatic-triangular-channel-gravity-current-box-model)

With constant buoyancy and no settling or entrainment, the box volume is proportional to $h^2\ell$. Thus $h=h_0\sqrt{x_0/\ell}$ for an initial lock length $x_0$. A [gravity-current front condition](#gravity-current-front-condition) gives $\dot\ell=F\sqrt{g'h_0}(x_0/\ell)^{1/4}$, so $\ell^{5/4}$ increases linearly with time. This is a late-time integral approximation; it does not reproduce the initial rarefaction or the detailed nose.

##### Constant-settling runout in a triangular valley

↑ **Parent:** [Prismatic triangular-channel gravity-current box model](#prismatic-triangular-channel-gravity-current-box-model)

For a dilute well-mixed particle current of conserved bulk volume $W$, triangular section $\lambda h^2$, constant particle settling speed $w_s$ and initial reduced gravity $g'_0$, put $s=\sqrt{\phi/\phi_0}$. The balances give $\dot X=B sX^{-1/4}$ and $\dot\phi=-2w_s\phi/h$, where $B=\operatorname{Fr}\sqrt{g'_0}(W/\lambda)^{1/4}$. Eliminating time gives $s=1-(X/R)^{7/4}$ and the displayed limiting runout. It is approached at infinite time. Early spreading has the inertial $t^{4/5}$ exponent, while settling limits the eventual reach.

###### Deposit profile of a finite triangular-valley particle current

↑ **Parent:** [Constant-settling runout in a triangular valley](#constant-settling-runout-in-a-triangular-valley)

Under the same box-model assumptions, $M_0=\rho_p\phi_0W$ is initial particle mass and $m_d$ is final deposited mass per downstream length. Integrate the vertical [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) across the instantaneous triangular-valley width $2\lambda h$ from arrival of the front at $x$ until settling is complete. This gives the displayed profile on $0\leq x\leq R$ and zero beyond the runout. Its integral is $M_0$, verifying particle mass conservation. Areal deposit density also depends on the lateral coordinate because the wetted valley width changes as the current thins.

// Target: geophysics.bigb

##### Hindered-settling runout invariant in a prismatic triangular channel

↑ **Parent:** [Prismatic triangular-channel gravity-current box model](#prismatic-triangular-channel-gravity-current-box-model)

In the [prismatic triangular-channel gravity-current box model](#prismatic-triangular-channel-gravity-current-box-model), take $h=h_0\sqrt{L/X}$ and $w(\phi)=w_0(1-\phi)$. Eliminating time gives $d\phi/[\sqrt\phi(1-\phi)]=-2w_0X^{3/4}dX/(\operatorname{Fr}\sqrt G h_0^{3/2}L^{3/4})$. Integration yields the displayed invariant with $K=4w_0/(7\operatorname{Fr}\sqrt G h_0^{3/2}L^{3/4})$. The positive-concentration branch approaches a finite [runout length of a gravity current](#runout-length-of-a-gravity-current) as time tends to infinity.

#### Detrainment-limited gravity-current runout

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

If a finite-volume [gravity current](#gravity-current) loses or dilutes the scalar that supplies its [reduced gravity](reduced-gravity.md), its front can approach a finite [runout length of a gravity current](#runout-length-of-a-gravity-current). A box model couples the scalar balance to a [gravity-current front condition](#gravity-current-front-condition); eliminating time then gives the front position directly as a function of the remaining scalar concentration.

#### Particle-laden gravity current

↑ **Parent:** [Gravity-current box model](#gravity-current-box-model)

A particle-laden gravity current is driven by the excess density of suspended particles. Deposition decreases its [reduced gravity](reduced-gravity.md), so a finite-volume current can approach a finite runout length.

##### Particle-laden current with suction

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

A steady well-mixed dilute [particle-laden gravity current](#particle-laden-gravity-current) above an absorbing porous bed loses carrier fluid at speed $W$ and particles at total downward speed $W+V$, where $V$ is their relative [settling velocity](fluid-mechanics.md#settling-velocity) magnitude. [Volume conservation](physics.md#volume-conservation) and the particle budget give $Q=Q_0-Wx$ and $\phi=(Q/Q_0)^{V/W}$ for $W>0$. The [momentum conservation](classical-mechanics.md#momentum-conservation) equation is $(Q^2/h+g'_0\phi h^2/2)'=-Wu$ if the withdrawn fluid carries its local horizontal [velocity](classical-mechanics.md#velocity). Consequently $uu'+g'_0\phi h'+g'_0h\phi'/2=0$. At $W=0$, $\phi=e^{-Vx/Q_0}$ and the momentum flux is constant.

##### Sedimenting rectangular-channel characteristic compatibility

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

With [reduced gravity](reduced-gravity.md) $b$ and [settling velocity](fluid-mechanics.md#settling-velocity) $V_s$, a mixed rectangular-channel current obeys $D h=-hu_x$, $D u=-bh_x-hb_x/2$, $D b=-V_sb/h$, where $D=\partial_t+u\partial_x$. The [characteristic speeds](partial-differential-equation.md#characteristic-speed) are $u,u\pm c$, with $c^2=bh$. Along the latter curves,

$$
du\pm\frac ch\,dh\pm\frac h{2c}\,db=\mp\frac{V_sc}{2h}\,dt.
$$

The density differential matters: $u\pm2c$ are [Riemann invariants](compressible-flow.md#riemann-invariant) only when the [reduced gravity](reduced-gravity.md) is constant without deposition.

##### Axisymmetric settling box model

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

An axisymmetric [gravity-current box model](#gravity-current-box-model) with no entrainment and negligible suspended-particle volume loss has constant bulk volume $\mathcal V$, uniform height $h$, and uniform particle volume fraction $c$. For an absorbing horizontal bed and downward [settling velocity](fluid-mechanics.md#settling-velocity) $w_s>0$, particle [mass conservation](continuum-mechanics.md#mass-conservation) gives $\dot c=-w_sc/h$. A constant front [Froude number](#froude-number) closes spreading by $\dot R=\operatorname{Fr}\sqrt{g_0ch}$, where $g_0=g(\rho_p-\rho_a)/\rho_a$ is buoyancy per unit volume fraction. This model describes the mixed bulk and its head closure, not the initial inertial blast or a resolved head shape.

###### Settling exposure for a particle size distribution

↑ **Parent:** [Axisymmetric settling box model](#axisymmetric-settling-box-model)

In a mixed [particle-laden gravity current](#particle-laden-gravity-current), a size class with settling speed $w$ has concentration $c(w,t)=c_0(w)e^{-wJ(t)}$. The shared [reduced gravity](reduced-gravity.md) is $g'(J)=\int g_0(w)c_0(w)e^{-wJ}\,dw$, and $dR^4/dJ=4\operatorname{Fr}(\mathcal V/\pi)^{3/2}\sqrt{g'(J)}$. Finite runout therefore requires $\int_0^\infty\sqrt{g'(J)}\,dJ<\infty$. A positive minimum settling speed guarantees this; a distribution with arbitrarily small settling speeds need not. For $g_0c_0(w)\sim Cw^p$ at zero, with $p>-1$, the integral converges precisely when $p>1$.

###### Monodisperse circular ash runout

↑ **Parent:** [Axisymmetric settling box model](#axisymmetric-settling-box-model)

With $A=\mathcal V/\pi$, $g'_0=g_0c_0$ and initial radius $R_0$, eliminating time from the [axisymmetric settling box model](#axisymmetric-settling-box-model) gives $\sqrt{c/c_0}=(R_\infty^4-R^4)/(R_\infty^4-R_0^4)$. Put $s_0=R_0^2/R_\infty^2$ and $\tau=4A/(w_sR_\infty^2)$. Then $R^2/R_\infty^2=\tanh[t/\tau+\operatorname{artanh}s_0]$. Thus the finite limiting runout is approached at infinite time; treating it as an exactly attained finite-time stopping point contradicts these balances.

###### Circular ash deposit profile

↑ **Parent:** [Monodisperse circular ash runout](#monodisperse-circular-ash-runout)

For the [monodisperse circular ash runout](#monodisperse-circular-ash-runout), integrate the local particle [deposition flux](fluid-mechanics.md#particle-deposition-flux) $\rho_pw_sc(t)$ from first arrival to infinite time. Here $s=\max(s_0,r^2/R_\infty^2)$ for $0\leq r<R_\infty$ and $s_0=R_0^2/R_\infty^2$. The displayed $\Sigma$ is deposited particle mass per horizontal area, and vanishes outside the limiting current. It is constant under the initial disk, then decreases to zero; integrating $2\pi r\Sigma$ gives the initial ash mass $\rho_pc_0\mathcal V$. A deposit thickness additionally requires its packing fraction or bulk deposit density.

##### Prismatic triangular-channel shallow water equations

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

For fixed channel width $b(z)=\beta z$, cross-sectional area is $A=\beta h^2/2$. With [reduced gravity](reduced-gravity.md) $G\phi$, uniform cross-sectional fields and downward [settling velocity](fluid-mechanics.md#settling-velocity) magnitude $w$, [volume conservation](physics.md#volume-conservation), [momentum](classical-mechanics.md#momentum) and [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) give

$$
h_t+uh_x+(h/2)u_x=0,\qquad u_t+uu_x+G\phi h_x+(Gh/3)\phi_x=0,\qquad\phi_t+u\phi_x=-2w\phi/h.
$$

The [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) force contains $\int_0^h(h-z)\beta z\,dz=\beta h^3/6$. No streamwise widening term occurs in a prismatic channel. Deposition uses the projected boundary width $\beta h$ under the vertical-settling model.

###### Sedimenting triangular-channel characteristic compatibility

↑ **Parent:** [Prismatic triangular-channel shallow water equations](#prismatic-triangular-channel-shallow-water-equations)

For the [prismatic triangular-channel shallow water equations](#prismatic-triangular-channel-shallow-water-equations), $c^2=G\phi h/2$. The [characteristic speeds](partial-differential-equation.md#characteristic-speed) are $u,u\pm c$. Along $dx/dt=u$, $d\phi/dt=-2w\phi/h$. Along $dx/dt=u\pm c$, the [hyperbolic system](partial-differential-equation.md#hyperbolic-system) has compatibility relation

$$
du\pm4\,dc\mp\frac{4c}{3\phi}\,d\phi=\mp\frac{4wc}{3h}\,dt.
$$

The [concentration](physics.md#concentration) differential cannot generally be discarded to obtain [Riemann invariants](compressible-flow.md#riemann-invariant) $u\pm4c$. Positive depth and [concentration](physics.md#concentration) are required for this nondegenerate form.

##### Buoyancy production in a particle-laden current

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

The integrated budget is $\partial_t(g^{\prime} h)+B_x=S_B-v_sg^{\prime}$. A steady spatial increase needs a source $S_B$ exceeding deposition, for example [sediment resuspension](fluid-mechanics.md#sediment-resuspension) or lateral particle input. In unsteady flow, local depletion can produce $B_x>0$ even without particle addition.

##### Weak-settling attenuation of a sloping gravity current

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

For slowly depositing particles, $B_x=-v_sB/(uh)$ and local adjustment gives $u\sim\beta_*B^{1/3}$ with the [constant-speed entraining gravity current on a slope](#constant-speed-entraining-gravity-current-on-a-slope) coefficient. At leading order $h\sim h_0+E(x-x_0)$ and $B^{1/3}=B_o^{1/3}-[v_s/(3\beta_*E)]\ln[1+E(x-x_0)/h_0]$. Its validity requires settling slow compared with the current and, for small $E$, compared with entrainment.

###### Formal sedimentation runout of a sloping gravity current

↑ **Parent:** [Weak-settling attenuation of a sloping gravity current](#weak-settling-attenuation-of-a-sloping-gravity-current)

Extrapolating the leading [weak-settling attenuation of a sloping gravity current](#weak-settling-attenuation-of-a-sloping-gravity-current) to zero flux gives $x_{\max}-x_0=(h_0/E)[\exp(3\beta_*EB_o^{1/3}/v_s)-1]$. Since speed tends to zero there, the weak-settling assumption fails in the terminal region; this is a formal leading-model estimate, not a uniformly accurate full-flow runout.

##### Steady depositing gravity current

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

A dilute, vertically mixed [particle-laden gravity current](#particle-laden-gravity-current) with no [fluid entrainment](fluid-mechanics.md#fluid-entrainment), bed erosion or carrier-fluid leakage obeys [volume conservation](physics.md#volume-conservation) $q=uh=\text{constant}$. With downward [settling velocity](fluid-mechanics.md#settling-velocity) magnitude $v_s$, an absorbing bed gives $q\,dg'/dx=-v_sg'$. The [variable-buoyancy shallow water equations](physics.md#variable-buoyancy-shallow-water-equations) conserve the kinematic momentum flux including [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure),

$$
g'(x)=g'_0e^{-v_sx/q},\qquad K=\frac{q^2}{h}+\frac12g'h^2.
$$

These equations describe a steady interior supplied continuously from upstream, not the moving nose of a finite-volume release. The depth follows one of the [depth branches of a steady depositing gravity current](#depth-branches-of-a-steady-depositing-gravity-current).

###### Bidisperse gravity-current deposition

↑ **Parent:** [Steady depositing gravity current](#steady-depositing-gravity-current)

In a [bidisperse particle suspension](fluid-mechanics.md#bidisperse-particle-suspension) transported by a [steady depositing gravity current](#steady-depositing-gravity-current), species with concentrations $c_i$ and downward [settling velocity](fluid-mechanics.md#settling-velocity) magnitudes $v_i$ satisfy $c_i(x)=c_{i0}e^{-v_ix/q}$. Their local [particle deposition fluxes](fluid-mechanics.md#particle-deposition-flux) are $v_ic_i$. The local deposited particle-volume fraction belonging to species one is

$$
f_1(x)=\frac{v_1c_{10}e^{-v_1x/q}}{v_1c_{10}e^{-v_1x/q}+v_2c_{20}e^{-v_2x/q}}.
$$

For $v_1>v_2>0$ and both species present, $f_1$ decreases strictly downstream, since $f_1'=(v_2-v_1)f_1(1-f_1)/q$. If $g'_i=g_{0i}c_i$, use $c_i=g'_i/g_{0i}$ rather than buoyancy ratios unless $g_{01}=g_{02}$. A number fraction additionally divides each species volume flux by its single-particle volume. Integrating deposition over $[0,x]$ instead gives cumulative weights $q c_{i0}(1-e^{-v_ix/q})$.

###### Depth branches of a steady depositing gravity current

↑ **Parent:** [Steady depositing gravity current](#steady-depositing-gravity-current)

For positive $q,K,g'$ in a [steady depositing gravity current](#steady-depositing-gravity-current), the function $K(h)=q^2/h+g'h^2/2$ has a unique minimum at $h_c=(q^2/g')^{1/3}$, where $\operatorname{Fr}=1$ and $K_c=3q^{4/3}(g')^{1/3}/2$. When $K>K_c$ there are two positive depth roots: $h_-<h_c$ is [supercritical flow](#supercritical-flow) and $h_+>h_c$ is [subcritical flow](#subcritical-flow). Differentiating the momentum invariant and using $g'_x=-v_sg'/q$ gives

$$
\frac{dh}{dx}=\frac{v_sh}{2q(1-\operatorname{Fr}^2)}.
$$

The supercritical depth decreases towards $q^2/K$ as $g'\downarrow0$, whereas the subcritical depth increases like $\sqrt{2K/g'}$. Because $K_c$ decreases downstream, an initially strict branch never reaches a finite-distance critical point. A critical inlet instead gives a singular depth derivative, so a smooth critical continuation is not justified by this model.

##### Heated particle-laden gravity current

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

A [heated particle-laden layer](fluid-mechanics.md#heated-particle-laden-layer) released along a bed forms a [gravity current](#gravity-current) while $g'=g(\gamma\phi-\theta)>0$. In a [gravity-current box model](#gravity-current-box-model), heating can make $g'$ vanish in finite time, whereas [settling velocity](fluid-mechanics.md#settling-velocity) alone can give finite [runout length of a gravity current](#runout-length-of-a-gravity-current) approached asymptotically.

###### Heated gravity-current runout

↑ **Parent:** [Heated particle-laden gravity current](#heated-particle-laden-gravity-current)

In a constant-volume [gravity-current box model](#gravity-current-box-model) without settling, $\phi=\phi_0$ and $g'=g\phi_0(\gamma-\beta t)$. A constant [Froude number](#froude-number) then gives finite [runout length of a gravity current](#runout-length-of-a-gravity-current) at the neutral-buoyancy time $\gamma/\beta$. Further motion requires a different physical model once the [stable density stratification](gravity-wave.md#stable-density-stratification) is lost.

##### Triangular-channel shallow water equations

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

In a channel with width $2\lambda xz$ at height $z$, a well-mixed [particle-laden gravity current](#particle-laden-gravity-current) of depth $h$ occupies area $\lambda xh^2$. Its [volume conservation](physics.md#volume-conservation), momentum and [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) balances give

$$
h_t+uh_x+(h/2)u_x=-uh/(2x),\quad
u_t+uu_x+d\phi h_x+(dh/3)\phi_x=0,\quad
\phi_t+u\phi_x=-2W_s\phi/h,
$$

where the [reduced gravity](reduced-gravity.md) is $g'=d\phi$. The $h/3$ coefficient is the cross-section-weighted mean of $h-z$ in the [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) force. The [characteristic curves](partial-differential-equation.md#characteristic-curve) have speeds $u$ and $u\pm\sqrt{g'h/2}$.

##### Triangular-channel gravity-current box model

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

A finite-volume [gravity-current box model](#gravity-current-box-model) in a widening triangular channel has volume proportional to $h^2L^2$, so $hL=K$ is constant. A [gravity-current front condition](#gravity-current-front-condition) and absorbing-bed [particle deposition flux](fluid-mechanics.md#particle-deposition-flux) give

$$
\dot L=\operatorname{Fr}\sqrt{dK\phi/L},\qquad \dot\phi=-2W_sL\phi/K.
$$

Eliminating time makes $\sqrt\phi$ affine in $L^{5/2}$, producing a finite limiting [runout length of a gravity current](#runout-length-of-a-gravity-current) despite an infinite idealized stopping time.

##### Runout length of a gravity current

↑ **Parent:** [Particle-laden gravity current](#particle-laden-gravity-current)

The runout length is the limiting horizontal distance reached by a gravity current after its driving buoyancy has been exhausted or balanced by resistance.

### Draining gravity current

↑ **Parent:** [Gravity current](#gravity-current)

A draining gravity current loses fluid through its substrate while spreading horizontally. For a two-dimensional viscous current of thickness $H(x,t)$ that loses fluid according to [pressure-dependent Darcy drainage](porous-media-flow.md#pressure-dependent-darcy-drainage),

$$
H_t=A(H^3H_x)_x-DH^{1-\beta},
\qquad A=\frac{\rho g}{3\mu},
$$

when the [hydrostatic pressure](fluid-mechanics.md#hydrostatic-pressure) is $p=\rho gH$ and $k/h\propto p^{-\beta}$.

#### Deep-substrate drainage of a gravity current

↑ **Parent:** [Draining gravity current](#draining-gravity-current)

Combining the [lubrication gravity-current flux](viscous-fluid-flow.md#lubrication-gravity-current-flux) with [vertical imbibition under a draining liquid layer](porous-media-flow.md#vertical-imbibition-under-a-draining-liquid-layer) gives

$$
h_t-\frac{g}{3\nu}(h^3h_x)_x=-\frac{gk}{\nu}(1+h/l)=-\phi l_t.
$$

The injected volume is the integral of $h+\phi l$, not just the surface current thickness. The model neglects horizontal subsurface flow and applies only where the substrate is wetted and the surface current supplies its drainage.

##### Cubic-input similarity for a draining gravity current

↑ **Parent:** [Deep-substrate drainage of a gravity current](#deep-substrate-drainage-of-a-gravity-current)

For a one-sided [draining gravity current](#draining-gravity-current) with injected volume per unit width $V_0(t/\tau)^3$, define

$$
C=\left(\frac{\nu V_0^2}{g\tau^6}\right)^{1/5},\quad
D=\left(\frac{gV_0^3}{\nu\tau^9}\right)^{1/5},\quad
\xi=\frac{x}{Dt^2},\quad h=CtH(\xi),\quad l=CtL(\xi).
$$

The [similarity solution](partial-differential-equation.md#similarity-solution) satisfies

$$
H-2\xi H'-\frac13(H^3H')'=-K(1+H/L),\qquad
\phi(L-2\xi L')=K(1+H/L),
$$

where $K=k[g^3\tau^3/(\nu^3V_0)]^{2/5}$. The inlet condition is $-H(0)^3H'(0)=9$, the integral of $H+\phi L$ is one, and both depths vanish at the advancing front. The endpoint $\xi_N$ gives $x_N=\xi_NDt^2$ and depends on $K$ and $\phi$.

#### Similarity exponents of a draining gravity current

↑ **Parent:** [Draining gravity current](#draining-gravity-current)

If a [draining gravity current](#draining-gravity-current) is supplied with [volume flux](fluid-mechanics.md#volumetric-flow-rate) proportional to $t^\alpha$, a first-kind [similarity solution](partial-differential-equation.md#similarity-solution) has

$$
H=t^aF(x/t^b),
\qquad
a=\frac{2\alpha+1}{5},
\qquad
b=\frac{3\alpha+4}{5},
$$

provided

$$
\beta=\frac1a=\frac5{2\alpha+1}.
$$

These relations follow by balancing the time derivative, horizontal [lubrication theory](viscous-fluid-flow.md#lubrication-theory) flux, vertical drainage, and imposed inlet flux.

### Lock-exchange flow

↑ **Parent:** [Gravity current](#gravity-current)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lock-exchange_flow)

Removing a barrier between fluids of different densities creates oppositely directed gravity currents. In an energy-conserving Boussinesq exchange through a full-depth opening, each layer occupies half the depth.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (93)

- [Broad-crested weir](#broad-crested-weir)
- [Buoyancy-gradient mixing-length closure](turbulence.md#buoyancy-gradient-mixing-length-closure)
- [Buoyant thermal](turbulent-plume.md#buoyant-thermal)
- [Buoyant thermal mass balance](turbulent-plume.md#buoyant-thermal-mass-balance)
- [Characteristic compatibility for an entraining triangular-channel current](#characteristic-compatibility-for-an-entraining-triangular-channel-current)
- [Coefficient of thermal expansion](thermodynamics.md#coefficient-of-thermal-expansion)
- [Deformation radius](geophysical-fluid-dynamics.md#deformation-radius)
- [Detrainment-limited gravity-current runout](#detrainment-limited-gravity-current-runout)
- [Entraining shallow-water current in a triangular channel](#entraining-shallow-water-current-in-a-triangular-channel)
- [Finite-Froude lock-release rarefaction](#finite-froude-lock-release-rarefaction)
- [Finite-volume triangular-channel current](#finite-volume-triangular-channel-current)
- [Fixed-speed pure-plume merger and flux conservation](turbulent-plume.md#fixed-speed-pure-plume-merger-and-flux-conservation)
- [Floating extensional viscous gravity current](#floating-extensional-viscous-gravity-current)
- [Front-regularized triangular-channel dam break](#front-regularized-triangular-channel-dam-break)
- [Froude number](#froude-number)
- [Heated particle-laden layer](fluid-mechanics.md#heated-particle-laden-layer)
- [Hindered-settling runout in a rectangular channel](#hindered-settling-runout-in-a-rectangular-channel)
- [Hydraulic flow in an inverted channel](#hydraulic-flow-in-an-inverted-channel)
- [Interfacial Richardson number](gravity-wave.md#interfacial-richardson-number)
- [Merger of two equal pure plumes](turbulent-plume.md#merger-of-two-equal-pure-plumes)
- [Newtonian grounding-line flux](geophysics.md#newtonian-grounding-line-flux)
- [Particle-laden gravity current](#particle-laden-gravity-current)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-43.md#5/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-52.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-76.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-75.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-83.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-84.md#6/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-90.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-74.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-79.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-80.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-71.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-79.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-69.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-73.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-70.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-70.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-74.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-330.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-345.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-345.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-345.md#3/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-345.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-345.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345.md#1/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345.md#1/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-345.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-345.md#2/b/solution)
- [Plume-fed doorway ventilation](fluid-mechanics.md#plume-fed-doorway-ventilation)
- [Potential-energy cost of homogenizing a linear stratification](gravity-wave.md#potential-energy-cost-of-homogenizing-a-linear-stratification)
- [Prismatic triangular-channel shallow water equations](#prismatic-triangular-channel-shallow-water-equations)
- [Sedimenting rectangular-channel characteristic compatibility](#sedimenting-rectangular-channel-characteristic-compatibility)
- [Self-similar starting plume](turbulent-plume.md#self-similar-starting-plume)
- [Settling exposure for a particle size distribution](#settling-exposure-for-a-particle-size-distribution)
- [Source-volume blocking of displacement ventilation](fluid-mechanics.md#source-volume-blocking-of-displacement-ventilation)
- [Starting-plume thermal Froude-number ratio](turbulent-plume.md#starting-plume-thermal-froude-number-ratio)
- [Symmetric line-plume filling-box front](turbulent-plume.md#symmetric-line-plume-filling-box-front)
- [Triangular-channel shallow water equations](#triangular-channel-shallow-water-equations)
- [Triangular-profile wall line plume](turbulent-plume.md#triangular-profile-wall-line-plume)
- [Two-sided top-hat line plume](turbulent-plume.md#two-sided-top-hat-line-plume)
- [Two successive hydraulic controls](#two-successive-hydraulic-controls)
- [Unsteady top-hat line-plume balances](turbulent-plume.md#unsteady-top-hat-line-plume-balances)
- [Variable-buoyancy shallow water equations](physics.md#variable-buoyancy-shallow-water-equations)
- [Variable-width shallow-water characteristics](physics.md#variable-width-shallow-water-characteristics)
- [Ventilated filling-box relaxation](fluid-mechanics.md#ventilated-filling-box-relaxation)
