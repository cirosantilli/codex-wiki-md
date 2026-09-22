# Compressible flow

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compressible_flow)

Compressible flow allows density to change materially and is required for finite-amplitude pressure waves and shocks.

**Table of contents**

- [Self-similar blast wave](#self-similar-blast-wave)
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
  - [Radial Mach number](#radial-mach-number)
  - [Subsonic flow](#subsonic-flow)
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
  - [Normal shock reflection at a rigid wall](#normal-shock-reflection-at-a-rigid-wall)
  - [Moving-interface conservation jump identity](#moving-interface-conservation-jump-identity)
  - [Normal shock tables](#normal-shock-tables)
  - [Shock frame](#shock-frame)
  - [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)
    - [Prandtl shock relation](#prandtl-shock-relation)
    - [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions)
      - [Shock compression ratio](#shock-compression-ratio)
    - [Piston-driven normal shock](#piston-driven-normal-shock)
      - [Piston-driven shock with specific-heat ratio three](#piston-driven-shock-with-specific-heat-ratio-three)
    - [Pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas)
      - [Entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock)
        - [Entropy production in successive weak shocks](#entropy-production-in-successive-weak-shocks)
  - [Weak shock](#weak-shock)
  - [Oblique shock](#oblique-shock)
    - [Shock polar](#shock-polar)
      - [Strong-shock polar for a perfect gas](#strong-shock-polar-for-a-perfect-gas)
        - [Maximum deflection through a strong perfect-gas shock](#maximum-deflection-through-a-strong-perfect-gas-shock)
    - [Weak-oblique-shock deflection](#weak-oblique-shock-deflection)
    - [Mach angle](#mach-angle)
      - [Mach cone](#mach-cone)

## Self-similar blast wave

↑ **Parent:** [Compressible flow](compressible-flow.md)

A [self-similar blast wave](#self-similar-blast-wave) is an expanding [shock wave](partial-differential-equation.md#shock-wave) whose post-shock profiles retain their shape in a rescaled radius or distance. A fixed explosion energy, ambient [mass density](fluid-mechanics.md#density) and geometry set the front scaling through conservation of total energy. The dimensionless coefficient requires the profiles and an energy-normalization convention.

### Thin-shell approximation for a spherical blast wave

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

Let a strong [shock wave](partial-differential-equation.md#shock-wave) of radius $R$ and speed $V$ sweep a uniform [mass density](fluid-mechanics.md#density) $\rho_0$ into a shell of mass $4\pi\rho_0R^3/3$ and speed $2V/(\gamma+1)$. If the cavity [pressure](thermodynamics.md#pressure) is $\alpha$ times the immediate post-shock [pressure](thermodynamics.md#pressure), shell [momentum](classical-mechanics.md#momentum) balance gives $R\dot V=3(\alpha-1)V^2$. Constant total [energy](classical-mechanics.md#energy) gives $R^3V^2=\mathrm{constant}$ and hence $\alpha=1/2$. Including shell internal and kinetic [energy](classical-mechanics.md#energy), and treating the cavity volume as $4\pi R^3/3$ to thin-shell accuracy, yields $R=\xi(E/\rho_0)^{1/5}t^{2/5}$ with $\xi^5=75(\gamma-1)(\gamma+1)^2/[16\pi(5\gamma-3)]$. This coefficient is approximate; resolving the shell's finite volume changes it.

### Spherical blast wave in a power-law ambient density

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

For an [energy](classical-mechanics.md#energy)-conserving strong spherical [shock wave](partial-differential-equation.md#shock-wave) expanding into [mass density](fluid-mechanics.md#density) $Cr^{-\beta}$, $0\leq\beta<3$, [dimensional analysis](physics.md#dimensional-analysis) gives the displayed radius law. Neglect ambient [pressure](thermodynamics.md#pressure), radiation losses and gravity in this blast-dominated approximation. Write $u=\dot R U(\xi)$, $\rho=CR^{-\beta}D(\xi)$ and $p=CR^{-\beta}\dot R^2P(\xi)$, with $\xi=r/R$. The radial [continuity equation](physics.md#continuity-equation), momentum equation and adiabatic [pressure](thermodynamics.md#pressure) equation reduce to

$$
(U-\xi)D'+D(U'+2U/\xi-\beta)=0,\qquad
(U-\xi)U'+\frac{\beta-3}{2}U=-P'/D,
$$



$$
(U-\xi)P'+[\gamma(U'+2U/\xi)-3]P=0.
$$

The [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions) give $U(1)=P(1)=2/(\gamma+1)$ and $D(1)=(\gamma+1)/(\gamma-1)$. The explosion [energy](classical-mechanics.md#energy) fixes the radius coefficient through $E=4\pi CR^{3-\beta}\dot R^2\int_0^1[DU^2/2+P/(\gamma-1)]\xi^2d\xi$.

#### Linear-profile spherical blast wave

↑ **Parent:** [Spherical blast wave in a power-law ambient density](#spherical-blast-wave-in-a-power-law-ambient-density)

The [similarity profiles](partial-differential-equation.md#similarity-profile) $U=2\xi/(\gamma+1)$, $D=(\gamma+1)\xi/(\gamma-1)$ and $P=2\xi^3/(\gamma+1)$ solve the spherical blast equations at the displayed ambient exponent. For $\gamma=5/3$, $\beta=2$ and $R^3=3Et^2/(2\pi C)$. The dimensional fields are $u=r/(2t)$, $\rho=8\pi C^2r/(3Et^2)$ and $p=2\pi C^2r^3/(9Et^4)$ for $0<r<R$. Their kinetic and internal [energies](classical-mechanics.md#energy) are equal. Substituting these profiles into all three equations and the shock conditions verifies the solution.

### Planar blast-wave energy scaling

↑ **Parent:** [Self-similar blast wave](#self-similar-blast-wave)

For a planar adiabatic explosion with energy per unit area $E$ in a uniform medium of [mass density](fluid-mechanics.md#density) $\rho_0$, the conserved energy has form $E=I\rho_0Z\dot Z^2$, with a finite positive integral $I$ of the [similarity profiles](partial-differential-equation.md#similarity-profile). Hence $Z=C(E/\rho_0)^{1/3}t^{2/3}$. If $E$ is shared by two fronts, its fraction assigned to either side is absorbed into $C$.

## Polytropic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A polytropic flow uses a [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state). When $K$ and the [adiabatic exponent](thermodynamics.md#heat-capacity-ratio) are constant, a smooth streamline has [specific enthalpy](thermodynamics.md#specific-enthalpy) $h=\gamma K\rho^{\gamma-1}/(\gamma-1)$ and [adiabatic sound speed](#adiabatic-sound-speed) $c_s^2=\gamma K\rho^{\gamma-1}$. Spatially varying entropy can make $K$ depend on streamline; the constant-$K$ spherical wind is a special case.

## Spherically symmetric adiabatic flow

↑ **Parent:** [Compressible flow](compressible-flow.md)

A smooth radial [compressible flow](compressible-flow.md) with a fixed [adiabatic exponent](thermodynamics.md#heat-capacity-ratio) conserves $r^2\rho u$ and $p/\rho^\gamma$. In a prescribed [Newtonian gravitational potential](classical-mechanics.md#newtonian-gravitational-potential), its [Bernoulli function](fluid-mechanics.md#bernoulli-function) is $u^2/2+c^2/(\gamma-1)+\Phi$, with $c$ the [adiabatic sound speed](#adiabatic-sound-speed). Eliminating the density derivative yields $(u-c^2/u)u'=2c^2/r-\Phi'$.

### Transonic spherical flow in a power-law potential

↑ **Parent:** [Spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow)

A smooth [transonic branch](#transonic-branch) in a [power-law gravitational potential](classical-mechanics.md#power-law-gravitational-potential) has $u_*^2=c_*^2=A\beta/(2r_*^\beta)$ at its [sonic point](#sonic-point). Substitution into the [Bernoulli function](fluid-mechanics.md#bernoulli-function) gives $\mathcal B=c_*^2[1/(\gamma-1)+1/2-2/\beta]$. The local [sonic-point slope discriminant](#sonic-point-slope-discriminant) distinguishes a genuine crossing from a degenerate everywhere-sonic scaling solution.

#### Transonic spherical accretion rate in a power-law potential

↑ **Parent:** [Transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential)

With reservoir density $\rho_\infty$ and [adiabatic sound speed](#adiabatic-sound-speed) $c_\infty$, put $q=2/\beta-1/2$ and $h=1-q(\gamma-1)>0$. The selected [mass accretion rate](astrophysics.md#mass-accretion-rate) is $4\pi\rho_\infty(A\beta/2)^{2/\beta}c_\infty^{1-4/\beta}h^{q-1/(\gamma-1)}$. It follows by evaluating the conserved spherical flux at the [sonic point](#sonic-point).

##### Endpoint limits of power-law spherical accretion

↑ **Parent:** [Transonic spherical accretion rate in a power-law potential](#transonic-spherical-accretion-rate-in-a-power-law-potential)

The dimensionless accretion factor $(1-q\delta)^{q-1/\delta}$ tends to $e^q$ as $\delta\to0$. For $q>0$, it tends to $1$ as $\delta\uparrow1/q$, although the [sonic point](#sonic-point) moves to the origin. Writing the latter logarithm as $-qh\ln h/(1-h)$ makes the finite limit transparent. These limits connect [transonic spherical accretion rate in a power-law potential](#transonic-spherical-accretion-rate-in-a-power-law-potential) to the [isothermal equation of state](#globally-isothermal-equation-of-state) and the limiting critical [adiabatic exponent](thermodynamics.md#heat-capacity-ratio).

#### Critical adiabatic exponent for spherical power-law flow

↑ **Parent:** [Transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential)

For $0<\beta<4$, a nondegenerate [transonic spherical flow in a power-law potential](#transonic-spherical-flow-in-a-power-law-potential) connected to infinity requires $\gamma<(4+\beta)/(4-\beta)$. For $\beta\geq4$, every finite $\gamma>1$ satisfies the local crossing condition; there is no finite upper bound. The uniformly valid inequality is $2\beta-(4-\beta)(\gamma-1)>0$.

## Isothermal shock

↑ **Parent:** [Compressible flow](compressible-flow.md)

An isothermal shock joins two states at the same [temperature](thermodynamics.md#temperature) and [isothermal sound speed](#isothermal-sound-speed). Mass and [momentum](classical-mechanics.md#momentum) conservation imply $u_1u_2=c_s^2$ for a nontrivial planar jump, so the compression ratio is the upstream isothermal Mach number squared. [Heat](thermodynamics.md#heat) exchange replaces adiabatic energy conservation across the gas alone.

### Cooling across an isothermal shock

↑ **Parent:** [Isothermal shock](#isothermal-shock)

The [specific enthalpy](thermodynamics.md#specific-enthalpy) is equal on both sides of an isothermal perfect-gas shock. The energy removed per unit area per unit time is $j(u_1^2-u_2^2)/2$, with $j>0$ the normal mass flux. Net cooling therefore selects compression shocks; an expansion jump requires heating.

## Fluid total-energy equation

↑ **Parent:** [Compressible flow](compressible-flow.md)

For an inviscid fluid with specific [internal energy](thermodynamics.md#internal-energy) $e$, let $E=\rho(e+|\mathbf u|^2/2)$. In a prescribed potential $\Phi$, $\partial_tE+\nabla\cdot[(E+p)\mathbf u]=-\rho\mathbf u\cdot\nabla\Phi+Q$, where $Q$ is external [heat](thermodynamics.md#heat) supply. A static gravitational potential can instead be included in the conserved energy.

## Spherical polytropic flow with adiabatic exponent three halves

↑ **Parent:** [Compressible flow](compressible-flow.md)

For steady spherical [isentropic flow](#isentropic-flow) with $p=K\rho^{3/2}$ around a point mass, put $j=r^2\rho v>0$ and $\mathcal E=v^2/2+2c^2-GM/r>0$. Eliminating the [mass density](fluid-mechanics.md#density) gives $c^2=[j(3K/2)^2]^{2/5}r^{-4/5}\mathcal M^{-2/5}$. With $r_s=GM/(4\mathcal E)$, $x=(r/r_s)^{1/5}$, $y=\mathcal M^{2/5}$ and $\lambda=[j(3K/2)^2]^{2/5}/(2\mathcal E r_s^{4/5})$, the [Bernoulli equation](fluid-mechanics.md#bernoulli-equation) reduces to $\lambda F(y)=F(x)$, where $F(t)=t^4+4/t$. Since $F$ has its unique minimum at $t=1$, a regular [sonic point](#sonic-point) requires $\lambda=1$ and $r=r_s$. One [transonic branch](#transonic-branch) is $y=x$, which has $v=\sqrt{2\mathcal E}$, $\rho\propto r^{-2}$ and $p\propto r^{-3}$. The decreasing branch has inner [free fall](classical-mechanics.md#free-fall) and an outer nearly static reservoir, giving [Bondi accretion](astrophysics.md#bondi-accretion) for inward [fluid flow](fluid-mechanics.md#fluid-flow). A nonradiative stationary [shock wave](partial-differential-equation.md#shock-wave) keeps $j,\mathcal E,r_s$ fixed but raises $K$, so $\lambda$ increases by the factor $(K_2/K_1)^{4/5}$. The inward transonic solution is the spherical $n=2$, $\gamma=3/2$ specialization of [transonic accretion in a power-law tube](#transonic-accretion-in-a-power-law-tube).

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

In a nonzero steady one-dimensional flow with an [isothermal equation of state](#globally-isothermal-equation-of-state) with $p=c_s^2\rho$ and constant cross section, the [continuity equation](physics.md#continuity-equation) gives $\rho u=\text{constant}$. Eliminating density from momentum gives $(u-c_s^2/u)u'=-\Phi'$. With [Mach number](#mach-number) $\mathcal M=|u|/c_s$, integration yields $\mathcal M^2/2-\ln\mathcal M+\Phi/c_s^2=C$. The function $f(\mathcal M)=\mathcal M^2/2-\ln\mathcal M$ has minimum $1/2$ at $\mathcal M=1$, so a smooth transonic crossing at $x_*$ requires a local maximum of $\Phi$ and $C=1/2+\Phi(x_*)/c_s^2$. At a nondegenerate maximum, $f=1/2+(\mathcal M-1)^2+\cdots$ gives $\mathcal M'(x_*)=\pm\sqrt{-\Phi''(x_*)/(2c_s^2)}$.

### Sonic-point slope discriminant

↑ **Parent:** [Sonic point](#sonic-point)

For [spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow) in a [power-law gravitational potential](classical-mechanics.md#power-law-gravitational-potential), let $X=(r_*/u_*)u_*'$ and $\delta=\gamma-1$. Differentiation at a [sonic point](#sonic-point) gives $(2+\delta)X^2+4\delta X+4\delta-2\beta=0$. Its discriminant is $8[2\beta-(4-\beta)\delta]$; a positive value gives the two local crossing directions.

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

Consider steady [isentropic flow](#isentropic-flow) toward a [Newtonian gravitational potential](classical-mechanics.md#newtonian-gravitational-potential) $-GM/r$ through a tube of cross-sectional area $A(r)=Cr^n$. Write $v>0$ for the inward speed and use a [polytropic equation of state](astrophysical-fluid-dynamics.md#polytropic-equation-of-state) with [specific-heat ratio](thermodynamics.md#heat-capacity-ratio) $\gamma>1$. [Mass conservation](continuum-mechanics.md#mass-conservation) and the [Euler equations for an inviscid fluid](fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) give

$$
\rho v A=\dot M,
\qquad
\left(v-\frac{c_s^2}{v}\right)v'=\frac{nc_s^2}{r}-\frac{GM}{r^2},
$$

where $c_s$ is the [adiabatic sound speed](#adiabatic-sound-speed). A regular [sonic point](#sonic-point) therefore has $v_s=c_s$ and $r_s=GM/(nc_s^2)$. The [Bernoulli equation](fluid-mechanics.md#bernoulli-equation), matched to a nearly stationary reservoir with [sound speed](#speed-of-sound) $c_0$, gives

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

For a spherical tube $n=2$, this recovers the $5/3$ threshold of [Bondi accretion](astrophysics.md#bondi-accretion); for a [dipolar flux-tube area](electromagnetism.md#dipolar-flux-tube-area), $n=3$ gives $7/5$. The tube approximation must remain valid between the reservoir matching region and the accretor.

## Mach number

↑ **Parent:** [Compressible flow](compressible-flow.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mach_number)

The Mach number is the ratio of flow speed to local sound speed.

### Radial Mach number

↑ **Parent:** [Mach number](#mach-number)

The radial [Mach number](#mach-number) is the source [velocity](classical-mechanics.md#velocity) projected toward the observer, divided by the [sound speed](#speed-of-sound). It enters the [moving-surface retarded Jacobian](linear-acoustics.md#moving-surface-retarded-jacobian) through $d|x-y(\tau)|/d\tau=-\widehat r\cdot v$. The sign is directional: a source moving toward the observer has positive $M_r$ and compressed arrival times.

### Subsonic flow

↑ **Parent:** [Mach number](#mach-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Subsonic_flow)

A subsonic flow has [Mach number](#mach-number) less than one, so its speed is below the local [sound speed](#speed-of-sound).

### Supersonic flow

↑ **Parent:** [Mach number](#mach-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersonic_flow)

A supersonic flow has [Mach number](#mach-number) greater than one, so the flow speed exceeds the local [sound speed](#speed-of-sound).

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

For positive smooth tube area $A$, the equation $q_Z-qq_\theta+q(\log A)'/2=0$ becomes $Q_\zeta-QQ_\theta=0$ under the displayed transformation. Indeed, $g'/g=-A'/(2A)$ cancels geometrical spreading and $\zeta'=g$ makes the remaining nonlinear and transport coefficients equal. Starting with $q(\theta,Z_0)=f(\theta)$ gives $Q=f(\xi)$ and $\theta=\xi-f(\xi)\zeta$; [characteristic crossing](partial-differential-equation.md#characteristic-crossing) first occurs when $\zeta\sup f'=1$, if that supremum is positive.

##### Shock distance for a spherical simple wave launched at finite radius

↑ **Parent:** [Area transformation of a nonlinear acoustic simple wave](#area-transformation-of-a-nonlinear-acoustic-simple-wave)

For area $A(R)=R^2$ and smooth data $q(\theta,R_0)=f(\theta)$ at $R_0>0$, the transformed distance is $\zeta=R_0\log(R/R_0)$. If $M=\sup f'>0$, the first [shock wave](partial-differential-equation.md#shock-wave) occurs at the displayed radius; if $M\leq0$, there is no forward characteristic crossing. Nontrivial bounded data cannot instead be imposed at $R=0$ in this outgoing simple-wave model: along every characteristic, $Rq$ is constant, so a bounded limit at the origin forces that constant to vanish. With distance measured from a finite emitting surface, use $A(Z)=(R_0+Z)^2$ and subtract $R_0$ from the shock radius.

#### Linearly degenerate characteristic field

↑ **Parent:** [Simple wave](#simple-wave)

A characteristic field is linearly degenerate if the directional derivative of its speed along its right [eigenvector](linear-operator-theory.md#eigenvector) vanishes. Its simple waves have constant propagation speed along the state curve, so they do not steepen by amplitude-dependent transport.

#### Simple wave in magnetohydrodynamics

↑ **Parent:** [Simple wave](#simple-wave)

An ideal-MHD simple wave traces a one-parameter state-space curve whose tangent is a right [eigenvector](linear-operator-theory.md#eigenvector) of the characteristic matrix. Its parameter obeys $q_t+v(q)q_x=0$ and its characteristic speed obeys the [Inviscid Burgers equation](partial-differential-equation.md#inviscid-burgers-equation). [Nonlinear Alfvén waves](astrophysical-fluid-dynamics.md#nonlinear-alfven-wave) are a linearly degenerate example.

##### Perpendicular fast magnetosonic simple wave

↑ **Parent:** [Simple wave in magnetohydrodynamics](#simple-wave-in-magnetohydrodynamics)

For a one-dimensional [velocity](classical-mechanics.md#velocity) perpendicular to a transverse [magnetic field](electromagnetism.md#magnetic-field), $c_f^2=\gamma p/\rho+B^2/(\mu_0\rho)$. The primitive-variable characteristic matrix has two advective [eigenvalues](linear-operator-theory.md#eigenvalue) and the two speeds $u\pm c_f$. Integrating the fast [eigenvectors](linear-operator-theory.md#eigenvector) keeps $p/\rho^\gamma$ and $B/\rho$ constant. The state parameter obeys $\rho_t+(u\pm c_f)\rho_x=0$, so the [characteristic speed](partial-differential-equation.md#characteristic-speed) satisfies the [Inviscid Burgers equation](partial-differential-equation.md#inviscid-burgers-equation).

###### Isothermal perpendicular magnetosonic simple wave

↑ **Parent:** [Perpendicular fast magnetosonic simple wave](#perpendicular-fast-magnetosonic-simple-wave)

With $B_x=0$, a fast [simple wave in magnetohydrodynamics](#simple-wave-in-magnetohydrodynamics) has constant $u_y$ and $B_y/\rho=K$. Its longitudinal velocity satisfies $du_x/d\rho=\pm c_f/\rho$, and $\rho_t+(u_x\pm c_f)\rho_x=0$. Along this state curve the speed derivative is $\pm[c_f/\rho+K^2/(2\mu_0c_f)]$, which is nonzero. Compressive profiles therefore exhibit [shock formation by characteristic intersection](#shock-formation-by-characteristic-intersection), unlike a [linearly degenerate characteristic field](#linearly-degenerate-characteristic-field).

#### Damping threshold for a simple wave

↑ **Parent:** [Simple wave](#simple-wave)

For $u_t+(c_0+bu)u_x=-\alpha u$, $b,\alpha>0$, the [characteristic curves](partial-differential-equation.md#characteristic-curve) are $u=e^{-\alpha t}u_0(\xi)$ and $x=c_0t+\xi+(b/\alpha)(1-e^{-\alpha t})u_0(\xi)$. If $m=\max[-u_0']>0$, finite-time [gradient blow-up](partial-differential-equation.md#gradient-blow-up) occurs precisely for $\alpha<bm$, at $t_s=-\alpha^{-1}\log(1-\alpha/(bm))$. Equality $\alpha=bm$ still gives a positive Jacobian at each finite time; only the limiting map degenerates.

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

### Normal shock reflection at a rigid wall

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

For a perfect-gas [normal shock wave](#normal-shock-wave) reflected from a stationary rigid wall, apply the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) using signed [velocity](classical-mechanics.md#velocity) in each [shock frame](#shock-frame). The once-shocked state is the common left state for both applications. Its two relative speeds are roots of $v^2-(\gamma+1)u_sv/2-\gamma p_s/\rho_s=0$. Their product and the [pressure](thermodynamics.md#pressure) jump eliminate the [velocity](classical-mechanics.md#velocity), giving the displayed relation. A strong incident [shock wave](partial-differential-equation.md#shock-wave) gives $p_1/p_s\to(3\gamma-1)/(\gamma-1)$.

### Moving-interface conservation jump identity

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

For a moving level surface, $n=\nabla S/|\nabla S|$, $v_n=-S_t/|\nabla S|$, and the [surface delta distribution](distribution-theory.md#surface-delta-distribution) is $\delta_s=|\nabla S|\delta(S)$. Piecewise classical conservation laws acquire a distributional flux defect $[b]\cdot n-v_n[a]$. Vanishing of this defect is the [Rankine-Hugoniot condition](partial-differential-equation.md#rankine-hugoniot-conditions).

### Normal shock tables

↑ **Parent:** [Normal shock wave](#normal-shock-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_shock_tables)

Normal shock tables tabulate upstream-to-downstream property ratios for a [normal shock wave](#normal-shock-wave), typically as functions of upstream [Mach number](#mach-number) and [heat capacity ratio](thermodynamics.md#heat-capacity-ratio). They encode the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) rather than defining the discontinuity itself.

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

These are the [Rankine-Hugoniot conditions](partial-differential-equation.md#rankine-hugoniot-conditions) specialized to the mass, momentum and energy fluxes of a [perfect gas](thermodynamics.md#ideal-gas).

#### Prandtl shock relation

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

For a stationary normal shock in a polytropic perfect gas, the upstream and downstream normal speeds obey $u_1u_2=c_{\rm cr}^2$, where $c_{\rm cr}$ is the sonic speed on their common Bernoulli streamline.

#### Strong-shock Rankine-Hugoniot conditions

↑ **Parent:** [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas)

When the upstream pressure is negligible, a perfect-gas shock has density ratio $(\gamma+1)/(\gamma-1)$. For $\gamma=5/3$, the downstream density is four times the upstream density.

##### Shock compression ratio

↑ **Parent:** [Strong-shock Rankine-Hugoniot conditions](#strong-shock-rankine-hugoniot-conditions)

The shock compression ratio is the downstream-to-upstream density ratio. For a strong perfect-gas shock,

$$
\chi=\frac{\rho_1}{\rho_0}=\frac{\gamma+1}{\gamma-1}.
$$

In the upstream rest frame, the downstream velocity is $2V_s/(\gamma+1)$ and its pressure is $2\rho_0V_s^2/(\gamma+1)$.

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

Let $P=p_2/p_1$ and $D=\rho_2/\rho_1$ be the [pressure](thermodynamics.md#pressure) and [mass density](fluid-mechanics.md#density) ratios across a [normal shock wave](#normal-shock-wave) in a [perfect gas](thermodynamics.md#ideal-gas) with [specific-heat ratio](thermodynamics.md#heat-capacity-ratio) $\gamma$. Eliminating the velocities from the [Rankine-Hugoniot conditions for a perfect gas](#rankine-hugoniot-conditions-for-a-perfect-gas) gives

$$
\frac{\gamma}{\gamma-1}(p_2/\rho_2-p_1/\rho_1)
=\frac12(p_2-p_1)(1/\rho_1+1/\rho_2),
\qquad
D=\frac{(\gamma+1)P+\gamma-1}{(\gamma-1)P+\gamma+1}.
$$

As $P\to\infty$, the ratio tends to the [shock compression ratio](#shock-compression-ratio) $(\gamma+1)/(\gamma-1)$.

##### Entropy production in a perfect-gas shock

↑ **Parent:** [Pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas)

For the [pressure-density Hugoniot relation for a perfect gas](#pressure-density-hugoniot-relation-for-a-perfect-gas), the change in [specific entropy](thermodynamics.md#specific-entropy) is $[s]/c_v=\log P-\gamma\log D(P)$, with $c_v$ the [specific heat capacity](thermodynamics.md#specific-heat-capacity) at constant volume. Its derivative is

$$
\frac{d([s]/c_v)}{dP}
=\frac{(\gamma^2-1)(P-1)^2}{P[(\gamma+1)P+\gamma-1][(\gamma-1)P+\gamma+1]}.
$$

It is positive for a compressive [normal shock wave](#normal-shock-wave) with $P>1$. For a [weak shock](#weak-shock) with $P=1+\delta$, integrating the leading term gives

$$
\frac{[s]}{c_v}=\frac{\gamma^2-1}{12\gamma^2}\delta^3+O(\delta^4).
$$

Thus the [entropy production](thermodynamics.md#entropy-production) is cubic in the small [pressure](thermodynamics.md#pressure) jump, even though the [mass density](fluid-mechanics.md#density) and [temperature](thermodynamics.md#temperature) changes already appear at first order.

###### Entropy production in successive weak shocks

↑ **Parent:** [Entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock)

For $N$ equal [weak shocks](#weak-shock) with individual [pressure](thermodynamics.md#pressure) ratio $1+\delta$ and total ratio $P_s=(1+\delta)^N$, [entropy production in a perfect-gas shock](#entropy-production-in-a-perfect-gas-shock) gives

$$
\frac{\Delta s}{c_v}
=\frac{\gamma^2-1}{12\gamma^2}\delta^2\log P_s\,[1+O(\delta)].
$$

At fixed $P_s>1$, this tends to zero as the compression is divided into increasingly many smaller [weak shocks](#weak-shock). A single finite [normal shock wave](#normal-shock-wave) instead gives the positive value $\log P_s-\gamma\log D(P_s)$. Gradual compression can consequently approach reversible [isentropic flow](#isentropic-flow) while an abrupt compression generates finite [entropy](thermodynamics.md#entropy).

### Weak shock

↑ **Parent:** [Normal shock wave](#normal-shock-wave)

A weak shock has a small relative pressure jump. Its density jump agrees with the reversible adiabatic prediction through second order in the pressure jump, while entropy production first appears at third order.

### Oblique shock

↑ **Parent:** [Normal shock wave](#normal-shock-wave)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Oblique_shock)

An oblique shock is inclined relative to the upstream velocity. In an inviscid perfect gas, the normal velocity satisfies the normal-shock jump conditions while the tangential velocity is continuous.

#### Shock polar

↑ **Parent:** [Oblique shock](#oblique-shock)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shock_polar)

A [shock polar](#shock-polar) is the locus of possible downstream [velocity](classical-mechanics.md#velocity) vectors, or an equivalent [pressure](thermodynamics.md#pressure)/deflection relation, as the orientation of an [oblique shock](#oblique-shock) varies for fixed upstream conditions. [Entropy](thermodynamics.md#entropy) admissibility selects physical compressive shocks. The strong-shock perfect-gas [velocity](classical-mechanics.md#velocity) polar is a circle, while finite-Mach polars have a different shape.

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

The Mach angle of a supersonic flow with Mach number $M>1$ is $\mu=\arcsin(M^{-1})$. Infinitesimal pressure disturbances lie on the corresponding Mach cone, and a weak oblique shock approaches this angle as its strength tends to zero.

##### Mach cone

↑ **Parent:** [Mach angle](#mach-angle)

The cone forming the envelope of sound wavefronts from a source moving supersonically at [Mach number](#mach-number) $M>1$. In the source frame the ray-velocity sphere is centered at $-Mc_0\mathbf e_x$ and has radius $c_0$. Its tangent rays make angle $\sin^{-1}(1/M)$ to the backward flight direction; all other emitted acoustic rays lie inside that cone.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4.md#38a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-314.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-314.md#2/a/solution)
- [Rankine-Hugoniot conditions](partial-differential-equation.md#rankine-hugoniot-conditions)
- [Riemann problem](partial-differential-equation.md#riemann-problem)
- [Self-similar ideal-gas rarefaction](partial-differential-equation.md#self-similar-ideal-gas-rarefaction)
- [Spherically symmetric adiabatic flow](#spherically-symmetric-adiabatic-flow)
