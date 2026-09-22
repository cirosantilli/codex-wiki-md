# Euler equations for an inviscid fluid

↑ **Parent:** [Fluid mechanics](fluid-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_equations_for_an_inviscid_fluid)

Euler’s equations express momentum conservation in a fluid without viscosity.

**Table of contents**

- [Euler equation in a uniformly rotating frame](#euler-equation-in-a-uniformly-rotating-frame)
- [Density scaling invariance of incompressible Euler flow](#density-scaling-invariance-of-incompressible-euler-flow)
- [Linearized Euler equations](#linearized-euler-equations)
- [Conservative energy flux of a polytropic ideal gas](#conservative-energy-flux-of-a-polytropic-ideal-gas)
- [Crocco form of the unsteady Euler equation](#crocco-form-of-the-unsteady-euler-equation)
- [Yudovich characteristic flow](#yudovich-characteristic-flow)
- [Bernoulli's principle](#bernoulli-s-principle)
  - [Venturi effect](#venturi-effect)
- [Axisymmetric inviscid flow between moving parallel plates](#axisymmetric-inviscid-flow-between-moving-parallel-plates)
- [Radial velocity](#radial-velocity)
- [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)
  - [Constant-tension balloon discharge](#constant-tension-balloon-discharge)
  - [Inviscid startup in a pressure-driven tube](#inviscid-startup-in-a-pressure-driven-tube)
  - [Linearly elastic balloon discharge](#linearly-elastic-balloon-discharge)
- [Clebsch-potential variational derivation of incompressible Euler flow](#clebsch-potential-variational-derivation-of-incompressible-euler-flow)
- [Bernoulli equation](#bernoulli-equation)
  - [Bernoulli invariant](#bernoulli-invariant)
  - [Hydraulic control over a smooth hump](#hydraulic-control-over-a-smooth-hump)
  - [Bernoulli function for planar constant-vorticity flow](#bernoulli-function-for-planar-constant-vorticity-flow)
  - [Steady rotating-frame Bernoulli integral](#steady-rotating-frame-bernoulli-integral)
  - [Bernoulli function](#bernoulli-function)
  - [Bernoulli equation over topography](#bernoulli-equation-over-topography)
  - [Draining time of a uniform tank through a siphon](#draining-time-of-a-uniform-tank-through-a-siphon)
- [Integral momentum equation](#integral-momentum-equation)
  - [Holding force on a contracting nozzle](#holding-force-on-a-contracting-nozzle)
  - [Force on a pipe junction](#force-on-a-pipe-junction)

## Euler equation in a uniformly rotating frame

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For constant [mass density](fluid-mechanics.md#density) $\rho_0$, a frame with constant [angular velocity](rigid-body-dynamics.md#angular-velocity) $\boldsymbol\Omega$ absorbs [centrifugal acceleration](mathematical-physics.md#centrifugal-acceleration) into reduced [pressure](pressure.md) $\Pi=p/\rho_0-|\boldsymbol\Omega\times\mathbf r|^2/2$. Indeed $\boldsymbol\Omega\times(\boldsymbol\Omega\times\mathbf r)=-\nabla|\boldsymbol\Omega\times\mathbf r|^2/2$. Transforming the [material acceleration](continuum-mechanics.md#material-acceleration) in the [Euler equations](euler-equations-for-an-inviscid-fluid.md) gives the displayed equation. The [Coriolis acceleration](mathematical-physics.md#coriolis-acceleration) remains velocity dependent and cannot be absorbed into a scalar potential. A conservative physical [body force](fluid-mechanics.md#body-force) can be included by adding its potential to $\Pi$.

## Density scaling invariance of incompressible Euler flow

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

A homogeneous fluid in a prescribed gravitational field obeys $D\mathbf u/Dt=-\nabla(p/\rho)+\mathbf g$ and $\nabla\cdot\mathbf u=0$. Multiplying both constant [mass density](fluid-mechanics.md#density) and [pressure](pressure.md) by the same positive factor preserves the [velocity](classical-mechanics.md#velocity) solution, provided initial and boundary data remain compatible. Thus velocity-only observations do not determine density in this model. Independently prescribed pressure gradients or the fluid's own gravity can break this invariance.

## Linearized Euler equations

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

The linearized Euler equations retain only first-order perturbations about a specified inviscid fluid state. Together with the linearized [continuity equation](mathematical-physics.md#continuity-equation) and a pressure-density constitutive relation, they describe small-amplitude [acoustic waves](fluid-mechanics.md#acoustic-wave). About a uniform resting state, $\rho_0\partial_t\mathbf u'=-\nabla p'$, $\partial_t\rho'+\rho_0\nabla\cdot\mathbf u'=0$, and an isentropic pressure perturbation has $p'=c_0^2\rho'$. Gradients and advection of a moving background must be retained when its variation is not negligible.

## Conservative energy flux of a polytropic ideal gas

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For an unmagnetized [ideal gas](ideal-gas.md) without gravity, the [pressure](pressure.md) equation gives internal-energy balance $\partial_te+\partial_x(u_xe)=-p\partial_xu_x$, where $e=p/(\gamma-1)$. The momentum equation gives kinetic-energy balance with source $-u_x\partial_xp$. Their sum is conservative with the displayed total-energy flux. Tangential [velocities](classical-mechanics.md#velocity) contribute to [kinetic energy](energy.md#kinetic-energy) even when all derivatives are in the normal direction. Smooth [polytropic flow](compressible-flow.md#polytropic-flow) advects its [entropy](entropy.md) parameter; a physical shock need not preserve that parameter across the discontinuity.

## Crocco form of the unsteady Euler equation

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For a fixed-composition inviscid fluid, [specific enthalpy](enthalpy.md#specific-enthalpy) satisfies $dw=Tds+dp/\rho$. Combining this identity with the [vorticity cross-product identity](vorticity.md#vorticity-cross-product-identity) gives the displayed equation, with $\boldsymbol\omega=\nabla\times\mathbf u$ and $\varepsilon=u^2/2+\Phi+w$. It exposes entropy gradients as the thermodynamic source of a mismatch between [Bernoulli function](#bernoulli-function) gradients and the vorticity term. In a steady [adiabatic process](first-law-of-thermodynamics.md#adiabatic-process), its projection along a [streamline](fluid-mechanics.md#streamline) makes $\varepsilon$ constant there.

## Yudovich characteristic flow

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For a planar Euler velocity obtained from vorticity in $L^\infty_{\mathrm{loc}}(dt;L^1\cap L^\infty)$, the [planar vorticity velocity kernel](vorticity.md#planar-vorticity-velocity-kernel) gives a locally integrable speed bound and [log-Lipschitz modulus](topological-analysis.md#log-lipschitz-modulus). Spatial mollification gives existence of global trajectories; the [Osgood uniqueness criterion](differential-equation.md#osgood-uniqueness-criterion) gives uniqueness and continuous dependence. Measurability in time and an initial trace are needed. This establishes the flow for a fixed Euler solution; nonlinear uniqueness of the Euler solution itself requires further comparison arguments.

<h2 id="bernoulli-s-principle">Bernoulli's principle</h2>

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli's_principle)

The [Bernoulli principle](#bernoulli-s-principle) relates [pressure](pressure.md), [kinetic energy](energy.md#kinetic-energy) per unit volume and [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) along a [streamline](fluid-mechanics.md#streamline) of [steady flow](fluid-mechanics.md#steady-flow) with [inviscid flow](fluid-mechanics.md#inviscid-flow). For constant [mass density](fluid-mechanics.md#density), the [Bernoulli equation](#bernoulli-equation) gives $p/\rho+u^2/2+\Phi$ constant along that [streamline](fluid-mechanics.md#streamline). Constancy across different [streamlines](fluid-mechanics.md#streamline) requires further hypotheses, such as [irrotational flow](vorticity.md#irrotational-flow).

Precisely, suppose a [fluid](fluid-mechanics.md#fluid) of constant positive [mass density](fluid-mechanics.md#density) obeys the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md), its [velocity field](fluid-mechanics.md#velocity-field) and [pressure](pressure.md) are steady, and the body [force](force.md) per unit [mass](classical-mechanics.md#mass) is $-\nabla\Phi$. Then

$$
B=\frac{p}{\rho}+\frac{|\mathbf u|^2}{2}+\Phi,\qquad \mathbf u\cdot\nabla B=0.
$$

Every term has units of [energy](energy.md) per unit [mass](classical-mechanics.md#mass). For a uniform gravitational field, [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) is $\Phi=gz$, up to an additive constant. The [pressure](pressure.md) term represents work by surrounding [fluid](fluid-mechanics.md#fluid), so acceleration can exchange [pressure](pressure.md) work with [kinetic energy](energy.md#kinetic-energy). Dotting the steady [Euler equations](euler-equations-for-an-inviscid-fluid.md) with $\mathbf u$ gives the displayed [directional derivative](multivariable-calculus.md#directional-derivative): this is why constancy follows a [streamline](fluid-mechanics.md#streamline). [Cambridge, Fluid Dynamics IB, Dynamics, section 2.4](https://www.damtp.cam.ac.uk/user/mem2/FLUIDS-IB/dyn.pdf)

Continue the horizontal water constriction example from [incompressible flow](fluid-mechanics.md#incompressible-flow). Assume negligible viscous losses, [steady flow](fluid-mechanics.md#steady-flow) and approximately [uniform flow](fluid-mechanics.md#uniform-flow) at both measurement sections, so the [streamline](fluid-mechanics.md#streamline) speeds there equal the mean speeds $0.20$ and $0.80\,\mathrm{m\,s^{-1}}$. Equal height cancels the [Newtonian gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-gravitational-potential) terms. The ideal [pressure](pressure.md) drop is

$$
p_1-p_2=\frac{\rho}{2}(U_2^2-U_1^2)=\frac{1000}{2}(0.80^2-0.20^2)=300\,\mathrm{Pa}.
$$

This is the [Venturi effect](#venturi-effect) in its ideal limit: the gain in [kinetic energy](energy.md#kinetic-energy) density is supplied by [pressure](pressure.md) work. Cambridge's treatment uses this relation to connect a measured [pressure](pressure.md) difference to [volumetric flow rate](fluid-mechanics.md#volumetric-flow-rate). [Cambridge, Fluid Dynamics IB, Dynamics, section 2.5](https://www.damtp.cam.ac.uk/user/mem2/FLUIDS-IB/dyn.pdf)

The $300\,\mathrm{Pa}$ result is conditional, rather than a prediction of the actual viscous pipe. [Mass conservation](continuum-mechanics.md#mass-conservation) fixes $Q$ and the ratio of mean speeds even with [viscosity](dynamic-viscosity.md), but nonuniform [velocity profiles](viscous-fluid-flow.md#velocity-profile) require an integrated [energy](energy.md) balance, and wall friction dissipates mechanical [energy](energy.md). A pump would supply additional work. In particular, constant mean speed in a straight pipe does not imply constant [pressure](pressure.md): [Poiseuille flow](viscous-fluid-flow.md#hagen-poiseuille-equation) needs a continuing [pressure gradient](fluid-mechanics.md#pressure-gradient) to overcome [viscosity](dynamic-viscosity.md). [UCL, Bernoulli's equation, assumptions and boundary limitations](https://uclnatsci.github.io/2021/Electromagnetism-Fluids-and-Waves/fluids/bernoulli.html)

### Venturi effect

↑ **Parent:** [Bernoulli's principle](#bernoulli-s-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Venturi_effect)

In ideal steady flow, a contraction of a pipe increases the speed and lowers the pressure. For constant [mass density](fluid-mechanics.md#density), equal body-force potential at the ends and approximately uniform endpoint speeds, [conservation of mass](continuum-mechanics.md#mass-conservation) and the [Bernoulli equation](#bernoulli-equation) give $\dot M=S_1S_2\sqrt{2\rho(p_1-p_2)/(S_1^2-S_2^2)}$ for flow from a wider to a narrower section. Elevation changes contribute a body-force potential difference, and nonuniform profiles or viscous losses require additional information.

// Target: probability-and-statistics.bigb

## Axisymmetric inviscid flow between moving parallel plates

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For plates $z=\pm h(t)$, incompressibility, impermeability and regularity on the axis determine a z-independent radial velocity $u_r=-r\dot h/(2h)$ and vertical velocity $u_z=z\dot h/h$. A possible azimuthal velocity requires additional rotational data; continuity alone does not determine it. For a smooth regular initial profile $U(r)$ independent of $z$, its azimuthal Euler equation transports it as $u_\theta(r,t)=\lambda U(\lambda r)$, where $\lambda=\sqrt{h/h_0}$. If the rotation is solid-body with angular velocity $\Omega(t)$, the [vorticity equation](mathematical-physics.md#vorticity-equation) gives $\Omega=\Omega_0h/h_0$. Along a particle path, $r^2h$ and $r^2\Omega$ are constant, illustrating [conservation of angular momentum](momentum.md#conservation-of-angular-momentum).

## Radial velocity

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

Radial velocity is the component of a velocity field along the line from a chosen centre to the point of observation.

## Unsteady Bernoulli equation

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For time-dependent [irrotational flow](vorticity.md#irrotational-flow) with $u=\nabla\phi$, constant [mass density](fluid-mechanics.md#density), and no body force, the [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) integrate to

$$
\partial_t\phi+\frac12|\nabla\phi|^2+\frac p\rho=C(t).
$$

A time-dependent change of gauge in $\phi$ may set $C(t)=0$.

This is the unsteady potential-flow version of [Bernoulli's principle](#bernoulli-s-principle), with a time-dependent potential gauge.

### Constant-tension balloon discharge

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

A spherical balloon feeding an inviscid uniform tube plug, with entrance excess [pressure](pressure.md) $2\gamma/R$, satisfies $L\dot u=2\gamma/(\rho R)$ and $4\pi R^2\dot R=-\pi a^2u$. Eliminating $u$ yields the displayed equation. Its [first integral](differential-equation.md#first-integral) is $R^4\dot R^2+KR^2=C$. From rest at radius $R_0$, $C=KR_0^2$; integration gives $t=R_0^2K^{-1/2}(\pi/4-\theta/2+\sin(2\theta)/4)$, where $\theta=\arcsin(R/R_0)$. The ideal emptying time is $\pi R_0^2/(4\sqrt K)$. Independently prescribed initial flow changes $C$ and therefore this time.

### Inviscid startup in a pressure-driven tube

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

For a slender tube of length $L$ supplied from a large reservoir with excess pressure $P$, negligible gravity and entrance inertia, the [Unsteady Bernoulli equation](#unsteady-bernoulli-equation) gives $L\dot U+U^2/2=P/\rho$. A stationary initial liquid column has the displayed speed and [volume flux](fluid-mechanics.md#volumetric-flow-rate) $\pi a^2U$ for tube radius $a$. The inertial term controls the early linear acceleration; the kinetic-energy term sets the terminal inviscid speed. This is a leading slender-tube model while the reservoir remains large and the tube full.

### Linearly elastic balloon discharge

↑ **Parent:** [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)

An inviscid uniform tube plug driven by entrance excess pressure $KV$ obeys $\rho L\dot u=KV$ and $\dot V=-\pi a^2u$. From rest, the first zero of $V$ occurs after a quarter harmonic period, independent of its initial volume. The maximum speed is proportional to that initial volume. Entrance losses, a reservoir kinetic head or independently prescribed initial flow change this ideal model.

## Clebsch-potential variational derivation of incompressible Euler flow

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For $\mathbf u=\nabla\phi+\beta\nabla\alpha$, the density

$$
\mathcal L=-\beta\alpha_t-\frac12|\mathbf u|^2
$$

gives incompressibility and material conservation of $\alpha$ and $\beta$. Differentiating the Clebsch representation then yields the Euler momentum equation with

$$
p=-\frac12|\mathbf u|^2-\phi_t-\beta\alpha_t.
$$

## Bernoulli equation

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)

For steady inviscid flow, pressure, kinetic energy density, and conservative potential are constant along a streamline.

### Bernoulli invariant

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

In a steady adiabatic inviscid fluid with a conservative body force, the [Bernoulli invariant](#bernoulli-invariant) is the displayed specific energy, constant along each [streamline](fluid-mechanics.md#streamline). Dotting the [Euler equations](euler-equations-for-an-inviscid-fluid.md) with velocity and using the [specific enthalpy](enthalpy.md#specific-enthalpy) identity gives $\mathbf u\cdot\nabla b=0$. In [ideal magnetohydrodynamics](ideal-magnetohydrodynamics.md), magnetic work need not vanish; the [planar ideal-MHD Bernoulli invariant](ideal-magnetohydrodynamics.md#planar-ideal-mhd-bernoulli-invariant) includes the corresponding electromagnetic correction.

### Hydraulic control over a smooth hump

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

A slowly varying, steady, inviscid channel flow has constant discharge $Q=uh$ per unit width and the displayed [Bernoulli equation](#bernoulli-equation). The bed-height function of depth has its maximum at $h_c=(Q^2/g)^{1/3}$, where the [Froude number](reduced-gravity.md#froude-number) is one. At a nondegenerate critical crest, a differentiable profile changes between the [subcritical flow](reduced-gravity.md#subcritical-flow) and [supercritical flow](reduced-gravity.md#supercritical-flow) branches. With subcritical upstream squared Froude number $F<1$ and upstream depth $h_1$, the shock-free supercritical downstream depth is $h_1(F+\sqrt{F^2+8F})/4$.

### Bernoulli function for planar constant-vorticity flow

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

With the [streamfunction](fluid-mechanics.md#stream-function) convention $(u,v)=(\psi_y,-\psi_x)$, constant scalar [vorticity](vorticity.md) gives $\mathbf u\times\boldsymbol\omega=-\omega\nabla\psi$. For steady inviscid constant-density flow without body force, this integrates to

$$
\tfrac12|\mathbf u|^2+\omega\psi+p/\rho=C
$$

throughout a connected fluid region. Reversing the streamfunction convention changes the sign of its term; the declared convention matters.

### Steady rotating-frame Bernoulli integral

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

For [steady flow](fluid-mechanics.md#steady-flow) of constant-density fluid in a uniformly rotating frame with conservative body forces, the displayed quantity is constant along each relative [streamline](fluid-mechanics.md#streamline). The [centrifugal potential](mathematical-physics.md#centrifugal-potential) contributes the negative quadratic term, and the [Coriolis force](mathematical-physics.md#coriolis-force) contributes no work because it is perpendicular to the relative velocity. The result follows by dotting the rotating [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md) with that velocity.

### Bernoulli function

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_function)

The Bernoulli function combines pressure, kinetic energy density, and conservative potential.

### Bernoulli equation over topography

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

For steady potential flow over small hills, linearized Bernoulli pressure combines a hydrostatic term $-\rho g\eta$ with a dynamic term $-\rho U\phi_x$.

### Draining time of a uniform tank through a siphon

↑ **Parent:** [Bernoulli equation](#bernoulli-equation)

If a tank and siphon tube have areas $A$ and $a$, the tube outlet is $H$ below an inlet initially submerged by $h_0$, and both free boundaries are at [atmospheric pressure](pressure.md#atmospheric-pressure), continuity and Bernoulli's equation give

$$
t=\sqrt{2}\left(\frac{A^2}{a^2}-1\right)^{1/2}
\frac{\sqrt{H+h_0}-\sqrt H}{\sqrt g}
$$

for the free surface to reach the inlet.

## Integral momentum equation

↑ **Parent:** [Euler equations for an inviscid fluid](euler-equations-for-an-inviscid-fluid.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_momentum_equation)

The integral momentum equation balances momentum flux, pressure, body force, and forces on a control volume.

### Holding force on a contracting nozzle

↑ **Parent:** [Integral momentum equation](#integral-momentum-equation)

For steady ideal flow through a horizontal contracting nozzle, [Bernoulli equation](#bernoulli-equation) gives inlet gauge pressure $p_0=\rho Q^2(A_1^{-2}-A_0^{-2})/2$. The [integral momentum equation](#integral-momentum-equation) gives the fluid's force on the nozzle as $p_0A_0-\rho Q^2(A_1^{-1}-A_0^{-1})$ in the outlet direction. Simplification yields the displayed nonnegative magnitude. The external holding force has equal magnitude and the opposite direction.

### Force on a pipe junction

↑ **Parent:** [Integral momentum equation](#integral-momentum-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Force_on_a_pipe_junction)

The force on a pipe junction follows by balancing inlet and outlet momentum fluxes and pressure forces.

## ↑ Ancestors (4)

1. [Fluid mechanics](fluid-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (63)

- [Annular inviscid-core displacement](physiological-fluid-dynamics.md#annular-inviscid-core-displacement)
- [Barotropic spherical accretion equation](fluid-mechanics.md#barotropic-spherical-accretion-equation)
- [Bernoulli's principle](#bernoulli-s-principle)
- [Blasius boundary layer](continuum-mechanics.md#blasius-boundary-layer)
- [Convective acceleration identity](vorticity.md#convective-acceleration-identity)
- [Euler limit](viscous-fluid-flow.md#euler-limit)
- [Inviscid core](viscous-fluid-flow.md#inviscid-core)
- [Inviscid flow](fluid-mechanics.md#inviscid-flow)
- [Linear homentropic acoustic equations](linear-acoustics.md#linear-homentropic-acoustic-equations)
- [Newtonian fluid derivation of the Raychaudhuri equation](cosmology.md#newtonian-fluid-derivation-of-the-raychaudhuri-equation)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2015/paper-1.md#2/b/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017.md#4/a/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2018.md#section-b/b3/solution)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2019.md#section-b/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4.md#7g/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-49.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3.md#18c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-64.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4.md#18d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3.md#18b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3.md#18b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-69.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-69.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3.md#18d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-76.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-78.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-59.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-59.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1.md#17b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-57.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#17c/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#17c/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-1.md#17c/c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4.md#18c/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2.md#7d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3.md#18d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-320.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-314.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-314.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3.md#38b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#9b/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#9b/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-346.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-314.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-346.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3.md#16c/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-314.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-314.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3.md#7d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-331.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-310.md#3/f/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2.md#section-b/b9/solution)
- [Peculiar-velocity equation](cosmology.md#peculiar-velocity-equation)
- [Steady rotating-frame Bernoulli integral](#steady-rotating-frame-bernoulli-integral)
- [Transonic accretion in a power-law tube](compressible-flow.md#transonic-accretion-in-a-power-law-tube)
- [Two-dimensional vortex dynamics](vorticity.md#two-dimensional-vortex-dynamics)
- [Uniform-vorticity circular flow in an annulus](vorticity.md#uniform-vorticity-circular-flow-in-an-annulus)
- [Unsteady Bernoulli equation](#unsteady-bernoulli-equation)
