# Paper 2

↑ **Parent:** [2014](../2014.md)

[Original public PDF, physical pages 164–169; examination dated 5 June 2014](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=164)

**Table of contents**

- [Section A](#section-a)
  - [A1](#section-a/a1)
    - [Solution](#section-a/a1/solution)
  - [A2](#section-a/a2)
    - [Solution](#section-a/a2/solution)
  - [A3](#section-a/a3)
    - [Solution](#section-a/a3/solution)
  - [A4](#section-a/a4)
    - [Solution](#section-a/a4/solution)
  - [A5](#section-a/a5)
    - [Solution](#section-a/a5/solution)
- [Section B](#section-b)
  - [B6](#section-b/b6)
    - [a](#section-b/b6/a)
      - [Solution](#section-b/b6/a/solution)
    - [b](#section-b/b6/b)
      - [Solution](#section-b/b6/b/solution)
    - [c](#section-b/b6/c)
      - [Solution](#section-b/b6/c/solution)
    - [d](#section-b/b6/d)
      - [Solution](#section-b/b6/d/solution)
  - [B7](#section-b/b7)
    - [Solution](#section-b/b7/solution)
  - [B8](#section-b/b8)
    - [a](#section-b/b8/a)
      - [Solution](#section-b/b8/a/solution)
    - [b](#section-b/b8/b)
      - [Solution](#section-b/b8/b/solution)
    - [c](#section-b/b8/c)
      - [Solution](#section-b/b8/c/solution)
    - [d](#section-b/b8/d)
      - [Solution](#section-b/b8/d/solution)
  - [B9](#section-b/b9)
    - [Solution](#section-b/b9/solution)
- [Section C](#section-c)
  - [C10](#section-c/c10)
    - [Solution](#section-c/c10/solution)
    - [a](#section-c/c10/a)
      - [Solution](#section-c/c10/a/solution)
    - [b](#section-c/c10/b)
      - [Solution](#section-c/c10/b/solution)
    - [Solution (cycle calculations)](#section-c/c10/solution-cycle-calculations)
  - [C11](#section-c/c11)
    - [Solution](#section-c/c11/solution)
    - [a](#section-c/c11/a)
      - [Solution](#section-c/c11/a/solution)
    - [b](#section-c/c11/b)
      - [Solution](#section-c/c11/b/solution)
    - [c](#section-c/c11/c)
      - [Solution](#section-c/c11/c/solution)
    - [Solution (film calculations)](#section-c/c11/solution-film-calculations)
  - [C12](#section-c/c12)
    - [Solution](#section-c/c12/solution)
  - [C13](#section-c/c13)
    - [Solution](#section-c/c13/solution)

## Section A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-a/a1">A1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a1/solution">Solution</h4>

↑ **Parent:** [A1](#section-a/a1)

Treat the vapour as an [ideal gas](../../ideal-gas.md), neglect the liquid's [molar volume](../../thermodynamics.md#molar-volume), and take the molar [latent heat](../../thermodynamic-potential.md#latent-heat) as constant across this small interval. Integrating the [Clausius-Clapeyron equation](../../thermodynamic-potential.md#clausius-clapeyron-relation) gives

$$
\ln\frac{p_2}{p_1}=\frac{L_m}{R}\left(\frac1{T_1}-\frac1{T_2}\right),
\qquad
\boxed{L_m=\frac{R\ln(1.1)}{1/230.7-1/233.4}
\simeq15.8\,\mathrm{kJ\,mol^{-1}}.}
$$

Only the [pressure](../../pressure.md) ratio enters, so conversion from atmospheres to pascals is unnecessary.

<h3 id="section-a/a2">A2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a2/solution">Solution</h4>

↑ **Parent:** [A2](#section-a/a2)

The [Hohmann transfer orbit](../../celestial-mechanics.md#hohmann-transfer-orbit) has [periapsis](../../celestial-mechanics.md#periapsis) $r$ and [apoapsis](../../celestial-mechanics.md#apoapsis) $2r$, so its [semi-major axis](../../celestial-mechanics.md#semi-major-axis) is $3r/2$. [Kepler's third law](../../mathematical-physics.md#kepler-s-third-law) gives a period $(3/2)^{3/2}$ times the original [orbital period](../../celestial-mechanics.md#orbital-period). Only half the [ellipse](../../euclidean-geometry.md#ellipse) is traversed:

$$
\boxed{t=\frac{T_0}{2}\left(\frac32\right)^{3/2}
\simeq22.0\,\mathrm h,\qquad T_0\simeq24\,\mathrm h.}
$$

The relevant radii are measured from [Earth](../../planetary-science.md#earth)'s centre, not its surface.

<h3 id="section-a/a3">A3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a3/solution">Solution</h4>

↑ **Parent:** [A3](#section-a/a3)

Use $N$ turns of mean radius $a\simeq1.05\,\mathrm{mm}$, including the wire radius, on a light nonmagnetic rod. With wire radius $r_w$, length $l$ and [density](../../fluid-mechanics.md#density) $\rho$, neglecting helical pitch gives

$$
m_B=NI\pi a^2,\qquad M=2\pi aN\rho\pi r_w^2,
\qquad J=M\left(\frac{l^2}{12}+\frac{a^2}{2}\right).
$$

The last expression is the transverse central [moment of inertia](../../rigid-body-dynamics.md#moment-of-inertia) of the uniformly distributed turns. The [magnetic torque](../../astrophysical-disk.md#surface-magnetic-torque-on-an-accretion-disk) is $-m_BB_h\sin\theta$, so the [small-angle magnetic dipole oscillation](../../electromagnetism.md#small-angle-magnetic-dipole-oscillation) obeys $J\ddot\theta+m_BB_h\theta=0$. Hence

$$
\boxed{T=2\pi\sqrt{\frac{2\pi\rho r_w^2}{IaB_h}
\left(\frac{l^2}{12}+\frac{a^2}{2}\right)}\simeq4.0\,\mathrm s.}
$$

The number of turns cancels. Taking the turn radius as $1.00\,\mathrm{mm}$ instead gives $4.04\,\mathrm s$, consistent at the accuracy of the thin-winding model. The rod's inertia, damping and lead-wire [torque](../../momentum.md#torque) are neglected.

<h3 id="section-a/a4">A4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a4/solution">Solution</h4>

↑ **Parent:** [A4](#section-a/a4)

For slow gyroscopic [precession](../../rigid-body-dynamics.md#precession), the gravitational [torque](../../momentum.md#torque) turns the spin [angular momentum](../../momentum.md#angular-momentum): $Mg\ell\sin\theta=\Omega I_3\omega\sin\theta$, with $I_3=MR^2/2$. Thus

$$
\Omega\simeq\frac{2g\ell}{R^2\omega},\qquad
\boxed{T_p\simeq\frac{\pi R^2\omega}{g\ell}
=1.61\,\mathrm s,\qquad\omega=40\pi\,\mathrm{s^{-1}}.}
$$

The inclination cancels at this order. More precisely, [uniform precession of a heavy symmetric top](../../rigid-body-dynamics.md#uniform-precession-of-a-heavy-symmetric-top) satisfies

$$
\frac{I_1}{M}\cos\theta\,\Omega^2
-\frac{I_3}{M}\omega\Omega+g\ell=0,
\qquad \frac{I_1}{M}=\frac{R^2}{4}+\ell^2.
$$

Its slow root gives $T_p\simeq1.57\,\mathrm s$. **About $1.6\,\mathrm s$** is the slow-precession answer; arbitrary initial conditions can also produce [nutation](../../rigid-body-dynamics.md#nutation) rather than exact steady [precession](../../rigid-body-dynamics.md#precession).

<h3 id="section-a/a5">A5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a5/solution">Solution</h4>

↑ **Parent:** [A5](#section-a/a5)

For a [waveguide](../../wave.md#waveguide) mode in a homogeneous nondispersive filling, $\omega^2=\omega_c^2+v^2k_z^2$. Its [phase velocity](../../dispersion-relation.md#phase-velocity) is $v_p=\omega/k_z$ and its [group velocity](../../dispersion-relation.md#group-velocity) is $v_g=d\omega/dk_z=v^2k_z/\omega$, giving

$$
\boxed{\frac{v_g}{v_p}=1-\frac{\omega_c^2}{\omega^2}
=1-\frac19=\frac89.}
$$

## Section B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/a">a</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b6/a)

The [Biot-Savart law](../../electromagnetism.md#biot-savart-law) gives the [magnetic field](../../magnetic-field.md) of a steady thin-wire [electric current](../../electric-charge.md#electric-current) in vacuum:

$$
\mathbf B(\mathbf r)=\frac{\mu_0I}{4\pi}
\int\frac{d\boldsymbol\ell'\times(\mathbf r-\mathbf r')}
{|\mathbf r-\mathbf r'|^3}.
$$

The cross product fixes the circulation direction by the [right-hand rule](../../electromagnetism.md#right-hand-rule); fields from different [electric current](../../electric-charge.md#electric-current) elements superpose. Integration gives $B=\mu_0I/(2\pi r)$ outside a straight infinite wire and $B=\mu_0I/(2a)$ at the centre of a circular loop of radius $a$. A distributed [electric current](../../electric-charge.md#electric-current) replaces $I\,d\boldsymbol\ell'$ by $\mathbf J\,dV'$. **This is a magnetostatic law:** arbitrary time-dependent [electric currents](../../electric-charge.md#electric-current) require retarded electromagnetic fields, not instantaneous substitution.

<h4 id="section-b/b6/b">b</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b6/b)

In [magnetostatics](../../electromagnetism.md#magnetostatics), [Ampère's circuital law](../../maxwell-equations.md#ampere-s-circuital-law) in vacuum is

$$
\oint_C\mathbf B\cdot d\boldsymbol\ell=\mu_0I_{\rm enc},
\qquad\nabla\times\mathbf B=\mu_0\mathbf J.
$$

It is especially useful when symmetry makes the tangential field constant on an [Amperian loop](../../maxwell-equations.md#amperian-loop). It gives $B=\mu_0I/(2\pi r)$ for an infinite straight wire, $B\simeq\mu_0nI$ inside a long [solenoid](../../magnetic-field.md#solenoid), and $B\simeq\mu NI/(2\pi r)$ in an ideal [toroid](../../differential-geometry.md#toroid). The long-solenoid and toroidal expressions neglect fringing.

For time-dependent fields, [displacement current](../../maxwell-equations.md#displacement-current) is essential:

$$
\oint_C\mathbf B\cdot d\boldsymbol\ell
=\mu_0I_{\rm enc}+\mu_0\epsilon_0\frac{d\Phi_E}{dt}.
$$

In matter, the corresponding macroscopic form is $\oint\mathbf H\cdot d\boldsymbol\ell=I_{\rm free}+d\!\int\mathbf D\cdot d\mathbf A/dt$. **The enclosed [electric current](../../electric-charge.md#electric-current) alone is sufficient only in the magnetostatic limit.**

<h4 id="section-b/b6/c">c</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b6/c)

Because $\nabla\cdot\mathbf B=0$, a [magnetic vector potential](../../electromagnetism.md#magnetic-vector-potential) can be introduced with $\mathbf B=\nabla\times\mathbf A$. It is not unique: $\mathbf A+\nabla\chi$ gives the same field. In [magnetostatics](../../electromagnetism.md#magnetostatics), the [Coulomb gauge](../../electromagnetism.md#coulomb-gauge) $\nabla\cdot\mathbf A=0$ gives $\nabla^2\mathbf A=-\mu_0\mathbf J$ in vacuum. For localized [electric currents](../../electric-charge.md#electric-current),

$$
\mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\int
\frac{\mathbf J(\mathbf r')}{|\mathbf r-\mathbf r'|}\,dV'.
$$

A [magnetic scalar potential](../../electromagnetism.md#magnetic-scalar-potential) is more restricted. In a simply connected current-free region of constant permeability, write $\mathbf B=-\nabla\psi$; then $\nabla^2\psi=0$. Alternatively define the scalar potential for $\mathbf H$, differing by a constant permeability factor. **A single-valued scalar potential generally cannot cover a domain encircling a net [electric current](../../electric-charge.md#electric-current)**, even where the local curl vanishes. The [vector](../../vector-space.md#vector) potential does not require the field itself to be curl-free.

<h4 id="section-b/b6/d">d</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b6/d)

Guided electromagnetic waves propagate along a structure whose boundaries select transverse field patterns. At a perfect conductor the tangential [electric field](../../electric-field.md) vanishes. In a hollow rectangular guide, TE modes have $E_z=0$ and TM modes have $H_z=0$. Their longitudinal [wavenumber](../../wave-equation.md#wavenumber) obeys

$$
k_z^2=\frac{\omega^2}{v^2}-k_\perp^2,
\qquad k_\perp^2=\left(\frac{m\pi}{a}\right)^2+
\left(\frac{n\pi}{b}\right)^2.
$$

Below the [waveguide cutoff frequency](../../electromagnetic-wave.md#waveguide-cutoff-frequency) $\omega_c=vk_\perp$, that mode is evanescent rather than freely propagating. TM modes require both indices positive; TE modes may have one zero but not both. For $a>b$, the lowest cutoff is the TE$_{10}$ mode, with $f_c=v/(2a)$. A hollow single-conductor guide has no TEM mode, whereas a two-conductor transmission line can support one without this geometrical cutoff.[§13.4, mode boundary conditions, index restrictions and lowest-cutoff discussion](../../physics-bibliography.md#electromagnetic-fields-and-energy-by-hermann-a-haus-and-james-r-melcher/rectangular-waveguide-modes)

For a propagating TE or TM mode, $v_p=v/\sqrt{1-\omega_c^2/\omega^2}$ and $v_g=v\sqrt{1-\omega_c^2/\omega^2}$. The [phase velocity](../../dispersion-relation.md#phase-velocity) can exceed $v$ without superluminal information transfer. Frequency-dependent group delay can broaden pulses; excitation of several modes adds intermodal [dispersion](../../dispersion-relation.md#wave-dispersion).

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

[Electromagnetic induction](../../electromagnetism.md#electromagnetic-induction) produces an [electromotive force](../../electric-charge.md#electromotive-force) when [magnetic flux linkage](../../electromagnetism.md#magnetic-flux-linkage) changes. For an oriented moving loop,

$$
\mathcal E=\oint(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell
=-\frac{d\Phi_B}{dt}.
$$

For a stationary loop this reduces to [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction), $\nabla\times\mathbf E=-\partial_t\mathbf B$. Motion in a static field can instead supply the motional term. [Lenz's law](../../maxwell-equations.md#lenz-s-law) gives the minus sign: the induced [electric current](../../electric-charge.md#electric-current) opposes the flux change, with the required electrical [energy](../../energy.md) supplied by mechanical [work](../../energy.md#work) or the field source.

For linear fixed-geometry circuits, flux linkages satisfy $\Lambda_1=L_1I_1+MI_2$ and $\Lambda_2=MI_1+L_2I_2$. [Self-inductance](../../electromagnetism.md#self-inductance) gives $\mathcal E_1=-L_1\dot I_1$; [mutual inductance](../../electromagnetism.md#mutual-inductance) gives the additional term $-M\dot I_2$. Reciprocity gives the same mutual coefficient for both circuits, with its sign determined by winding orientation. The stored field [energy](../../energy.md) is

$$
W_B=\frac12L_1I_1^2+\frac12L_2I_2^2+MI_1I_2,
\qquad |M|\le\sqrt{L_1L_2}.
$$

The bound follows from nonnegative [energy](../../energy.md) for arbitrary [electric currents](../../electric-charge.md#electric-current). In a linear medium the equivalent field expression is $W_B=\tfrac12\int\mathbf B\cdot\mathbf H\,dV$.

An ideal [electrical transformer](../../electrical-engineering.md#transformer-electrical-engineering) links both windings with one changing core flux, giving $V_1/V_2=N_1/N_2$ for corresponding voltage magnitudes. A loaded secondary drives an opposing magnetomotive force and increases primary [electric current](../../electric-charge.md#electric-current); ideally $I_1/I_2=N_2/N_1$ and input and output powers agree. **A [electrical transformer](../../electrical-engineering.md#transformer-electrical-engineering) exchanges voltage for [electric current](../../electric-charge.md#electric-current), not for extra [power](../../energy.md#power).** Real devices have winding resistance, leakage flux, eddy-current and [hysteresis](../../critical-phenomenon.md#hysteresis) losses, and finite magnetizing [electric current](../../electric-charge.md#electric-current). A steady DC input gives no continuing secondary voltage after the switching transient and may cause excessive primary [electric current](../../electric-charge.md#electric-current) or core saturation.

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/a">a</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b8/a)

An isotropic linear elastic solid has two independent elastic constants. For infinitesimal [strain](../../continuum-mechanics.md#strain),

$$
\sigma_{ij}=2G\epsilon_{ij}+\lambda\epsilon_{kk}\delta_{ij},
\qquad K=\lambda+\frac23G.
$$

The [shear modulus](../../elasticity-physics.md#shear-modulus) $G$ governs shape change and the [bulk modulus](../../elasticity-physics.md#bulk-modulus) $K$ governs volume change. [Young's modulus](../../elasticity-physics.md#young-s-modulus) $E$ and [Poisson's ratio](../../elasticity-physics.md#poisson-s-ratio) $\nu$ are equivalent parameters:

$$
G=\frac{E}{2(1+\nu)},\qquad K=\frac{E}{3(1-2\nu)}.
$$

Positive [strain](../../continuum-mechanics.md#strain) [energy](../../energy.md) requires $G,K>0$, hence $-1<\nu<1/2$; $\nu\to1/2$ is the incompressible limit. Small-amplitude bulk waves have speeds $c_P=\sqrt{(K+4G/3)/\rho}$ and $c_S=\sqrt{G/\rho}$. **Isotropy removes directional dependence, not the distinction between compression and shear.** These laws apply within the elastic small-strain regime, not after yielding or fracture.

<h4 id="section-b/b8/b">b</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b8/b)

For a rigid body about a chosen origin,

$$
I_{ij}=\int\rho(\mathbf r)(r^2\delta_{ij}-r_ir_j)\,dV,
\qquad \mathbf L=\mathbf I\boldsymbol\omega,
\qquad T_{\rm rot}=\frac12\boldsymbol\omega\cdot\mathbf I\boldsymbol\omega.
$$

The [inertia tensor](../../rigid-body-dynamics.md#inertia-tensor) is real and symmetric, so [orthogonal](../../inner-product.md#orthogonal-vectors) [principal axes](../../rigid-body-dynamics.md#principal-axis) diagonalize it. [Angular momentum](../../momentum.md#angular-momentum) is parallel to [angular velocity](../../rigid-body-dynamics.md#angular-velocity) for rotation about a [principal axis](../../rigid-body-dynamics.md#principal-axis), but need not be parallel in a general direction. Its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are the [principal moments of inertia](../../rigid-body-dynamics.md#principal-moment-of-inertia).

If the origin is translated from the [centre of mass](../../classical-mechanics.md#center-of-mass) by $\mathbf a$, the parallel-axis theorem becomes $I_{ij}=I_{ij}^{\rm CM}+M(a^2\delta_{ij}-a_ia_j)$. In body axes, Euler's equation is $\boldsymbol\tau=(d\mathbf L/dt)_{\rm body}+\boldsymbol\omega\times\mathbf L$. Thus **the full [tensor](../../multilinear-algebra.md#tensor) is needed whenever the rotation is not confined to one fixed [principal axis](../../rigid-body-dynamics.md#principal-axis)**.

<h4 id="section-b/b8/c">c</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b8/c)

For two bodies interacting through $U(\mathbf r_1-\mathbf r_2)$, define

$$
\mathbf R=\frac{m_1\mathbf r_1+m_2\mathbf r_2}{M},\quad
\mathbf r=\mathbf r_1-\mathbf r_2,\quad
M=m_1+m_2,\quad\mu=\frac{m_1m_2}{M}.
$$

Their [kinetic energy](../../energy.md#kinetic-energy) separates exactly:

$$
T=\frac12M\dot{\mathbf R}^{\,2}+\frac12\mu\dot{\mathbf r}^{\,2}.
$$

Without external forces, the [centre of mass](../../classical-mechanics.md#center-of-mass) moves uniformly while $\mu\ddot{\mathbf r}=-\nabla U$. **The relative orbit is a one-body problem with [reduced mass](../../classical-mechanics.md#reduced-mass) $\mu$**, not generally either individual [mass](../../classical-mechanics.md#mass). For $m_2\gg m_1$, $\mu\simeq m_1$; for equal masses $m$, $\mu=m/2$. If the interaction is central, relative [angular momentum](../../momentum.md#angular-momentum) is conserved and the relative motion is planar.

<h4 id="section-b/b8/d">d</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b8/d)

[Dynamic viscosity](../../dynamic-viscosity.md) measures resistance to a [velocity](../../classical-mechanics.md#velocity) gradient. In Newtonian simple shear, $\tau_{xy}=\eta\,\partial u_x/\partial y$; positive [viscosity](../../dynamic-viscosity.md) dissipates mechanical [energy](../../energy.md) into [heat](../../heat.md). [Kinematic viscosity](../../dynamic-viscosity.md#kinematic-viscosity) is $\nu=\eta/\rho$. For an incompressible fluid of constant [viscosity](../../dynamic-viscosity.md),

$$
\rho\left(\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u\right)
=-\nabla p+\eta\nabla^2\mathbf u+\mathbf f.
$$

Scaling [velocity](../../classical-mechanics.md#velocity) by $U$ and length by $L$ gives the [Reynolds number](../../dynamic-viscosity.md#reynolds-number) $\mathrm{Re}=\rho UL/\eta=UL/\nu$, the ratio of inertial to viscous terms. At small [Reynolds number](../../dynamic-viscosity.md#reynolds-number), creeping-flow approximations neglect inertia; at large [Reynolds number](../../dynamic-viscosity.md#reynolds-number), inertia dominates much of the bulk but [viscosity](../../dynamic-viscosity.md) can remain crucial in boundary layers. **A large [Reynolds number](../../dynamic-viscosity.md#reynolds-number) permits instability and [turbulence](../../turbulence.md); it does not by itself specify a universal transition threshold.** Geometry and disturbances also matter.

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

A [central potential](../../energy.md#central-potential) conserves [angular momentum](../../momentum.md#angular-momentum) and confines a nonradial orbit to a plane. With [reduced mass](../../classical-mechanics.md#reduced-mass) $\mu$, the radial motion obeys

$$
E=\frac12\mu\dot r^2+U_{\rm eff}(r),\qquad
U_{\rm eff}=U(r)+\frac{L^2}{2\mu r^2}.
$$

Turning points satisfy $E=U_{\rm eff}$. A radially bounded allowed interval gives bound motion, whereas an interval reaching infinity permits escape. The [energy](../../energy.md) sign alone classifies these only with suitable assumptions about $U(\infty)$ and barriers. Circular orbits satisfy $U_{\rm eff}'=0$ and are radially stable when $U_{\rm eff}''>0$. Bound orbits in a general [central potential](../../energy.md#central-potential) need not close: successive periapses can precess.

For attractive inverse-square gravity, $U=-\kappa/r$ and

$$
r=\frac{p}{1+e\cos\phi},\quad p=\frac{L^2}{\mu\kappa},\quad
 e^2=1+\frac{2EL^2}{\mu\kappa^2}.
$$

Ellipses have $E<0$, $e<1$, and the attracting centre at a focus; parabolic and hyperbolic escape have $e=1$ and $e>1$. Conservation of [angular momentum](../../momentum.md#angular-momentum) gives equal swept areas in equal times. The inverse-square law additionally yields $T^2=4\pi^2a^3/[G(m_1+m_2)]$. These are Kepler's laws; a harmonic [central potential](../../energy.md#central-potential) is another example with closed bound orbits, while generic central laws produce [precession](../../rigid-body-dynamics.md#precession).

In a [gravitational assist](../../celestial-mechanics.md#gravitational-assist), a spacecraft's asymptotic [speed](../../classical-mechanics.md#speed) relative to a planet is approximately unchanged but its direction turns. Transforming to the frame in which the planet has [velocity](../../classical-mechanics.md#velocity) $\mathbf V$ gives

$$
\Delta\varepsilon=\mathbf V\cdot(\mathbf u_{\rm out}-\mathbf u_{\rm in}).
$$

The spacecraft can gain or lose orbital [energy](../../energy.md); the planet supplies the compensating [energy](../../energy.md) and [momentum](../../momentum.md), with a very small [velocity](../../classical-mechanics.md#velocity) change because of its large [mass](../../classical-mechanics.md#mass).

Repulsive Coulomb scattering instead has $U=\kappa_C/r$. For incident relative [kinetic energy](../../energy.md#kinetic-energy) $E$ and [impact parameter](../../classical-mechanics.md#impact-parameter) $b$, the hyperbolic orbit gives

$$
b=\frac{\kappa_C}{2E}\cot\frac\theta2,\qquad
\boxed{\frac{d\sigma}{d\Omega}=\left(\frac{\kappa_C}{4E}\right)^2
\csc^4\frac\theta2.}
$$

This [Rutherford scattering](../../atomic-physics.md#rutherford-scattering) formula follows by equating the incident annulus $2\pi b\,db$ to the scattered solid-angle ring. It assumes classical elastic scattering by a point Coulomb centre; screening, finite nuclear size or quantum effects can change the applicable regime.

## Section C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

A [heat engine](../../thermodynamics.md#heat-engine) operates cyclically, absorbing [heat](../../heat.md) $Q_h$ from a hotter source, rejecting [heat](../../heat.md) $Q_c$ to a colder sink and delivering net [work](../../energy.md#work) $W=Q_h-Q_c$. Its efficiency is $\eta=W/Q_h$. The working substance returns to its original state; the reservoirs and surroundings need not.

<h4 id="section-c/c10/a">a</h4>

↑ **Parent:** [C10](#section-c/c10)

<h5 id="section-c/c10/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c10/a)

Suppose an engine were more efficient than a reversible Carnot engine between the same reservoirs. Couple it to a reversed Carnot engine, scaling the cycles to have equal [work](../../energy.md#work). With no net external [work](../../energy.md#work), their combined effect would be to transfer [heat](../../heat.md) from the colder reservoir to the hotter one, contradicting the [Second law of thermodynamics](../../second-law-of-thermodynamics.md). **No such engine can exceed $\eta_C=1-T_c/T_h$.** Equivalently, the cyclic [entropy](../../entropy.md) inequality gives $-Q_h/T_h+Q_c/T_c\ge0$, hence the same bound.

<h4 id="section-c/c10/b">b</h4>

↑ **Parent:** [C10](#section-c/c10)

<h5 id="section-c/c10/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c10/b)

The reversible working substance changes [entropy](../../entropy.md) by $Q_h/T_h$ on its hot isotherm and $-Q_c/T_c$ on its cold isotherm, with zero change on the two reversible adiabats. Closure requires $Q_h/T_h=Q_c/T_c$. The substance has zero [entropy](../../entropy.md) change over a cycle, while the reservoirs have changes $-Q_h/T_h$ and $Q_c/T_c$. Thus **$\Delta S_{\rm universe}=0$** for the complete [Carnot cycle](../../second-law-of-thermodynamics.md#carnot-cycle).

<h4 id="section-c/c10/solution-cycle-calculations">Solution (cycle calculations)</h4>

↑ **Parent:** [C10](#section-c/c10)

Put $P_*=p_1V_1=nRT_1$. For the specified [ideal gas](../../ideal-gas.md), $C_V=3nR/2$, $C_p=5nR/2$ and $\gamma=5/3$. Isobaric expansion doubles [temperature](../../temperature.md), so $T_2=2T_1$. Reversible adiabatic closure gives $TV^{\gamma-1}=\mathrm{constant}$, hence

$$
x\equiv\frac{T_3}{T_1}=2^{-2/3}=0.62996,
\qquad
\boxed{W_{31}^{\rm on}=\frac32(1-x)P_*=0.5551P_*.}
$$

There is no [heat](../../heat.md) input on that compression. The other stages give

$$
Q_{12}=\frac52P_*,\quad W_{12}^{\rm by}=P_*,\quad
\boxed{Q_{23}=\frac32(x-2)P_*=-2.0551P_*.}
$$

Therefore $W_{\rm net}^{\rm by}=P_*-W_{31}^{\rm on}=0.44494P_*$ and

$$
\boxed{\eta=\frac{0.44494}{2.5}=0.17798\simeq17.8\%.}
$$

The hot reservoir changes [entropy](../../entropy.md) by $-Q_{12}/(2.5T_1)=-P_*/T_1$. The cold reservoir changes by $-Q_{23}/(0.5T_1)=4.11012P_*/T_1$. Since the gas completes a cycle,

$$
\boxed{\Delta S_{\rm universe}=3.11012\,\frac{p_1V_1}{T_1}>0.}
$$

Although the mechanical paths can be quasistatic, [heat](../../heat.md) flows across finite [temperature](../../temperature.md) differences in both contacts. This [entropy](../../entropy.md) generation explains why the efficiency is well below the Carnot value $1-0.5/2.5=80\%$ between these reservoirs.

For an isothermal final compression at $T_1$, the preceding constant-volume cooling must instead end at $T_3=T_1$; keeping the old state 3 would not close the cycle. Compression then requires [work](../../energy.md#work) $P_*\ln2$, while the [heat](../../heat.md) input remains $5P_*/2$. Thus

$$
\boxed{\eta_{\rm iso}=\frac{1-\ln2}{5/2}=0.12274\simeq12.3\%,}
$$

which is **lower**: this isothermal compression occurs at a higher [temperature](../../temperature.md) throughout than the original adiabat and consumes more [work](../../energy.md#work). It also rejects [heat](../../heat.md) during compression.

<a id="section-c/c10/image-energy-balance-and-entropy-production-in-each-stage-of-the-three-stage-engine"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2-b2-cycle-balances.png)

**[Figure 1](#section-c/c10/image-energy-balance-and-entropy-production-in-each-stage-of-the-three-stage-engine). Energy balance and entropy production in each stage of the three-stage engine**.

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/solution">Solution</h4>

↑ **Parent:** [C11](#section-c/c11)

With $F=U-TS$, the [thermodynamics of a liquid film](../../surface-tension.md#thermodynamics-of-a-liquid-film) gives

$$
\boxed{dF=-S\,dT+\gamma\,dA.}
$$

Equality of mixed derivatives of $F(T,A)$ gives the [Maxwell relation](../../thermodynamics.md#maxwell-relations)

$$
\boxed{\left(\frac{\partial S}{\partial A}\right)_T
=-\left(\frac{\partial\gamma}{\partial T}\right)_A.}
$$

Use the [area](../../differential-geometry.md#surface-area) convention already specified by $\gamma\,dA$; do not insert an additional factor for two film faces.

<h4 id="section-c/c11/a">a</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/a/solution">Solution</h5>

↑ **Parent:** [A](#section-c/c11/a)

Since $\gamma'=d\gamma/dT<0$, the [Maxwell relation](../../thermodynamics.md#maxwell-relations) gives $(\partial S/\partial A)_T=-\gamma'>0$. Thus **isothermal stretching increases the film's [entropy](../../entropy.md)**.

<h4 id="section-c/c11/b">b</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/b/solution">Solution</h5>

↑ **Parent:** [B](#section-c/c11/b)

At fixed [area](../../differential-geometry.md#surface-area), $(\partial S/\partial T)_A=C_A/T$. Therefore

$$
dS=\frac{C_A}{T}\,dT-\gamma'\,dA.
$$

For reversible adiabatic stretching, $dS=0$ and

$$
\boxed{\left(\frac{dT}{dA}\right)_S=\frac{T\gamma'}{C_A}<0.}
$$

The film **cools**, assuming positive [heat capacity](../../heat.md#heat-capacity). Adiabaticity alone would not ensure constant [entropy](../../entropy.md) if the deformation were irreversible.

<h4 id="section-c/c11/c">c</h4>

↑ **Parent:** [C11](#section-c/c11)

<h5 id="section-c/c11/c/solution">Solution</h5>

↑ **Parent:** [C](#section-c/c11/c)

Substitute the [entropy](../../entropy.md) differential into the given first law:

$$
dU=T\left(\frac{C_A}{T}dT-\gamma'dA\right)+\gamma dA,
\qquad
\boxed{dU=C_A\,dT+(\gamma-T\gamma')\,dA.}
$$

<h4 id="section-c/c11/solution-film-calculations">Solution (film calculations)</h4>

↑ **Parent:** [C11](#section-c/c11)

Reading the approximately straight trend in the supplied graph gives $\gamma(330\,\mathrm K)\simeq22\,\mathrm{mN\,m^{-1}}$ and $\gamma'\simeq-0.13\,\mathrm{mN\,m^{-1}\,K^{-1}}$. These are graph-read estimates, not more precise material constants. For $\Delta A=10^{-4}\,\mathrm{m^2}$, reversible isothermal stretching gives

$$
\boxed{W_{\rm on}=\gamma\Delta A\simeq2.2\,\mathrm{\mu J},
\qquad Q=T\Delta S=-T\gamma'\Delta A\simeq4.3\,\mathrm{\mu J}.}
$$

Both are positive: stretching does mechanical [work](../../energy.md#work) on the film and requires [heat](../../heat.md) input to prevent cooling. Its [internal energy](../../internal-energy.md) increases by about $6.5\,\mathrm{\mu J}$.

Write $\gamma=\alpha-\beta T$, with $\beta=-\gamma'\simeq1.3\times10^{-4}\,\mathrm{J\,m^{-2}\,K^{-1}}$. Constant $C_A$ then makes the reversible adiabatic condition

$$
\boxed{C_A\ln(T/T_*)+\beta A=\mathrm{constant},}
$$

where $T_*$ is an arbitrary fixed reference [temperature](../../temperature.md); absorbing it into the constant gives the requested logarithm convention. Hence

$$
T_f=T_i e^{-\beta\Delta A/C_A},\qquad
\boxed{\Delta T\simeq-\frac{\beta T_i\Delta A}{C_A}
\simeq-6.1\times10^{-5}\,\mathrm K.}
$$

Here $C_A=0.070\,\mathrm{J\,K^{-1}}$. Since $\gamma-T\gamma'=\alpha$, integration gives $\Delta U=C_A(T_f-T_i)+\alpha\Delta A$. To first order this is

$$
\boxed{\Delta U\simeq\gamma(T_i)\Delta A\simeq+2.2\,\mathrm{\mu J}.}
$$

There is no [heat](../../heat.md) exchange on this reversible adiabat. **Cooling and increasing [internal energy](../../internal-energy.md) are compatible:** positive [area](../../differential-geometry.md#surface-area) [work](../../energy.md#work) more than offsets the decrease of the temperature-dependent [energy](../../energy.md) term.

<h3 id="section-c/c12">C12</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c12/solution">Solution</h4>

↑ **Parent:** [C12](#section-c/c12)

In the [canonical ensemble](../../canonical-ensemble.md), $Z(\beta)=\sum_i e^{-\beta E_i}$ normalizes the probabilities $p_i=e^{-\beta E_i}/Z$. For temperature-independent levels,

$$
\boxed{\overline E=-\frac{1}{Z}\frac{dZ}{d\beta}
=-\frac{d\ln Z}{d\beta},\qquad
C=\frac{d\overline E}{dT}
=-\frac{1}{k_BT^2}\frac{d\overline E}{d\beta}.}
$$

The [derivative](../../calculus.md#derivative) holds external parameters, including [magnetic field](../../magnetic-field.md), fixed.

For one [independent symmetric three-level system](../../canonical-ensemble.md#independent-symmetric-three-level-system) put $\epsilon=\mu B$ and $x=\beta\epsilon$. Then $Z=1+2\cosh x$ and

$$
\boxed{\overline E=-\frac{2\epsilon\sinh x}{1+2\cosh x}.}
$$

At nonzero fixed field, the ground state dominates as $T\to0$, so $\overline E\to-\mu|B|$. At high [temperature](../../temperature.md) all three levels become nearly equally populated and their mean tends to zero from below. At fixed positive [temperature](../../temperature.md) the [energy](../../energy.md) is even in $B$, is quadratic near zero field, and approaches $-\mu|B|$ at large $|B|$ as the lowest level becomes occupied. The [heat capacity](../../heat.md#heat-capacity) vanishes both when excitations are frozen out and when populations are almost equal, with a positive [Schottky anomaly](../../heat.md#schottky-anomaly) between those limits.

<a id="section-c/c12/image-three-level-mean-energy-versus-temperature-and-field-and-its-schottky-heat-capacity-peak"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2014/paper-2-b2-three-level-curves.png)

**[Figure 2](#section-c/c12/image-three-level-mean-energy-versus-temperature-and-field-and-its-schottky-heat-capacity-peak). Three-level mean energy versus temperature and field, and its Schottky heat-capacity peak**.

At $|x|\ll1$, expanding the hyperbolic functions gives

$$
\boxed{\overline E\simeq-\frac{2\mu^2B^2}{3k_BT},
\qquad C\simeq\frac{2\mu^2B^2}{3k_BT^2}.}
$$

Interpreting the stated [heat capacity](../../heat.md#heat-capacity) on the same one-atom basis as the preceding calculation, its tail coefficient gives

$$
\boxed{\mu=\frac1B\sqrt{\frac{3ak_B}{2}}
\simeq2.89\times10^{-5}\,\mathrm{eV\,T^{-1}}
=4.64\times10^{-24}\,\mathrm{J\,T^{-1}}\simeq0.500\,\mu_B.}
$$

Here $k_B=8.61733\times10^{-5}\,\mathrm{eV\,K^{-1}}$ is used consistently with $a$ in electronvolt kelvin. For a sample of $N$ independent atoms, the total coefficient would be $N$ times the one-atom coefficient; it must first be divided by $N$.

Finally, two derivatives of $Z$ supply the second [energy](../../energy.md) moment:

$$
\overline{E^2}=\frac{Z''}{Z},\qquad
\frac{d\overline E}{d\beta}
=-\left(\frac{Z''}{Z}-\frac{Z'^2}{Z^2}\right)
=-\operatorname{Var}(E).
$$

Combining this with the heat-capacity [derivative](../../calculus.md#derivative) yields the [canonical energy fluctuation](../../canonical-ensemble.md#canonical-energy-fluctuation) relation

$$
\boxed{C=\frac{\operatorname{Var}(E)}{k_BT^2},
\qquad\Delta E=\sqrt{k_BT^2C}.}
$$

It also explains why this canonical [heat capacity](../../heat.md#heat-capacity) is nonnegative.[§§1.3.1–1.3.2, printed pages 18–20, equations (1.25)–(1.27)](../../physics-bibliography.md#statistical-physics-by-david-tong)

<h3 id="section-c/c13">C13</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c13/solution">Solution</h4>

↑ **Parent:** [C13](#section-c/c13)

**Molecules.** In a dilute classical gas, collisions establish a [Maxwell-Boltzmann distribution](../../quantum-ideal-gas-statistics.md#maxwell-boltzmann-distribution). The normalized [speed](../../classical-mechanics.md#speed) distribution and its first two moments are

$$
f(v)=4\pi\left(\frac{m}{2\pi k_BT}\right)^{3/2}v^2e^{-mv^2/(2k_BT)},
\quad \overline v=\sqrt{\frac{8k_BT}{\pi m}},\quad
\overline{v^2}=\frac{3k_BT}{m}.
$$

[Momentum](../../momentum.md) transfer to a wall gives $p=nm\overline{v^2}/3=nk_BT$. Translational [internal energy](../../internal-energy.md) is $U=3Nk_BT/2$; rotational and vibrational degrees of freedom add [energy](../../energy.md) when thermally populated, without changing the dilute ideal-gas [pressure](../../pressure.md) law. Classical [equipartition](../../canonical-ensemble.md#equipartition-theorem) gives $k_BT/2$ per quadratic contribution, but quantum level spacing can freeze out modes.

Only the molecules moving towards a surface contribute to its one-sided number flux:

$$
J=\frac14n\overline v=\frac{p}{\sqrt{2\pi mk_BT}}.
$$

For an [effusive molecular energy flux](../../kinetic-theory.md#effusive-molecular-energy-flux), faster molecules are preferentially sampled, giving mean translational [energy](../../energy.md) $2k_BT$ per crossing molecule and $F_E=2k_BTJ$. This differs from multiplying $J$ by the bulk mean $3k_BT/2$. Collisions and finite molecular interactions produce transport and departures from the ideal-gas [equation of state](../../pressure.md#equation-of-state).

**[Photons](../../quantum-mechanics.md#photon).** All [photons](../../quantum-mechanics.md#photon) travel at $c$ in vacuum, so their thermal distribution is over [frequency](../../wave.md#frequency), not over a range of speeds. The two polarizations and Bose-Einstein occupation with zero [chemical potential](../../chemical-potential.md) give

$$
u_\nu\,d\nu=\frac{8\pi h\nu^3}{c^3}
\frac{d\nu}{e^{h\nu/(k_BT)}-1},\qquad
u\equiv\int_0^\infty u_\nu\,d\nu=a_RT^4,
\quad a_R=\frac{8\pi^5k_B^4}{15h^3c^3}.
$$

Here the spectral quantity is $u_\nu$ and the total [energy](../../energy.md) [density](../../fluid-mechanics.md#density) is $u$. [Momentum flux](../../mathematical-physics.md#momentum-flux) gives $p=u/3$, while isotropic angular averaging gives the one-sided [energy](../../energy.md) flux $F_E=cu/4=\sigma_{\rm SB}T^4$ through a small aperture of a black-body cavity. The [photon](../../quantum-mechanics.md#photon) number flux is similarly $cn_\gamma/4$.

**Both pressures arise from [momentum](../../momentum.md) transfer, but their [equations of state](../../pressure.md#equation-of-state) differ:** a classical molecular gas has $pV=Nk_BT$ with fixed molecule number, whereas a [photon gas](../../statistical-physics.md#photon-gas) has $pV=U/3$, $U=a_RVT^4$ and an equilibrium [photon](../../quantum-mechanics.md#photon) number that changes with [temperature](../../temperature.md). [Photon](../../quantum-mechanics.md#photon) creation and absorption by the walls are essential to the zero-chemical-potential equilibrium description.

## ↑ Ancestors (11)

1. [2014](../2014.md)
2. [Past exam of the physics B course of the University of Cambridge](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge.md)
3. [Physics B course of the University of Cambridge](../../university-of-cambridge.md#physics-b-course-of-the-university-of-cambridge)
4. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
