# Gravitational instability of an astrophysical disk

↑ **Parent:** [Astrophysical disk](astrophysics.md#astrophysical-disk)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitational_instability_of_an_astrophysical_disk)

Disk self-gravity can overcome pressure and rotational support, producing growing density disturbances, spiral structure, or fragmentation.

**Table of contents**

- [Uniformly rotating gas-sheet dispersion relation](#uniformly-rotating-gas-sheet-dispersion-relation)
  - [Marginal fragmentation wavelength of a rotating sheet](#marginal-fragmentation-wavelength-of-a-rotating-sheet)
  - [Unstable wavenumber band of a rotating gas sheet](#unstable-wavenumber-band-of-a-rotating-gas-sheet)
- [Magnetic subcriticality of a razor-thin disk](#magnetic-subcriticality-of-a-razor-thin-disk)
- [Secular gravitational instability of an astrophysical disk](#secular-gravitational-instability-of-an-astrophysical-disk)
  - [Dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag)
    - [Positive-root criterion for dust self-gravity with drag](#positive-root-criterion-for-dust-self-gravity-with-drag)
    - [Weak-drag secular gravitational growth rate](#weak-drag-secular-gravitational-growth-rate)
      - [Turbulent mixing of a secularly unstable dust layer](#turbulent-mixing-of-a-secularly-unstable-dust-layer)
      - [Finite-size secular gravitational criterion](#finite-size-secular-gravitational-criterion)
    - [Weak-drag dust density waves](#weak-drag-dust-density-waves)
- [Toomre's stability criterion](#toomre-s-stability-criterion)
  - [Toomre marginal algebraic growth](#toomre-marginal-algebraic-growth)
  - [Softened Toomre dispersion relation](#softened-toomre-dispersion-relation)
    - [Critical Toomre parameter with exponential softening](#critical-toomre-parameter-with-exponential-softening)
    - [Most unstable softened disk wavenumber](#most-unstable-softened-disk-wavenumber)
  - [Toomre parameter](#toomre-parameter)
  - [Disk mass form of the Toomre criterion](#disk-mass-form-of-the-toomre-criterion)
  - [Gravito-turbulent self-regulation](#gravito-turbulent-self-regulation)
    - [Gravitoturbulent viscosity](#gravitoturbulent-viscosity)
  - [Polytropic vertical structure of a self-gravitating disk](#polytropic-vertical-structure-of-a-self-gravitating-disk)
  - [Self-gravitating radius of an accretion disk](#self-gravitating-radius-of-an-accretion-disk)
- [Shearing sheet](#shearing-sheet)
  - [Shearing box](#shearing-box)
    - [Energy decay criterion for a viscous-resistive shearing box](#energy-decay-criterion-for-a-viscous-resistive-shearing-box)
    - [Shearing-periodic boundary condition](#shearing-periodic-boundary-condition)
      - [Spectral gap of a shearing-periodic box](#spectral-gap-of-a-shearing-periodic-box)
      - [Volume averages in a shearing box](#volume-averages-in-a-shearing-box)
  - [Axisymmetric geostrophic mode](#axisymmetric-geostrophic-mode)
  - [Infinite gravitating particle lattice](#infinite-gravitating-particle-lattice)
    - [Instability threshold of a gravitating particle lattice](#instability-threshold-of-a-gravitating-particle-lattice)
    - [Gravitating lattice Fourier kernel](#gravitating-lattice-fourier-kernel)
  - [Polytropic elliptical patch in a shearing sheet](#polytropic-elliptical-patch-in-a-shearing-sheet)
  - [Axisymmetric compressible shearing-sheet waves](#axisymmetric-compressible-shearing-sheet-waves)
  - [Pressureless dust fluid in a shearing sheet](#pressureless-dust-fluid-in-a-shearing-sheet)
    - [Forced dust epicycle with aerodynamic drag](#forced-dust-epicycle-with-aerodynamic-drag)
      - [Resonant dust entrainment by an epicyclic gas wave](#resonant-dust-entrainment-by-an-epicyclic-gas-wave)
        - [Density contrast of an entrained dust wave](#density-contrast-of-an-entrained-dust-wave)
  - [Orbital shear parameter](#orbital-shear-parameter)
  - [Particle Lagrangian in a shearing sheet](#particle-lagrangian-in-a-shearing-sheet)
    - [Jacobi energy in a shearing sheet](#jacobi-energy-in-a-shearing-sheet)
  - [Dissipative spreading of a planetary ring](#dissipative-spreading-of-a-planetary-ring)
  - [Kida vortex](#kida-vortex)
    - [Particle attraction in an elliptical shearing-sheet vortex](#particle-attraction-in-an-elliptical-shearing-sheet-vortex)
    - [Pressure Hessian of an elliptical shearing-sheet vortex](#pressure-hessian-of-an-elliptical-shearing-sheet-vortex)
  - [Stratified incompressible shearing sheet](#stratified-incompressible-shearing-sheet)
  - [Keplerian shearing sheet](#keplerian-shearing-sheet)
    - [Vertical shear instability](#vertical-shear-instability)
      - [Maximum growth rate of the vertical shear instability](#maximum-growth-rate-of-the-vertical-shear-instability)
      - [Exact single-phase incompressible perturbation of a shear flow](#exact-single-phase-incompressible-perturbation-of-a-shear-flow)
      - [Energy balance of the incompressible vertical-shear model](#energy-balance-of-the-incompressible-vertical-shear-model)
    - [Convective overstability](#convective-overstability)
      - [Convective overstability growth rate](#convective-overstability-growth-rate)
    - [Axisymmetric vertical mode of a shearing sheet](#axisymmetric-vertical-mode-of-a-shearing-sheet)
      - [Thermal energy mode of a shearing sheet](#thermal-energy-mode-of-a-shearing-sheet)
  - [Vortensity](#vortensity)
    - [Linearized vortensity](#linearized-vortensity)
      - [Linearized vortensity conservation](#linearized-vortensity-conservation)
        - [Forced axisymmetric density mode with vortensity](#forced-axisymmetric-density-mode-with-vortensity)
  - [Shearing wave](#shearing-wave)
    - [Exact incompressible shearing wave](#exact-incompressible-shearing-wave)
      - [Exact magnetic shearing wave](#exact-magnetic-shearing-wave)
        - [Zero-mean magnetic shearing wave](#zero-mean-magnetic-shearing-wave)
          - [Cubic-exponent decay of a nonaxisymmetric shearing wave](#cubic-exponent-decay-of-a-nonaxisymmetric-shearing-wave)
      - [Two-dimensional viscous shearing wave](#two-dimensional-viscous-shearing-wave)
        - [Optimal transient amplification of a viscous shearing wave](#optimal-transient-amplification-of-a-viscous-shearing-wave)
    - [Helicity invariant of an inviscid shearing wave](#helicity-invariant-of-an-inviscid-shearing-wave)
    - [Barotropic shearing-wave gravitational amplitude system](#barotropic-shearing-wave-gravitational-amplitude-system)
    - [Shearing-wave ansatz](#shearing-wave-ansatz)
    - [Shearing-wave oscillator](#shearing-wave-oscillator)
    - [Swing of a shearing wave](#swing-of-a-shearing-wave)
  - [Inertial-acoustic wave](#inertial-acoustic-wave)
    - [Density-wave dispersion relation in a non-self-gravitating disk](#density-wave-dispersion-relation-in-a-non-self-gravitating-disk)
      - [Zero-frequency balanced mode of an axisymmetric disk](#zero-frequency-balanced-mode-of-an-axisymmetric-disk)
  - [Satellite-forced density wave in an astrophysical disk](#satellite-forced-density-wave-in-an-astrophysical-disk)
  - [Thermal relaxation in a self-gravitating disk](#thermal-relaxation-in-a-self-gravitating-disk)
  - [Shearing-sheet tidal potential](#shearing-sheet-tidal-potential)
    - [Isothermal shearing-sheet energy conservation](#isothermal-shearing-sheet-energy-conservation)
  - [Viscous-convective instability](#viscous-convective-instability)

## Uniformly rotating gas-sheet dispersion relation

↑ **Parent:** [Gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md)

For a homogeneous inviscid [razor-thin disk approximation](astrophysics.md#razor-thin-disk-approximation) with [solid-body rotation](classical-mechanics.md#solid-body-rotation) and barotropic [sound speed](compressible-flow.md#speed-of-sound) $c$, the compressive wave branch obeys $\omega^2=c^2k^2-2\pi G\Sigma_0|k|+4\Omega^2$. The [razor-thin disk Poisson kernel](astrophysics.md#razor-thin-disk-poisson-kernel) supplies the [self-gravity](classical-mechanics.md#self-gravity) term, and the [radial epicyclic frequency](astrophysics.md#radial-epicyclic-frequency) is $2|\Omega|$. Growing modes have $\omega^2<0$; a separate zero-frequency balanced mode can also exist.

### Marginal fragmentation wavelength of a rotating sheet

↑ **Parent:** [Uniformly rotating gas-sheet dispersion relation](#uniformly-rotating-gas-sheet-dispersion-relation)

At fixed $\Sigma_0,\Omega\ne0$, slowly decreasing $c$ first reaches a zero of the wave-frequency minimum at $c=\pi G\Sigma_0/(2|\Omega|)$. The corresponding [wavelength](wave-equation.md#wavelength) is $\ell=\pi^2G\Sigma_0/(2\Omega^2)$. It estimates the spacing and scale of growing density concentrations just below marginality; linear theory does not determine the final nonlinear clump radius.

### Unstable wavenumber band of a rotating gas sheet

↑ **Parent:** [Uniformly rotating gas-sheet dispersion relation](#uniformly-rotating-gas-sheet-dispersion-relation)

Put $Q=2|\Omega|c/(\pi G\Sigma_0)$. The [uniformly rotating gas-sheet dispersion relation](#uniformly-rotating-gas-sheet-dispersion-relation) has growing waves precisely for $Q<1$, at $q_-<|k|<q_+$ with $q_\pm=(\pi G\Sigma_0/c^2)(1\pm\sqrt{1-Q^2})$. [Pressure](thermodynamics.md#pressure) stabilizes short waves and rotation stabilizes long waves. Equality $Q=1$ is marginal; $Q\geq1$ is the gas [Toomre stability criterion](#toomre-s-stability-criterion).

## Magnetic subcriticality of a razor-thin disk

↑ **Parent:** [Gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md)

For an isolated cold initially resting razor-thin disk, the displayed pointwise bound makes the absolute [gravity-equivalent magnetic surface density](electromagnetism.md#gravity-equivalent-magnetic-surface-density) smaller than its actual [surface density](astrophysics.md#surface-density-of-a-disk). The [positive-kernel comparison of thin-disk fields](astrophysics.md#positive-kernel-comparison-of-thin-disk-fields) then makes the integrand in the [horizontal virial balance of a cold magnetized fluid](galaxy.md#horizontal-virial-balance-of-a-cold-magnetized-fluid) negative above and below the disk. Consequently its radial second moment begins to decrease. This establishes initial contraction in the global virial sense, not inward acceleration of every individual fluid element or unlimited subsequent collapse.

## Secular gravitational instability of an astrophysical disk

↑ **Parent:** [Gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md)

Secular gravitational instability uses dissipation to weaken the epicyclic support that stabilizes a disk dynamically. It can therefore grow more slowly than an orbital time in parameter ranges where the inviscid disk is stable.

### Dust gravitational dispersion relation with gas drag

↑ **Parent:** [Secular gravitational instability of an astrophysical disk](#secular-gravitational-instability-of-an-astrophysical-disk)

The local axisymmetric density/velocity system of a pressured dust layer with linear [gas drag](fluid-mechanics.md#gas-drag) and a fixed [Keplerian shearing sheet](#keplerian-shearing-sheet) gas flow has this cubic [dispersion relation](wave-equation.md#dispersion-relation). The $\Omega/2$ azimuthal velocity coefficient includes advection of the [Keplerian shear](planetary-science.md#keplerian-shear). The [razor-thin disk Poisson kernel](astrophysics.md#razor-thin-disk-poisson-kernel) supplies the $|k|$ self-gravity term. Keeping the full amplitude [determinant](linear-algebra.md#determinant) retains the zero-frequency branch and avoids dividing out the secular mode.

#### Positive-root criterion for dust self-gravity with drag

↑ **Parent:** [Dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag)

For any nonzero positive drag, the cubic [dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag) is negative at $s=0$ if $\omega^2<\Omega^2$ and positive at sufficiently large positive $s$. The [intermediate value theorem](calculus.md#intermediate-value-theorem) therefore guarantees a growing real root. This existence argument is independent of the weak-drag expansion and includes the dynamically unstable $\omega^2<0$ regime.

#### Weak-drag secular gravitational growth rate

↑ **Parent:** [Dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag)

The mode originating at the neutral root grows for $0<\omega^2<\Omega^2$. At small nonzero $|k|$ this gives $s_{\mathrm{sec}}\sim2\pi\epsilon G\sigma_0|k|/\Omega$. [Gas drag](fluid-mechanics.md#gas-drag) transfers angular momentum to the fixed gas flow and permits [secular gravitational instability](#secular-gravitational-instability-of-an-astrophysical-disk) even for a dust [Toomre parameter](#toomre-parameter) above unity. If $\omega^2<0$, the small-root continuation is damped, while a separate dynamical root grows. The formula is singular at $\omega^2=0$.

##### Turbulent mixing of a secularly unstable dust layer

↑ **Parent:** [Weak-drag secular gravitational growth rate](#weak-drag-secular-gravitational-growth-rate)

[Turbulence](turbulence.md) can raise dust random speeds, increase layer thickness and mix density enhancements by [eddy diffusion](turbulence.md#eddy-diffusion), delaying [secular gravitational instability](#secular-gravitational-instability-of-an-astrophysical-disk). On sufficiently long wavelengths, weak-drag growth is proportional to $|k|$, whereas simple diffusive damping is proportional to $k^2$. Thus diffusion alone need not remove all long-wave growth in an infinite idealization, although finite size and lifetime can make it ineffective. Coherent turbulent concentration can also increase local [surface density](astrophysics.md#surface-density-of-a-disk), so the net effect requires a stochastic transport model.

##### Finite-size secular gravitational criterion

↑ **Parent:** [Weak-drag secular gravitational growth rate](#weak-drag-secular-gravitational-growth-rate)

For a dust layer of extent $L$, its smallest admissible wavenumber is of order $1/L$. The [secular gravitational instability](#secular-gravitational-instability-of-an-astrophysical-disk) band ends at $k_{\mathrm{crit}}=2\pi G\sigma_0/c^2=2/(QH)$, with [Toomre parameter](#toomre-parameter) $Q=c\Omega/(\pi G\sigma_0)$ and $H=c/\Omega$. Requiring an admissible mode in the band gives $Q\lesssim L/H$. Boundary conditions fix the order-unity prefactor; a finite disk lifetime also limits practical growth.

#### Weak-drag dust density waves

↑ **Parent:** [Dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag)

For fixed $\omega^2=\Omega^2-2\pi G\sigma_0|k|+c^2k^2>0$, the two oscillatory roots of the [dust gravitational dispersion relation with gas drag](#dust-gravitational-dispersion-relation-with-gas-drag) acquire negative real parts at first order in $\epsilon$. Their frequencies have no first-order shift. The expansion is not uniform near $\omega^2=0$, where the oscillation and damping scales can become comparable.

<h2 id="toomre-s-stability-criterion">Toomre's stability criterion</h2>

↑ **Parent:** [Gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toomre's_stability_criterion)

For a razor-thin isothermal gas disk,

$$
Q=\frac{c_s\kappa}{\pi G\Sigma}.
$$

Axisymmetric disturbances are stable when $Q\geq1$: pressure stabilizes short wavelengths, epicyclic motion stabilizes long wavelengths, and self-gravity drives intermediate wavelengths.

### Toomre marginal algebraic growth

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

At the marginal radial [wavenumber](wave-equation.md#wavenumber), the [forced axisymmetric density mode with vortensity](#forced-axisymmetric-density-mode-with-vortensity) has zero squared frequency. Its [mass density](fluid-mechanics.md#density) amplitude is $C_0+C_1t-\Omega\Sigma_0^2q't^2$. Thus there is no exponential instability but nonzero conserved [vortensity](#vortensity) can force quadratic growth, and a homogeneous generalized mode can grow linearly. The spectral boundary $Q=1$ of the [Toomre stability criterion](#toomre-s-stability-criterion) must not be mistaken for boundedness of every initial-value solution.

### Softened Toomre dispersion relation

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

Linear axisymmetric compressive modes of a [barotropic closure of a razor-thin disk](astrophysics.md#barotropic-closure-of-a-razor-thin-disk) combine radial epicyclic restoration, softened [self-gravity](classical-mechanics.md#self-gravity) and [pressure](thermodynamics.md#pressure). The [off-plane razor-thin Poisson kernel](astrophysics.md#off-plane-razor-thin-poisson-kernel) supplies the exponential gravity reduction. Here $k$ is the nonnegative radial [wavenumber](wave-equation.md#wavenumber) magnitude. The full linear system also has an [axisymmetric geostrophic mode](#axisymmetric-geostrophic-mode).

#### Critical Toomre parameter with exponential softening

↑ **Parent:** [Softened Toomre dispersion relation](#softened-toomre-dispersion-relation)

The [most unstable softened disk wavenumber](#most-unstable-softened-disk-wavenumber) minimizes the squared mode frequency. Instability is $Q<Q_c$, while $Q\ge Q_c$ is spectrally stable for this compressive pair. Since $s_*<(1+\delta)^{-1}$, $Q_c^2<(1+2\delta)/(1+\delta)^2\le1$. At zero [gravitational softening](galaxy.md#gravitational-softening) both bounds become equality. The physical path with fixed $\kappa\epsilon/c_s$ obeys $\delta=(\kappa\epsilon/c_s)/Q$.

#### Most unstable softened disk wavenumber

↑ **Parent:** [Softened Toomre dispersion relation](#softened-toomre-dispersion-relation)

With $s=Q c_sk/\kappa$ and $\delta=\kappa\epsilon/(Q c_s)$, maximize $F(s)=2se^{-\delta s}-s^2$. Its unique positive critical point satisfies the displayed equation. For positive [gravitational softening](galaxy.md#gravitational-softening), $e^{-\delta s_*}<1$ and $1-\delta s_*>0$, giving the strict bound. Unsoftened gravity has $s_*=1$.

### Toomre parameter

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

For a razor-thin fluid disk with [sound speed](compressible-flow.md#speed-of-sound) or effective random speed $c$, [surface density](astrophysics.md#surface-density-of-a-disk) $\Sigma$ and radial epicyclic frequency $\kappa$, $Q=c\kappa/(\pi G\Sigma)$ compares pressure and rotational support with [self-gravity](classical-mechanics.md#self-gravity). The local axisymmetric fluid [Toomre stability criterion](#toomre-s-stability-criterion) is $Q\geq1$. For a [Keplerian shearing sheet](#keplerian-shearing-sheet), $\kappa=\Omega$. Collisionless stellar disks use a different numerical normalization; gas drag can permit secular growth even when this fluid parameter exceeds unity.

### Disk mass form of the Toomre criterion

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

In a star-dominated [Keplerian disk](astrophysics.md#keplerian-disk) with $H\simeq c_s/\Omega$ and characteristic disk mass $M_D\sim\pi r^2\Sigma$, the [Toomre stability criterion](#toomre-s-stability-criterion) becomes $Q\sim(H/r)(M_*/M_D)$. Thus instability can occur at a disk-to-star mass ratio comparable to the small [disk aspect ratio](astrophysics.md#disk-aspect-ratio). The numerical coefficient depends on whether $M_D$ means a local annular estimate or integrated enclosed mass.

### Gravito-turbulent self-regulation

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

In a cooling self-gravitating disk, $Q<1$ excites gravitational turbulence whose dissipation raises the sound speed, while $Q>1$ suppresses that heating and lets cooling lower the sound speed. A sustained state can therefore regulate itself near $Q\simeq1$.

#### Gravitoturbulent viscosity

↑ **Parent:** [Gravito-turbulent self-regulation](#gravito-turbulent-self-regulation)

A mixing-length estimate for gravitational turbulence takes the largest unstable wavelength $\ell$ and orbital growth rate $\Omega$, giving turbulent velocity $u_{\rm turb}\sim\Omega\ell$ and kinematic viscosity $\nu\sim u_{\rm turb}\ell\sim\Omega\ell^2$.

### Polytropic vertical structure of a self-gravitating disk

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

For $P=K\rho^{1+1/n}$, dimensionless pseudo-enthalpy $w=n(\rho/\rho_0)^{1/n}$, and $\zeta=\Omega z/c_0$, vertical hydrostatic balance and the [Poisson equation](partial-differential-equation.md#poisson-equation) reduce to

$$
w''+\frac4{n^nQ_0}w^n=-1.
$$

The midplane conditions are $w(0)=n$ and $w'(0)=0$, and the first zero gives the disk surface.

### Self-gravitating radius of an accretion disk

↑ **Parent:** [Toomre's stability criterion](#toomre-s-stability-criterion)

The self-gravitating radius of an accretion disk is the radius at which its [Toomre stability criterion](#toomre-s-stability-criterion) reaches $Q=1$. Beyond it, a smooth thin disk is vulnerable to spiral structure, gravitational transport, or fragmentation.

## Shearing sheet

↑ **Parent:** [Gravitational instability of an astrophysical disk](gravitational-instability-of-an-astrophysical-disk.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shearing_sheet)

The shearing sheet is a local Cartesian approximation to a differentially rotating disk. It retains Coriolis force, linearized tidal gravity, and a background linear shear.

### Shearing box

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A [shearing box](#shearing-box) solves the [shearing sheet](#shearing-sheet) equations in a finite domain with periodic azimuthal and vertical faces and a [shearing-periodic boundary condition](#shearing-periodic-boundary-condition) on its radial faces. It follows a small region rotating at a reference orbital frequency. The model can sustain stress and exchange energy with its imposed differential rotation, but its identified radial faces do not represent a global disk mass sink.

#### Energy decay criterion for a viscous-resistive shearing box

↑ **Parent:** [Shearing box](#shearing-box)

For zero mean velocity and [magnetic field](electromagnetism.md#magnetic-field) in a [shearing box](#shearing-box), the perturbation energy obeys $\dot E\le2(|A|-4\pi^2\eta/L^2)E$ when kinematic viscosity and magnetic diffusivity agree. Bound the work of [Reynolds stress](turbulence.md#reynolds-stress) and [Maxwell stress tensor](electromagnetism.md#maxwell-stress-tensor) by $2|A|E$, and use the [spectral gap of a shearing-periodic box](#spectral-gap-of-a-shearing-periodic-box) to bound dissipation below. Thus the displayed bound on [magnetic Reynolds number](astrophysical-fluid-dynamics.md#magnetic-reynolds-number) guarantees exponential decay and excludes sustained turbulence.

#### Shearing-periodic boundary condition

↑ **Parent:** [Shearing box](#shearing-box)

For background velocity $-2Ax\mathbf e_y$, opposite radial faces of a [shearing box](#shearing-box) are identified after the displayed azimuthal shift, modulo $L_y$. Products and spatial derivatives inherit this condition. Their radial surface integrals cancel because a translation preserves an integral over a periodic azimuthal interval.

##### Spectral gap of a shearing-periodic box

↑ **Parent:** [Shearing-periodic boundary condition](#shearing-periodic-boundary-condition)

For zero-mean fields in a [shearing box](#shearing-box), [Fourier modes](fourier-analysis.md#fourier-mode) have wavevectors $(2\pi n/L_x+2At\,2\pi m/L_y,2\pi m/L_y,2\pi p/L_z)$. A nonzero azimuthal or vertical index supplies at least $2\pi/L$, where $L$ is the largest box side; otherwise the nonzero radial index does. [Parseval identity](fourier-analysis.md#parseval-identity) gives the displayed [Poincaré inequality](sobolev-space.md#poincare-inequality) uniformly in time.

##### Volume averages in a shearing box

↑ **Parent:** [Shearing-periodic boundary condition](#shearing-periodic-boundary-condition)

Periodic azimuthal and vertical boundary terms vanish. Radial boundary terms cancel after the azimuthal translation prescribed by the [shearing-periodic boundary condition](#shearing-periodic-boundary-condition). Consequently the [volume average](measure-theory.md#volume-average) of a divergence is zero, enabling integration by parts for the smooth shearing-periodic fields.

### Axisymmetric geostrophic mode

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A stationary [mass density](fluid-mechanics.md#density) disturbance can be balanced by a changed azimuthal [velocity](classical-mechanics.md#velocity) in a [shearing sheet](#shearing-sheet). The [continuity](calculus.md#continuous-function) and azimuthal equations give zero [radial velocity](fluid-mechanics.md#radial-velocity), while the radial equation balances [Coriolis force](physics.md#coriolis-force) against [pressure](thermodynamics.md#pressure) and gravity. This mode is separate from the density-wave pair in the [softened Toomre dispersion relation](#softened-toomre-dispersion-relation) and is lost if one divides every equation by frequency.

### Infinite gravitating particle lattice

↑ **Parent:** [Shearing sheet](#shearing-sheet)

An infinite gravitating particle lattice with spacing $h$ in the azimuthal direction is a shearing-sheet equilibrium when all particles sit at $x_n=0,y_n=nh$. Opposite-neighbor accelerations cancel absolutely. The linear gravitational response to pair displacement differences has transverse and longitudinal coefficients $1$ and $-2$, divided by $h^3|j-n|^3$.

#### Instability threshold of a gravitating particle lattice

↑ **Parent:** [Infinite gravitating particle lattice](#infinite-gravitating-particle-lattice)

For $q=GmF(hk)/(h^3\Omega^2)$, the squared dimensionless growth rates are $s^2/\Omega^2=(q-1\pm\sqrt{9q^2-26q+1})/2$. Exponential growth begins for $q>(13-4\sqrt{10})/9$. Since the [gravitating lattice Fourier kernel](#gravitating-lattice-fourier-kernel) is largest at $hk=\pi$, the full infinite lattice is exponentially unstable when $Gm/(h^3\Omega^2)>(13-4\sqrt{10})/[9F(\pi)]$. Marginal repeated imaginary roots and zero-frequency secular modes require separate treatment.

#### Gravitating lattice Fourier kernel

↑ **Parent:** [Infinite gravitating particle lattice](#infinite-gravitating-particle-lattice)

The discrete normal modes of an [infinite gravitating particle lattice](#infinite-gravitating-particle-lattice) involve $F(\xi)=2\sum_{l=1}^\infty(1-\cos(l\xi))/l^3$. It is even, nonnegative and $2\pi$-periodic. Its derivative is a positive reciprocal-square sine series for $0<\xi<\pi$, so its maxima occur exactly at odd multiples of $\pi$, with $F(\pi)=(7/2)\zeta(3)$.

### Polytropic elliptical patch in a shearing sheet

↑ **Parent:** [Shearing sheet](#shearing-sheet)

The steady planar velocity $\mathbf u=\alpha y\mathbf e_x-\beta x\mathbf e_y$ supports a bounded polytropic patch when $\alpha=(\beta^2-3\Omega^2)/\beta$ and $\sqrt3\Omega<\beta<2\Omega$. Its [polytropic enthalpy](thermodynamics.md#polytropic-enthalpy) is $Q=Q_0-(2\Omega-\beta)(\beta x^2+\alpha y^2)/2$ with $Q_0>0$. Its [fluid free boundary](fluid-mechanics.md#fluid-free-boundary) is the material ellipse $\beta x^2+\alpha y^2=2Q_0/(2\Omega-\beta)$. No additional self-gravity potential is part of this model.

### Axisymmetric compressible shearing-sheet waves

↑ **Parent:** [Shearing sheet](#shearing-sheet)

In an unstratified [Keplerian shearing sheet](#keplerian-shearing-sheet) with [sound speed](compressible-flow.md#speed-of-sound) $c$, the four linear velocity-density equations yield $\omega^4-(\Omega^2+c^2k^2)\omega^2+\Omega^2c^2k_z^2=0$. The lower-frequency branch approaches the [inertial wave](geophysical-fluid-dynamics.md#inertial-wave) relation $\omega^2=\Omega^2k_z^2/k^2$ for $ck\gg\Omega$; the upper branch is predominantly acoustic.

### Pressureless dust fluid in a shearing sheet

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A dilute dust component can be approximated as a pressureless fluid with velocity $\mathbf v$ and [surface density of a disk](astrophysics.md#surface-density-of-a-disk) $\Sigma_d$. In a gas velocity $\mathbf u$, linear [drag force](fluid-mechanics.md#drag-physics) gives acceleration $-(\mathbf v-\mathbf u)/t_s$ for positive [aerodynamic stopping time](fluid-mechanics.md#aerodynamic-stopping-time) $t_s$. Its equations include [Coriolis acceleration](physics.md#coriolis-acceleration), the [shearing-sheet tidal potential](#shearing-sheet-tidal-potential), and $\partial_t\Sigma_d+\nabla\cdot(\Sigma_d\mathbf v)=0$. Neglecting gas backreaction is justified only when the prescribed-gas approximation is appropriate. Strong orbit crossing or appreciable dust velocity dispersion can invalidate the single-valued pressureless-fluid description.

#### Forced dust epicycle with aerodynamic drag

↑ **Parent:** [Pressureless dust fluid in a shearing sheet](#pressureless-dust-fluid-in-a-shearing-sheet)

Let $v_x,v_y$ and $u_x,u_y$ be the dust and gas velocity perturbations after subtracting the common background shear, suppressing primes. Put $t_s>0$ for the [aerodynamic stopping time](fluid-mechanics.md#aerodynamic-stopping-time). Linear axisymmetric dust perturbations about a [Keplerian shearing sheet](#keplerian-shearing-sheet) obey $D_\epsilon v_x-2\Omega v_y=\epsilon\Omega u_x$ and $D_\epsilon v_y+\Omega v_x/2=\epsilon\Omega u_y$, with $\epsilon\Omega=t_s^{-1}>0$. Eliminating $v_y$ gives

$$
[\partial_t^2+2\epsilon\Omega\partial_t+(1+\epsilon^2)\Omega^2]v_x=\epsilon\Omega\partial_tu_x+\epsilon^2\Omega^2u_x+2\epsilon\Omega^2u_y.
$$

Thus a gas epicycle $u_x=u\cos(kx-\Omega t)$, $u_y=u\sin(kx-\Omega t)/2$ supplies both $2\epsilon\Omega^2u\sin(kx-\Omega t)$ and $\epsilon^2\Omega^2u\cos(kx-\Omega t)$. Keeping the latter is necessary for an exact linear equation beyond first order in drag. The homogeneous roots are $-\epsilon\Omega\pm i\Omega$, separating damping from epicyclic frequency.

##### Resonant dust entrainment by an epicyclic gas wave

↑ **Parent:** [Forced dust epicycle with aerodynamic drag](#forced-dust-epicycle-with-aerodynamic-drag)

If the prescribed gas velocity is itself a free [epicyclic motion](astrophysics.md#epicyclic-motion) solution, subtract its two momentum equations from the [forced dust epicycle with aerodynamic drag](#forced-dust-epicycle-with-aerodynamic-drag) equations. The velocity difference obeys a damped epicycle and decays as $e^{-\epsilon\Omega t}$. Therefore dust approaches the gas velocity with identical phase and amplitude for every positive drag rate. At zero drag the difference does not decay, so the late-time limit is nonuniform as drag vanishes. A finite-wavelength [inertial-acoustic wave](#inertial-acoustic-wave) is detuned from the free epicycle; matching its phase and amplitude in the weak-drag limit additionally requires $|\omega-\Omega|\ll\epsilon\Omega$. For a gas density wave of frequency $\omega$, the exact radial transfer amplitude is

$$
\frac{V_x}{U_x}=\frac{\epsilon\Omega[\epsilon\Omega-i\omega-i\Omega^2/\omega]}{(\epsilon\Omega-i\omega)^2+\Omega^2},
$$

obtained by solving the two dust equations and using $U_y=-i\Omega U_x/(2\omega)$. At $\omega=\Omega$ it is exactly one.

###### Density contrast of an entrained dust wave

↑ **Parent:** [Resonant dust entrainment by an epicyclic gas wave](#resonant-dust-entrainment-by-an-epicyclic-gas-wave)

Let $\Sigma_{d0}$ be the uniform background dust [surface density of a disk](astrophysics.md#surface-density-of-a-disk) and $\delta_d=(\Sigma_d-\Sigma_{d0})/\Sigma_{d0}$ its fractional perturbation. Here $k$ is the radial [wavenumber](wave-equation.md#wavenumber), $\Omega$ is the epicyclic frequency and $u$ is a real velocity amplitude. For that uniform background and late velocity $v_x=u\cos(kx-\Omega t)$, linear dust [continuity equation](physics.md#continuity-equation) gives $\partial_t\delta_d=-\partial_xv_x=ku\sin(kx-\Omega t)$. Integrating yields the displayed formula. The coherent travelling-wave fractional excess is $|ku|/\Omega$, with validity requiring this number much smaller than one. The static term $C(x)$ records initial density and transient displacement: drag damps velocity, but supplies no density diffusion. The long-wavelength gas wave has the same fractional density amplitude, so entrainment alone does not produce an additional dust-to-gas ratio enhancement at this order.

### Orbital shear parameter

↑ **Parent:** [Shearing sheet](#shearing-sheet)

The orbital shear parameter measures the fractional radial decrease in orbital angular frequency. A [Kepler orbit](classical-mechanics.md#kepler-orbit) has $q=3/2$, while rigid rotation has $q=0$. The [radial epicyclic frequency](astrophysics.md#radial-epicyclic-frequency) obeys $\kappa_r^2=2(2-q)\Omega^2$; this follows by differentiating the squared [specific angular momentum](classical-mechanics.md#specific-angular-momentum) $h^2=r^4\Omega^2$.

### Particle Lagrangian in a shearing sheet

↑ **Parent:** [Shearing sheet](#shearing-sheet)

Expand a unit-mass particle's [Lagrangian](calculus-of-variations.md#lagrangian) about an axisymmetric [circular orbit](classical-mechanics.md#circular-orbit) of radius $r_0$ and frequency $\Omega_0$, using $r=r_0+x$ and $\varphi=\Omega_0t+y/r_0$. Circular-orbit balance removes the linear radial term; [total-time-derivative invariance of a Lagrangian](classical-mechanics.md#total-time-derivative-invariance-of-a-lagrangian) removes $r_0\Omega_0\dot y$. To second order,

$$
L_2=\frac12(\dot x^2+\dot y^2+\dot z^2)+2\Omega_0x\dot y-\Phi_t,
\qquad
\Phi_t=-q\Omega_0^2x^2+\frac12\Omega_z^2z^2.
$$

Here $q$ is the [orbital shear parameter](#orbital-shear-parameter) and $\Omega_z$ is the [vertical epicyclic frequency](astrophysics.md#vertical-epicyclic-frequency). The [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) retain the local [Coriolis acceleration](physics.md#coriolis-acceleration) and tidal gravity.

#### Jacobi energy in a shearing sheet

↑ **Parent:** [Particle Lagrangian in a shearing sheet](#particle-lagrangian-in-a-shearing-sheet)

The time-independent [particle Lagrangian in a shearing sheet](#particle-lagrangian-in-a-shearing-sheet) has conserved rotating-frame energy

$$
\varepsilon_J=\sum_i\dot q_i\frac{\partial L_2}{\partial\dot q_i}-L_2
=\frac12(\dot x^2+\dot y^2+\dot z^2)-q\Omega_0^2x^2+\frac12\Omega_z^2z^2.
$$

The velocity-linear [Coriolis acceleration](physics.md#coriolis-acceleration) term cancels from this expression. Up to the reference-orbit constant, it is the second-order expansion of inertial [specific orbital energy](classical-mechanics.md#specific-orbital-energy) minus $\Omega_0$ times inertial [specific angular momentum](classical-mechanics.md#specific-angular-momentum). Its negative radial tidal term allows [inelastic collisions](classical-mechanics.md#inelastic-collision) to lower the total energy while increasing the radial extent of a ring.

### Dissipative spreading of a planetary ring

↑ **Parent:** [Shearing sheet](#shearing-sheet)

In a [Keplerian shearing sheet](#keplerian-shearing-sheet), an [epicyclic guiding center](astrophysics.md#epicyclic-guiding-center) $x_0$ carries rotating-frame energy $-3\Omega^2x_0^2/8$, plus nonnegative radial and vertical oscillation energies. [Inelastic collisions](classical-mechanics.md#inelastic-collision) dissipate the total [Jacobi energy in a shearing sheet](#jacobi-energy-in-a-shearing-sheet), while [momentum conservation](classical-mechanics.md#momentum-conservation) preserves $\sum x_0$. Thus $\sum x_0^2$ must grow: the ring spreads about its fixed mean radius. The effect is an [angular momentum transport](classical-mechanics.md#angular-momentum-transport) process, with some particles moving inward and others outward.

### Kida vortex

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A Kida vortex is an exact elliptical patch of uniform vorticity embedded in a linear shear flow. In a Keplerian shearing sheet its aspect ratio controls both the circulation period and the stability of three-dimensional perturbations.

#### Particle attraction in an elliptical shearing-sheet vortex

↑ **Parent:** [Kida vortex](#kida-vortex)

The material-boundary and [vorticity](fluid-mechanics.md#vorticity) conditions give $\alpha=S/[r(r-1)]$ and $\beta=Sr/(r-1)$. A pressureless particle subject to [linear drag](fluid-mechanics.md#linear-drag), [Coriolis acceleration](physics.md#coriolis-acceleration) and tidal gravity has the [drag-polynomial stability for all positive stopping rates](dynamical-systems.md#drag-polynomial-stability-for-all-positive-stopping-rates) with $K=2\Omega(2\Omega-S)$, $L=\Omega(\alpha+\beta-S)$ and $P=\alpha\beta$. In [Keplerian shear](planetary-science.md#keplerian-shear), $K/\Omega^2=1$, $L/\Omega^2=3(r+1)/[2r(r-1)]$ and $P/\Omega^2=9/[4(r-1)^2]$. The exact criterion is $r\geq3$, including the boundary $K=L>P$ at $r=3$. Attraction is local to the centre under the prescribed interior velocity field; a trajectory leaving the patch cannot be followed using that field alone.

#### Pressure Hessian of an elliptical shearing-sheet vortex

↑ **Parent:** [Kida vortex](#kida-vortex)

For the incompressible velocity $u_x=\alpha y$, $u_y=-\beta x$ in a [shearing sheet](#shearing-sheet), advection produces $-\alpha\beta(x,y)$ and the [Coriolis acceleration](physics.md#coriolis-acceleration) produces $(2\Omega\beta x,2\Omega\alpha y)$. Including the radial tide $2\Omega Sx$ gives $p/\rho=(Ax^2+By^2)/2+C$. A material ellipse has $\beta=r^2\alpha$. A vortex patch is immersed in surrounding fluid, so this [pressure](thermodynamics.md#pressure) need not vanish on its boundary; imposing that condition would describe a different free-boundary problem.

### Stratified incompressible shearing sheet

↑ **Parent:** [Shearing sheet](#shearing-sheet)

The stratified incompressible shearing sheet adds a buoyancy displacement $\theta$ with $D\theta/Dt=u_z$ and acceleration $-N^2\theta\mathbf e_z$. Axisymmetric plane waves obey

$$
\omega^2=\frac{k_z^2\Omega^2+k_x^2N^2}{k_x^2+k_z^2},
$$

interpolating between inertial and buoyancy oscillations.

### Keplerian shearing sheet

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A Keplerian shearing sheet has background velocity $\mathbf u_0=-(3/2)\Omega x\mathbf e_y$, radial shear rate $S=3\Omega/2$, and radial epicyclic frequency $\kappa_r=\Omega$.

#### Vertical shear instability

↑ **Parent:** [Keplerian shearing sheet](#keplerian-shearing-sheet)

Vertical shear instability destabilizes differential rotation that varies with height, when buoyancy restoration is absent or sufficiently weakened. In the homogeneous [incompressible flow](fluid-mechanics.md#incompressible-flow) model with background $U_y=-3\Omega x/2+q\Omega z$, an axisymmetric perturbation with [wavevector](continuum-mechanics.md#wavevector) $(k_x,0,k_z)\ne0$ has

$$
s^2=\Omega^2\frac{2qk_xk_z-k_z^2}{k_x^2+k_z^2}.
$$

The pressure-free radial/vertical momentum equation and the azimuthal equation give this result after using [incompressibility](fluid-mechanics.md#incompressible-flow). Growth requires $2qk_xk_z>k_z^2$, so a small vertical shear favors nearly radial wavevectors. Here $q$ is the vertical shear amplitude, distinct from the [orbital shear parameter](#orbital-shear-parameter) $3/2$. Stratification, cooling and boundaries can change this simplified criterion.

##### Maximum growth rate of the vertical shear instability

↑ **Parent:** [Vertical shear instability](#vertical-shear-instability)

For the unstratified local [vertical shear instability](#vertical-shear-instability), maximize $s^2/\Omega^2=(2qR-1)/(1+R^2)$ over $R=k_x/k_z$. Its derivative vanishes when $qR^2-R-q=0$. For $q>0$ the maximum uses $R=(1+\sqrt{1+4q^2})/(2q)$, and substitution gives the displayed expression. For small $q$, $R\sim q^{-1}$ and $s_{\max}=\Omega q(1-q^2/2+O(q^4))$. Changing the sign of the shear changes the preferred sign of $R$ but gives the same maximum magnitude; there is no exponential growth at $q=0$.

##### Exact single-phase incompressible perturbation of a shear flow

↑ **Parent:** [Vertical shear instability](#vertical-shear-instability)

For a perturbation $\mathbf u'=\tilde{\mathbf u}f(\mathbf k\cdot\mathbf x)e^{st}$ with constant $\tilde{\mathbf u},\mathbf k$ and nonconstant differentiable $f$, [incompressibility](fluid-mechanics.md#incompressible-flow) forces $\mathbf k\cdot\tilde{\mathbf u}=0$. Consequently $\mathbf u'\cdot\nabla\mathbf u'=ff'e^{2st}(\mathbf k\cdot\tilde{\mathbf u})\tilde{\mathbf u}=0$. About a shear depending only on $x,z$ and directed along $y$, an axisymmetric such perturbation therefore obeys its linear amplitude equations exactly, including at finite amplitude in this homogeneous model. For [pressure](thermodynamics.md#pressure) $P'=\tilde P g(\xi)e^{st}$, nonzero [pressure](thermodynamics.md#pressure) requires $g'=Cf$, and $C$ can be absorbed into $\tilde P$; choose $g'=f$. This relation does not imply $g=f$ for an arbitrary profile.

##### Energy balance of the incompressible vertical-shear model

↑ **Parent:** [Vertical shear instability](#vertical-shear-instability)

For constant density $\rho_0$ and body force $\Omega^2(3x-2qz)\mathbf e_x$, dotting the [incompressible flow](fluid-mechanics.md#incompressible-flow) momentum equation with $\rho_0\mathbf u$ gives the [kinetic energy](classical-mechanics.md#kinetic-energy) flux $(K+P)\mathbf u$ and source $\rho_0\Omega^2(3x-2qz)u_x$, where $K=\rho_0|\mathbf u|^2/2$. [Coriolis acceleration](physics.md#coriolis-acceleration) does no work. Absorbing $\Phi_t=-3\Omega^2x^2/2$ gives the displayed balance. For nonzero $q$, the remaining force has [curl](calculus.md#curl) $-2\Omega^2q\mathbf e_y$, so it cannot be incorporated into a scalar mechanical potential. The model can exchange energy with its maintained vertical-shear background; at $q=0$ ordinary [Jacobi energy in a shearing sheet](#jacobi-energy-in-a-shearing-sheet) conservation is recovered under zero boundary flux.

#### Convective overstability

↑ **Parent:** [Keplerian shearing sheet](#keplerian-shearing-sheet)

An adverse radial [specific entropy](thermodynamics.md#specific-entropy) gradient can drive an oscillatory instability through the finite lag supplied by [thermal conduction](thermodynamics.md#thermal-conduction) or relaxation. This differs from a [viscous-convective instability](#viscous-convective-instability), in which viscosity changes rotational stabilization.

##### Convective overstability growth rate

↑ **Parent:** [Convective overstability](#convective-overstability)

For $|N^2|\ll\Omega^2$, this leading amplitude-growth rate is largest at [thermal diffusion rate of a Fourier mode](thermodynamics.md#thermal-diffusion-rate-of-a-fourier-mode) $\beta=\Omega$, giving $\sigma_{\rm max}=-N^2/(4\Omega)$ when $N^2<0$.

#### Axisymmetric vertical mode of a shearing sheet

↑ **Parent:** [Keplerian shearing sheet](#keplerian-shearing-sheet)

A horizontal-velocity perturbation depending only on height has zero vertical velocity for nonzero [wavenumber](wave-equation.md#wavenumber) under [incompressibility](fluid-mechanics.md#incompressible-flow). Its [pressure](thermodynamics.md#pressure) amplitude then vanishes in the unstratified vertical momentum equation.

##### Thermal energy mode of a shearing sheet

↑ **Parent:** [Axisymmetric vertical mode of a shearing sheet](#axisymmetric-vertical-mode-of-a-shearing-sheet)

The nonoscillatory thermal branch of the radially stratified [shearing sheet](#shearing-sheet) spectrum. Its decoupled small-buoyancy limit is a diffusing scalar perturbation.

### Vortensity

↑ **Parent:** [Shearing sheet](#shearing-sheet)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vortensity)

Vortensity is [absolute vorticity](fluid-mechanics.md#absolute-vorticity) divided by surface density. In a two-dimensional inviscid barotropic flow, it is conserved along fluid trajectories.

#### Linearized vortensity

↑ **Parent:** [Vortensity](#vortensity)

Linearized vortensity is the first-order perturbation of vortensity about a background flow. For a shearing wave in a uniform Keplerian sheet, its amplitude is constant.

##### Linearized vortensity conservation

↑ **Parent:** [Linearized vortensity](#linearized-vortensity)

Linearized vortensity conservation is the perturbative form of material vortensity conservation. In an inviscid barotropic shearing sheet, the linearized vortensity obeys $Df'/Dt=0$.

###### Forced axisymmetric density mode with vortensity

↑ **Parent:** [Linearized vortensity conservation](#linearized-vortensity-conservation)

For a radial mode with constant nonzero [wavenumber](wave-equation.md#wavenumber) in an inviscid [razor-thin disc](astrophysics.md#razor-thin-disk-approximation), eliminate velocity using continuity and the conserved [linearized vortensity](#linearized-vortensity). The resulting oscillator has $\omega_k^2=\kappa^2+c_s^2k^2-2\pi G\Sigma_0|k|$. The [vortensity](#vortensity) gives a constant forcing and hence the stationary balanced component when $\omega_k^2>0$. It is lost by an ansatz that divides every amplitude equation by a nonzero frequency. Negative squared frequency gives exponential instability; zero frequency allows secular growth.

### Shearing wave

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A shearing wave is a local disturbance whose wavevector evolves under background shear. In a Keplerian sheet, $k_x(t)=k_x(0)+(3/2)\Omega k_yt$.

#### Exact incompressible shearing wave

↑ **Parent:** [Shearing wave](#shearing-wave)

For background shear $\mathbf u_0=-2Ax\mathbf e_y$, take $\mathbf u'=\operatorname{Re}[\mathbf v(t)e^{i\mathbf k(t)\cdot\mathbf r}]$ with real $\mathbf k$ and $\mathbf k\cdot\mathbf v=0$. Then $\mathbf u'\cdot\nabla\mathbf u'=0$ pointwise, including conjugate terms. Choosing $\dot k_x=2Ak_y$, $\dot k_y=\dot k_z=0$ cancels background phase [advection](fluid-mechanics.md#advection). The resulting linear [amplitude](physics.md#wave-amplitude) equations are therefore exact finite-amplitude solutions of the incompressible [Navier-Stokes equation](viscous-fluid-flow.md#navier-stokes-equation) in this unbounded or compatible shearing-periodic setting.

// Target: gravitational-instability-of-an-astrophysical-disk.bigb

##### Exact magnetic shearing wave

↑ **Parent:** [Exact incompressible shearing wave](#exact-incompressible-shearing-wave)

In an incompressible [shearing sheet](#shearing-sheet), a single real-wavevector velocity and magnetic Fourier mode transverse to that wavevector has identically zero quadratic self-advection and cross-advection. Advecting its phase by background shear and stretching its spatially uniform field give the displayed evolution laws. Their opposite contributions keep the [Alfvén frequency](astrophysical-fluid-dynamics.md#alfven-frequency) constant. The resulting viscous and resistive wave-amplitude equations are exact finite-amplitude solutions; physical pressure adjusts to the quadratic magnetic-pressure terms.

###### Zero-mean magnetic shearing wave

↑ **Parent:** [Exact magnetic shearing wave](#exact-magnetic-shearing-wave)

In an incompressible [shearing sheet](#shearing-sheet) with background velocity $-2Ax\mathbf e_y$, take both the perturbation [velocity](classical-mechanics.md#velocity) and the entire [magnetic field](electromagnetism.md#magnetic-field) to be real single [Fourier modes](fourier-analysis.md#fourier-mode) with a common real [wavevector](continuum-mechanics.md#wavevector) and transverse amplitudes. Then every quadratic directional derivative vanishes, including terms involving complex conjugates. There is no uniform background magnetic field and consequently no linear magnetic-tension coupling between the amplitudes. Advecting the phase requires $\dot k_x=2Ak_y$, $\dot k_y=\dot k_z=0$. The velocity amplitude obeys $\dot{\widetilde{\mathbf v}}-2A\widetilde v_x\mathbf e_y+2\boldsymbol\Omega\times\widetilde{\mathbf v}=-i\mathbf k\widetilde\psi-\nu k^2\widetilde{\mathbf v}$; the magnetic amplitude obeys the displayed equation. The modified pressure includes [magnetic pressure](astrophysical-fluid-dynamics.md#magnetic-pressure); the physical pressure can contain a mean and second harmonic even when the modified pressure is a single mode.

###### Cubic-exponent decay of a nonaxisymmetric shearing wave

↑ **Parent:** [Zero-mean magnetic shearing wave](#zero-mean-magnetic-shearing-wave)

For a [zero-mean magnetic shearing wave](#zero-mean-magnetic-shearing-wave), the real [wavevector](continuum-mechanics.md#wavevector) satisfies $k_x=k_{x0}+2Ak_yt$, with $k_y,k_z$ constant. Dotting the velocity-amplitude equation with its [complex conjugate](complex-analysis.md#complex-conjugate) eliminates [Coriolis force](physics.md#coriolis-force) and pressure work, giving $d|\widetilde{\mathbf v}|^2/dt=4A\operatorname{Re}(\widetilde v_x\widetilde v_y^*)-2\nu k^2|\widetilde{\mathbf v}|^2$. The inequality $2|v_xv_y|\le|\mathbf v|^2$ proves the displayed bound; the magnetic bound has the same form with $\eta$ replacing $\nu$. Now

$$
\int_0^t k(s)^2\,ds=(k_{x0}^2+k_y^2+k_z^2)t+2Ak_{x0}k_yt^2+\frac43A^2k_y^2t^3.
$$

For $Ak_y\ne0$ and positive [kinematic viscosity](fluid-mechanics.md#kinematic-viscosity) and [magnetic diffusivity](astrophysical-fluid-dynamics.md#magnetic-diffusivity), the negative cubic exponent dominates the linear shear-work bound, so both amplitudes tend to zero. Transient growth is allowed. Positivity matters: an inviscid vertical velocity mode with $k_z=0$ can remain constant, and an ideal vertical magnetic mode with $k_z=0$ can also remain constant.

##### Two-dimensional viscous shearing wave

↑ **Parent:** [Exact incompressible shearing wave](#exact-incompressible-shearing-wave)

For $k_z=v_z=0$ and $k_y\ne0$, define $Z=i(k_xv_y-k_yv_x)$. Uniform rotation does not enter its evolution: $\dot Z=-\nu k^2Z$, $v_x=ik_yZ/k^2$ and $v_y=-ik_xZ/k^2$. With $T=k_x/k_y$ and $\mathrm{Re}=A/(\nu k_y^2)$, the perturbation [energy](classical-mechanics.md#energy) ratio is $E(T)/E(T_0)=[(1+T_0^2)/(1+T^2)]\exp[-(T+T^3/3-T_0-T_0^3/3)/\mathrm{Re}]$. Leading waves can gain [energy](classical-mechanics.md#energy) as shear reduces their [wavevector](continuum-mechanics.md#wavevector) magnitude, before [viscosity](fluid-mechanics.md#dynamic-viscosity) and subsequent winding damp them.

// Target: hydrodynamic-stability.bigb

###### Optimal transient amplification of a viscous shearing wave

↑ **Parent:** [Two-dimensional viscous shearing wave](#two-dimensional-viscous-shearing-wave)

For the shearing-wave [energy](classical-mechanics.md#energy) profile, stationary points satisfy $-2\mathrm{Re}\,T=(1+T^2)^2$. At large [Reynolds number](fluid-mechanics.md#reynolds-number), the initial minimum is at $T_-\sim-(2\mathrm{Re})^{1/3}$ and the subsequent maximum is at $T_+\sim-1/(2\mathrm{Re})$. Their [energy](classical-mechanics.md#energy) ratio is $G_{\max}\sim(2\mathrm{Re})^{2/3}e^{-2/3}$. The [Reynolds number](fluid-mechanics.md#reynolds-number) here uses $A$, half the background shear rate; using $2A$ instead changes the coefficient convention.

// Target: astrophysics.bigb

#### Helicity invariant of an inviscid shearing wave

↑ **Parent:** [Shearing wave](#shearing-wave)

For a solenoidal velocity amplitude $\mathbf v$ with $\mathbf k=(k_x,-\Omega tk_x,k_z)$ and $\dot{\mathbf v}+\Omega v_y\widehat{\mathbf x}=-i\mathbf kq$, differentiating $\mathbf k\cdot\mathbf v=0$ gives $q=2i\Omega k_xv_y/K^2$, where $K^2=|\mathbf k|^2$. Thus $\dot v_y=2\Omega k_xk_yv_y/K^2$ and $\dot v_z=2\Omega k_xk_zv_y/K^2$. For the real helicity quantity $H=ik_x(v_yv_z^*-v_zv_y^*)$, the mixed forcing terms cancel, leaving $\dot H=2\Omega k_xk_yH/K^2=-\dot K^2H/K^2$. Consequently

$$
H(t)K(t)^2=H(0)(k_x^2+k_z^2).
$$

The invariant is a consequence of inviscid linear shear dynamics, not a claim that $H$ itself is constant under the shear.

#### Barotropic shearing-wave gravitational amplitude system

↑ **Parent:** [Shearing wave](#shearing-wave)

A [shearing-wave ansatz](#shearing-wave-ansatz) in a uniform inviscid isothermal [shearing sheet](#shearing-sheet) removes background advection when the radial [wavevector](continuum-mechanics.md#wavevector) grows as $k_x(t)=k_x(0)+Sk_yt$. The [razor-thin disk Poisson kernel](astrophysics.md#razor-thin-disk-poisson-kernel) reduces the pressure-plus-gravity amplitude to $[c_s^2-2\pi G\Sigma_0/k]\widetilde\Sigma'/\Sigma_0$. Continuity couples it to $ik_xv_x+ik_yv_y$, while the two momentum equations have rotational couplings $-2\Omega v_y$ and $(2\Omega-S)v_x$. The [linearized vortensity](#linearized-vortensity) amplitude remains constant, because the barotropic [pressure](thermodynamics.md#pressure) and gravitational forces have zero [curl](calculus.md#curl) and the background [vortensity](#vortensity) is uniform.

#### Shearing-wave ansatz

↑ **Parent:** [Shearing wave](#shearing-wave)

The shearing-wave ansatz writes a perturbation as a time-dependent amplitude times $\exp[i k_x(t)x+i k_yy]$, choosing $k_x(t)$ so that background advection does not leave an explicit factor of position in the amplitude equations.

#### Shearing-wave oscillator

↑ **Parent:** [Shearing wave](#shearing-wave)

For an unforced inertial-acoustic disturbance, the shearing-wave amplitude obeys a time-dependent oscillator equation whose frequency depends on $k_x(t)=k_x(0)+Sk_yt$. Fourier transformation of the corresponding stationary forced equation turns radial wavenumber into the oscillator's time-like coordinate.

#### Swing of a shearing wave

↑ **Parent:** [Shearing wave](#shearing-wave)

During the swing of a shearing wave, the radial wavenumber passes through zero and the disturbance changes from leading to trailing before winding ever more tightly.

### Inertial-acoustic wave

↑ **Parent:** [Shearing sheet](#shearing-sheet)

An inertial-acoustic wave in a rotating compressible disk is restored jointly by pressure and epicyclic motion. For an axisymmetric radial wave in a Keplerian sheet, $\omega^2=\Omega^2+c_s^2k_x^2$.

#### Density-wave dispersion relation in a non-self-gravitating disk

↑ **Parent:** [Inertial-acoustic wave](#inertial-acoustic-wave)

Let $c_s^2=(dP/d\Sigma)_0$ be the [barotropic closure of a razor-thin disk](astrophysics.md#barotropic-closure-of-a-razor-thin-disk) sound-speed squared and $\kappa_r$ the [radial epicyclic frequency](astrophysics.md#radial-epicyclic-frequency), with $\kappa_r^2=2(2-q_r)\Omega^2$ for [orbital shear parameter](#orbital-shear-parameter) $q_r$. For a radial axisymmetric [normal mode](wave-equation.md#normal-mode) in a uniform barotropic [shearing sheet](#shearing-sheet), let $U_x,U_y$ be velocity amplitudes and $\sigma$ the surface-density amplitude. Linear momentum gives $-i\omega U_x=2\Omega U_y-ikc_s^2\sigma/\Sigma_0$ and $-i\omega U_y=-\kappa_r^2U_x/(2\Omega)$; mass conservation gives $\omega\sigma=k\Sigma_0U_x$. Eliminating the amplitudes for $\omega\ne0$ proves the displayed dispersion relation. The rotational term is epicyclic restoration; the [pressure](thermodynamics.md#pressure) term is acoustic restoration. Without a perturbed gravitational potential, no self-gravity term belongs in the formula.

##### Zero-frequency balanced mode of an axisymmetric disk

↑ **Parent:** [Density-wave dispersion relation in a non-self-gravitating disk](#density-wave-dispersion-relation-in-a-non-self-gravitating-disk)

Besides the two propagating [inertial-acoustic wave](#inertial-acoustic-wave) branches, a uniform barotropic [Keplerian shearing sheet](#keplerian-shearing-sheet) has a stationary branch balancing [pressure](thermodynamics.md#pressure) against [Coriolis acceleration](physics.md#coriolis-acceleration). For radial wavenumber $k\ne0$, setting $\omega=0$ in continuity gives $U_x=0$, and radial momentum gives the displayed azimuthal balance. The full determinant is proportional to $\omega(\omega^2-\Omega^2-c_s^2k^2)$. At $k=0$ the stationary branch is a uniform column-density change; it is not a travelling density wave.

### Satellite-forced density wave in an astrophysical disk

↑ **Parent:** [Shearing sheet](#shearing-sheet)

A satellite-forced density wave is a compressive disk response to the satellite's periodic tidal potential. In a local corotating sheet, propagating zones lie where the relative orbital motion is supersonic.

### Thermal relaxation in a self-gravitating disk

↑ **Parent:** [Shearing sheet](#shearing-sheet)

Thermal relaxation drives the local sound speed toward an equilibrium value on a cooling time $\tau$. Fast relaxation gives an isothermal response, while slow relaxation gives an adiabatic response.

### Shearing-sheet tidal potential

↑ **Parent:** [Shearing sheet](#shearing-sheet)

For a frame rotating about a Keplerian circular orbit, radial gravity and centrifugal acceleration combine to give $\Phi_t=-3\Omega^2x^2/2$.

#### Isothermal shearing-sheet energy conservation

↑ **Parent:** [Shearing-sheet tidal potential](#shearing-sheet-tidal-potential)

For constant [isothermal sound speed](compressible-flow.md#isothermal-sound-speed), time-independent [shearing-sheet tidal potential](#shearing-sheet-tidal-potential) $\Phi_t$, and inviscid flow, define $E=\Sigma u^2/2+c_s^2\Sigma\ln(\Sigma/\Sigma_{\rm ref})+\Sigma\Phi_t$. The [barotropic energy density](fluid-mechanics.md#barotropic-energy-density) and [kinetic energy](classical-mechanics.md#kinetic-energy) balances combine to give $\partial_tE+\nabla\cdot[(E+P)\mathbf u]=0$. [Coriolis acceleration](physics.md#coriolis-acceleration) does no work. Integral conservation requires vanishing net boundary [energy flux](physics.md#energy-flux).

### Viscous-convective instability

↑ **Parent:** [Shearing sheet](#shearing-sheet)

Viscous-convective instability is slow growth in a rotating fluid with an adverse buoyancy gradient when viscosity weakens epicyclic stabilization.

## ↑ Ancestors (5)

1. [Astrophysical disk](astrophysics.md#astrophysical-disk)
2. [Astrophysics](astrophysics.md)
3. [Branches of physics](physics.md#branches-of-physics)
4. [Physics](physics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (3)

- [Core accretion](planetary-science.md#core-accretion)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-57.md#2/f/solution)
- [Self-gravity](classical-mechanics.md#self-gravity)
