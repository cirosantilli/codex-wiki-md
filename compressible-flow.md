# Compressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressible_flow)

Compressible flow allows density to change materially and is required for finite-amplitude pressure waves and shocks.

**Table of contents**

- [Transonic flow](#transonic-flow)
- [Stagnation temperature](#stagnation-temperature)
- [Choked flow](#choked-flow)
- [Quasi-one-dimensional flow](#quasi-one-dimensional-flow)
- [Isothermal flow through molecular hydrogen formation](#isothermal-flow-through-molecular-hydrogen-formation)
- [Self-similar blast wave](#self-similar-blast-wave)
  - [Spherical blast-wave similarity energy integrals](#spherical-blast-wave-similarity-energy-integrals)
  - [Pressure similarity in a spherical blast wave](#pressure-similarity-in-a-spherical-blast-wave)
  - [Thin-shell approximation for a spherical blast wave](#thin-shell-approximation-for-a-spherical-blast-wave)
  - [Spherical blast wave in a power-law ambient density](#spherical-blast-wave-in-a-power-law-ambient-density)
    - [Linear-profile spherical blast wave](#linear-profile-spherical-blast-wave)
  - [Planar blast-wave energy scaling](#planar-blast-wave-energy-scaling)
- [Polytropic flow](#polytropic-flow)
- [Spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow)
  - [Transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential)
    - [Transonic spherical accretion rate in a power-law potential](#transonic-spherical-accretion-rate-in-a-power-law-potential)
      - [Endpoint limits of power-law spherical accretion](#endpoint-limits-of-power-law-spherical-accretion)
    - [Critical adiabatic exponent for spherical power-law flow](#critical-adiabatic-exponent-for-spherical-power-law-flow)
- [Isothermal shock](#isothermal-shock)
  - [Dissociating isothermal shock](#dissociating-isothermal-shock)
  - [Cooling across an isothermal shock](#cooling-across-an-isothermal-shock)
- [Fluid total-energy equation](#fluid-total-energy-equation)
- [Spherical polytropic flow with adiabatic exponent three halves](#spherical-polytropic-flow-with-adiabatic-exponent-three-halves)
- [Speed of sound](#speed-of-sound)
  - [Sound-crossing time](#sound-crossing-time)
  - [Isothermal sound speed](#isothermal-sound-speed)
  - [Adiabatic sound speed](#adiabatic-sound-speed)
- [Isentropic flow](#isentropic-flow)
  - [Isentropic Euler equations](#isentropic-euler-equations)
  - [Homentropic flow](#homentropic-flow)
- [Globally isothermal equation of state](#globally-isothermal-equation-of-state)
- [Sonic point](#sonic-point)
  - [Plane-parallel isothermal sonic transition at a potential maximum](#plane-parallel-isothermal-sonic-transition-at-a-potential-maximum)
  - [Sonic-point slope discriminant](#sonic-point-slope-discriminant)
  - [Critical speed of a polytropic flow](#critical-speed-of-a-polytropic-flow)
  - [Transonic branch](#transonic-branch)
    - [Transonic accretion in a power-law tube](#transonic-accretion-in-a-power-law-tube)
- [Mach number](#mach-number)
  - [Moving-point acoustic wavefronts](#moving-point-acoustic-wavefronts)
  - [Radial Mach number](#radial-mach-number)
  - [Subsonic flow](#subsonic-flow)
  - [Sonic flow](#sonic-flow)
  - [Supersonic flow](#supersonic-flow)
- [Riemann invariant](#riemann-invariant)
  - [Riemann invariants for one-dimensional isentropic flow](#riemann-invariants-for-one-dimensional-isentropic-flow)
    - [Vacuum formation at an accelerating withdrawing piston](#vacuum-formation-at-an-accelerating-withdrawing-piston)
  - [Simple wave](#simple-wave)
    - [Area transformation of a nonlinear acoustic simple wave](#area-transformation-of-a-nonlinear-acoustic-simple-wave)
      - [Shock distance for a spherical simple wave launched at finite radius](#shock-distance-for-a-spherical-simple-wave-launched-at-finite-radius)
    - [Linearly degenerate characteristic field](#linearly-degenerate-characteristic-field)
    - [Simple wave in magnetohydrodynamics](#simple-wave-in-magnetohydrodynamics)
      - [Perpendicular fast magnetosonic simple wave](#perpendicular-fast-magnetosonic-simple-wave)
        - [Isothermal perpendicular magnetosonic simple wave](#isothermal-perpendicular-magnetosonic-simple-wave)
    - [Damping threshold for a simple wave](#damping-threshold-for-a-simple-wave)
    - [Receding-piston rarefaction wave](#receding-piston-rarefaction-wave)
      - [Vacuum formation behind a receding piston](#vacuum-formation-behind-a-receding-piston)
      - [Singular small-power piston emission time](#singular-small-power-piston-emission-time)
  - [Pressure in a perfect-gas simple wave](#pressure-in-a-perfect-gas-simple-wave)
  - [Shock formation by characteristic intersection](#shock-formation-by-characteristic-intersection)
- [Normal shock wave](#normal-shock-wave)
  - [Shock tube](#shock-tube)
  - [Normal shock reflection at a rigid wall](#normal-shock-reflection-at-a-rigid-wall)
  - [Moving-interface conservation jump identity](#moving-interface-conservation-jump-identity)
  - [Normal shock tables](#normal-shock-tables)
  - [Shock frame](#shock-frame)
  - [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)
    - [Prandtl shock relation](#prandtl-shock-relation)
    - [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions)
      - [Energy fluxes of a strong adiabatic shock](#energy-fluxes-of-a-strong-adiabatic-shock)
      - [Shock compression ratio](#shock-compression-ratio)
        - [Planar shock compression of a finite slab](#planar-shock-compression-of-a-finite-slab)
          - [Mach-number convention in shock unbinding estimates](#mach-number-convention-in-shock-unbinding-estimates)
    - [Piston-driven normal shock](#piston-driven-normal-shock)
      - [Piston-driven shock with specific-heat ratio three](#piston-driven-shock-with-specific-heat-ratio-three)
    - [Pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas)
      - [Entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock)
        - [Entropy production in successive weak shocks](#entropy-production-in-successive-weak-shocks)
  - [Weak shock](#weak-shock)
  - [Oblique shock](#oblique-shock)
    - [Strong oblique-shock angle branches](#strong-oblique-shock-angle-branches)
    - [Shock polar](#shock-polar)
      - [Strong-shock polar for a perfect gas](#strong-shock-polar-for-a-perfect-gas)
        - [Maximum deflection through a strong perfect-gas shock](#maximum-deflection-through-a-strong-perfect-gas-shock)
    - [Weak-oblique-shock deflection](#weak-oblique-shock-deflection)
    - [Mach angle](#mach-angle)
      - [Mach cone](#mach-cone)

## Transonic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A [compressible flow](compressible-flow.md) that passes between subsonic and supersonic regions. A smooth steady crossing of a [sonic point](#sonic-point) requires the corresponding regularity condition; a discontinuous transition can instead involve a [shock wave](transport-equation.md#shock-wave).

## Stagnation temperature

↑ **Parent:** [Compressible flow](compressible-flow.md)

The [temperature](temperature.md) reached by bringing a flow to rest adiabatically while converting its [kinetic energy](energy.md#kinetic-energy) to enthalpy. For a calorically [perfect gas](ideal-gas.md), $T_{\rm stag}=T+u^2/(2c_p)=T[1+(\gamma-1)M^2/2]$. It is conserved across an adiabatic normal shock even though [entropy](entropy.md) increases and [stagnation pressure](fluid-mechanics.md#stagnation-pressure) decreases.

## Choked flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

Flow whose [mass](classical-mechanics.md#mass) flux is limited by a sonic condition in a controlling section, for fixed upstream thermodynamic conditions. In a smooth isentropic converging-diverging [nozzle](fluid-mechanics.md#nozzle), the throat reaches [Mach number](#mach-number) one. Lowering downstream [pressure](pressure.md) further cannot indefinitely increase that fixed-upstream throat [mass](classical-mechanics.md#mass) flux; shocks and downstream structure can still change.

## Quasi-one-dimensional flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A model representing a passage by its varying cross-sectional area and approximately uniform section-averaged flow variables. It neglects detailed transverse [velocity](classical-mechanics.md#velocity) and thermodynamic structure. In a smooth lossless [nozzle](fluid-mechanics.md#nozzle), conservation laws then connect area to [Mach number](#mach-number); this model does not by itself determine the curved sonic surface of an arbitrary multidimensional passage.

## Isothermal flow through molecular hydrogen formation

↑ **Parent:** [Compressible flow](compressible-flow.md)

Across a thin steady transition with negligible external impulse, [mass conservation](continuum-mechanics.md#mass-conservation) and [momentum conservation](momentum.md#momentum-conservation) give the displayed relations. If the gas stays isothermal while neutral atomic [hydrogen](chemical-substance.md#hydrogen) becomes [molecular hydrogen](chemical-substance.md#molecular-hydrogen), the mean particle [mass](classical-mechanics.md#mass) doubles and $a_2^2=a_1^2/2$ for its [isothermal sound speed](#isothermal-sound-speed). Let $J=u_1+a_1^2/u_1$. The downstream subsonic branch has $u_2=[J-\sqrt{J^2-2a_1^2}]/2$, $\rho_2/\rho_1=u_1/u_2$, and $p_2-p_1=\rho_1u_1(u_1-u_2)>0$.

For $u_1\ll a_1$, the leading behavior is $u_2\simeq u_1/2$, $\rho_2\simeq2\rho_1$ and $p_2\simeq p_1$, at unchanged [temperature](temperature.md). Radiation of the molecular binding energy prevents that released energy from necessarily heating the gas; it does not, by itself, establish an isothermal thermal closure. If temperature evolution is allowed, an energy balance and a cooling model are required to determine all four changes uniquely.

## Self-similar blast wave

↑ **Parent:** [Compressible flow](compressible-flow.md)

A [self-similar blast wave](#self-similar-blast-wave) is an expanding [shock wave](transport-equation.md#shock-wave) whose post-shock profiles retain their shape in a rescaled radius or distance. A fixed explosion energy, ambient [mass density](fluid-mechanics.md#density) and geometry set the front scaling through conservation of total energy. The dimensionless coefficient requires the profiles and an energy-normalization convention.

### Spherical blast-wave similarity energy integrals

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

Use the fields of [pressure similarity in a spherical blast wave](#pressure-similarity-in-a-spherical-blast-wave), with front radius $R=\xi_0\ell$. Since $\rho_0\ell^5/t^2=E$, changing the radial integration variable to $\xi$ gives

$$
E_{\rm kin}=2\pi E\int_0^{\xi_0}\xi^4f_\rho f_u^2\,d\xi,\qquad
E_{\rm int}=\frac{4\pi E}{\gamma-1}\int_0^{\xi_0}\xi^2f_p\,d\xi.
$$

Both are time independent for fixed integrable [similarity profiles](partial-differential-equation.md#similarity-profile) and constant front coordinate $\xi_0$. With explosion energy $E$ and negligible external energy input or losses, their sum equals $E$. This normalization, together with shock matching and regularity, fixes the dimensionless blast coefficient rather than [dimensional analysis](mathematical-physics.md#dimensional-analysis) alone.

### Pressure similarity in a spherical blast wave

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

For a spherical [self-similar blast wave](#self-similar-blast-wave), put $\ell=(Et^2/\rho_0)^{1/5}$, $\xi=r/\ell$, $\rho=\rho_0f_\rho(\xi)$ and $u=(r/t)f_u(\xi)$. The radial [Euler equation](euler-equations-for-an-inviscid-fluid.md) then requires $p=\rho_0(\ell/t)^2f_p(\xi)$, where

$$
f_p'=-\xi f_\rho\left[f_u^2-f_u+\xi\left(f_u-\frac25\right)f_u'\right].
$$

This follows from $\partial_t\xi=-2\xi/(5t)$ and $\partial_r\xi=1/\ell$. The momentum equation alone leaves a spatially uniform additive [pressure](pressure.md) undetermined. The scale-free strong-shock boundary data fix that freedom consistently with the displayed similarity scaling; an independently prescribed ambient pressure introduces another scale.

### Thin-shell approximation for a spherical blast wave

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

Let a strong [shock wave](transport-equation.md#shock-wave) of radius $R$ and speed $V$ sweep a uniform [mass density](fluid-mechanics.md#density) $\rho_0$ into a shell of mass $4\pi\rho_0R^3/3$ and speed $2V/(\gamma+1)$. If the cavity [pressure](pressure.md) is $\alpha$ times the immediate post-shock [pressure](pressure.md), shell [momentum](momentum.md) balance gives $R\dot V=3(\alpha-1)V^2$. Constant total [energy](energy.md) gives $R^3V^2=\mathrm{constant}$ and hence $\alpha=1/2$. Including shell internal and kinetic [energy](energy.md), and treating the cavity volume as $4\pi R^3/3$ to thin-shell accuracy, yields $R=\xi(E/\rho_0)^{1/5}t^{2/5}$ with $\xi^5=75(\gamma-1)(\gamma+1)^2/[16\pi(5\gamma-3)]$. This coefficient is approximate; resolving the shell's finite volume changes it.

### Spherical blast wave in a power-law ambient density

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

For an [energy](energy.md)-conserving strong spherical [shock wave](transport-equation.md#shock-wave) expanding into [mass density](fluid-mechanics.md#density) $Cr^{-\beta}$, $0\leq\beta<3$, [dimensional analysis](mathematical-physics.md#dimensional-analysis) gives the displayed radius law. Neglect ambient [pressure](pressure.md), radiation losses and gravity in this blast-dominated approximation. Write $u=\dot R U(\xi)$, $\rho=CR^{-\beta}D(\xi)$ and $p=CR^{-\beta}\dot R^2P(\xi)$, with $\xi=r/R$. The radial [continuity equation](mathematical-physics.md#continuity-equation), momentum equation and adiabatic [pressure](pressure.md) equation reduce to

$$
(U-\xi)D'+D(U'+2U/\xi-\beta)=0,\qquad
(U-\xi)U'+\frac{\beta-3}{2}U=-P'/D,
$$



$$
(U-\xi)P'+[\gamma(U'+2U/\xi)-3]P=0.
$$

The [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions) give $U(1)=P(1)=2/(\gamma+1)$ and $D(1)=(\gamma+1)/(\gamma-1)$. The explosion [energy](energy.md) fixes the radius coefficient through $E=4\pi CR^{3-\beta}\dot R^2\int_0^1[DU^2/2+P/(\gamma-1)]\xi^2d\xi$.

#### Linear-profile spherical blast wave

↑ **Parent:** [Spherical blast wave in a power-law ambient density](#spherical-blast-wave-in-a-power-law-ambient-density)

The [similarity profiles](partial-differential-equation.md#similarity-profile) $U=2\xi/(\gamma+1)$, $D=(\gamma+1)\xi/(\gamma-1)$ and $P=2\xi^3/(\gamma+1)$ solve the spherical blast equations at the displayed ambient exponent. For $\gamma=5/3$, $\beta=2$ and $R^3=3Et^2/(2\pi C)$. The dimensional fields are $u=r/(2t)$, $\rho=8\pi C^2r/(3Et^2)$ and $p=2\pi C^2r^3/(9Et^4)$ for $0<r<R$. Their kinetic and internal [energies](energy.md) are equal. Substituting these profiles into all three equations and the shock conditions verifies the solution.

### Planar blast-wave energy scaling

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

For a planar adiabatic explosion with energy per unit area $E$ in a uniform medium of [mass density](fluid-mechanics.md#density) $\rho_0$, the conserved energy has form $E=I\rho_0Z\dot Z^2$, with a finite positive integral $I$ of the [similarity profiles](partial-differential-equation.md#similarity-profile). Hence $Z=C(E/\rho_0)^{1/3}t^{2/3}$. If $E$ is shared by two fronts, its fraction assigned to either side is absorbed into $C$.

## Polytropic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A polytropic flow uses a [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state). When $K$ and the [adiabatic exponent](ideal-gas.md#heat-capacity-ratio) are constant, a smooth streamline has [specific enthalpy](enthalpy.md#specific-enthalpy) $h=\gamma K\rho^{\gamma-1}/(\gamma-1)$ and [adiabatic sound speed](#adiabatic-sound-speed) $c_s^2=\gamma K\rho^{\gamma-1}$. Spatially varying entropy can make $K$ depend on streamline; the constant-$K$ spherical wind is a special case.

## Spherically symmetric adiabatic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A smooth radial [compressible flow](compressible-flow.md) with a fixed [adiabatic exponent](ideal-gas.md#heat-capacity-ratio) conserves $r^2\rho u$ and $p/\rho^\gamma$. In a prescribed [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential), its [Bernoulli function](euler-equations-for-an-inviscid-fluid.md#bernoulli-function) is $u^2/2+c^2/(\gamma-1)+\Phi$, with $c$ the [adiabatic sound speed](#adiabatic-sound-speed). Eliminating the density derivative yields $(u-c^2/u)u'=2c^2/r-\Phi'$.

### Transonic spherical flow in a power-law potential

↑ **Parent:** [Spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow)

A smooth [transonic branch](#transonic-branch) in a [power-law gravitational potential](newton-s-law-of-universal-gravitation.md#power-law-gravitational-potential) has $u_*^2=c_*^2=A\beta/(2r_*^\beta)$ at its [sonic point](#sonic-point). Substitution into the [Bernoulli function](euler-equations-for-an-inviscid-fluid.md#bernoulli-function) gives $\mathcal B=c_*^2[1/(\gamma-1)+1/2-2/\beta]$. The local [sonic-point slope discriminant](#sonic-point-slope-discriminant) distinguishes a genuine crossing from a degenerate everywhere-sonic scaling solution.

#### Transonic spherical accretion rate in a power-law potential

↑ **Parent:** [Transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential)

With reservoir density $\rho_\infty$ and [adiabatic sound speed](#adiabatic-sound-speed) $c_\infty$, put $q=2/\beta-1/2$ and $h=1-q(\gamma-1)>0$. The selected [mass accretion rate](astrophysical-black-hole.md#mass-accretion-rate) is $4\pi\rho_\infty(A\beta/2)^{2/\beta}c_\infty^{1-4/\beta}h^{q-1/(\gamma-1)}$. It follows by evaluating the conserved spherical flux at the [sonic point](#sonic-point).

##### Endpoint limits of power-law spherical accretion

↑ **Parent:** [Transonic spherical accretion rate in a power-law potential](#transonic-spherical-accretion-rate-in-a-power-law-potential)

The dimensionless accretion factor $(1-q\delta)^{q-1/\delta}$ tends to $e^q$ as $\delta\to0$. For $q>0$, it tends to $1$ as $\delta\uparrow1/q$, although the [sonic point](#sonic-point) moves to the origin. Writing the latter logarithm as $-qh\ln h/(1-h)$ makes the finite limit transparent. These limits connect [transonic spherical accretion rate in a power-law potential](#transonic-spherical-accretion-rate-in-a-power-law-potential) to the [isothermal equation of state](#globally-isothermal-equation-of-state) and the limiting critical [adiabatic exponent](ideal-gas.md#heat-capacity-ratio).

#### Critical adiabatic exponent for spherical power-law flow

↑ **Parent:** [Transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential)

For $0<\beta<4$, a nondegenerate [transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential) connected to infinity requires $\gamma<(4+\beta)/(4-\beta)$. For $\beta\geq4$, every finite $\gamma>1$ satisfies the local crossing condition; there is no finite upper bound. The uniformly valid inequality is $2\beta-(4-\beta)(\gamma-1)>0$.

## Isothermal shock

↑ **Parent:** [Compressible flow](compressible-flow.md)

An isothermal shock joins two states at the same [temperature](temperature.md) and [isothermal sound speed](#isothermal-sound-speed). Mass and [momentum](momentum.md) conservation imply $u_1u_2=c_s^2$ for a nontrivial planar jump, so the compression ratio is the upstream isothermal Mach number squared. [Heat](heat.md) exchange replaces adiabatic energy conservation across the gas alone.

### Dissociating isothermal shock

↑ **Parent:** [Isothermal shock](#isothermal-shock)

Suppose molecular [hydrogen](chemical-substance.md#hydrogen) is fully dissociated into atoms across a steady planar [shock](transport-equation.md#shock-wave), with the same far-upstream and far-downstream [temperature](temperature.md) and negligible binding-energy mass correction. The upstream [isothermal sound speed](#isothermal-sound-speed) obeys $a_1^2=k_BT/(2m_H)$, while $a_2^2=2a_1^2$. Conservation of mass gives $\chi=\rho_2/\rho_1=u_1/u_2$. Momentum conservation then gives $u_1^2+a_1^2=u_1^2/\chi+2a_1^2\chi$, producing the displayed quadratic with $\mathcal M_1=u_1/a_1$.

The high root approaches $\mathcal M_1^2/2$ at large upstream Mach number. Its real compressive domain is $\mathcal M_1\ge1+\sqrt2$. At the endpoint the downstream flow is sonic; above it the high root is subsonic downstream. Completion of dissociation and maintenance of equal temperatures additionally require a consistent chemical and radiative energy budget. The two flux equations alone do not establish that physical realizability.

### Cooling across an isothermal shock

↑ **Parent:** [Isothermal shock](#isothermal-shock)

The [specific enthalpy](enthalpy.md#specific-enthalpy) is equal on both sides of an isothermal perfect-gas shock. The energy removed per unit area per unit time is $j(u_1^2-u_2^2)/2$, with $j>0$ the normal mass flux. Net cooling therefore selects compression shocks; an expansion jump requires heating.

## Fluid total-energy equation

↑ **Parent:** [Compressible flow](compressible-flow.md)

For an inviscid fluid with specific [internal energy](internal-energy.md) $e$, let $E=\rho(e+|\mathbf u|^2/2)$. In a prescribed potential $\Phi$, $\partial_tE+\nabla\cdot[(E+p)\mathbf u]=-\rho\mathbf u\cdot\nabla\Phi+Q$, where $Q$ is external [heat](heat.md) supply. A static gravitational potential can instead be included in the conserved energy.

## Spherical polytropic flow with adiabatic exponent three halves

↑ **Parent:** [Compressible flow](compressible-flow.md)

For steady spherical [isentropic flow](#isentropic-flow) with $p=K\rho^{3/2}$ around a point mass, put $j=r^2\rho v>0$ and $\mathcal E=v^2/2+2c^2-GM/r>0$. Eliminating the [mass density](fluid-mechanics.md#density) gives $c^2=[j(3K/2)^2]^{2/5}r^{-4/5}\mathcal M^{-2/5}$. With $r_s=GM/(4\mathcal E)$, $x=(r/r_s)^{1/5}$, $y=\mathcal M^{2/5}$ and $\lambda=[j(3K/2)^2]^{2/5}/(2\mathcal E r_s^{4/5})$, the [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation) reduces to $\lambda F(y)=F(x)$, where $F(t)=t^4+4/t$. Since $F$ has its unique minimum at $t=1$, a regular [sonic point](#sonic-point) requires $\lambda=1$ and $r=r_s$. One [transonic branch](#transonic-branch) is $y=x$, which has $v=\sqrt{2\mathcal E}$, $\rho\propto r^{-2}$ and $p\propto r^{-3}$. The decreasing branch has inner [free fall](newton-s-law-of-universal-gravitation.md#free-fall) and an outer nearly static reservoir, giving [Bondi accretion](astrophysical-black-hole.md#bondi-accretion) for inward [fluid flow](fluid-mechanics.md#fluid-flow). A nonradiative stationary [shock wave](transport-equation.md#shock-wave) keeps $j,\mathcal E,r_s$ fixed but raises $K$, so $\lambda$ increases by the factor $(K_2/K_1)^{4/5}$. The inward transonic solution is the spherical $n=2$, $\gamma=3/2$ specialization of [transonic accretion in a power-law tube](#transonic-accretion-in-a-power-law-tube).

## Speed of sound

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Speed_of_sound)

The speed of sound is the propagation speed of a small pressure disturbance through a medium.

### Sound-crossing time

↑ **Parent:** [Speed of sound](#speed-of-sound)

### Isothermal sound speed

↑ **Parent:** [Speed of sound](#speed-of-sound)

The isothermal sound speed is $a_i^2=(\partial p/\partial\rho)_T$. For an ideal gas it is $a_i^2=p/\rho=\mathcal R T/\mu$.

### Adiabatic sound speed

↑ **Parent:** [Speed of sound](#speed-of-sound)

The adiabatic sound speed is $v_s^2=(\partial p/\partial\rho)_s$. For a perfect gas it is $v_s^2=\gamma p/\rho$.

## Isentropic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isentropic_flow)

An isentropic flow has constant entropy along the fluid and contains no entropy-producing shocks or dissipation. For a perfect gas, $p/\rho^\gamma$ is constant and $c_s^2=\gamma p/\rho\propto\rho^{\gamma-1}$.

### Isentropic Euler equations

↑ **Parent:** [Isentropic flow](#isentropic-flow)

In one spatial dimension, inviscid isentropic mass and momentum conservation are

$$
\rho_t+(\rho u)_x=0,
\qquad
u_t+uu_x+\rho^{-1}p_x=0,
\qquad p=p(\rho).
$$

### Homentropic flow

↑ **Parent:** [Isentropic flow](#isentropic-flow)

A homentropic flow has one spatially uniform entropy value throughout the fluid. It is therefore isentropic along every fluid trajectory, and its pressure can be treated as a single-valued function of density.

## Globally isothermal equation of state

↑ **Parent:** [Compressible flow](compressible-flow.md)

A globally isothermal fluid has spatially and temporally constant sound speed $c_s$ and pressure $p=c_s^2\rho$. Maintaining this relation generally requires heat exchange rather than adiabatic evolution.

## Sonic point

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sonic_point)

A sonic point is a point at which the flow speed equals the local [sound speed](#speed-of-sound), so the [Mach number](#mach-number) is one.

### Plane-parallel isothermal sonic transition at a potential maximum

↑ **Parent:** [Sonic point](#sonic-point)

In a nonzero steady one-dimensional flow with an [isothermal equation of state](#globally-isothermal-equation-of-state) with $p=c_s^2\rho$ and constant cross section, the [continuity equation](mathematical-physics.md#continuity-equation) gives $\rho u=\text{constant}$. Eliminating density from momentum gives $(u-c_s^2/u)u'=-\Phi'$. With [Mach number](#mach-number) $\mathcal M=|u|/c_s$, integration yields $\mathcal M^2/2-\ln\mathcal M+\Phi/c_s^2=C$. The function $f(\mathcal M)=\mathcal M^2/2-\ln\mathcal M$ has minimum $1/2$ at $\mathcal M=1$, so a smooth transonic crossing at $x_*$ requires a local maximum of $\Phi$ and $C=1/2+\Phi(x_*)/c_s^2$. At a nondegenerate maximum, $f=1/2+(\mathcal M-1)^2+\cdots$ gives $\mathcal M'(x_*)=\pm\sqrt{-\Phi''(x_*)/(2c_s^2)}$.

### Sonic-point slope discriminant

↑ **Parent:** [Sonic point](#sonic-point)

For [spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow) in a [power-law gravitational potential](newton-s-law-of-universal-gravitation.md#power-law-gravitational-potential), let $X=(r_*/u_*)u_*'$ and $\delta=\gamma-1$. Differentiation at a [sonic point](#sonic-point) gives $(2+\delta)X^2+4\delta X+4\delta-2\beta=0$. Its discriminant is $8[2\beta-(4-\beta)\delta]$; a positive value gives the two local crossing directions.

### Critical speed of a polytropic flow

↑ **Parent:** [Sonic point](#sonic-point)

For a steady polytropic streamline with Bernoulli function $C_B$, the critical speed is the sound speed at which the scalar mass flux $\rho u$ is maximal. It satisfies

$$
c_{\rm cr}^2=\frac{2(\gamma-1)}{\gamma+1}C_B.
$$

### Transonic branch

↑ **Parent:** [Sonic point](#sonic-point)

A transonic branch is a solution that passes continuously between subsonic and supersonic flow through a regular [sonic point](#sonic-point).

#### Transonic accretion in a power-law tube

↑ **Parent:** [Transonic branch](#transonic-branch)

Consider steady [isentropic flow](#isentropic-flow) toward a [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) $-GM/r$ through a tube of cross-sectional area $A(r)=Cr^n$. Write $v>0$ for the inward speed and use a [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state) with [specific-heat ratio](ideal-gas.md#heat-capacity-ratio) $\gamma>1$. [Mass conservation](continuum-mechanics.md#mass-conservation) and the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) give

$$
\rho v A=\dot M,
\qquad
\left(v-\frac{c_s^2}{v}\right)v'=\frac{nc_s^2}{r}-\frac{GM}{r^2},
$$

where $c_s$ is the [adiabatic sound speed](#adiabatic-sound-speed). A regular [sonic point](#sonic-point) therefore has $v_s=c_s$ and $r_s=GM/(nc_s^2)$. The [Bernoulli equation](euler-equations-for-an-inviscid-fluid.md#bernoulli-equation), matched to a nearly stationary reservoir with [sound speed](#speed-of-sound) $c_0$, gives

$$
\frac{v^2}{2}+\frac{c^2}{\gamma-1}-\frac{GM}{r}=\frac{c_0^2}{\gamma-1},
\qquad
c_s^2=\frac{2c_0^2}{(2n+1)-(2n-1)\gamma}.
$$

For $n>1/2$, a finite positive [sonic point](#sonic-point) requires $1<\gamma<(2n+1)/(2n-1)$. Differentiating the flow equation at that point, with $x=r_sv'_s/c_s$, gives

$$
(\gamma+1)x^2+2n(\gamma-1)x+n^2(\gamma-1)-n=0.
$$

Its [discriminant](polynomial.md#discriminant) is $4n[(2n+1)-(2n-1)\gamma]$, so the same bound permits real regular slopes. The branch on which the [Mach number](#mach-number) rises inward selects the negative sign in

$$
x=\frac{-n(\gamma-1)\pm\sqrt{n[(2n+1)-(2n-1)\gamma]}}{\gamma+1}.
$$

For a spherical tube $n=2$, this recovers the $5/3$ threshold of [Bondi accretion](astrophysical-black-hole.md#bondi-accretion); for a [dipolar flux-tube area](magnetic-field.md#dipolar-flux-tube-area), $n=3$ gives $7/5$. The tube approximation must remain valid between the reservoir matching region and the accretor.

## Mach number

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mach_number)

The [Mach number](#mach-number) is the ratio of [fluid flow](fluid-mechanics.md#fluid-flow) speed to local [sound speed](#speed-of-sound).

More precisely, the [Mach number](#mach-number) is the [dimensionless quantity](physics.md#dimensionless-quantity)

$$
M=\frac{|\mathbf v_{\mathrm{body}}-\mathbf u_{\mathrm{gas}}|}{c}=\frac{U}{c},
$$

where $U$ is the magnitude of the body's [relative velocity](classical-mechanics.md#relative-velocity) through the surrounding [gas](thermodynamics.md#gas), and $c>0$ is the local [sound speed](#speed-of-sound) measured in the [gas](thermodynamics.md#gas) rest [reference frame](mathematical-physics.md#reference-frame). For a [fluid flow](fluid-mechanics.md#fluid-flow) past a stationary body, the same [Mach number](#mach-number) uses the local [fluid](fluid-mechanics.md#fluid) speed in the body's rest [reference frame](mathematical-physics.md#reference-frame). A [Mach number](#mach-number) below, equal to, or above one means [subsonic flow](#subsonic-flow), [sonic flow](#sonic-flow), or [supersonic flow](#supersonic-flow), respectively. The denominator is a property of the local [gas](thermodynamics.md#gas): its [sound speed](#speed-of-sound) depends on [temperature](temperature.md) and composition.[Mach Number, paragraphs defining the speed ratio and dependence on gas type and temperature; flight-regime list](physics-bibliography.md#mach-number-nasa-glenn-research-center)

The [relative velocity](classical-mechanics.md#relative-velocity) matters even when the body is at rest in a [wind tunnel](fluid-mechanics.md#wind-tunnel). A uniform change of [reference frame](mathematical-physics.md#reference-frame) subtracts the same [velocity](classical-mechanics.md#velocity) from body and [gas](thermodynamics.md#gas), so their [relative velocity](classical-mechanics.md#relative-velocity) and the [Mach number](#mach-number) stay unchanged under a [Galilean transformation](special-relativity.md#galilean-transformation). Ground speed alone cannot supply $U$ when there is wind. For an original collinear example, a body moving at $680\,\mathrm{m\,s^{-1}}$ over the ground through [gas](thermodynamics.md#gas) moving in the same direction at $170\,\mathrm{m\,s^{-1}}$ has $U=510\,\mathrm{m\,s^{-1}}$. With a stipulated [sound speed](#speed-of-sound) $c=340\,\mathrm{m\,s^{-1}}$, its [Mach number](#mach-number) is $1.5$, rather than $2$. A moving observer changes apparent [acoustic wave](fluid-mechanics.md#acoustic-wave) arrival times, as in the [radial Mach number](#radial-mach-number), without changing the body's [Mach number](#mach-number) relative to the [gas](thermodynamics.md#gas).

Why is the threshold one so useful? [Acoustic waves](fluid-mechanics.md#acoustic-wave) carry small [pressure](pressure.md) disturbances at the [sound speed](#speed-of-sound). In [subsonic flow](#subsonic-flow), such information can travel upstream relative to the body; in a uniform [supersonic flow](#supersonic-flow), it is swept downstream. The [Mach cone](#mach-cone) turns this difference in communication into visible geometry. Matching [Mach number](#mach-number) between a [wind tunnel](fluid-mechanics.md#wind-tunnel) and flight is therefore essential to matching [compressible flow](compressible-flow.md) effects.[Mach Number, paragraphs on downstream propagation and matching wind-tunnel and flight Mach numbers](physics-bibliography.md#mach-number-nasa-glenn-research-center)

An actual [supersonic wind tunnel](fluid-mechanics.md#supersonic-wind-tunnel) experiment makes the distinction between [wavefronts](physical-optics.md#wavefront) and [shock waves](transport-equation.md#shock-wave) concrete. In NASA Glenn's 1-by-1-foot [wind tunnel](fluid-mechanics.md#wind-tunnel), interchangeable converging-diverging [nozzle](fluid-mechanics.md#nozzle) blocks set the [Mach number](#mach-number). A strut-mounted exhaust-[nozzle](fluid-mechanics.md#nozzle) model had a nosecone, an air plenum and transparent sidewalls for [schlieren photography](geometrical-optics.md#schlieren-photography). Before installing the model, the researchers photographed the empty test section: two [shock wave](transport-equation.md#shock-wave) patterns originated at a wall joint after the [nozzle](fluid-mechanics.md#nozzle) block. This control guided model placement to keep reflected [shock waves](transport-equation.md#shock-wave) away from the plume-study region. The rig included internal [total pressure](fluid-mechanics.md#stagnation-pressure) and [static pressure](fluid-mechanics.md#static-pressure) sensing and a traversing external [static pressure](fluid-mechanics.md#static-pressure) probe. A baseline [nozzle](fluid-mechanics.md#nozzle) and previous [pressure](pressure.md) data supplied a planned validation comparison; the report distinguishes this plan from the observed empty-tunnel control. This establishes an apparatus origin for those visible [shock waves](transport-equation.md#shock-wave), not a measurement of the [Mach cone](#mach-cone) from an infinitesimal source. The reported finite [shock wave](transport-equation.md#shock-wave) angle cannot simply be inserted into the [Mach angle](#mach-angle) formula to calibrate $M$: [shock wave](transport-equation.md#shock-wave) strength and geometry also matter.[Wind Tunnel Model Design for the Study of Plume Effects on Sonic Boom for Isolated Exhaust Nozzles, NASA/TM-2010-216259, §II printed p. 2; §§IV–V printed pp. 8–9; Figs. 7–10 and concluding remarks printed p. 10](physics-bibliography.md#wind-tunnel-model-design-for-the-study-of-plume-effects-on-sonic-boom-for-isolated-exhaust-nozzles-by-raymond-s-castner)

In conventional [schlieren photography](geometrical-optics.md#schlieren-photography), a bright slit source and two concave mirrors send parallel [light rays](geometrical-optics.md#light-ray) through the [wind tunnel](fluid-mechanics.md#wind-tunnel) and focus them at a knife edge before an [optical camera](optical-instrument.md#optical-camera). Spatial changes in [mass density](fluid-mechanics.md#density) cause [refraction](optics.md#refraction); the knife edge converts the deflection into image contrast, making [shock waves](transport-equation.md#shock-wave) visible. This is the general optical principle, rather than a specification of every component in the preceding rig. A photograph projects a three-dimensional [fluid flow](fluid-mechanics.md#fluid-flow) into two dimensions; contrast alone does not provide a calibrated [pressure](pressure.md) jump or [acoustic wave](fluid-mechanics.md#acoustic-wave) amplitude.[Schlieren Flow Visualization, paragraphs describing the two-mirror slit-source and knife-edge system, density-gradient contrast, and two-dimensional recording of three-dimensional shocks](physics-bibliography.md#schlieren-flow-visualization-nasa-glenn-research-center)

### Moving-point acoustic wavefronts

↑ **Parent:** [Mach number](#mach-number)

Take a steady moving point source in uniform resting [gas](thermodynamics.md#gas), with constant [sound speed](#speed-of-sound) $c$ and source [velocity](classical-mechanics.md#velocity) $U\mathbf e_x$. Place the source at the origin at the current [time](classical-mechanics.md#time-in-physics) $t=0$. In the [linear acoustics](linear-acoustics.md) model, an emission at an earlier [time](classical-mechanics.md#time-in-physics) $\tau<0$ has a spherical [wavefront](physical-optics.md#wavefront) centered at $(U\tau,0,0)$ with radius $-c\tau$. An axial cross-section is the [circle](topology.md#circle) in the displayed equation. It is centered at the old release position, not the source's present position. The circles describe the geometry of weak [acoustic waves](fluid-mechanics.md#acoustic-wave), not a measured [shock wave](transport-equation.md#shock-wave) or its [pressure](pressure.md) jump.

For $M=0.5$, every old [circle](topology.md#circle) contains the present source because its center is $U|\tau|$ from the origin while its radius is the larger distance $c|\tau|$. It reaches ahead of the source. For $M=2$, the rightmost point of every old [circle](topology.md#circle) is $(U-c)\tau<0$: the source outruns all of its old [wavefronts](physical-optics.md#wavefront). The continuously emitted [wavefronts](physical-optics.md#wavefront) have a common [geometric envelope](geometry-and-topology.md#envelope-mathematics), the [Mach cone](#mach-cone). The plotted discrete release times sample this continuous family; rotating the axial section about the motion axis recovers the three-dimensional construction.

<a id="image-subsonic-and-supersonic-acoustic-wavefronts-from-a-moving-point"></a>
![](moving-source-acoustic-wavefronts.png)

**[Figure 1](#image-subsonic-and-supersonic-acoustic-wavefronts-from-a-moving-point). Subsonic and supersonic acoustic wavefronts from a moving point**. Original axial cross-sections at $t=0$ for [Mach numbers](#mach-number) $0.5$ and $2$. With an arbitrary positive [time](classical-mechanics.md#time-in-physics) scale $T$, the sampled release times are $\tau/T=-0.5,-1,\ldots,-3$. Each [circle](topology.md#circle) has center $(U\tau,0)$ and radius $-c\tau$; red lines give the [Mach cone](#mach-cone) section. This weak [linear acoustics](linear-acoustics.md) model predicts geometry, not measured [shock wave](transport-equation.md#shock-wave) or [sonic boom](fluid-mechanics.md#sonic-boom) strength.

### Radial Mach number

↑ **Parent:** [Mach number](#mach-number)

The radial [Mach number](#mach-number) is the source [velocity](classical-mechanics.md#velocity) projected toward the observer, divided by the [sound speed](#speed-of-sound). It enters the [moving-surface retarded Jacobian](linear-acoustics.md#moving-surface-retarded-jacobian) through $d|x-y(\tau)|/d\tau=-\widehat r\cdot v$. The sign is directional: a source moving toward the observer has positive $M_r$ and compressed arrival times.

### Subsonic flow

↑ **Parent:** [Mach number](#mach-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subsonic_flow)

A subsonic flow has [Mach number](#mach-number) less than one, so its speed is below the local [sound speed](#speed-of-sound).

For uniform [gas](thermodynamics.md#gas) moving at $U\mathbf e_x$ past a resting body, an upstream-directed [acoustic wave](fluid-mechanics.md#acoustic-wave) has body-frame [velocity](classical-mechanics.md#velocity) $(U-c)\mathbf e_x$. When $0\leq M<1$, this [velocity](classical-mechanics.md#velocity) points upstream. This is why the body can influence the upstream [fluid flow](fluid-mechanics.md#fluid-flow) through small [pressure](pressure.md) disturbances.

### Sonic flow

↑ **Parent:** [Mach number](#mach-number)

A [sonic flow](#sonic-flow) has [Mach number](#mach-number) exactly one: the local [fluid](fluid-mechanics.md#fluid) speed relative to the body equals the local [sound speed](#speed-of-sound). In uniform [gas](thermodynamics.md#gas) flowing at $U=c$ past a resting body, an upstream-directed [acoustic wave](fluid-mechanics.md#acoustic-wave) has zero body-frame [velocity](classical-mechanics.md#velocity). A [sonic point](#sonic-point) is a location where this equality holds. In the [moving-point acoustic wavefronts](#moving-point-acoustic-wavefronts) construction, old [spheres](euclidean-geometry.md#sphere) touch the source at the origin; the [Mach angle](#mach-angle) tends to $90^\circ$ as the [supersonic flow](#supersonic-flow) approaches this threshold.

### Supersonic flow

↑ **Parent:** [Mach number](#mach-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersonic_flow)

A supersonic flow has [Mach number](#mach-number) greater than one, so the flow speed exceeds the local [sound speed](#speed-of-sound).

For uniform [gas](thermodynamics.md#gas) moving at $U\mathbf e_x$ past a resting body, even an [acoustic wave](fluid-mechanics.md#acoustic-wave) directed against the [fluid flow](fluid-mechanics.md#fluid-flow) has body-frame [velocity](classical-mechanics.md#velocity) $(U-c)\mathbf e_x$ downstream. More generally, an [acoustic wave](fluid-mechanics.md#acoustic-wave) travelling along a [unit vector](vector-space.md#unit-vector) $\mathbf n$ has body-frame [velocity](classical-mechanics.md#velocity) $U\mathbf e_x+c\mathbf n$; its $x$ component is at least $U-c>0$. All such weak signals move downstream and their possible directions fit inside a [Mach cone](#mach-cone).

## Riemann invariant

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_invariant)

For one-dimensional homentropic ideal-gas flow,

$$
R_\pm=u\pm\frac{2(c-c_0)}{\gamma-1}
$$

is constant along the characteristic $dx/dt=u\pm c$.

### Riemann invariants for one-dimensional isentropic flow

↑ **Parent:** [Riemann invariant](#riemann-invariant)

For a barotropic pressure law with $c^2=dp/d\rho$, the invariants

$$
R_\pm=u\pm\int^\rho\frac{c(s)}s\,ds
$$

obey $[\partial_t+(u\pm c)\partial_x]R_\pm=0$.

#### Vacuum formation at an accelerating withdrawing piston

↑ **Parent:** [Riemann invariants for one-dimensional isentropic flow](#riemann-invariants-for-one-dimensional-isentropic-flow)

An initially resting perfect gas with adiabatic index $\gamma>1$ next to a piston $X(t)=-ft^2/2$ develops a smooth rarefaction. The incoming invariant gives $c_p=c_0-(\gamma-1)ft/2$. Pressure falls as $p_p=p_0(1-t/t_v)^{2\gamma/(\gamma-1)}$ until $t_v$, when the piston speed is $2c_0/(\gamma-1)$. Thereafter the gas edge moves at that limiting constant speed while the piston accelerates away, opening a vacuum gap.

### Simple wave

↑ **Parent:** [Riemann invariant](#riemann-invariant)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_wave)

A simple wave is a region of a hyperbolic flow in which one [Riemann invariant](#riemann-invariant) is constant throughout, leaving the other invariant to determine all fluid variables.

#### Area transformation of a nonlinear acoustic simple wave

↑ **Parent:** [Simple wave](#simple-wave)

For positive smooth tube area $A$, the equation $q_Z-qq_\theta+q(\log A)'/2=0$ becomes $Q_\zeta-QQ_\theta=0$ under the displayed transformation. Indeed, $g'/g=-A'/(2A)$ cancels geometrical spreading and $\zeta'=g$ makes the remaining nonlinear and transport coefficients equal. Starting with $q(\theta,Z_0)=f(\theta)$ gives $Q=f(\xi)$ and $\theta=\xi-f(\xi)\zeta$; [characteristic crossing](transport-equation.md#characteristic-crossing) first occurs when $\zeta\sup f'=1$, if that supremum is positive.

##### Shock distance for a spherical simple wave launched at finite radius

↑ **Parent:** [Area transformation of a nonlinear acoustic simple wave](#area-transformation-of-a-nonlinear-acoustic-simple-wave)

For area $A(R)=R^2$ and smooth data $q(\theta,R_0)=f(\theta)$ at $R_0>0$, the transformed distance is $\zeta=R_0\log(R/R_0)$. If $M=\sup f'>0$, the first [shock wave](transport-equation.md#shock-wave) occurs at the displayed radius; if $M\leq0$, there is no forward characteristic crossing. Nontrivial bounded data cannot instead be imposed at $R=0$ in this outgoing simple-wave model: along every characteristic, $Rq$ is constant, so a bounded limit at the origin forces that constant to vanish. With distance measured from a finite emitting surface, use $A(Z)=(R_0+Z)^2$ and subtract $R_0$ from the shock radius.

#### Linearly degenerate characteristic field

↑ **Parent:** [Simple wave](#simple-wave)

A characteristic field is linearly degenerate if the directional derivative of its speed along its right [eigenvector](linear-operator-theory.md#eigenvector) vanishes. Its simple waves have constant propagation speed along the state curve, so they do not steepen by amplitude-dependent transport.

#### Simple wave in magnetohydrodynamics

↑ **Parent:** [Simple wave](#simple-wave)

An ideal-MHD simple wave traces a one-parameter state-space curve whose tangent is a right [eigenvector](linear-operator-theory.md#eigenvector) of the characteristic matrix. Its parameter obeys $q_t+v(q)q_x=0$ and its characteristic speed obeys the [Inviscid Burgers equation](transport-equation.md#inviscid-burgers-equation). [Nonlinear Alfvén waves](ideal-magnetohydrodynamics.md#nonlinear-alfven-wave) are a linearly degenerate example.

##### Perpendicular fast magnetosonic simple wave

↑ **Parent:** [Simple wave in magnetohydrodynamics](#simple-wave-in-magnetohydrodynamics)

For a one-dimensional [velocity](classical-mechanics.md#velocity) perpendicular to a transverse [magnetic field](magnetic-field.md), $c_f^2=\gamma p/\rho+B^2/(\mu_0\rho)$. The primitive-variable characteristic matrix has two advective [eigenvalues](linear-operator-theory.md#eigenvalue) and the two speeds $u\pm c_f$. Integrating the fast [eigenvectors](linear-operator-theory.md#eigenvector) keeps $p/\rho^\gamma$ and $B/\rho$ constant. The state parameter obeys $\rho_t+(u\pm c_f)\rho_x=0$, so the [characteristic speed](transport-equation.md#characteristic-speed) satisfies the [Inviscid Burgers equation](transport-equation.md#inviscid-burgers-equation).

###### Isothermal perpendicular magnetosonic simple wave

↑ **Parent:** [Perpendicular fast magnetosonic simple wave](#perpendicular-fast-magnetosonic-simple-wave)

With $B_x=0$, a fast [simple wave in magnetohydrodynamics](#simple-wave-in-magnetohydrodynamics) has constant $u_y$ and $B_y/\rho=K$. Its longitudinal velocity satisfies $du_x/d\rho=\pm c_f/\rho$, and $\rho_t+(u_x\pm c_f)\rho_x=0$. Along this state curve the speed derivative is $\pm[c_f/\rho+K^2/(2\mu_0c_f)]$, which is nonzero. Compressive profiles therefore exhibit [shock formation by characteristic intersection](#shock-formation-by-characteristic-intersection), unlike a [linearly degenerate characteristic field](#linearly-degenerate-characteristic-field).

#### Damping threshold for a simple wave

↑ **Parent:** [Simple wave](#simple-wave)

For $u_t+(c_0+bu)u_x=-\alpha u$, $b,\alpha>0$, the [characteristic curves](transport-equation.md#characteristic-curve) are $u=e^{-\alpha t}u_0(\xi)$ and $x=c_0t+\xi+(b/\alpha)(1-e^{-\alpha t})u_0(\xi)$. If $m=\max[-u_0']>0$, finite-time [gradient blow-up](transport-equation.md#gradient-blow-up) occurs precisely for $\alpha<bm$, at $t_s=-\alpha^{-1}\log(1-\alpha/(bm))$. Equality $\alpha=bm$ still gives a positive Jacobian at each finite time; only the limiting map degenerates.

#### Receding-piston rarefaction wave

↑ **Parent:** [Simple wave](#simple-wave)

For a piston receding from initially stationary homentropic gas, the right-moving [simple wave](#simple-wave) has $R_-=0$, so $c=c_0+(\gamma-1)u/2$. A $C_+$ characteristic emitted by the piston at time $s$ carries $u=\dot X_p(s)$ and is the straight line

$$
x=X_p(s)+\left[c_0+\frac{\gamma+1}{2}\dot X_p(s)\right](t-s).
$$

##### Vacuum formation behind a receding piston

↑ **Parent:** [Receding-piston rarefaction wave](#receding-piston-rarefaction-wave)

The gas state at a receding piston reaches vacuum when $\dot X_p=-2c_0/(\gamma-1)$, because then the [sound speed](#speed-of-sound) and [mass density](fluid-mechanics.md#density) both vanish. If the piston subsequently recedes faster, a vacuum gap opens between it and the gas boundary, which continues with velocity $-2c_0/(\gamma-1)$.

##### Singular small-power piston emission time

↑ **Parent:** [Receding-piston rarefaction wave](#receding-piston-rarefaction-wave)

For $X_p(t)=-t^{1+\alpha}/(1+\alpha)$ with $0<\alpha\ll1$, a point on the ray $x=(c_0-a)t$, $0<a<(\gamma+1)/2$, receives the characteristic emitted at the exponentially small time

$$
s\sim\left(\frac{2a}{\gamma+1}\right)^{1/\alpha}.
$$

Although $s\to0$, the piston speed $-s^\alpha$ has the finite limit $-2a/(\gamma+1)$, producing the centered-rarefaction profile of the singular limit $\alpha=0$.

### Pressure in a perfect-gas simple wave

↑ **Parent:** [Riemann invariant](#riemann-invariant)

In a right-moving simple wave entering gas initially at rest with sound speed $c_0$, the other Riemann invariant is constant, so

$$
c=c_0+\frac{\gamma-1}{2}u.
$$

The isentropic relation

$$
\frac p{p_0}=\left(\frac c{c_0}\right)^{2\gamma/(\gamma-1)}
$$

converts the velocity disturbance into its nonlinear pressure disturbance.

### Shock formation by characteristic intersection

↑ **Parent:** [Riemann invariant](#riemann-invariant)

A smooth compressive simple wave forms a shock when characteristics first intersect. If characteristics are parametrized by their emission time $\tau$, the first shock occurs at the minimum positive time for which $\partial x(\tau,t)/\partial\tau=0$.

## Normal shock wave

↑ **Parent:** [Compressible flow](compressible-flow.md)

A normal shock is a discontinuity perpendicular to the flow direction across which mass, momentum, and total energy fluxes are conserved.

Property ratios for this discontinuity are tabulated in [normal shock tables](#normal-shock-tables).

### Shock tube

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

A tube in which releasing an initial [pressure](pressure.md) difference produces a shock, often accompanied by an expansion wave and a contact surface. Spatially separated [pressure](pressure.md) probes can measure shock arrival speed and jump size. The shock and the contact surface must be identified separately when interpreting the downstream state.

### Normal shock reflection at a rigid wall

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

For a perfect-gas [normal shock wave](#normal-shock-wave) reflected from a stationary rigid wall, apply the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) using signed [velocity](classical-mechanics.md#velocity) in each [shock frame](#shock-frame). The once-shocked state is the common left state for both applications. Its two relative speeds are roots of $v^2-(\gamma+1)u_sv/2-\gamma p_s/\rho_s=0$. Their product and the [pressure](pressure.md) jump eliminate the [velocity](classical-mechanics.md#velocity), giving the displayed relation. A strong incident [shock wave](transport-equation.md#shock-wave) gives $p_1/p_s\to(3\gamma-1)/(\gamma-1)$.

### Moving-interface conservation jump identity

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

For a moving level surface, $n=\nabla S/|\nabla S|$, $v_n=-S_t/|\nabla S|$, and the [surface delta distribution](distribution-theory.md#surface-delta-distribution) is $\delta_s=|\nabla S|\delta(S)$. Piecewise classical conservation laws acquire a distributional flux defect $[b]\cdot n-v_n[a]$. Vanishing of this defect is the [Rankine-Hugoniot condition](transport-equation.md#rankine-hugoniot-conditions).

### Normal shock tables

↑ **Parent:** [Normal shock wave](#normal-shock-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_shock_tables)

Normal shock tables tabulate upstream-to-downstream property ratios for a [normal shock wave](#normal-shock-wave), typically as functions of upstream [Mach number](#mach-number) and [heat capacity ratio](ideal-gas.md#heat-capacity-ratio). They encode the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) rather than defining the discontinuity itself.

### Shock frame

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

The shock frame is an inertial reference frame in which the shock is stationary. A travelling shock then becomes a steady flow through a fixed discontinuity.

### Rankine-Hugoniot conditions for a perfect gas

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

In the rest frame of a one-dimensional shock, states with velocities $w_0,w_1$ satisfy

$$
\rho_0w_0=\rho_1w_1,
$$



$$
p_0+\rho_0w_0^2=p_1+\rho_1w_1^2,
$$

and

$$
\frac{\gamma p_0}{(\gamma-1)\rho_0}+\frac12w_0^2
=\frac{\gamma p_1}{(\gamma-1)\rho_1}+\frac12w_1^2.
$$

These are the [Rankine-Hugoniot conditions](transport-equation.md#rankine-hugoniot-conditions) specialized to the mass, momentum and energy fluxes of a [perfect gas](ideal-gas.md).

#### Prandtl shock relation

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

For a stationary normal shock in a polytropic perfect gas, the upstream and downstream normal speeds obey $u_1u_2=c_{\rm cr}^2$, where $c_{\rm cr}$ is the sonic speed on their common Bernoulli streamline.

#### Strong-shock Rankine-Hugoniot conditions

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

When the upstream pressure is negligible, a perfect-gas shock has density ratio $(\gamma+1)/(\gamma-1)$. For $\gamma=5/3$, the downstream density is four times the upstream density.

##### Energy fluxes of a strong adiabatic shock

↑ **Parent:** [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions)

In the rest frame of a strong planar [shock wave](transport-equation.md#shock-wave), a perfect gas has $\rho_2/\rho_1=(\gamma+1)/(\gamma-1)$, $u_2/u_1=(\gamma-1)/(\gamma+1)$ and $p_2=2\rho_1u_1^2/(\gamma+1)$. Its downstream [specific internal energy](internal-energy.md#specific-internal-energy) is $\epsilon_2=p_2/[(\gamma-1)\rho_2]=2u_1^2/(\gamma+1)^2$. Multiplying by mass flux $j=\rho_1u_1$ gives the internal-energy flux in the title. The lost bulk [kinetic energy](energy.md#kinetic-energy) flux instead equals $j(u_1^2-u_2^2)/2=\gamma F_{\rm int}$: this includes downstream pressure work and is the increase of [specific enthalpy](enthalpy.md#specific-enthalpy) flux in the cold-upstream limit. Neither quantity is a temperature change per unit time of a fixed target mass without further information about that target.

##### Shock compression ratio

↑ **Parent:** [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions)

The shock compression ratio is the downstream-to-upstream density ratio. For a strong perfect-gas shock,

$$
\chi=\frac{\rho_1}{\rho_0}=\frac{\gamma+1}{\gamma-1}.
$$

In the upstream rest frame, the downstream velocity is $2V_s/(\gamma+1)$ and its pressure is $2\rho_0V_s^2/(\gamma+1)$.

###### Planar shock compression of a finite slab

↑ **Parent:** [Shock compression ratio](#shock-compression-ratio)

A plane shock moving at speed $V_s$ through initially stationary gas has upstream speed $u_1=V_s$ and downstream speed $u_2=V_s/\chi$ in the [shock frame](#shock-frame), where $\chi$ is the [shock compression ratio](#shock-compression-ratio). Transforming back to the initial slab frame gives $v_2=V_s-u_2$. At the breakout time $L/V_s$, a uniform downstream slab has thickness $L-v_2L/V_s=L/\chi$. The strong monatomic limit has $\chi=4$, hence $L_2=L/4$ and $v_2=3V_s/4$. This uses a maintained planar post-shock state; boundary rarefactions and variations of shock speed can change the actual thickness of a freely evolving finite cloud.

###### Mach-number convention in shock unbinding estimates

↑ **Parent:** [Planar shock compression of a finite slab](#planar-shock-compression-of-a-finite-slab)

For a strong monatomic shock, the [planar shock compression of a finite slab](#planar-shock-compression-of-a-finite-slab) gives bulk speed $3V_s/4$ and kinetic energy $E_{\rm bulk}=9M_cV_s^2/32$. The initial [internal energy](internal-energy.md) is $E_{\rm th}=3M_cp/(2\rho)$. A bulk-ballistic escape estimate $E_{\rm bulk}\gtrsim W$ uses positive binding-energy magnitude $W$, not negative gravitational potential energy. With [adiabatic sound speed](#adiabatic-sound-speed) $c_{\rm ad}^2=5p/(3\rho)$ it yields the first displayed coefficient. Using the [isothermal sound speed](#isothermal-sound-speed) $c_T^2=p/\rho$ instead yields $16/3\simeq5.3$. The definitions obey $\mathcal M_T^2=(5/3)\mathcal M_{\rm ad}^2$. Heating, subsequent expansion and energy loss can alter the physical escape threshold, so the coefficient is not independent of the energy budget and Mach convention.

#### Piston-driven normal shock

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

If a piston moves at speed $V$ into stationary perfect gas and drives a shock at speed $U$, then the shock-frame upstream and downstream speeds are $U$ and $U-V$. If $p_2-p_1=\beta p_1$, the jump conditions give

$$
V^2=
\frac{2\beta^2}{2\gamma+(\gamma+1)\beta}
\frac{p_1}{\rho_1},
\qquad
\frac{U^2}{c_1^2}
=1+\frac{\gamma+1}{2\gamma}\beta.
$$

##### Piston-driven shock with specific-heat ratio three

↑ **Parent:** [Piston-driven normal shock](#piston-driven-normal-shock)

If a shock travels into stationary gas at speed $V$ while the downstream piston and gas travel at $V/3$, then for $\gamma=3$,

$$
\frac{\rho_1}{\rho_0}=\frac32,
\qquad
\frac{p_1}{p_0}=4,
\qquad
V=3\sqrt{\frac{p_0}{\rho_0}}.
$$

#### Pressure-density Hugoniot relation for a perfect gas

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

Let $P=p_2/p_1$ and $D=\rho_2/\rho_1$ be the [pressure](pressure.md) and [mass density](fluid-mechanics.md#density) ratios across a [normal shock wave](#normal-shock-wave) in a [perfect gas](ideal-gas.md) with [specific-heat ratio](ideal-gas.md#heat-capacity-ratio) $\gamma$. Eliminating the velocities from the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) gives

$$
\frac{\gamma}{\gamma-1}(p_2/\rho_2-p_1/\rho_1)
=\frac12(p_2-p_1)(1/\rho_1+1/\rho_2),
\qquad
D=\frac{(\gamma+1)P+\gamma-1}{(\gamma-1)P+\gamma+1}.
$$

As $P\to\infty$, the ratio tends to the [shock compression ratio](#shock-compression-ratio) $(\gamma+1)/(\gamma-1)$.

##### Entropy production in a perfect-gas shock

↑ **Parent:** [Pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas)

For the [pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas), the change in [specific entropy](entropy.md#specific-entropy) is $[s]/c_v=\log P-\gamma\log D(P)$, with $c_v$ the [specific heat capacity](heat.md#specific-heat-capacity) at constant volume. Its derivative is

$$
\frac{d([s]/c_v)}{dP}
=\frac{(\gamma^2-1)(P-1)^2}{P[(\gamma+1)P+\gamma-1][(\gamma-1)P+\gamma+1]}.
$$

It is positive for a compressive [normal shock wave](#normal-shock-wave) with $P>1$. For a [weak shock](#weak-shock) with $P=1+\delta$, integrating the leading term gives

$$
\frac{[s]}{c_v}=\frac{\gamma^2-1}{12\gamma^2}\delta^3+O(\delta^4).
$$

Thus the [entropy production](stochastic-thermodynamics.md#entropy-production) is cubic in the small [pressure](pressure.md) jump, even though the [mass density](fluid-mechanics.md#density) and [temperature](temperature.md) changes already appear at first order.

###### Entropy production in successive weak shocks

↑ **Parent:** [Entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock)

For $N$ equal [weak shocks](#weak-shock) with individual [pressure](pressure.md) ratio $1+\delta$ and total ratio $P_s=(1+\delta)^N$, [entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock) gives

$$
\frac{\Delta s}{c_v}
=\frac{\gamma^2-1}{12\gamma^2}\delta^2\log P_s\,[1+O(\delta)].
$$

At fixed $P_s>1$, this tends to zero as the compression is divided into increasingly many smaller [weak shocks](#weak-shock). A single finite [normal shock wave](#normal-shock-wave) instead gives the positive value $\log P_s-\gamma\log D(P_s)$. Gradual compression can consequently approach reversible [isentropic flow](#isentropic-flow) while an abrupt compression generates finite [entropy](entropy.md).

### Weak shock

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

A weak shock has a small relative pressure jump. Its density jump agrees with the reversible adiabatic prediction through second order in the pressure jump, while entropy production first appears at third order.

### Oblique shock

↑ **Parent:** [Normal shock wave](#normal-shock-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oblique_shock)

An oblique shock is inclined relative to the upstream velocity. In an inviscid perfect gas, the normal velocity satisfies the normal-shock jump conditions while the tangential velocity is continuous.

#### Strong oblique-shock angle branches

↑ **Parent:** [Oblique shock](#oblique-shock)

Measure shock angle $\beta$ from the incident flow to the shock front, and deflection $\theta$ towards it. The strong normal-compression ratio and continuity of tangential [velocity](classical-mechanics.md#velocity) give $\tan\beta=[(\gamma+1)/(\gamma-1)]\tan(\beta-\theta)$. Angle-addition identities reduce this to $\sin(2\beta-\theta)=\gamma\sin\theta$. The two title branches exist for $0<\theta<\arcsin(1/\gamma)$ and merge at $\beta=\pi/4+\theta/2$. As $\theta\to0$, their formal limits are $(\gamma+1)\theta/2$ and $\pi/2-(\gamma-1)\theta/2$. The weak-branch expansion requires $M\sin\beta\gg1$; at finite [Mach number](#mach-number) its true zero-deflection limit is the [Mach angle](#mach-angle).

#### Shock polar

↑ **Parent:** [Oblique shock](#oblique-shock)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shock_polar)

A [shock polar](#shock-polar) is the locus of possible downstream [velocity](classical-mechanics.md#velocity) vectors, or an equivalent [pressure](pressure.md)/deflection relation, as the orientation of an [oblique shock](#oblique-shock) varies for fixed upstream conditions. [Entropy](entropy.md) admissibility selects physical compressive shocks. The strong-shock perfect-gas [velocity](classical-mechanics.md#velocity) polar is a circle, while finite-Mach polars have a different shape.

##### Strong-shock polar for a perfect gas

↑ **Parent:** [Shock polar](#shock-polar)

The normal [velocity](classical-mechanics.md#velocity) is reduced by $q$ in the strong-shock limit while tangential [velocity](classical-mechanics.md#velocity) is unchanged. If the upstream speed is $U$ and the shock normal makes angle $\beta$ with its direction, then $u_X=U[1-(1-q)\cos^2\beta]$ and $u_Y=\pm U(1-q)\cos\beta\sin\beta$. Eliminating the angle gives the displayed circle, centered at $\gamma U/(\gamma+1)$ with radius $U/(\gamma+1)$. It is the limiting [shock polar](#shock-polar) in downstream [velocity](classical-mechanics.md#velocity) space.

###### Maximum deflection through a strong perfect-gas shock

↑ **Parent:** [Strong-shock polar for a perfect gas](#strong-shock-polar-for-a-perfect-gas)

For the circle with center distance $a=\gamma U/(\gamma+1)$ and radius $R=U/(\gamma+1)$, the most deflected ray from the origin is tangent. The right triangle formed by the origin, center and tangency point gives $\sin\delta_{\max}=R/a=1/\gamma$. This is a velocity-vector deflection angle, not the angle of the shock normal.

#### Weak-oblique-shock deflection

↑ **Parent:** [Oblique shock](#oblique-shock)

If $p_2/p_1=1+\epsilon$ with $0<\epsilon\ll1$ and the upstream Mach number is $M_1>1$, the shock angle is the Mach angle to leading order and the flow deflection is

$$
\theta\simeq\frac{\epsilon}{\gamma}
\frac{\sqrt{M_1^2-1}}{M_1^2}.
$$

The normal speed decreases, so the downstream flow turns toward the shock front.

#### Mach angle

↑ **Parent:** [Oblique shock](#oblique-shock)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mach_angle)

The [Mach angle](#mach-angle) of a [supersonic flow](#supersonic-flow) with [Mach number](#mach-number) $M>1$ is $\mu=\arcsin(M^{-1})$. Infinitesimal [pressure](pressure.md) disturbances lie on the corresponding [Mach cone](#mach-cone), and a weak [oblique shock](#oblique-shock) approaches this angle as its strength tends to zero.

The [Mach angle](#mach-angle) is the half-angle between a [Mach cone](#mach-cone) generator and its backward motion axis for a steady point source in a uniform three-dimensional medium with [isotropy](continuum-mechanics.md#isotropy) and constant [sound speed](#speed-of-sound). It obeys

$$
\sin\mu=\frac{c}{U}=\frac{1}{M},\qquad 0<\mu<\frac{\pi}{2},\quad M>1.
$$

The relation concerns weak [acoustic waves](fluid-mechanics.md#acoustic-wave) in [linear acoustics](linear-acoustics.md). It is not the angle of a finite [oblique shock](#oblique-shock) produced by finite turning of the [fluid flow](fluid-mechanics.md#fluid-flow); that angle also depends on the deflection and the [gas](thermodynamics.md#gas) properties.[Mach Angle, geometric construction and displayed sin(mu)=1/M and mu=asin(1/M) equations](physics-bibliography.md#mach-angle-nasa-glenn-research-center)

For a short proof, choose an old emission in the [moving-point acoustic wavefronts](#moving-point-acoustic-wavefronts) construction and set $s=-\tau>0$. Its [circle](topology.md#circle) has center $(-Us,0)$ and radius $cs$. A [tangent line](calculus.md#tangent-line) from the present source at the origin meets the [circle](topology.md#circle) at a [right angle](euclidean-geometry.md#right-angle) to its radius. The resulting [right triangle](euclidean-geometry.md#right-triangle) has hypotenuse $Us$ and opposite side $cs$, giving the displayed [sine](geometry-and-topology.md#sine) ratio. The emission age cancels: every [wavefront](physical-optics.md#wavefront) has the same tangent directions, so a continuum of expanding [spheres](euclidean-geometry.md#sphere) produces one simple [Mach cone](#mach-cone).

In an original example, stipulate uniform [gas](thermodynamics.md#gas) with [sound speed](#speed-of-sound) $c=340\,\mathrm{m\,s^{-1}}$ and a source moving through it at $U=680\,\mathrm{m\,s^{-1}}$. Then $M=2$ and $\mu=\arcsin(1/2)=30^\circ$. An emission one second earlier is now a [sphere](euclidean-geometry.md#sphere) centered $680\,\mathrm m$ behind the source with radius $340\,\mathrm m$. The selected [sound speed](#speed-of-sound) defines this example; it is not a constant for air at every [temperature](temperature.md). The [Mach angle](#mach-angle) decreases as $M$ increases: its [derivative](calculus.md#derivative) is $-1/(M\sqrt{M^2-1})$ in [radians](geometry-and-topology.md#radian), and its [limits](calculus.md#limit-of-a-function) are $90^\circ$ as $M\downarrow1$ and $0$ as $M\to\infty$.

<a id="image-mach-half-angle-decreases-as-the-gas-relative-speed-ratio-increases"></a>
![](mach-angle-versus-speed-ratio.png)

**[Figure 2](#image-mach-half-angle-decreases-as-the-gas-relative-speed-ratio-increases). Mach half-angle decreases as the gas-relative speed ratio increases**. Original plot of the [Mach angle](#mach-angle) $\mu=\arcsin(1/M)$ for $M>1$, with the constructed $M=2$, $\mu=30^\circ$ example. The open point at $M=1$ marks a [limit](calculus.md#limit-of-a-function), not a finite [supersonic](#supersonic-flow) cone. This weak-wave prediction gives neither a finite-deflection [oblique shock](#oblique-shock) angle nor measured [sonic boom](fluid-mechanics.md#sonic-boom) strength.

##### Mach cone

↑ **Parent:** [Mach angle](#mach-angle)

The [Mach cone](#mach-cone) forms the [geometric envelope](geometry-and-topology.md#envelope-mathematics) of [acoustic wave](fluid-mechanics.md#acoustic-wave) [wavefronts](physical-optics.md#wavefront) from a source moving at a [supersonic](#supersonic-flow) [Mach number](#mach-number) $M>1$. In the source [reference frame](mathematical-physics.md#reference-frame) the ray-[velocity](classical-mechanics.md#velocity) [sphere](euclidean-geometry.md#sphere) is centered at $-Mc_0\mathbf e_x$ and has radius $c_0$. Its tangent rays make [angle](geometry-and-topology.md#angle) $\sin^{-1}(1/M)$ to the backward flight direction; all other emitted acoustic rays lie inside that [Mach cone](#mach-cone).

The [Mach cone](#mach-cone) is the [geometric envelope](geometry-and-topology.md#envelope-mathematics) of the [spheres](euclidean-geometry.md#sphere) in [moving-point acoustic wavefronts](#moving-point-acoustic-wavefronts). To obtain its axial boundary without a diagram, put $s=-\tau>0$ and impose the [geometric envelope](geometry-and-topology.md#envelope-mathematics) conditions $F=0$ and $\partial_sF=0$ on

$$
F(x,y,s)=(x+Us)^2+y^2-c^2s^2.
$$

The [partial derivative](multivariable-calculus.md#partial-derivative) condition gives $x=-(U^2-c^2)s/U$. Substituting into $F=0$ gives $y^2=c^2(U^2-c^2)s^2/U^2$, hence

$$
y=\pm\frac{-x}{\sqrt{M^2-1}},\quad x<0,
\qquad
\sqrt{y^2+z^2}=\frac{-x}{\sqrt{M^2-1}}quad\text{in three dimensions}.
$$

For $M=2$, the [Mach cone](#mach-cone) section has slope magnitude $1/\sqrt3$, consistent with a [Mach angle](#mach-angle) of $30^\circ$. If emission begins at a finite [time](classical-mechanics.md#time-in-physics), the reached region is limited by the oldest [wavefront](physical-optics.md#wavefront); the infinite cone describes the steady geometric boundary obtained with an indefinitely long source history. In a uniformly moving [gas](thermodynamics.md#gas), [advection](fluid-mechanics.md#advection) shifts each emission's [sphere](euclidean-geometry.md#sphere) by the gas [velocity](classical-mechanics.md#velocity) times its age; working with the source's [relative velocity](classical-mechanics.md#relative-velocity) through the [gas](thermodynamics.md#gas) restores the same construction.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (14)

- [de Laval nozzle](fluid-mechanics.md#de-laval-nozzle)
- [Dynamic pressure](lift-force.md#dynamic-pressure)
- [Mach number](#mach-number)
- [Nozzle](fluid-mechanics.md#nozzle)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#38a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-314.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-314.md#2/a/solution)
- [Rankine-Hugoniot conditions](transport-equation.md#rankine-hugoniot-conditions)
- [Riemann problem](transport-equation.md#riemann-problem)
- [Self-similar ideal-gas rarefaction](transport-equation.md#self-similar-ideal-gas-rarefaction)
- [Spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow)
- [Stagnation pressure](fluid-mechanics.md#stagnation-pressure)
- [Transonic flow](#transonic-flow)
- [Viscous stress tensor](dynamic-viscosity.md#viscous-stress-tensor)
