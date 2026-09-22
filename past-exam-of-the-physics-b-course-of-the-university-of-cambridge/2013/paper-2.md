# Paper 2

↑ **Parent:** [2013](../2013.md)

[Original public PDF, physical pages 150–155; examination dated 5 June 2013](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1#page=150)

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
  - [C11](#section-c/c11)
    - [Solution](#section-c/c11/solution)
  - [C12](#section-c/c12)
    - [Solution](#section-c/c12/solution)
    - [i](#section-c/c12/i)
      - [Solution](#section-c/c12/i/solution)
    - [ii](#section-c/c12/ii)
      - [Solution](#section-c/c12/ii/solution)
    - [iii](#section-c/c12/iii)
      - [Solution](#section-c/c12/iii/solution)
  - [C13](#section-c/c13)
    - [Solution](#section-c/c13/solution)

## Section A

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-a/a1">A1</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a1/solution">Solution</h4>

↑ **Parent:** [A1](#section-a/a1)

For the [force on a current loop in a bilinear magnetic field](../../relativistic-electromagnetism.md#force-on-a-current-loop-in-a-bilinear-magnetic-field), the arrow gives current in the positive $y$ direction on the edge $x=a$, and in the negative $x$ direction on the edge $y=a$. Use $d\mathbf F=I\,d\boldsymbol\ell\times\mathbf B$. The edges on the coordinate axes contribute zero because the applied field vanishes there. The other two give

$$
\mathbf F_{x=a}=I\alpha a\int_0^a y\,dy\,\hat{\mathbf x},\qquad
\mathbf F_{y=a}=I\alpha a\int_0^a x\,dx\,\hat{\mathbf y}.
$$

Thus the force on the square itself, excluding the supply leads, is

$$
\boxed{\mathbf F=\frac{I\alpha a^3}{2}(\hat{\mathbf x}+\hat{\mathbf y})
=2.5(\hat{\mathbf x}+\hat{\mathbf y})\,\mathrm N,\quad |\mathbf F|=3.54\,\mathrm N.}
$$

It lies in the plane along the diagonal towards increasing $x$ and $y$, at $45^\circ$ to either positive axis.

<h3 id="section-a/a2">A2</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a2/solution">Solution</h4>

↑ **Parent:** [A2](#section-a/a2)

In the ideal [semidiurnal tide](../../newton-s-law-of-universal-gravitation.md#semidiurnal-tide) model, successive high tides occur after the [Earth](../../planetary-science.md#earth)–[Moon](../../planetary-science.md#moon) relative angle advances by $\pi$. Since the motions have the same sense, subtract their [angular speeds](../../rigid-body-dynamics.md#angular-speed):

$$
\boxed{\Delta t=\frac{\pi}{\Omega_E-\Omega_M}
=\frac1{2(T_E^{-1}-T_M^{-1})}.}
$$

The lunar [orbital period](../../celestial-mechanics.md#orbital-period) is sidereal, so the consistent terrestrial [rotation](../../riemannian-geometry.md#rotation-mathematics) period is $T_E=23.9345\,\mathrm h$. With $T_M=27.3\times24\,\mathrm h$, this gives **about 12 h 25 min**. The sidereal terrestrial period is distinct from the 24-hour solar day.[Orbital parameters, sidereal rotation period 23.9345 h and length of day 24 h](../../physics-bibliography.md#earth-fact-sheet-by-national-aeronautics-and-space-administration)

If the [Earth](../../planetary-science.md#earth)'s [rotation](../../riemannian-geometry.md#rotation-mathematics) is approximated as one revolution in 24 hours, the same calculation instead gives **12 h 27 min**. That small difference is the day convention, not a change of sign in the relative [angular speed](../../rigid-body-dynamics.md#angular-speed). Actual coastal [tide](../../newton-s-law-of-universal-gravitation.md#tide) times also depend on ocean dynamics and the solar [tide](../../newton-s-law-of-universal-gravitation.md#tide).

<h3 id="section-a/a3">A3</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a3/solution">Solution</h4>

↑ **Parent:** [A3](#section-a/a3)

For the [uniform magnetic field in an off-axis cylindrical cavity](../../electromagnetism.md#uniform-magnetic-field-in-an-off-axis-cylindrical-cavity), let $\mathbf b$ point from the conductor's axis to the hole's axis and let the current flow in $+z$. Its uniform [current density](../../electric-charge.md#current-density) in the metal is

$$
\mathbf J=\frac{I}{\pi(R^2-a^2)}\hat{\mathbf z}.
$$

Superpose a complete cylinder carrying $\mathbf J$ and a cylinder occupying the hole carrying $-\mathbf J$. Inside a uniformly filled cylinder, [Ampère's law](../../maxwell-equations.md#ampere-s-circuital-law) gives $\mathbf B=(\mu_0/2)\mathbf J\times\mathbf r$. For any point in the cavity,

$$
\mathbf B=\frac{\mu_0}{2}\bigl[\mathbf J\times\mathbf r-\mathbf J\times(\mathbf r-\mathbf b)\bigr]
=\boxed{\frac{\mu_0I}{2\pi(R^2-a^2)}\,\hat{\mathbf z}\times\mathbf b.}
$$

There is no remaining position dependence, so the field is uniform. Its magnitude is $\mu_0Ib/[2\pi(R^2-a^2)]$, perpendicular to the axis-offset [vector](../../vector-space.md#vector) in the cross-sectional plane. Reversing the current reverses the field.

<h3 id="section-a/a4">A4</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a4/solution">Solution</h4>

↑ **Parent:** [A4](#section-a/a4)

Use the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame) equilibrium model, in which the [centrifugal potential](../../mathematical-physics.md#centrifugal-potential) [energy](../../energy.md) of a particle of [mass](../../classical-mechanics.md#mass) $m_i$ is $U_i(r)=-m_i\omega^2r^2/2$. The [Boltzmann distribution](../../thermodynamics.md#boltzmann-distribution) then gives

$$
\frac{n_i(r)}{n_i(a)}=
\exp\left[\frac{m_i\omega^2(r^2-a^2)}{2k_BT}\right].
$$

Define the concentration ratio as $c=n_1/n_2$. At the axis,

$$
\boxed{c_{\rm axis}=c_{\rm wall}
\exp\left[\frac{(m_2-m_1)\omega^2a^2}{2k_BT}\right].}
$$

Thus the axis favours the lighter species. The expression assumes a dilute classical mixture at one [temperature](../../temperature.md), equilibrium in the [rotating reference frame](../../mathematical-physics.md#rotating-reference-frame), and sampling sufficiently close to $r=0$.

<h3 id="section-a/a5">A5</h3>

↑ **Parent:** [Section A](#section-a)

<h4 id="section-a/a5/solution">Solution</h4>

↑ **Parent:** [A5](#section-a/a5)

Define $q=N_+-N_-$, where $N_+$ counts particles in the $+\epsilon$ level. Then $N_\pm=(N\pm q)/2$, so

$$
\boxed{U=\epsilon q,\qquad
S=k_B\ln\frac{N!}{[(N+q)/2]!\,[(N-q)/2]!}.}
$$

The [binomial entropy of independent two-level particles](../../canonical-ensemble.md#binomial-entropy-of-independent-two-level-particles) follows from counting which of the $N$ independently labelled particles occupy each nondegenerate level. This is the usual distinguishable, or localized, two-level model; occupation constraints of a degenerate quantum gas would require different counting.

For large occupations, [Stirling's approximation](../../real-analysis.md#stirling-formula) with $x=q/N$ gives

$$
\boxed{S\simeq Nk_B\left[\ln2-\frac{1+x}{2}\ln(1+x)-\frac{1-x}{2}\ln(1-x)\right].}
$$

Allowed $q$ runs from $-N$ to $N$ in steps of two. [Entropy](../../entropy.md) is largest near equal populations and is zero when all particles occupy one level; use $0\ln0=0$ at the endpoints.

## Section B

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-b/b6">B6</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b6/a">a</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b6/a)

In vacuum, **[displacement current](../../maxwell-equations.md#displacement-current) contributes the additional term** $\epsilon_0\partial\mathbf E/\partial t$:

$$
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t}.
$$

Taking the divergence and using [Gauss law](../../maxwell-equations.md#gauss-s-law) gives $\nabla\cdot\mathbf J+\partial\rho/\partial t=0$, the local conservation of charge. Without [displacement current](../../maxwell-equations.md#displacement-current) the curl equation would incorrectly require a divergence-free current even during charge accumulation.

For a charging [capacitor](../../electromagnetism.md#capacitor), a surface cutting the wire carries conduction current while a surface passing through the gap carries changing [electric flux](../../electric-field.md#electric-flux). The [displacement current](../../maxwell-equations.md#displacement-current) term makes the circulation independent of the spanning surface. It is not transport of free charge across the vacuum gap. In matter the macroscopic equation is $\nabla\times\mathbf H=\mathbf J_f+\partial\mathbf D/\partial t$, with [electric polarization](../../electromagnetism.md#polarization-density) included in $\mathbf D$. Together with [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction), the vacuum equations give [electromagnetic waves](../../electromagnetic-wave.md) of [speed](../../classical-mechanics.md#speed) $1/\sqrt{\mu_0\epsilon_0}$.

<h4 id="section-b/b6/b">b</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b6/b)

An applied [electric field](../../electric-field.md) displaces [bound charges](../../electromagnetism.md#bound-charge) or reorients permanent dipoles, producing [electric polarization](../../electromagnetism.md#polarization-density) $\mathbf P$, the dipole moment per unit volume. It gives [bound charges](../../electromagnetism.md#bound-charge) $\rho_b=-\nabla\cdot\mathbf P$ and $\sigma_b=\mathbf P\cdot\mathbf n$. Define

$$
\mathbf D=\epsilon_0\mathbf E+\mathbf P,\qquad
\mathbf P=\epsilon_0\chi_e\mathbf E,\qquad
\epsilon=\epsilon_0(1+\chi_e)
$$

for a **linear isotropic [dielectric](../../permittivity.md#dielectric)**. Then $\nabla\cdot\mathbf D=\rho_f$ separates free charge from the bound-charge response. Electronic, ionic and orientational [electric polarization](../../electromagnetism.md#polarization-density) respond on different timescales; real [permittivity](../../permittivity.md) is [frequency](../../wave.md#frequency) dependent, and its dissipative part describes [dielectric loss](../../permittivity.md#dielectric-loss).

A uniform [dielectric](../../permittivity.md#dielectric) filling a [parallel-plate capacitor](../../electromagnetism.md#parallel-plate-capacitor) raises its [capacitance](../../electromagnetism.md#capacitance) to $\epsilon A/d$. At fixed charge this reduces field [energy](../../energy.md) $Q^2/(2C)$; at fixed [voltage](../../random-walk.md#voltage) the stored [energy](../../energy.md) $CV^2/2$ increases because the [voltage](../../random-walk.md#voltage) source supplies charge and [energy](../../energy.md). Insulation and [energy](../../energy.md) storage are useful applications, limited by loss and [dielectric breakdown](../../permittivity.md#dielectric-breakdown). Static interface conditions are continuous tangential $\mathbf E$ and a jump in normal $\mathbf D$ equal to free surface charge.

<h4 id="section-b/b6/c">c</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b6/c)

**A current in one circuit links [magnetic flux](../../magnetic-field.md#magnetic-flux) through another.** It produces [magnetic flux linkage](../../electromagnetism.md#magnetic-flux-linkage) through another. With fixed geometry and a linear reciprocal medium, choose consistent winding orientations and write

$$
\Lambda_1=L_1I_1+MI_2,\qquad \Lambda_2=MI_1+L_2I_2.
$$

The shared coefficient is **[mutual inductance](../../electromagnetism.md#mutual-inductance)**; reversal of one winding reverses its sign. [Faraday's law of induction](../../maxwell-equations.md#faraday-s-law-of-induction) gives the mutual induced emf $\mathcal E_2=-M\dot I_1$ for fixed $M$. The minus sign expresses [Lenz's law](../../maxwell-equations.md#lenz-s-law).

The [magnetic energy](../../electromagnetic-wave.md#magnetic-energy) is

$$
W=\tfrac12L_1I_1^2+MI_1I_2+\tfrac12L_2I_2^2.
$$

Nonnegative [energy](../../energy.md) for every current pair requires $|M|\leq\sqrt{L_1L_2}$, motivating the coupling coefficient $M/\sqrt{L_1L_2}$. Transformers use strong common flux to exchange [energy](../../energy.md) between circuits; leakage flux reduces coupling. A shared core increases linkage, but saturation, [hysteresis](../../critical-phenomenon.md#hysteresis) and eddy-current losses limit the linear description. A moving geometry also contributes $-I_1\dot M$ to the mutual emf.

<h4 id="section-b/b6/d">d</h4>

↑ **Parent:** [B6](#section-b/b6)

<h5 id="section-b/b6/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b6/d)

Find the potential from $\mathbf E=-\nabla\phi$ and $\nabla\cdot(\epsilon\nabla\phi)=-\rho_f$. One must specify boundary data: a potential on each Dirichlet boundary, a normal displacement on each Neumann boundary, or an appropriate mixture. Conductors are equipotentials; at [dielectric](../../permittivity.md#dielectric) interfaces $\phi$ is continuous and the normal displacement jumps by the specified free surface charge. With no singular dipole sheet, tangential [electric field](../../electric-field.md) is continuous.

To establish [uniqueness of Poisson equation](../../analysis.md#uniqueness-of-poisson-equation), subtract two solutions with the same charge and boundary data, writing their difference as $u$. [Integration by parts](../../calculus.md#integration-by-parts) gives

$$
\int_V\epsilon|\nabla u|^2\,dV
=\int_{\partial V}u\epsilon\partial_nu\,dA,
$$

since $\nabla\cdot(\epsilon\nabla u)=0$. The right side vanishes for identical Dirichlet data, identical Neumann data, or their usual mixed combination. Interface terms cancel under the homogeneous difference conditions. With positive [permittivity](../../permittivity.md), $\nabla u=0$: **the field is unique**, and the potential is unique if any suitable reference potential is fixed. For a pure Neumann problem an additive constant remains, and the prescribed outward displacement flux must equal the enclosed free charge. This theorem justifies image-charge solutions once their boundary data have been checked.

<h3 id="section-b/b7">B7</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b7/solution">Solution</h4>

↑ **Parent:** [B7](#section-b/b7)

[Magnetization](../../electromagnetism.md#magnetization) $\mathbf M$ is [magnetic dipole moment](../../electromagnetism.md#magnetic-dipole-moment) per unit volume. In SI units,

$$
\mathbf B=\mu_0(\mathbf H+\mathbf M),\qquad
\mathbf M=\chi\mathbf H,\qquad \mu=\mu_0(1+\chi)
$$

in a linear isotropic response. The internal field matters: for a uniformly magnetized [ellipsoid](../../euclidean-geometry.md#ellipsoid) it is $\mathbf H_{\rm int}=\mathbf H_{\rm applied}-\mathbf N_d\mathbf M$. Sample shape therefore affects an apparent [magnetic susceptibility](../../statistical-physics.md#magnetic-susceptibility).

**[Diamagnetism](../../electromagnetism.md#diamagnetism)** opposes the applied field, giving small negative [magnetic susceptibility](../../statistical-physics.md#magnetic-susceptibility) from the induced orbital response. It is often only weakly [temperature](../../temperature.md) dependent. **[Paramagnetism](../../electromagnetism.md#paramagnetism)** aligns pre-existing moments and gives positive [magnetic susceptibility](../../statistical-physics.md#magnetic-susceptibility); independent localized moments obey approximately $\chi=C/T$ in weak fields before saturating. [Pauli paramagnetism](../../quantum-ideal-gas-statistics.md#pauli-paramagnetism) of conduction electrons is a different, weakly temperature-dependent mechanism.

**[Ferromagnetism](../../electromagnetism.md#ferromagnetism)** involves collective exchange-driven alignment and spontaneous [magnetization](../../electromagnetism.md#magnetization) below the [Curie temperature](../../electromagnetism.md#curie-temperature). A specimen can nevertheless have nearly zero total moment because [magnetic domains](../../electromagnetism.md#magnetic-domain) point in different directions. Field-driven domain-wall motion and [rotation](../../riemannian-geometry.md#rotation-mathematics) change the net [magnetization](../../electromagnetism.md#magnetization). [Antiferromagnets](../../electromagnetism.md#antiferromagnetism) have compensating ordered sublattices below a [Néel temperature](../../electromagnetism.md#neel-temperature); [ferrimagnets](../../electromagnetism.md#ferrimagnetism) have oppositely ordered but unequal sublattice moments and retain a net moment. Ferrites are useful examples of electrically resistive ferrimagnetic core materials.

Ferromagnetic response is nonlinear and history dependent. A [hysteresis](../../critical-phenomenon.md#hysteresis) loop displays [remanent magnetization](../../electromagnetism.md#remanent-magnetization), [magnetic coercivity](../../critical-phenomenon.md#magnetic-coercivity) and saturation. A single constant [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) cannot describe the entire loop: differential [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) describes its local slope. The quasistatic [energy](../../energy.md) loss per unit volume and cycle is the loop [area](../../differential-geometry.md#surface-area) $\oint H\,dB$. [Soft magnetic materials](../../electromagnetism.md#soft-magnetic-material) have low [magnetic coercivity](../../critical-phenomenon.md#magnetic-coercivity) and usually high useful [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism); [hard magnetic materials](../../electromagnetism.md#hard-magnetic-material) retain [magnetization](../../electromagnetism.md#magnetization) and suit permanent magnets.

**An [electromagnet](../../magnetic-field.md#electromagnet) normally uses a soft, high-permeability core** to guide flux generated by a coil. For a uniform-section core with length $\ell_c$ and air gap $g$, neglecting leakage and fringing,

$$
NI\simeq H_c\ell_c+\frac{Bg}{\mu_0},\qquad
\boxed{B\simeq\frac{\mu_0NI}{g+\ell_c/\mu_r}.}
$$

An air gap can dominate the [magnetic reluctance](../../electromagnetism.md#magnetic-reluctance) even when the core [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) is large. Core saturation limits the improvement with current, while winding resistance causes heating. For alternating operation, laminations suppress eddy-current loops in metallic cores; high-resistivity ferrites also reduce those losses. Low [hysteresis](../../critical-phenomenon.md#hysteresis) loss is important in repeatedly cycled cores, whereas high [magnetic coercivity](../../critical-phenomenon.md#magnetic-coercivity) is valuable in a permanent magnet. Useful design therefore depends on the full magnetic response, electrical losses and operating [frequency](../../wave.md#frequency), rather than the largest quoted [magnetic permeability](../../maxwell-equations.md#permeability-electromagnetism) alone.

<h3 id="section-b/b8">B8</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b8/a">a</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/a/solution">Solution</h5>

↑ **Parent:** [A](#section-b/b8/a)

[Generalized coordinates](../../lagrangian-mechanics.md#generalized-coordinate) incorporate [holonomic constraints](../../classical-mechanics.md#holonomic-constraint) without solving separately for every constraint force. For conservative mechanics use $L=T-V$. The [principle of stationary action](../../lagrangian-mechanics.md#principle-of-stationary-action) makes the [action](../../lagrangian-mechanics.md#action) $\int L\,dt$ stationary for variations vanishing at the endpoints. [Integration by parts](../../calculus.md#integration-by-parts) gives

$$
\boxed{\frac{d}{dt}\frac{\partial L}{\partial\dot q_i}-\frac{\partial L}{\partial q_i}=0.}
$$

The [canonical momentum](../../hamiltonian-mechanics.md#canonical-momentum) is $p_i=\partial L/\partial\dot q_i$. A [cyclic coordinate](../../lagrangian-mechanics.md#cyclic-coordinate) gives conserved $p_i$; absent explicit time dependence, $\sum_i p_i\dot q_i-L$ is conserved. These are symmetry–conservation relationships, not assumptions that all momenta are constant. Nonconservative generalized forces enter the right side.

For example, a pendulum has $L=m\ell^2\dot\theta^2/2+mg\ell\cos\theta$, giving $m\ell^2\ddot\theta+mg\ell\sin\theta=0$. The method extends directly to coupled coordinates and velocity-dependent interactions when the correct [Lagrangian](../../calculus-of-variations.md#lagrangian) is used; $T-V$ with a position-only potential is not the most general form.

<h4 id="section-b/b8/b">b</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/b/solution">Solution</h5>

↑ **Parent:** [B](#section-b/b8/b)

[Viscosity](../../dynamic-viscosity.md) transfers [momentum](../../momentum.md) between adjacent fluid layers. A [Newtonian fluid](../../viscous-fluid-flow.md#newtonian-fluid) has [shear stress](../../viscous-fluid-flow.md#shear-stress) proportional to [strain](../../continuum-mechanics.md#strain) rate: for simple shear, $\boxed{\tau_{xy}=\eta\,\partial u_x/\partial y}$. Thus parallel plates of [area](../../differential-geometry.md#surface-area) $A$, separation $d$ and relative [speed](../../classical-mechanics.md#speed) $U$ require force magnitude $\eta AU/d$ in a steady linear profile.

For an incompressible isotropic [Newtonian fluid](../../viscous-fluid-flow.md#newtonian-fluid),

$$
\sigma_{ij}=-p\delta_{ij}+\eta(\partial_i u_j+\partial_j u_i),\qquad
\rho\frac{D\mathbf u}{Dt}=-\nabla p+\eta\nabla^2\mathbf u+\rho\mathbf g
$$

for constant [viscosity](../../dynamic-viscosity.md). With [strain-rate tensor](../../viscous-fluid-flow.md#strain-rate-tensor) $e_{ij}$, the [viscous dissipation](../../stokes-flow.md#viscous-dissipation) rate per unit volume is $2\eta e_{ij}e_{ij}\geq0$. [Kinematic viscosity](../../dynamic-viscosity.md#kinematic-viscosity) $\nu=\eta/\rho$ is the [momentum](../../momentum.md) diffusivity: a disturbance spreads over distance of order $\sqrt{\nu t}$.

The [Reynolds number](../../dynamic-viscosity.md#reynolds-number) $\rho UL/\eta$ compares inertial and viscous forces. Small [Reynolds number](../../dynamic-viscosity.md#reynolds-number) supports a creeping-flow approximation, while large values permit thin viscous [boundary layers](../../continuum-mechanics.md#boundary-layer) and possible [turbulence](../../turbulence.md). It does not mean molecular [viscosity](../../dynamic-viscosity.md) has disappeared. Gas [viscosity](../../dynamic-viscosity.md) results from molecular [momentum](../../momentum.md) transport; a liquid's microscopic transport depends strongly on intermolecular interactions. Non-Newtonian materials require a more general constitutive law.

<h4 id="section-b/b8/c">c</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/c/solution">Solution</h5>

↑ **Parent:** [C](#section-b/b8/c)

For an attractive [inverse-square potential](../../energy.md#inverse-square-potential), let the [reduced mass](../../classical-mechanics.md#reduced-mass) be $\mu$, potential $-k/r$, and nonzero orbital [angular momentum](../../momentum.md#angular-momentum) $\ell$. Conservation of [angular momentum](../../momentum.md#angular-momentum) makes the orbit planar. The orbit equation is

$$
\boxed{r=\frac{\ell^2/(\mu k)}{1+e\cos\varphi},\qquad
e^2=1+\frac{2E\ell^2}{\mu k^2}.}
$$

Positive relative [energy](../../energy.md) gives $e>1$ and an unbound [hyperbolic Kepler orbit](../../celestial-mechanics.md#hyperbolic-kepler-orbit), arriving from and returning to infinity. Its asymptotes satisfy $\cos\varphi_\infty=-1/e$. At infinity $E=\mu v_\infty^2/2$ and $\ell=\mu b v_\infty$ for [impact parameter](../../classical-mechanics.md#impact-parameter) $b$, so the deflection angle is

$$
\boxed{\chi=2\arcsin(1/e)
=2\arctan\frac{k}{\mu b v_\infty^2}.}
$$

This describes gravitational encounters in the Newtonian two-body approximation. The body speeds up near [periapsis](../../celestial-mechanics.md#periapsis) while total [energy](../../energy.md) remains positive. It is distinct from an elliptic bound orbit and from the zero-energy parabolic limit; repulsive Coulomb scattering also gives hyperbolae but uses a different orientation of the force and orbit.

<h4 id="section-b/b8/d">d</h4>

↑ **Parent:** [B8](#section-b/b8)

<h5 id="section-b/b8/d/solution">Solution</h5>

↑ **Parent:** [D](#section-b/b8/d)

For a homogeneous isotropic solid with small displacement $\mathbf u$, [linear elasticity](../../elasticity-physics.md#linear-elasticity) gives $\sigma_{ij}=\lambda_L(\nabla\cdot\mathbf u)\delta_{ij}+2\mu e_{ij}$. [Momentum](../../momentum.md) balance becomes

$$
\rho\,\partial_t^2\mathbf u=(\lambda_L+\mu)\nabla(\nabla\cdot\mathbf u)+\mu\nabla^2\mathbf u.
$$

A [plane wave](../../wave-function.md#plane-wave) with displacement parallel to its [wavevector](../../elasticity-physics.md#wavevector) is longitudinal, whereas perpendicular displacement is transverse. Writing $K=\lambda_L+2\mu/3$ for the [bulk modulus](../../elasticity-physics.md#bulk-modulus) and $\mu$ for the [shear modulus](../../elasticity-physics.md#shear-modulus), their bulk speeds are

$$
\boxed{c_P=\sqrt{\frac{K+4\mu/3}{\rho}},\qquad c_S=\sqrt{\frac{\mu}{\rho}}.}
$$

There are two independent transverse polarizations. The [bulk modulus](../../elasticity-physics.md#bulk-modulus) supplies resistance to compression; shear rigidity supplies transverse restoring [stress](../../continuum-mechanics.md#stress). An ordinary fluid has no static shear rigidity and cannot sustain these propagating bulk shear waves. A thin rod with freely contracting sides instead has longitudinal [speed](../../classical-mechanics.md#speed) $\sqrt{Y/\rho}$, because its lateral [boundary conditions](../../differential-equation.md#boundary-condition) differ from a bulk [plane wave](../../wave-function.md#plane-wave). [Reflection](../../linear-algebra.md#reflection-mathematics), [refraction](../../optics.md#refraction) and mode conversion occur at interfaces; a free surface also supports [Rayleigh waves](../../wave-equation.md#rayleigh-wave).

<h3 id="section-b/b9">B9</h3>

↑ **Parent:** [Section B](#section-b)

<h4 id="section-b/b9/solution">Solution</h4>

↑ **Parent:** [B9](#section-b/b9)

For torque-free [rotation](../../riemannian-geometry.md#rotation-mathematics), [angular momentum](../../momentum.md#angular-momentum) is fixed in inertial space, but [angular velocity](../../rigid-body-dynamics.md#angular-velocity) need not point along it. In principal body axes,

$$
I_1\dot\omega_1+(I_3-I_2)\omega_2\omega_3=0
$$

and cyclic permutations. A [symmetric top](../../rigid-body-dynamics.md#symmetric-top) with transverse moment $A$ and axial moment $C$ has constant $\omega_3$, while $\omega_1+i\omega_2$ rotates in body coordinates at signed [frequency](../../wave.md#frequency) $(C-A)\omega_3/A$. The symmetry axis precesses around the fixed [angular momentum](../../momentum.md#angular-momentum) in space at rate $L/A$. These body-frame and space-frame rates describe different motions and need not coincide.

**[Poinsot construction](../../rigid-body-dynamics.md#poinsot-s-ellipsoid)** expresses the same torque-free motion geometrically. The [energy](../../energy.md) [ellipsoid](../../euclidean-geometry.md#ellipsoid) $\sum I_i\omega_i^2=2T$ is fixed in the body. Its normal at the angular-velocity point is parallel to $\mathbf L$, and $\mathbf L\cdot\boldsymbol\omega=2T$ places that point in a fixed plane perpendicular to $\mathbf L$. The [ellipsoid](../../euclidean-geometry.md#ellipsoid) rolls on this invariable plane without slipping: the instantaneous [velocity](../../classical-mechanics.md#velocity) of its contact point is proportional to $\boldsymbol\omega\times\boldsymbol\omega=0$. The contact curve is the [polhode](../../rigid-body-dynamics.md#polhode) on the body [ellipsoid](../../euclidean-geometry.md#ellipsoid) and the [herpolhode](../../rigid-body-dynamics.md#herpolhode) on the plane.[§3.4, Euler equations, stability and Poinsot construction](../../physics-bibliography.md#classical-dynamics-by-david-tong)

For $I_1<I_2<I_3$, linearization about spin $\Omega$ on the third axis gives

$$
\ddot\omega_1=-\Omega^2\frac{(I_3-I_2)(I_3-I_1)}{I_1I_2}\omega_1.
$$

The extreme-moment axes are stable; the intermediate one is unstable. The [major-axis relaxation theorem](../../rigid-body-dynamics.md#major-axis-relaxation-theorem) adds weak internal dissipation while retaining negligible external [torque](../../momentum.md#torque). At fixed $L$,

$$
T=\sum_i\frac{L_i^2}{2I_i}\geq\boxed{\frac{L^2}{2I_3}.}
$$

[Energy](../../energy.md) loss favours [rotation](../../riemannian-geometry.md#rotation-mathematics) about the axis of largest principal moment. Here “major axis” means maximum inertia, not necessarily the body's longest geometric direction. **A perfectly rigid torque-free body does not dissipatively settle**; its [energy](../../energy.md) is conserved. Distinguishing stability from relaxation also explains why minimum-inertia [rotation](../../riemannian-geometry.md#rotation-mathematics) can be stable in the ideal rigid model.

**Forced [precession](../../rigid-body-dynamics.md#precession)** occurs when an external [torque](../../momentum.md#torque) changes $\mathbf L$, with $\dot{\mathbf L}=\boldsymbol\tau$. For steady [precession](../../rigid-body-dynamics.md#precession), $\boldsymbol\tau=\boldsymbol\Omega_p\times\mathbf L$. A rapidly spinning, pivoted heavy [gyroscope](../../momentum.md#gyroscope) has $L\simeq C\omega_3$ along its symmetry axis, giving

$$
\boxed{\Omega_p\simeq\frac{Mg\ell}{C\omega_3}.}
$$

The [torque](../../momentum.md#torque) is perpendicular to the nearly axial [angular momentum](../../momentum.md#angular-momentum), so it mainly changes its direction. For a steady inclined [symmetric top](../../rigid-body-dynamics.md#symmetric-top), the more complete condition is

$$
A\Omega_p^2\cos\theta-C\omega_3\Omega_p+Mg\ell=0.
$$

It exhibits slow and fast [precession](../../rigid-body-dynamics.md#precession) branches when real solutions exist. A generic release excites [nutation](../../rigid-body-dynamics.md#nutation) as well: inclination oscillates instead of staying fixed. Axis constraints and bearing forces must be included when specifying which [angular momentum](../../momentum.md#angular-momentum) and pivot are being used.

## Section C

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="section-c/c10">C10</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c10/solution">Solution</h4>

↑ **Parent:** [C10](#section-c/c10)

For [speed](../../classical-mechanics.md#speed) distribution $f(v)$ normalized to one and isotropic directions, the incident number flux is

$$
J=n\int_0^\infty vf(v)\,dv\,
\frac1{4\pi}\int_0^{2\pi}d\phi\int_0^{\pi/2}\cos\theta\sin\theta\,d\theta
=\boxed{\frac14n\overline v.}
$$

The positive normal [velocity](../../classical-mechanics.md#velocity) weights the population reaching the wall. Consequently its mean translational [energy](../../energy.md) is

$$
\langle E\rangle_{\rm hit}=\frac m2\frac{\int_0^\infty v^5e^{-av^2}\,dv}{\int_0^\infty v^3e^{-av^2}\,dv}
=\frac m2\frac{a^{-3}}{(2a^2)^{-1}}
=\boxed{2k_BT},\qquad a=\frac{m}{2k_BT}.
$$

The bulk value $3k_BT/2$ would omit the arrival weighting.

For the two vessels, let $r=\sqrt{T_1/T_0}$, with subscripts h and c for hot and cold. Equal opposing [effusion](../../kinetic-theory.md#effusion) rates give $p_h/\sqrt{T_1}=p_c/\sqrt{T_0}$. Number conservation in equal, fixed volumes adds $p_h/T_1+p_c/T_0=2p_0/T_0$. Hence

$$
\boxed{p_c=\frac{2p_0r}{1+r},\quad p_h=\frac{2p_0r^2}{1+r},\quad
p_h-p_c=\frac{2p_0r(r-1)}{1+r}.}
$$

Both final [pressures](../../pressure.md) must be determined; holding the cold [temperature](../../temperature.md) fixed does not hold its [particle number](../../physics.md#particle-number) fixed.

For aperture [area](../../differential-geometry.md#surface-area) $A_h=\pi d^2/4$, the common one-way flux is $J=p_c/\sqrt{2\pi m k_BT_0}$. The translational [heat](../../heat.md) transfer from hot to cold is therefore

$$
\boxed{\dot Q=2k_B(T_1-T_0)A_hJ.}
$$

This is the total [heat](../../heat.md) transfer for a monatomic gas with no active internal modes, neglecting radiation and conduction through vessel walls. For a molecular gas, add $A_hJ[u_{\rm int}(T_1)-u_{\rm int}(T_0)]$ for its [internal energy](../../internal-energy.md) per molecule. The maintained unequal [temperatures](../../temperature.md) describe a stationary nonequilibrium state even though the net particle current is zero.

<h3 id="section-c/c11">C11</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c11/solution">Solution</h4>

↑ **Parent:** [C11](#section-c/c11)

A [thermodynamic potential](../../thermodynamic-potential.md) packages the equilibrium state in variables suited to the imposed constraints. For a simple fluid, $U(S,V,N)$ has differential $dU=T\,dS-p\,dV+\mu\,dN$. [Legendre transforms](../../convex-optimization.md#convex-conjugate) give $H=U+pV$, $F=U-TS$ and $G=U+pV-TS$, with [natural variables of a thermodynamic potential](../../thermodynamic-potential.md#natural-variables-of-a-thermodynamic-potential) $(S,p,N)$, $(T,V,N)$ and $(T,p,N)$ respectively. At fixed [particle number](../../physics.md#particle-number), **[Helmholtz free energy](../../thermodynamic-potential.md#helmholtz-free-energy) is minimized at fixed $T,V$; [Gibbs free energy](../../thermodynamic-potential.md#gibbs-free-energy) at fixed $T,p$**.

A flow vessel is an open [control volume](../../fluid-mechanics.md#control-volume), even if its walls are enclosed. For each inlet, [pressure](../../pressure.md) forces carry flow [work](../../energy.md#work) $p\,dV$ in addition to [internal energy](../../internal-energy.md). The steady first-law balance is

$$
\sum_{\rm in}\dot m(h+v^2/2+gz)+\dot Q-\dot W_{\rm shaft}
=\sum_{\rm out}\dot m(h+v^2/2+gz).
$$

With no [heat](../../heat.md) exchange, shaft [work](../../energy.md#work), or significant kinetic and gravitational [energy](../../energy.md) differences, the [enthalpy](../../enthalpy.md) fluxes are equal. [Mass](../../classical-mechanics.md#mass) flow must also balance. This equality concerns mass-flow-weighted specific enthalpies, not an unweighted sum over pipes.

Use the [liquefaction yield with separate warm-gas and liquid outlets](../../temperature.md#liquefaction-yield-with-separate-warm-gas-and-liquid-outlets). The wording specifies that the outgoing gas is at 14 K; it does not require the outgoing [liquid](../../thermodynamics.md#liquid) to have that [temperature](../../temperature.md). The two outlet streams need not be in mutual [thermal equilibrium](../../thermal-equilibrium.md). Taking $H$ as the printed [specific enthalpy](../../enthalpy.md#specific-enthalpy), the [steady-flow energy balance](../../enthalpy.md#steady-flow-energy-balance) gives

$$
H(p)=\alpha H_\ell+(1-\alpha)H(p_0),\qquad
\boxed{\alpha=\frac{H(p_0)-H(p)}{H(p_0)-H_\ell}.}
$$

For fixed outlet enthalpies the greatest yield occurs at the smallest inlet [enthalpy](../../enthalpy.md). **Among the tabulated [pressures](../../pressure.md) this is 30 atm.** Approximating the atmospheric-pressure gas [enthalpy](../../enthalpy.md) by the tabulated zero-pressure limiting value gives

$$
\boxed{\alpha\simeq\frac{8.74-7.18}{8.74-1.01}=0.202,\quad p\simeq30\,\mathrm{atm}.}
$$

This uses a low-pressure approximation: $p_0=1$ atm is not literally the zero-pressure table entry. Linear interpolation to 1 atm would instead give $H(p_0)\simeq8.651\times10^4\,\mathrm{J\,kg^{-1}}$ and $\alpha\simeq0.193$. The sparse table does not determine an exact continuous optimum between entries.

Atmospheric-pressure liquid [helium](../../chemical-substance.md#helium) must be much colder than the 14 K gas outlet: its normal boiling point is about 4.224 K.[Helium-4 characteristic-property table: normal boiling point 4.224 K](../../physics-bibliography.md#index-of-semiconductor-process-gases-helium-by-national-institute-of-standards-and-technology) A [counterflow heat exchanger](../../heat.md#counterflow-heat-exchanger) can return cold gas through the incoming stream before that gas leaves the overall [control volume](../../fluid-mechanics.md#control-volume), while the collected [liquid](../../thermodynamics.md#liquid) leaves separately at the cold end. This is a possible interpretation of the whole apparatus, rather than an extra diagram specified by the question. The enthalpy calculation needs only the stated inlet and outlet properties; it does not assume one equilibrium vessel containing both phases at 14 K. In particular, $H(p_0)-H_\ell$ is an outlet-stream enthalpy difference, not the [latent heat](../../thermodynamic-potential.md#latent-heat) of vaporization at one common [temperature](../../temperature.md).

<h3 id="section-c/c12">C12</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c12/solution">Solution</h4>

↑ **Parent:** [C12](#section-c/c12)

A [heat pump](../../thermodynamics.md#heat-pump) delivers $Q_H=Q_S+W$: electrical [work](../../energy.md#work) moves [heat](../../heat.md) from a source as well as contributing [energy](../../energy.md) itself. Its heating [coefficient of performance](../../thermodynamics.md#coefficient-of-performance) can therefore exceed one, whereas direct resistance heating supplies at most its electrical input as useful room [heat](../../heat.md). For an ideal reversible pump,

$$
\mathrm{COP}_H=\frac{T_H}{T_H-T_S},\qquad W=Q_H\frac{T_H-T_S}{T_H},
$$

with absolute [temperatures](../../temperature.md) and $T_S<T_H$. This is an ideal limit; actual costs also depend on compressor performance and tariffs.

For the [annual ground-temperature wave](../../diffusion-equation.md#annual-ground-temperature-wave), model the soil as a homogeneous semi-infinite conductor, with depth positive downward and a prescribed surface [temperature](../../temperature.md). Here $\kappa$ is [thermal conductivity](../../heat.md#thermal-conductivity) and $C$ is [heat capacity](../../heat.md#heat-capacity) per unit volume, so the [thermal diffusivity](../../heat.md#thermal-diffusivity) is $\kappa/C$. Conservation of [energy](../../energy.md) gives $C\partial_tT=\kappa\partial_z^2T$. After transients decay, put $T-T_0=\operatorname{Re}[A e^{i\omega t-qz}]$. Substitution gives $q^2=i\omega C/\kappa$; the solution bounded at depth uses $q=(1+i)/\delta$. Matching the surface then gives

$$
\boxed{\delta=\sqrt{\frac{2\kappa}{\omega C}},\quad
T_S=T_0-T_Ae^{-z/\delta}\cos(\omega t-z/\delta).}
$$

This approximation identifies the ground surface with air [temperature](../../temperature.md) and neglects the pump's perturbation of the ground, as required by the model. The attenuation and phase delay arise from [heat](../../heat.md) [diffusion](../../thermodynamics.md#diffusion), not propagation at one fixed wave [speed](../../classical-mechanics.md#speed).

The graph below covers a full annual cycle. At $z/\delta=\pi/2$, the amplitude is $20e^{-\pi/2}=4.16$ K and the minimum lags January by a quarter-year. At $z/\delta=\pi$, the amplitude is only $0.864$ K and the minimum lags by half a year: the ground is slightly warmer than its annual mean in January.

<a id="section-c/c12/image-annual-air-and-ground-temperatures-with-attenuation-and-depth-dependent-phase-delay"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2-b2-seasonal-source.png)

**[Figure 1](#section-c/c12/image-annual-air-and-ground-temperatures-with-attenuation-and-depth-dependent-phase-delay). Annual air and ground temperatures, with attenuation and depth-dependent phase delay**.

The [seasonal source depth for a reversible heat pump](../../thermodynamics.md#seasonal-source-depth-for-a-reversible-heat-pump) has a subtle limit: a deep source approaches $T_0$ and avoids severe winter cooling, but infinite depth is not the thermal optimum of this single-frequency model. In January, with $x=z/\delta$, maximize $T_S=T_0-T_Ae^{-x}\cos x$. The first and largest maximum is at $x=3\pi/4$, where $\cos x+\sin x=0$, giving **$z=3\pi\delta/4$ and $T_S\simeq16.34^\circ\mathrm C$**. It is also the optimum of the ideal annually integrated heating [work](../../energy.md#work): the heating load is even about January, so its weighted sine term integrates to zero and the depth dependence is again proportional to $e^{-x}\cos x$. Installation cost, finite tube spacing, [heat](../../heat.md) extraction, weather and real pump performance alter this result. The supplied model therefore supports a finite seasonal thermal optimum, while not fixing a practical burial depth in metres.

<h4 id="section-c/c12/i">i</h4>

↑ **Parent:** [C12](#section-c/c12)

<h5 id="section-c/c12/i/solution">Solution</h5>

↑ **Parent:** [I](#section-c/c12/i)

The coldest day has outside [temperature](../../temperature.md) $-5^\circ\mathrm C$, so the indoor–outdoor [temperature](../../temperature.md) difference is 25 K. If $K$ is the building's heat-loss coefficient, the required heating rate is $\dot Q_H=25K$. For direct electrical heating,

$$
\boxed{\dot W_{\rm direct}=\dot Q_H.}
$$

This sets the reference electrical cost for the same delivered [heat](../../heat.md) and tariff.

<h4 id="section-c/c12/ii">ii</h4>

↑ **Parent:** [C12](#section-c/c12)

<h5 id="section-c/c12/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#section-c/c12/ii)

For the ideal reversible comparison, $T_H=293.15$ K and the coldest air source is $268.15$ K. Thus

$$
\boxed{\mathrm{COP}_{\rm air}=\frac{293.15}{25}=11.73,\qquad
\frac{W_{\rm air}}{W_{\rm direct}}=\frac{25}{293.15}=0.0853.}
$$

A real air-source pump uses more [work](../../energy.md#work) than this reversible lower bound, and its low-temperature performance is not specified.

<h4 id="section-c/c12/iii">iii</h4>

↑ **Parent:** [C12](#section-c/c12)

<h5 id="section-c/c12/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#section-c/c12/iii)

A source much deeper than the annual penetration depth has $T_S\simeq288.15$ K. Therefore

$$
\boxed{\mathrm{COP}_{\rm ground}=\frac{293.15}{5}=58.63,\quad
\frac{W_{\rm ground}}{W_{\rm direct}}=\frac5{293.15}=0.0171.}
$$

The ideal coldest-day electrical-input ratios are **direct : air-source : deep-ground = 1 : 0.0853 : 0.0171**. The deep source needs one fifth of the ideal air-source [work](../../energy.md#work). These ratios compare equal useful heating, and do not include excavation, circulation losses or an assumed real compressor efficiency.

<h3 id="section-c/c13">C13</h3>

↑ **Parent:** [Section C](#section-c)

<h4 id="section-c/c13/solution">Solution</h4>

↑ **Parent:** [C13](#section-c/c13)

[Phase equilibrium](../../thermodynamics.md#phase-equilibrium) minimizes [Gibbs free energy](../../thermodynamic-potential.md#gibbs-free-energy) at specified [temperature](../../temperature.md), [pressure](../../pressure.md) and composition. Coexisting phases have equal [temperature](../../temperature.md), [pressure](../../pressure.md) and [chemical potential](../../chemical-potential.md). For a pure substance, a first-order transition has continuous equilibrium [Gibbs free energy](../../thermodynamic-potential.md#gibbs-free-energy) but a jump in its first derivatives, such as [entropy](../../entropy.md) or volume; the [latent heat](../../thermodynamic-potential.md#latent-heat) is $T\Delta S$. Continuous transitions lack that [latent heat](../../thermodynamic-potential.md#latent-heat) and can instead have singular or discontinuous higher responses.

The van der Waals molar equation

$$
p=\frac{RT}{v-b}-\frac a{v^2}
$$

combines an excluded-volume correction with attractive interactions. Its inflection conditions give

$$
\boxed{v_c=3b,\quad T_c=\frac{8a}{27Rb},\quad p_c=\frac{a}{27b^2}.}
$$

Below $T_c$, the oscillatory isotherm contains a mechanically unstable segment with $(\partial p/\partial v)_T>0$. Equilibrium instead replaces the loop by a constant-pressure coexistence line. Equality of chemical potentials gives the [Maxwell construction](../../thermodynamic-potential.md#maxwell-construction),

$$
\int_{v_\ell}^{v_g}[p(v,T)-p_{\rm sat}]\,dv=0.
$$

On isothermal compression the gas reaches saturation, then converts progressively into liquid at fixed [pressure](../../pressure.md). The mean [molar volume](../../thermodynamics.md#molar-volume) obeys $v=(1-x)v_\ell+xv_g$, where $x$ is the gas fraction. Metastable superheated or supercooled states can persist when [nucleation](../../critical-phenomenon.md#nucleation) is delayed; they are not the global equilibrium selected by this construction.

<a id="section-c/c13/image-illustrative-reduced-van-der-waals-coexistence-and-a-generic-pure-substance-phase-diagram"></a>
![](../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2013/paper-2-b2-phase-coexistence.png)

**[Figure 2](#section-c/c13/image-illustrative-reduced-van-der-waals-coexistence-and-a-generic-pure-substance-phase-diagram). Illustrative reduced van der Waals coexistence and a generic pure-substance phase diagram**.

A [pressure](../../pressure.md)–[temperature](../../temperature.md) [phase diagram](../../thermodynamic-potential.md#phase-diagram) contains coexistence curves separating solid, liquid and gas. Three phases meet at a [triple point](../../thermodynamic-potential.md#triple-point); the liquid–gas coexistence curve ends at a [thermodynamic critical point](../../critical-phenomenon.md#thermodynamic-critical-point), above which liquid and gas can be connected without crossing a first-order phase boundary. A generic solid–liquid line continues beyond the liquid–gas critical [temperature](../../temperature.md). For one component the [Gibbs phase rule](../../thermodynamic-potential.md#phase-rule) is $F=3-P$, so a three-phase equilibrium fixes both [temperature](../../temperature.md) and [pressure](../../pressure.md).

Along a two-phase coexistence curve, $d\mu=-s\,dT+v\,dp$ for each phase gives

$$
\boxed{\frac{dp}{dT}=\frac{\Delta s}{\Delta v}=\frac{L}{T\Delta v}.}
$$

This is the Clapeyron equation, valid with consistent molar or specific quantities. For vaporization, neglecting the liquid volume and treating the vapour as ideal gives $\Delta v\simeq RT/p$, hence $d\ln p/dT=L/(RT^2)$. With approximately constant molar [latent heat](../../thermodynamic-potential.md#latent-heat),

$$
\boxed{\ln\frac{p_2}{p_1}=-\frac LR\left(\frac1{T_2}-\frac1{T_1}\right).}
$$

This Clausius–Clapeyron approximation explains the rapid rise of vapour [pressure](../../pressure.md) with [temperature](../../temperature.md). It fails close to the [thermodynamic critical point](../../critical-phenomenon.md#thermodynamic-critical-point), where phase volumes converge, and is not a universal expression for melting. The sign of a melting-line slope depends on its volume change; water's denser liquid gives a familiar negative slope.

## ↑ Ancestors (11)

1. [2013](../2013.md)
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
