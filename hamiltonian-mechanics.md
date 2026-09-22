# Hamiltonian mechanics

↑ **Parent:** [Classical mechanics](classical-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamiltonian_mechanics)

Hamiltonian mechanics describes phase-space evolution through a Hamiltonian and the symplectic structure.

**Table of contents**

- [Adiabatic invariant](#adiabatic-invariant)
  - [Circular-shell adiabatic contraction](#circular-shell-adiabatic-contraction)
    - [Inner NFW contraction to a flat rotation curve](#inner-nfw-contraction-to-a-flat-rotation-curve)
  - [Particle-speed invariant between slowly approaching walls](#particle-speed-invariant-between-slowly-approaching-walls)
- [Hamiltonian system](#hamiltonian-system)
  - [Hénon-Heiles system](#henon-heiles-system)
    - [Hénon-Heiles potential](#henon-heiles-potential)
  - [Inverted quartic oscillator phase portrait](#inverted-quartic-oscillator-phase-portrait)
- [Conformal mechanics](#conformal-mechanics)
  - [Special conformal charge of inverse-square mechanics](#special-conformal-charge-of-inverse-square-mechanics)
- [Hamilton-Jacobi equation](#hamilton-jacobi-equation)
  - [Complete integral of the Hamilton-Jacobi equation](#complete-integral-of-the-hamilton-jacobi-equation)
- [Phase-space action](#phase-space-action)
  - [Relativistic particle phase-space action](#relativistic-particle-phase-space-action)
    - [Pseudoclassical spinning particle](#pseudoclassical-spinning-particle)
      - [Spinning-particle Dirac quantization](#spinning-particle-dirac-quantization)
      - [Spin from Grassmann bilinears](#spin-from-grassmann-bilinears)
    - [Light-cone Hamiltonian](#light-cone-hamiltonian)
    - [Worldline einbein](#worldline-einbein)
      - [Proper-time gauge for a massive worldline einbein](#proper-time-gauge-for-a-massive-worldline-einbein)
      - [Proper-time modulus](#proper-time-modulus)
        - [Worldline gauge-orbit determinant](#worldline-gauge-orbit-determinant)
- [Canonical variables](#canonical-variables)
  - [Canonical pair](#canonical-pair)
- [Leapfrog integration](#leapfrog-integration)
- [Hamiltonian flow](#hamiltonian-flow)
  - [Isotropic harmonic oscillator flow](#isotropic-harmonic-oscillator-flow)
  - [Uniform support bound from a coercive conserved energy](#uniform-support-bound-from-a-coercive-conserved-energy)
  - [Global characteristic flow for a Hamiltonian with bounded Hessian](#global-characteristic-flow-for-a-hamiltonian-with-bounded-hessian)
  - [Quadratic rotational Lie-Poisson dynamics](#quadratic-rotational-lie-poisson-dynamics)
- [Integral of motion](#integral-of-motion)
  - [Jacobi integral of a rigidly rotating potential](#jacobi-integral-of-a-rigidly-rotating-potential)
  - [Isolating integral](#isolating-integral)
    - [Isolating integrals and orbital closure dimension](#isolating-integrals-and-orbital-closure-dimension)
  - [Conserved quantity](#conserved-quantity)
- [Canonical momentum](#canonical-momentum)
  - [Canonical angular momentum across a solenoid fringe](#canonical-angular-momentum-across-a-solenoid-fringe)
  - [Canonical momentum sign in the affine particle action](#canonical-momentum-sign-in-the-affine-particle-action)
  - [Boundary-term shift of canonical field momenta](#boundary-term-shift-of-canonical-field-momenta)
- [Phase space](#phase-space)
  - [Velocity space](#velocity-space)
  - [Phase-space area](#phase-space-area)
  - [Phase-space trajectory](#phase-space-trajectory)
- [Hamiltonian](#hamiltonian)
  - [Hamilton's equations](#hamilton-s-equations)
- [Poisson bracket](#poisson-bracket)
  - [Poisson-commuting functions](#poisson-commuting-functions)
  - [Dirac bracket](#dirac-bracket)
    - [Graded Dirac bracket](#graded-dirac-bracket)
  - [Graded Poisson bracket](#graded-poisson-bracket)
  - [Jacobi identity for the Poisson bracket](#jacobi-identity-for-the-poisson-bracket)
    - [Poisson bracket of conserved quantities](#poisson-bracket-of-conserved-quantities)
      - [Poisson bracket of time-dependent conserved quantities](#poisson-bracket-of-time-dependent-conserved-quantities)
  - [Hamiltonian conservation law](#hamiltonian-conservation-law)
    - [Hamiltonian energy balance](#hamiltonian-energy-balance)
    - [Energy balance for an autonomous Lagrangian](#energy-balance-for-an-autonomous-lagrangian)
  - [Phase-space dilation generator](#phase-space-dilation-generator)
  - [Poisson bracket in complex canonical coordinates](#poisson-bracket-in-complex-canonical-coordinates)
    - [Anti-Hermitian quadratic Hamiltonian](#anti-hermitian-quadratic-hamiltonian)
- [Variational derivative](#variational-derivative)
  - [Hamiltonian field equation](#hamiltonian-field-equation)
    - [Hamiltonian evolution equation](#hamiltonian-evolution-equation)
- [Canonical transformation](#canonical-transformation)
  - [First-order canonical removal of a cubic oscillator perturbation](#first-order-canonical-removal-of-a-cubic-oscillator-perturbation)
    - [Second harmonic and mean displacement of a weakly cubic oscillator](#second-harmonic-and-mean-displacement-of-a-weakly-cubic-oscillator)
  - [Hyperbolic canonical chart for a quadratic oscillator](#hyperbolic-canonical-chart-for-a-quadratic-oscillator)
  - [Exact quadratic normal form for a perturbed linear rotor](#exact-quadratic-normal-form-for-a-perturbed-linear-rotor)
  - [Canonical completion of independent commuting functions](#canonical-completion-of-independent-commuting-functions)
  - [Type-two generating function for a canonical transformation](#type-two-generating-function-for-a-canonical-transformation)
  - [Type-one generating function for a canonical transformation](#type-one-generating-function-for-a-canonical-transformation)
- [Integrable Hamiltonian system](#integrable-hamiltonian-system)
  - [Superintegrable Hamiltonian system](#superintegrable-hamiltonian-system)
  - [Integrals of an irrational two-frequency oscillator](#integrals-of-an-irrational-two-frequency-oscillator)
  - [Hamiltonian period lattice](#hamiltonian-period-lattice)
  - [Stäckel potential](#stackel-potential)
    - [Orbit volume in an axisymmetric Stäckel potential](#orbit-volume-in-an-axisymmetric-stackel-potential)
    - [Axisymmetric Stäckel third integral](#axisymmetric-stackel-third-integral)
  - [First integrals in involution](#first-integrals-in-involution)
  - [Invariant torus](#invariant-torus)
    - [Quasiperiodic motion](#quasiperiodic-motion)
      - [Supremum of two incommensurate harmonic modes](#supremum-of-two-incommensurate-harmonic-modes)
      - [Incommensurate harmonic-oscillator orbit](#incommensurate-harmonic-oscillator-orbit)
  - [Direct product of integrable Hamiltonian systems](#direct-product-of-integrable-hamiltonian-systems)
  - [Liouville integrability of the isotropic harmonic oscillator](#liouville-integrability-of-the-isotropic-harmonic-oscillator)
  - [Liouville–Arnold theorem](#liouville-arnold-theorem)
  - [Action-angle variables](#action-angle-variables)
    - [Delaunay variables](#delaunay-variables)
    - [Action integral](#action-integral)
    - [Action variable](#action-variable)
      - [Radial action of a bound Kepler orbit](#radial-action-of-a-bound-kepler-orbit)
      - [Adiabatic invariance of the action](#adiabatic-invariance-of-the-action)
        - [Adiabatic particle between moving parallel walls](#adiabatic-particle-between-moving-parallel-walls)
        - [Adiabatic parameter scaling from an action](#adiabatic-parameter-scaling-from-an-action)
        - [Adiabatic invariance of an orbital action](#adiabatic-invariance-of-an-orbital-action)
          - [Adiabatic actions do not preserve orbital closure](#adiabatic-actions-do-not-preserve-orbital-closure)
      - [Radial action](#radial-action)
        - [Radial action of a Kepler orbit](#radial-action-of-a-kepler-orbit)
      - [Action of the one-dimensional Kepler collision orbit](#action-of-the-one-dimensional-kepler-collision-orbit)
- [Liouville's theorem (Hamiltonian)](#liouville-s-theorem-hamiltonian)

## Adiabatic invariant

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

A quantity conserved to leading order when a parameter varies slowly compared with the natural motion period. The [action variable](#action-variable) of a regular periodic Hamiltonian orbit is a standard example, as explained by [adiabatic invariance of the action](#adiabatic-invariance-of-the-action).

### Circular-shell adiabatic contraction

↑ **Parent:** [Adiabatic invariant](#adiabatic-invariant)

In a slowly changing spherical [gravitational potential](newton-s-law-of-universal-gravitation.md#newtonian-potential-of-a-point-mass), [angular momentum](momentum.md#angular-momentum) is exactly conserved and the [radial action](#radial-action) is an [adiabatic invariant](#adiabatic-invariant). An initially [circular orbit](classical-mechanics.md#circular-orbit) remains circular in the adiabatic limit, so $J_r=0$ and $L^2=GrM(r)$ give the displayed shell relation. If dark-matter shells do not cross, their enclosed dark mass is also conserved. A density profile alone does not specify this orbital model: eccentric-orbit populations require their full action distribution.

#### Inner NFW contraction to a flat rotation curve

↑ **Parent:** [Circular-shell adiabatic contraction](#circular-shell-adiabatic-contraction)

An inner [NFW profile](large-scale-structure-of-the-universe.md#navarro-frenk-white-profile) has $M_i(r_i)=Ar_i^2$, where $A=2\pi\rho_s r_s$. If the final total [circular speed](galaxy.md#circular-speed) is $V$, [circular-shell adiabatic contraction](#circular-shell-adiabatic-contraction) gives $r_i=(V^2/(GA))^{1/3}r^{2/3}$ and $M'_D=A^{1/3}(V^2/G)^{2/3}r^{4/3}$. Thus $\rho'_D=A^{1/3}(V^2/G)^{2/3}r^{-5/3}/(3\pi)$. The total density producing the flat curve is $V^2/(4\pi Gr^2)$, so the dark fraction tends to zero as $r^{1/3}$ despite its increase relative to the original cusp.

### Particle-speed invariant between slowly approaching walls

↑ **Parent:** [Adiabatic invariant](#adiabatic-invariant)

An [elastic collision](classical-mechanics.md#elastic-collision) with a wall moving toward the particle at speed $V$ changes the particle speed by approximately $2V$ when recoil is negligible. The collision rate is approximately $v/\ell$ for $v\gg V$, and $\dot\ell=-2V$, yielding $\dot v/v=-\dot\ell/\ell$. For a freely moving finite wall of mass $M$, the neglected recoil changes the increment by order $(m/M)v$, so relative accuracy also requires $(m/M)(v/V)\ll1$.

// Target: classical-mechanics.bigb

## Hamiltonian system

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

A dynamical system on a [symplectic manifold](symplectic-geometry.md#symplectic-manifold) whose vector field is generated by a [Hamiltonian](#hamiltonian). In [canonical variables](#canonical-variables) it obeys [Hamilton's equations](#hamilton-s-equations).

<h3 id="henon-heiles-system">Hénon-Heiles system</h3>

↑ **Parent:** [Hamiltonian system](#hamiltonian-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hénon–Heiles_system)

The Hénon-Heiles system is a [Hamiltonian system](#hamiltonian-system) with two [degrees of freedom](classical-mechanics.md#degree-of-freedom) and [Hamiltonian function](symplectic-geometry.md#hamiltonian-function)

$$
H=\frac12(p_x^2+p_y^2)+V(x,y),\qquad V(x,y)=\frac12(x^2+y^2)+x^2y-\frac13y^3.
$$

Its [Hamilton's equations](#hamilton-s-equations) give $\ddot x=-x-2xy$ and $\ddot y=-y-x^2+y^2$. Its [potential energy](energy.md#potential-energy) combines an isotropic quadratic minimum with a cubic interaction.

<h4 id="henon-heiles-potential">Hénon-Heiles potential</h4>

↑ **Parent:** [Hénon-Heiles system](#henon-heiles-system)

The [potential energy](energy.md#potential-energy) $V(x,y)=\tfrac12(x^2+y^2)+x^2y-y^3/3$ in the [Hénon-Heiles system](#henon-heiles-system) has the following expression in [polar coordinates](multivariable-calculus.md#polar-coordinates):

$$
V=\frac12r^2+\frac13r^3\sin(3\theta),
$$

so it is invariant under rotation through $2\pi/3$. Solving $\nabla V=0$ gives a strict [local minimum](analysis.md#local-minimum) at the origin and three [saddle points](analysis.md#saddle-point), at $(0,1)$ and $(\pm\sqrt3/2,-1/2)$. All three [saddle points](analysis.md#saddle-point) have value $1/6$. Their common [level set](topology.md#level-set) factors exactly:

$$
6V-1=(2y+1)\bigl[3x^2-(y-1)^2\bigr].
$$

Thus this [level set](topology.md#level-set) is the union of the three lines $y=-1/2$ and $y=1\pm\sqrt3x$. They bound an equilateral triangle containing the [local minimum](analysis.md#local-minimum). The [Hessian matrix](multivariable-calculus.md#hessian-matrix) is the identity at the origin; at each of the other three [stationary points](calculus-of-variations.md#stationary-point) it has [eigenvalues](linear-operator-theory.md#eigenvalue) $3$ and $-1$. For energies $0\leq E<1/6$, the central accessible region is bounded; above that value the three saddle passages allow paths from the centre to arbitrarily large radius. This follows directly from the radial potential: in each direction with $\sin(3\theta)<0$, its radial maximum occurs at $r=-1/\sin(3\theta)$, with value $1/[6\sin^2(3\theta)]\geq1/6$.

### Inverted quartic oscillator phase portrait

↑ **Parent:** [Hamiltonian system](#hamiltonian-system)

The [autonomous planar system](dynamical-systems.md#autonomous-planar-system) $\dot x=y-2y^3$, $\dot y=-x$ preserves $K$. Its origin is a [center equilibrium](dynamical-systems.md#center-equilibrium) and $(0,\pm1/\sqrt2)$ are [saddle equilibria](dynamical-systems.md#saddle-equilibrium). The level $K=1/4$ is $x=\pm(y^2-1/2)$: its two inner arcs are [heteroclinic orbits](dynamical-systems.md#heteroclinic-orbit) enclosing periodic motion, while its outer branches connect saddles to escaping trajectories. Since $|\dot y|\sim y^2$ on escaping levels, infinity is reached in finite time. Adding $\alpha x/2$ to $\dot x$ gives $\dot K=\alpha x^2$, so positive $\alpha$ produces outward crossing of central levels and breaks the equal-energy heteroclinic connections.

## Conformal mechanics

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

A one-dimensional particle with $H=p^2/2+g/x^2$ admits conserved time-translation, dilation and special-conformal charges. Their [Poisson brackets](#poisson-bracket) form the [sl2R Lie algebra](semisimple-lie-algebra.md#sl2r-lie-algebra). The homogeneity of the [inverse-square potential](energy.md#inverse-square-potential) is what allows the symmetry.

### Special conformal charge of inverse-square mechanics

↑ **Parent:** [Conformal mechanics](#conformal-mechanics)

For the extended canonical variables with $\{t,E\}=-1$ and $\{x,p\}=1$, the charge $K=t^2E-txp+x^2/2$ generates a special conformal transformation. Its time derivative is $2te(E-H)$, so it is conserved on the [constraint surface](classical-mechanics.md#constraint-surface). With a time-dependent parameter $\beta$, the multiplier varies as $\delta e=-2te\beta$ and the action variation is $\dot\beta K-d(\beta x^2/2)/d\lambda$.

## Hamilton-Jacobi equation

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

A principal function $S(q,t)$ obeys the [Hamilton-Jacobi equation](#hamilton-jacobi-equation) $\partial_tS+H(q,\partial_qS,t)=0$. A complete solution generates [canonical momentum](#canonical-momentum) components $p_j=\partial_jS$ and local canonical coordinates constant along motion. For a time-independent [Hamiltonian](#hamiltonian), $S=W(q)-Et$ reduces the equation to $H(q,\partial_qW)=E$. Additive separation of $W$ yields conserved separation constants, subject to local regularity and independence.

### Complete integral of the Hamilton-Jacobi equation

↑ **Parent:** [Hamilton-Jacobi equation](#hamilton-jacobi-equation)

A complete integral depends on as many independent parameters as configuration coordinates and supplies a locally invertible [canonical transformation](#canonical-transformation) to constants of motion. For a type-one generating function $G(q,Q,t)$, require a nondegenerate mixed-derivative matrix in the relevant local chart. Solving $G_t+H(q,G_q,t)=0$ makes the transformed [Hamiltonian](#hamiltonian) zero, so both new canonical coordinates and new [canonical momenta](#canonical-momentum) are constant. An arbitrary parameter-deficient solution does not ensure such a transformation.

## Phase-space action

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

A phase-space [action](lagrangian-mechanics.md#action) treats [canonical variables](#canonical-variables) as independent fields. Varying them gives [Hamilton's equations](#hamilton-s-equations); [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) can impose constraints.

### Relativistic particle phase-space action

↑ **Parent:** [Phase-space action](#phase-space-action)

The [worldline einbein](#worldline-einbein) imposes the relativistic [mass-shell condition](bosonic-string-theory.md#string-mass-shell-condition). With the [Minkowski metric](special-relativity.md#minkowski-metric) of signature $(-,+,\ldots,+)$, its [first-class constraint](classical-mechanics.md#first-class-constraint) is $\varphi=(p^2+M^2)/2$.

#### Pseudoclassical spinning particle

↑ **Parent:** [Relativistic particle phase-space action](#relativistic-particle-phase-space-action)

A pseudoclassical spinning particle supplements ordinary position and momentum by odd [Grassmann variables](multilinear-algebra.md#grassmann-variable). An even multiplier imposes $p^2=0$ and an odd multiplier imposes $p\cdot\zeta=0$. The odd symplectic term gives $\{\zeta^m,\zeta^n\}_{D}=-i\eta^{mn}$. Quantization represents these variables by a [Clifford algebra](algebra-over-a-field.md#clifford-algebra), producing a spinor wavefunction.

##### Spinning-particle Dirac quantization

↑ **Parent:** [Pseudoclassical spinning particle](#pseudoclassical-spinning-particle)

Quantizing the odd [Dirac brackets](#dirac-bracket) yields $\{\widehat\zeta^m,\widehat\zeta^n\}_+=\eta^{mn}$. The [constraint](classical-mechanics.md#constraint-mechanics) $p\cdot\zeta=0$ is then the [massless Dirac equation](relativistic-quantum-field.md#massless-dirac-equation) on a spinor. Its square enforces $p^2=0$, matching the even [constraint](classical-mechanics.md#constraint-mechanics). The spin bilinear is represented by $-i[\gamma^m,\gamma^n]/4$ in this action convention.

##### Spin from Grassmann bilinears

↑ **Parent:** [Pseudoclassical spinning particle](#pseudoclassical-spinning-particle)

The odd particle variables form an even antisymmetric tensor through their bilinear. Adding it to orbital angular momentum gives a conserved Lorentz [Noether charge](classical-field-theory.md#noether-charge). The particle and odd-variable equations make the two time derivatives cancel. After [spinning-particle Dirac quantization](#spinning-particle-dirac-quantization), the bilinear becomes the spinor Lorentz generator rather than an ordinary commuting classical spin vector.

#### Light-cone Hamiltonian

↑ **Parent:** [Relativistic particle phase-space action](#relativistic-particle-phase-space-action)

With $ds^2=-2dx^+dx^-+dx_i^2$, $x^+=t$, and $p_-\ne0$, the [mass-shell condition](bosonic-string-theory.md#string-mass-shell-condition) gives $H=-p_+=-(p_i^2+\mu^2)/(2p_-)$. In the future-directed sector $p^+=-p_->0$, this is $(p_i^2+\mu^2)/(2p^+)$. Its [Schrödinger equation](mathematical-physics.md#schrodinger-equation) is equivalent to the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) after multiplication by $2p_-$.

#### Worldline einbein

↑ **Parent:** [Relativistic particle phase-space action](#relativistic-particle-phase-space-action)

An einbein specifies a one-dimensional [metric tensor](general-relativity.md#metric-tensor) along a [worldline](special-relativity.md#world-line). In the [relativistic particle phase-space action](#relativistic-particle-phase-space-action) it is the [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) for the [mass-shell condition](bosonic-string-theory.md#string-mass-shell-condition) and transforms as $\delta e=\dot\epsilon$ under the corresponding canonical [gauge transformation](electromagnetism.md#gauge-transformation). After eliminating the [momentum](momentum.md), its geometric interpretation depends on the normalization of the particle [action](lagrangian-mechanics.md#action).

##### Proper-time gauge for a massive worldline einbein

↑ **Parent:** [Worldline einbein](#worldline-einbein)

For the [relativistic particle](special-relativity.md#relativistic-particle) action $S=(m/2)\int[g_{\mu\nu}\dot x^\mu\dot x^\nu/e-e]d\lambda$, varying the [worldline einbein](#worldline-einbein) gives $g_{\mu\nu}\dot x^\mu\dot x^\nu=-e^2$. On the positive-einbein branch the [proper time](special-relativity.md#proper-time) satisfies $ds=e\,d\lambda$. A [reparametrization](differential-geometry.md#reparametrization) with $\lambda'=s$ sets the transformed einbein to one, making the [geodesic equation](riemannian-geometry.md#geodesic-equation) affinely parametrized. This gauge choice is made after retaining the einbein [mass shell](special-relativity.md#mass-shell) constraint; fixing the action first would discard that equation. If the parameter interval is held fixed at both ends, its integrated [proper length](special-relativity.md#proper-length) is a modulus and cannot be arbitrarily changed by endpoint-preserving transformations.

##### Proper-time modulus

↑ **Parent:** [Worldline einbein](#worldline-einbein)

The constant mode of the [worldline einbein](#worldline-einbein) is not removed by [gauge transformations](electromagnetism.md#gauge-transformation) whose parameters vanish at the ends of a fixed interval. This Schwinger proper-time parameter remains integrated over after [gauge fixing](relativistic-quantum-field.md#gauge-fixing). For $\varphi=(p^2+M^2)/2$, the geometric on-shell proper length is $M\int e\,dt$.

###### Worldline gauge-orbit determinant

↑ **Parent:** [Proper-time modulus](#proper-time-modulus)

On a unit interval with gauge parameters vanishing at its ends, $e=s+\dot\epsilon$ separates the [worldline einbein](#worldline-einbein) into its invariant average $s$ and a [canonical gauge transformation](classical-mechanics.md#canonical-gauge-transformation). The Jacobian for nonconstant modes is $\det\partial_t$ between the appropriate boundary-condition spaces. On a circle its prime excludes the constant gauge-parameter zero mode. This [Faddeev-Popov determinant](relativistic-quantum-field.md#faddeev-popov-determinant) can be represented by anticommuting $b,c$ fields with an action proportional to $\int b\dot c\,dt$.

## Canonical variables

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

[Phase space](#phase-space) coordinates are canonical when their [Poisson brackets](#poisson-bracket) have the form $\{q^I,p_J\}=\delta^I_J$, with the position-position and momentum-momentum brackets zero.

### Canonical pair

↑ **Parent:** [Canonical variables](#canonical-variables)

A canonical pair consists of a coordinate and its [canonical momentum](#canonical-momentum), with [Poisson bracket](#poisson-bracket) $\{q,p\}=1$.

## Leapfrog integration

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Leapfrog_integration)

The leapfrog integrator alternates half-steps for momentum with a full step for position and a final momentum half-step. It is reversible, symplectic, and second-order accurate.

## Hamiltonian flow

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

Hamiltonian flow is the phase-space evolution generated by [Hamilton's equations](#hamilton-s-equations) for a fixed [Hamiltonian](#hamiltonian).

### Isotropic harmonic oscillator flow

↑ **Parent:** [Hamiltonian flow](#hamiltonian-flow)

For $H_\omega=(|v|^2+\omega^2|x|^2)/2$, the displayed linear [Hamiltonian flow](#hamiltonian-flow) solves $\dot X=V$, $\dot V=-\omega^2X$. Its inverse is $S_{-t}$, its determinant is one and it preserves $H_\omega$. The zero-frequency limit is the shear $(x,v)\mapsto(x+tv,v)$.

### Uniform support bound from a coercive conserved energy

↑ **Parent:** [Hamiltonian flow](#hamiltonian-flow)

For homogeneous [Hamiltonian Liouville equation](kinetic-theory.md#hamiltonian-liouville-equation) transport with autonomous $H$, compact initial support remains in the fixed energy sublevel determined by its maximum initial energy. If these sublevels are compact, this proves uniform compact support without solving the flow. The harmonic energy $H_\omega=(|v|^2+\omega^2|x|^2)/2$ has this property exactly when $\omega\ne0$; at zero frequency spatial free streaming can escape every compact set.

### Global characteristic flow for a Hamiltonian with bounded Hessian

↑ **Parent:** [Hamiltonian flow](#hamiltonian-flow)

If $H$ is $C^2$ and its spatial [Hessian matrix](multivariable-calculus.md#hessian-matrix) is uniformly bounded on every finite time interval, its [Hamiltonian vector field](symplectic-geometry.md#hamiltonian-vector-field) is globally [Lipschitz continuous](real-analysis.md#lipschitz-continuity) in [phase space](#phase-space) with at most linear growth. The [Picard-Lindelöf theorem](differential-equation.md#picard-lindelof-theorem) and [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) give a unique [Hamiltonian flow](#hamiltonian-flow) for all finite forward and backward times. Bounds on $\nabla_zH(t,0)$ follow from time continuity on compact intervals.

### Quadratic rotational Lie-Poisson dynamics

↑ **Parent:** [Hamiltonian flow](#hamiltonian-flow)

With the displayed signed [Lie-Poisson bracket](symplectic-geometry.md#lie-poisson-bracket) and evolution $\dot F=\{F,H\}$, the equations are $\dot x_1=2(C-B)x_2x_3$, $\dot x_2=2(A-C)x_3x_1$, and $\dot x_3=2(B-A)x_1x_2$. The energy and the [Casimir function of a Poisson manifold](symplectic-geometry.md#casimir-function-of-a-poisson-manifold) $x_1^2+x_2^2+x_3^2$ are conserved. For $A=1/(2I_1)$, $B=1/(2I_2)$, $C=1/(2I_3)$ with positive inertias, these are the [Euler equations for a torque-free rigid body](rigid-body-dynamics.md#euler-equations-for-a-torque-free-rigid-body). Reversing the bracket while fixing $H$ reverses time orientation.

## Integral of motion

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integral_of_motion)

An integral of motion is a function on [phase space](#phase-space) that remains constant along every trajectory. If it has no explicit time dependence, $I(q,p)$ is an integral exactly when its [Poisson bracket](#poisson-bracket) with the [Hamiltonian](#hamiltonian) vanishes: $\{I,H\}=0$.

### Jacobi integral of a rigidly rotating potential

↑ **Parent:** [Integral of motion](#integral-of-motion)

For $\Phi(R,\phi-\Omega t,z)$ with constant pattern angular velocity $\Omega$, ordinary specific [energy](energy.md) satisfies $\dot E=\partial_t\Phi=-\Omega\partial_\phi\Phi$ and specific axial [angular momentum](momentum.md#angular-momentum) satisfies $\dot L_z=-\partial_\phi\Phi$. Their combination $E_J$ is conserved. This is the rotating-frame [integral of motion](#integral-of-motion); in the [circular restricted three-body problem](celestial-mechanics.md#circular-restricted-three-body-problem), the usual [Jacobi constant](celestial-mechanics.md#jacobi-constant) is an affine rescaling of it. Thus time dependence in an inertial frame does not alone imply the absence of all integrals.

### Isolating integral

↑ **Parent:** [Integral of motion](#integral-of-motion)

An isolating integral is a regular single-valued [integral of motion](#integral-of-motion) whose fixed value restricts accessible [phase space](#phase-space) to a lower-dimensional level set. Functional independence of several such integrals means their differentials are linearly independent on the region considered. A central potential has [specific orbital energy](celestial-mechanics.md#specific-orbital-energy) and the three components of [specific angular momentum](celestial-mechanics.md#specific-angular-momentum) as four generically independent integrals. A [Kepler orbit](celestial-mechanics.md#kepler-orbit) has a fifth independent integral supplied by its fixed apsidal direction, encoded by the [Laplace-Runge-Lenz vector](classical-mechanics.md#laplace-runge-lenz-vector); its vector components obey two constraints with energy and angular momentum. Circular and radial orbits are degenerate cases of this count.

#### Isolating integrals and orbital closure dimension

↑ **Parent:** [Isolating integral](#isolating-integral)

In three-dimensional autonomous mechanics, a regular common level set of $N$ independent [isolating integrals](#isolating-integral) has dimension $6-N$ in [phase space](#phase-space). If an [orbit](dynamical-systems.md#orbit-dynamical-system) is dense in a $d$-dimensional [invariant torus](#invariant-torus) and the integrals characterize its closure, $N=6-d$. A generic three-frequency regular [orbit](dynamical-systems.md#orbit-dynamical-system) has three integrals; a spherical nonclosed rosette has energy and three components of [specific angular momentum](celestial-mechanics.md#specific-angular-momentum), with two-dimensional closure and four integrals. A periodic nonstationary [orbit](dynamical-systems.md#orbit-dynamical-system) has one-dimensional closure and can be isolated by five independent [orbit](dynamical-systems.md#orbit-dynamical-system) labels on the invariant family. The maximum is five wherever the [Hamiltonian vector field](symplectic-geometry.md#hamiltonian-vector-field) is nonzero, since all integral differentials annihilate that field. A single resonant [orbit](dynamical-systems.md#orbit-dynamical-system) need not yield an additional smooth single-valued integral on an open neighborhood; global superintegrability is stronger than orbital closure.

### Conserved quantity

↑ **Parent:** [Integral of motion](#integral-of-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conserved_quantity)

A conserved quantity is a quantity that remains constant along the time evolution of a system. In [Hamiltonian mechanics](hamiltonian-mechanics.md), a possibly time-dependent phase-space function $F$ is conserved exactly when $\partial_tF+\{F,H\}=0$.

## Canonical momentum

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_momentum)

The canonical momentum conjugate to a generalized coordinate $q_i$ is $p_i=\partial L/\partial\dot q_i$.

### Canonical angular momentum across a solenoid fringe

↑ **Parent:** [Canonical momentum](#canonical-momentum)

For an axisymmetric [magnetic vector potential](electromagnetism.md#magnetic-vector-potential), the conserved angular canonical [momentum](momentum.md) is $p_\theta=\gamma m\rho^2\dot\theta+q\rho A_\theta$. A particle arriving parallel to a solenoid axis from a field-free region has $p_\theta=0$. In a uniform field, $A_\theta=B\rho/2$ and $\dot\theta=-qB/(2\gamma m)$ wherever $\rho\neq0$. The mechanical angular momentum changes through the fringe while the canonical quantity remains constant. Static magnetic fields also conserve $\gamma mc^2$; the azimuthal kick therefore reduces axial kinetic motion rather than increasing total speed.

### Canonical momentum sign in the affine particle action

↑ **Parent:** [Canonical momentum](#canonical-momentum)

For the affine action $S=-\tfrac m2\int g_{\mu\nu}\dot x^\mu\dot x^\nu d\tau$ with signature $(-+++)$, differentiating with respect to velocity gives the displayed [canonical momentum](#canonical-momentum). Future-oriented proper time in a conformally flat metric yields $P_i^c=-a\gamma mv_i$, whereas the conventional future-directed mechanical momentum has $q_i=a\gamma mv_i$. Changing the action's overall sign interchanges these canonical labels but leaves its classical geodesics unchanged. Both labels are conserved by spatial [translation invariance](physics.md#translation-invariance), and either gives the same physical momentum magnitude proportional to $a^{-1}$. The sign should be stated when comparing a worldline canonical covector with a positive-frequency field-mode label.

### Boundary-term shift of canonical field momenta

↑ **Parent:** [Canonical momentum](#canonical-momentum)

If the spatially integrated [Lagrangian](calculus-of-variations.md#lagrangian) changes by $dB[\Phi]/dt$, where $B$ depends on fields and their spatial derivatives but not velocities, the [canonical momentum](#canonical-momentum) components change by $\pi_a\mapsto\pi_a+\delta B/\delta\Phi_a$. This follows by varying $dB/dt$ and using spatial [integration by parts](calculus.md#integration-by-parts). The canonical one-form changes by the exact variation $\delta B$, so the [symplectic form](symplectic-geometry.md#symplectic-form) and [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) are preserved. For the two [Feynman gauge](relativistic-quantum-field.md#feynman-gauge) Maxwell densities, $B=\int A_0\partial_iA_i\,d^3x$ gives shifts $\Delta\pi^0=\partial_iA_i$ and $\Delta\pi^i=-\partial_iA_0$. Boundary flux must vanish for this spatial functional calculation.

## Phase space

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Phase_space)

Phase space has one position coordinate $q_i$ and one conjugate momentum $p_i$ for every degree of freedom; a point $(q,p)$ specifies an instantaneous mechanical state.

### Velocity space

↑ **Parent:** [Phase space](#phase-space)

Velocity space is the space of velocity vectors at a fixed spatial position. Integrating a [galactic distribution function](galaxy.md#galactic-distribution-function) over velocity space produces [mass density](fluid-mechanics.md#density); its normalized moments determine mean velocity and [velocity dispersion](galaxy.md#velocity-dispersion).

### Phase-space area

↑ **Parent:** [Phase space](#phase-space)

The symplectic area enclosed by a closed orbit in a two-dimensional phase plane. With the orientation of Hamiltonian motion it is $\oint p\,dq=2\pi I$, where $I$ is the [action variable](#action-variable).

### Phase-space trajectory

↑ **Parent:** [Phase space](#phase-space)

An [integral curve of a vector field](multivariable-calculus.md#integral-curve-of-a-vector-field) in phase space, representing the positions and momenta of a moving system. A periodic one-dimensional Hamiltonian orbit encloses the area used to define the [action variable](#action-variable).

## Hamiltonian

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

The Hamiltonian is a function of canonical position and momentum that generates time evolution through Hamilton's equations.

<h3 id="hamilton-s-equations">Hamilton's equations</h3>

↑ **Parent:** [Hamiltonian](#hamiltonian)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamilton's_equations)

For canonical coordinates $(q_i,p_i)$ and Hamiltonian $H$,

$$
\dot q_i=\frac{\partial H}{\partial p_i},
\qquad
\dot p_i=-\frac{\partial H}{\partial q_i}.
$$

## Poisson bracket

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_bracket)

In canonical coordinates,

$$
\{F,G\}=\sum_i\left(
\frac{\partial F}{\partial q_i}\frac{\partial G}{\partial p_i}
-\frac{\partial F}{\partial p_i}\frac{\partial G}{\partial q_i}
\right).
$$

### Poisson-commuting functions

↑ **Parent:** [Poisson bracket](#poisson-bracket)

Functions $F_i$ for which $\{F_i,F_j\}=0$ for all pairs. Their [Hamiltonian vector fields](symplectic-geometry.md#hamiltonian-vector-field) commute, and each is constant along the flows of the others. When they are [integrals of motion](#integral-of-motion) of a [Hamiltonian](#hamiltonian), they are [first integrals in involution](#first-integrals-in-involution).

### Dirac bracket

↑ **Parent:** [Poisson bracket](#poisson-bracket)

Second-class constraints $\chi_a$ with invertible bracket matrix can be eliminated with a modified bracket. For an ordinary even constraint set it is $\{F,G\}_D=\{F,G\}-\{F,\chi_a\}(C^{-1})^{ab}\{\chi_b,G\}$, $C_{ab}=\{\chi_a,\chi_b\}$. Graded constraints require the matching graded sign convention.

#### Graded Dirac bracket

↑ **Parent:** [Dirac bracket](#dirac-bracket)

A [Dirac bracket](#dirac-bracket) on a graded phase space eliminates second-class constraints while respecting the [graded Poisson bracket](#graded-poisson-bracket). The fermionic kinetic term $i\psi^m\dot\psi_m/2$ gives $\{\psi^m,\psi^n\}_D=-i\eta^{mn}$. Quantization then gives $\{\widehat\psi^m,\widehat\psi^n\}_+=\eta^{mn}$.

### Graded Poisson bracket

↑ **Parent:** [Poisson bracket](#poisson-bracket)

An even Poisson bracket on a space with commuting and anticommuting variables obeys $\{F,G\}=-(-1)^{|F||G|}\{G,F\}$ and the graded Leibniz rule. In particular the bracket of two odd functions is symmetric. Quantization turns the odd-odd bracket into an anticommutator.

### Jacobi identity for the Poisson bracket

↑ **Parent:** [Poisson bracket](#poisson-bracket)

The Poisson bracket satisfies

$$
\{F,\{G,H\}\}+\{G,\{H,F\}\}+\{H,\{F,G\}\}=0.
$$

#### Poisson bracket of conserved quantities

↑ **Parent:** [Jacobi identity for the Poisson bracket](#jacobi-identity-for-the-poisson-bracket)

If $F$ and $G$ have no explicit time dependence and satisfy $\{F,H\}=\{G,H\}=0$, the Jacobi identity gives $\{\{F,G\},H\}=0$. Their Poisson bracket is therefore also conserved.

##### Poisson bracket of time-dependent conserved quantities

↑ **Parent:** [Poisson bracket of conserved quantities](#poisson-bracket-of-conserved-quantities)

The [derivative](calculus.md#derivative) $D_t=\partial_t+\{\,\cdot\,,H\}$ is a derivation of the [Poisson bracket](#poisson-bracket): $D_t\{f,g\}=\{D_tf,g\}+\{f,D_tg\}$. The time [derivative](calculus.md#derivative) part obeys the [product rule](calculus.md#product-rule), and the [Hamiltonian](#hamiltonian) part obeys it by the [Jacobi identity](lie-algebra.md#jacobi-identity). Therefore explicitly time-dependent conserved quantities also have a conserved [Poisson bracket](#poisson-bracket).

### Hamiltonian conservation law

↑ **Parent:** [Poisson bracket](#poisson-bracket)

Along a trajectory generated by the [Hamiltonian](#hamiltonian) $H$,

$$
\frac{dF}{dt}=\frac{\partial F}{\partial t}+\{F,H\}.
$$

Thus a time-independent observable is conserved exactly when its [Poisson bracket](#poisson-bracket) with $H$ vanishes.

#### Hamiltonian energy balance

↑ **Parent:** [Hamiltonian conservation law](#hamiltonian-conservation-law)

Along [Hamilton's equations](#hamilton-s-equations), spatial derivatives of the [Hamiltonian function](symplectic-geometry.md#hamiltonian-function) cancel in its total time derivative. Thus $dH/dt=\partial_tH$. An autonomous [Hamiltonian function](symplectic-geometry.md#hamiltonian-function) is conserved; explicit time dependence generally prevents conservation even though [phase space](#phase-space) is still preserved.

#### Energy balance for an autonomous Lagrangian

↑ **Parent:** [Hamiltonian conservation law](#hamiltonian-conservation-law)

For an autonomous [Lagrangian](calculus-of-variations.md#lagrangian) $L(x,\dot x)$, define its [action](lagrangian-mechanics.md#action) $A=\int L\,dt$ and [Hamiltonian](#hamiltonian) $H=\dot xL_{\dot x}-L$. The [chain rule](calculus.md#chain-rule) gives

$$
\dot H=\dot x\left(\frac d{dt}L_{\dot x}-L_x\right)
=-\dot x\frac{\delta A}{\delta x}.
$$

Thus the identity holds along forced trajectories as well as solutions of the homogeneous [Euler-Lagrange equation](analysis.md#euler-lagrange-equation). Explicit time dependence adds $-\partial_tL$; stochastic work requires a consistent regularization or the [Stratonovich chain rule](stochastic-calculus.md#stratonovich-chain-rule).

### Phase-space dilation generator

↑ **Parent:** [Poisson bracket](#poisson-bracket)

The function $D=q\cdot p$ generates the canonical scaling $(q,p)\mapsto(e^tq,e^{-t}p)$. An observable $F$ is invariant under this scaling exactly when

$$
\{F,D\}=q\cdot\nabla_qF-p\cdot\nabla_pF=0.
$$

### Poisson bracket in complex canonical coordinates

↑ **Parent:** [Poisson bracket](#poisson-bracket)

For $z_j=q_j+ip_j$ and $\bar z_j=q_j-ip_j$,

$$
\{f,g\}
=-2i\frac{\partial f}{\partial z_j}
\frac{\partial g}{\partial\bar z_j}
+2i\frac{\partial g}{\partial z_j}
\frac{\partial f}{\partial\bar z_j}.
$$

This follows from $\partial_{q_j}=\partial_{z_j}+\partial_{\bar z_j}$ and $\partial_{p_j}=i\partial_{z_j}-i\partial_{\bar z_j}$.

#### Anti-Hermitian quadratic Hamiltonian

↑ **Parent:** [Poisson bracket in complex canonical coordinates](#poisson-bracket-in-complex-canonical-coordinates)

For an anti-Hermitian matrix $A$, the real quadratic Hamiltonian

$$
I_A=\frac1{2i}\bar z^TAz
$$

satisfies

$$
\{I_A,I_B\}=-I_{[A,B]}.
$$

Thus $A\mapsto-I_A$ realizes the matrix commutator as a Poisson bracket; it is the quadratic moment-map construction for the unitary action.

## Variational derivative

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

For a functional $H[u]$, its variational derivative is defined by

$$
\left.\frac d{d\epsilon}H[u+\epsilon v]\right|_{\epsilon=0}
=\int\frac{\delta H}{\delta u}v\,dx
$$

after integrating derivatives of $v$ by parts and discarding the boundary terms.

### Hamiltonian field equation

↑ **Parent:** [Variational derivative](#variational-derivative)

For a complex field $\psi$, the canonical Hamiltonian evolution convention

$$
i\psi_t=\frac{\delta H}{\delta\overline\psi}
$$

is accompanied by its complex conjugate equation.

#### Hamiltonian evolution equation

↑ **Parent:** [Hamiltonian field equation](#hamiltonian-field-equation)

An evolution equation has Hamiltonian form when a Hamiltonian operator applied to the [variational derivative](#variational-derivative) of a functional gives its time [derivative](calculus.md#derivative). The induced functional bracket must satisfy the Poisson properties, including Jacobi.

## Canonical transformation

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Canonical_transformation)

A canonical transformation preserves the symplectic form and hence all Poisson brackets. In one degree of freedom, an invertible map $(q,p)\mapsto(Q,P)$ is canonical exactly when $\{Q,P\}_{q,p}=1$.

### First-order canonical removal of a cubic oscillator perturbation

↑ **Parent:** [Canonical transformation](#canonical-transformation)

The accompanying [momentum](momentum.md) map is $p=P+2\lambda XP/(m\omega^2)$. Its [Poisson bracket](#poisson-bracket) is one up to second-order corrections. Substitution into $p^2/(2m)+m\omega^2x^2/2+\lambda x^3$ cancels all terms linear in $\lambda$, leaving a harmonic [Hamiltonian](#hamiltonian) to that order. The map is local and perturbative, not an exact global removal of an unbounded cubic potential.

#### Second harmonic and mean displacement of a weakly cubic oscillator

↑ **Parent:** [First-order canonical removal of a cubic oscillator perturbation](#first-order-canonical-removal-of-a-cubic-oscillator-perturbation)

With $\vartheta=\omega t+\delta$, a weak cubic potential produces a nonzero mean position and a second harmonic at first order. There is no first-order [frequency](wave.md#frequency) shift. Higher-order [frequency](wave.md#frequency) changes can accumulate [phase](wave.md#phase-waves) over sufficiently long times, so the first-order expression is not a uniform all-time approximation.

### Hyperbolic canonical chart for a quadratic oscillator

↑ **Parent:** [Canonical transformation](#canonical-transformation)

For $p>0$, $Q=\sqrt{2p}\sinh q$ and $P=\sqrt{2p}\cosh q$ satisfy $\{Q,P\}=1$. They transform $p\cosh2q$ into $(Q^2+P^2)/2$. Their inverse is $p=(P^2-Q^2)/2$ and $q=\operatorname{artanh}(Q/P)$, so the chart covers only $P>|Q|$, not the whole oscillator plane. Oscillator evolution beyond that wedge is not a global real continuation of the original variables.

### Exact quadratic normal form for a perturbed linear rotor

↑ **Parent:** [Canonical transformation](#canonical-transformation)

For $H=\omega\cdot y+\frac12|y|^2+\epsilon V(x)$ with a [Diophantine frequency vector](diophantine-approximation.md#diophantine-frequency-vector), solve $\mathcal D_\omega u=\langle V\rangle-V$ and apply [translated conjugacy of a Diophantine vector field](fourier-series.md#translated-conjugacy-of-a-diophantine-vector-field) to $w=\epsilon\nabla u$. Set $\eta=\epsilon\nabla u+a$ and use the [symplectic cotangent lift with a closed momentum shift](symplectic-geometry.md#symplectic-cotangent-lift-with-a-closed-momentum-shift). The transformed [Hamiltonian](#hamiltonian) is exactly $E+\omega\cdot y'+\frac12y'^T D\chi^{-1}D\chi^{-T}y'+\frac12|\eta\circ\chi|^2$, where $E=\epsilon\langle V\rangle+\omega\cdot a$. Since $a=O(\epsilon^2)$, the last term is an angular potential of order $\epsilon^2$ and the quadratic coefficient is identity plus $O(\epsilon)$. The construction is on a smaller angular strip and momentum ball.

### Canonical completion of independent commuting functions

↑ **Parent:** [Canonical transformation](#canonical-transformation)

Independent functions $Q_1,\ldots,Q_n$ on a $2n$-dimensional [symplectic manifold](symplectic-geometry.md#symplectic-manifold) can locally form the position half of canonical coordinates exactly when $\{Q_i,Q_j\}=0$ throughout a neighbourhood. Their commuting [Hamiltonian vector fields](symplectic-geometry.md#hamiltonian-vector-field) span the fibres of $Q$. Flow from a transverse section gives coordinates $(Q,t)$ with $\omega=\sum dt_i\wedge dQ_i+\beta(Q)$. Write $\beta=d\alpha$ locally and take $P_i=-t_i-\alpha_i(Q)$. Then $\omega=\sum dQ_i\wedge dP_i$.

### Type-two generating function for a canonical transformation

↑ **Parent:** [Canonical transformation](#canonical-transformation)

A function $S(q,P)$ generates a canonical transformation through

$$
p=\frac{\partial S}{\partial q},
\qquad
Q=\frac{\partial S}{\partial P}.
$$

### Type-one generating function for a canonical transformation

↑ **Parent:** [Canonical transformation](#canonical-transformation)

A function $\Phi(q,Q)$ generates a canonical transformation through

$$
p=\frac{\partial\Phi}{\partial q},
\qquad
P=-\frac{\partial\Phi}{\partial Q}.
$$

## Integrable Hamiltonian system

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)

Liouville integrability means having $n$ almost-everywhere independent first integrals in mutual Poisson involution.

For a Hamiltonian phase space of dimension $2n$, Liouville integrability means $n$ functionally independent conserved quantities with pairwise vanishing [Poisson brackets](#poisson-bracket). This is the Hamiltonian specialization of [integrable systems](integrable-systems.md).

### Superintegrable Hamiltonian system

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

A [superintegrable Hamiltonian system](#superintegrable-hamiltonian-system) with $n$ degrees of freedom has more than $n$ functionally independent [integrals of motion](#integral-of-motion), including an integrable set of $n$ in involution. At a regular nonzero [Hamiltonian vector field](symplectic-geometry.md#hamiltonian-vector-field), at most $2n-1$ independent integral differentials can annihilate the flow. A maximally superintegrable system attains that bound. The three-dimensional [Kepler orbit](celestial-mechanics.md#kepler-orbit) has five independent integrals through energy, angular momentum and the [Laplace-Runge-Lenz vector](classical-mechanics.md#laplace-runge-lenz-vector). A closed orbit on one isolated resonance is weaker than maximal superintegrability on an open phase-space region.

### Integrals of an irrational two-frequency oscillator

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

On the regular set of two uncoupled oscillators with irrational frequency ratio, every continuous globally defined [integral of motion](#integral-of-motion) is constant on each fixed-action [flat torus](second-fundamental-form.md#flat-torus), because every orbit is dense there. A differentiable integral is consequently a function of the two actions, so its [differential of a smooth map](smooth-manifold.md#differential-of-a-smooth-map) lies in their span. Local angle combinations can still give extra local integrals; they fail to be single-valued on the torus.

### Hamiltonian period lattice

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

For a compact connected regular level of $n$ independent [Poisson-commuting functions](#poisson-commuting-functions), the periods of their joint flow form a full-rank discrete subgroup $\Lambda\subset\mathbb R^n$. The level is $\mathbb R^n/\Lambda$. A local smooth basis of these periods determines [action integrals](#action-integral) and the normalized periodic fields used to construct [action-angle variables](#action-angle-variables).

<h3 id="stackel-potential">Stäckel potential</h3>

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

A [Stäckel potential](#stackel-potential) allows additive separation of the [Hamilton-Jacobi equation](#hamilton-jacobi-equation) in an orthogonal coordinate system. In axisymmetric [prolate spheroidal coordinates](general-relativity.md#prolate-spheroidal-coordinates), the relative-potential form is $\psi=[G(\lambda)-G(\mu)]/(\lambda-\mu)$. It gives [energy](energy.md), axial [angular momentum](momentum.md#angular-momentum) and an independent third separation [integral](integral.md). Here $G$ is a one-variable generating function, not the gravitational constant. Generic bounded [orbits](dynamical-systems.md#orbit-dynamical-system) are regular invariant-torus motions; resonance and coordinate degeneracy require separate treatment.

<h4 id="orbit-volume-in-an-axisymmetric-stackel-potential">Orbit volume in an axisymmetric Stäckel potential</h4>

↑ **Parent:** [Stäckel potential](#stackel-potential)

For fixed $E,l,I$, separated motion obeys $p_\tau^2=[E\tau+G(\tau)-I+(\alpha-\beta)l^2/(2(\tau+\alpha))]/[2(\tau+\alpha)(\tau+\beta)]$. Allowed intervals are where this is nonnegative, with turning points and coordinate-fold endpoints treated separately. A generic nonresonant bound [orbit](dynamical-systems.md#orbit-dynamical-system) with $l\ne0$ circulates azimuthally and densely samples a projected [volume](geometry-and-topology.md#volume) bounded by confocal spheroids and hyperboloids. It is not uniformly distributed in [volume](geometry-and-topology.md#volume). Resonant or zero-angular-momentum [orbits](dynamical-systems.md#orbit-dynamical-system) can project to lower-dimensional regions; integrability alone does not imply that every [orbit](dynamical-systems.md#orbit-dynamical-system) fills a three-dimensional shell.

<h4 id="axisymmetric-stackel-third-integral">Axisymmetric Stäckel third integral</h4>

↑ **Parent:** [Stäckel potential](#stackel-potential)

For $H=\tfrac12\sum p_j^2/h_j^2-\psi$, $l=p_\phi$ and a [Stäckel potential](#stackel-potential), multiplying the separated [Hamilton-Jacobi equation](#hamilton-jacobi-equation) by $\lambda-\mu$ gives $2(\tau+\alpha)(\tau+\beta)p_\tau^2-(\alpha-\beta)l^2/[2(\tau+\alpha)]-G(\tau)-E\tau=-I$ for both $\tau=\lambda,\mu$. Eliminating $E$ gives $I=\tfrac12[\mu v_\lambda^2+\lambda v_\mu^2+(\lambda+\mu+\alpha)v_\phi^2]-[\mu G(\lambda)-\lambda G(\mu)]/(\lambda-\mu)$. Physical components are $v_j=h_j\dot q_j$ and $p_j=h_jv_j$. Separation proves conservation locally; direct [Poisson brackets](#poisson-bracket) extend it across regular coordinate patches.

### First integrals in involution

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

First integrals are in involution when every pair has zero [Poisson bracket](#poisson-bracket). An $n$-degree-of-freedom Hamiltonian system is [Liouville integrable](#integrable-hamiltonian-system) when it has $n$ almost-everywhere independent first integrals in involution.

### Invariant torus

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

An invariant torus is a subset homeomorphic to a [torus](topological-surface.md#torus) and preserved by a [flow](dynamical-systems.md#flow-map). In [action-angle variables](#action-angle-variables), an integrable Hamiltonian flow moves linearly in the angular coordinates of each regular invariant torus.

The torus is a particular [invariant manifold](dynamical-systems.md#invariant-manifold); its toroidal topology is an extra condition beyond invariance.

#### Quasiperiodic motion

↑ **Parent:** [Invariant torus](#invariant-torus)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quasiperiodic_motion)

A quasiperiodic orbit on a torus has angular coordinates $\theta(t)=\theta(0)+\omega t$ modulo $2\pi$. It is [periodic](dynamical-systems.md#periodic-orbit) exactly when the nonzero frequencies are commensurate; rationally independent frequencies produce a dense orbit.

##### Supremum of two incommensurate harmonic modes

↑ **Parent:** [Quasiperiodic motion](#quasiperiodic-motion)

For $x(t)=A\cos\omega_1t+B\cos\omega_2t$ with irrational [frequency](wave.md#frequency) ratio and nonzero [amplitudes](wave.md#wave-amplitude), $|x|\le|A|+|B|$. The [phase](wave.md#phase-waves) trajectory is dense on the two-torus, so this bound is a [supremum](real-analysis.md#supremum). The required exact [phase](wave.md#phase-waves) alignment may never occur at finite time. Thus an exam's maximum-amplitude estimate can be a limiting bound rather than an attained displacement; finite observation intervals have smaller maxima.

##### Incommensurate harmonic-oscillator orbit

↑ **Parent:** [Quasiperiodic motion](#quasiperiodic-motion)

For two uncoupled [harmonic oscillators](classical-mechanics.md#simple-harmonic-motion) with nonzero amplitudes and irrational frequency ratio $\omega_1/\omega_2$, the orbit is bounded but not [periodic](dynamical-systems.md#periodic-orbit). It winds quasiperiodically on a two-dimensional [invariant torus](#invariant-torus); a common period would force the frequency ratio to be rational.

### Direct product of integrable Hamiltonian systems

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

The direct product of integrable Hamiltonian systems is integrable. Pull each family's commuting [integrals of motion](#integral-of-motion) back to the product [phase space](#phase-space). Integrals from different factors have zero [Poisson bracket](#poisson-bracket) because they use disjoint canonical coordinates, and their [differentials](multivariable-calculus.md#total-differential) are independent wherever the differentials within each factor are independent.

### Liouville integrability of the isotropic harmonic oscillator

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)

For

$$
H=\frac12\sum_{j=1}^n(q_j^2+p_j^2),
$$

the functions $I_j=(q_j^2+p_j^2)/2$ are independent almost everywhere, Poisson commute, and sum to $H$. A regular common level $I_j=c_j>0$ is the product of circles of radii $\sqrt{2c_j}$, hence an invariant $n$-torus. Allowing some $c_j=0$ gives lower-dimensional singular tori.

<h3 id="liouville-arnold-theorem">Liouville–Arnold theorem</h3>

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liouville–Arnold_theorem)

A compact connected regular common level of $n$ commuting integrals is an $n$-torus with local action-angle coordinates.

### Action-angle variables

↑ **Parent:** [Integrable Hamiltonian system](#integrable-hamiltonian-system)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Action-angle_variables)

For a one-degree-of-freedom closed orbit, action-angle coordinates make the Hamiltonian a function $H(I)$ and give $\dot I=0$, $\dot\phi=dH/dI$.

#### Delaunay variables

↑ **Parent:** [Action-angle variables](#action-angle-variables)

For a bound noncollision [Kepler orbit](celestial-mechanics.md#kepler-orbit) with gravitational parameter $\mu$, the canonical actions per unit mass are $\mathcal L=\sqrt{\mu a}$, $\mathcal G=\mathcal L\sqrt{1-e^2}$ and $\mathcal H=\mathcal G\cos i$. Their angles are [mean anomaly](celestial-mechanics.md#mean-anomaly) $\ell$, [argument of periapsis](celestial-mechanics.md#argument-of-periapsis) $\omega$ and [longitude of ascending node](celestial-mechanics.md#longitude-of-ascending-node) $\Omega$. The [Hamiltonian](#hamiltonian) is $-\mu^2/(2\mathcal L^2)$, so only $\ell$ advances in the unperturbed problem. In the prograde spherical-action chart, $J_r=\mathcal L-\mathcal G$, $J_\theta=\mathcal G-\mathcal H$, $J_\phi=\mathcal H$; the type-two [canonical transformation](#canonical-transformation) is generated by $F_2=(\mathcal L-\mathcal G)w_r+(\mathcal G-\mathcal H)w_\theta+\mathcal H w_\phi$. Retrograde spherical actions have $J_\theta=\mathcal G-|\mathcal H|$, so the absolute value cannot be dropped globally. Circular and coplanar limits are singular angle charts, not singular orbits.

#### Action integral

↑ **Parent:** [Action-angle variables](#action-angle-variables)

Near a regular [Lagrangian torus](symplectic-geometry.md#lagrangian-torus), choose a one-form $\lambda$ with $d\lambda=-\omega$ and a basis of fibre cycles $\gamma_j$. The action $I_j=(2\pi)^{-1}\int_{\gamma_j}\lambda$ has [differential of a smooth map](smooth-manifold.md#differential-of-a-smooth-map) $dI_j=(2\pi)^{-1}\sum_i t_i^{(j)}dF_i$, where $t^{(j)}$ is the corresponding joint-flow period. Nonsingularity of the period matrix makes these actions local coordinates transverse to the tori.

#### Action variable

↑ **Parent:** [Action-angle variables](#action-angle-variables)

With angle period $2\pi$, the action is the enclosed phase-space area divided by $2\pi$:

$$
I=(2\pi)^{-1}\oint p\,dq.
$$

This is the action component of [action-angle variables](#action-angle-variables), rather than the entire coordinate construction.

##### Radial action of a bound Kepler orbit

↑ **Parent:** [Action variable](#action-variable)

For $H=p_r^2/2+\ell^2/(2r^2)-k/r$, a noncollision bound orbit has $\ell\ne0$ and $-k^2/(2\ell^2)\leq E<0$. Its radial action is $\sqrt{-2E}/\pi$ times $\int_\alpha^\beta\sqrt{(r-\alpha)(\beta-r)}\,dr/r$, where $\alpha,\beta=[k\mp\sqrt{k^2+2E\ell^2}]/(-2E)$. Evaluating the integral gives the displayed action and $H=-k^2/[2(I_r+|\ell|)^2]$. The angular and radial frequencies have equal magnitudes, explaining closed orbits rather than generic quasiperiodicity. The circular limit has $I_r=0$; zero angular momentum gives collision in the unregularized phase space.

##### Adiabatic invariance of the action

↑ **Parent:** [Action variable](#action-variable)

When a Hamiltonian parameter varies slowly compared with the orbital period and no separatrix is crossed, the action changes only at higher adiabatic order.

The action is an [adiabatic invariant](#adiabatic-invariant) under these assumptions; other slowly varying systems can have different adiabatic invariants.

###### Adiabatic particle between moving parallel walls

↑ **Parent:** [Adiabatic invariance of the action](#adiabatic-invariance-of-the-action)

For a one-dimensional particle of energy $E$ between walls separated by $L$, the unnormalized action is

$$
\mathcal I=\oint p\,dq=2L\sqrt{2mE}.
$$

Adiabatic conservation gives $E(t)L(t)^2=\text{constant}$.

###### Adiabatic parameter scaling from an action

↑ **Parent:** [Adiabatic invariance of the action](#adiabatic-invariance-of-the-action)

If an action has parameter dependence $I\propto\sqrt{m/|E|}$, adiabatic conservation implies $|E|\propto m$.

###### Adiabatic invariance of an orbital action

↑ **Parent:** [Adiabatic invariance of the action](#adiabatic-invariance-of-the-action)

When a gravitational potential changes slowly relative to an orbital period, the orbital actions remain constant provided no separatrix is crossed. In a spherical potential, angular momentum is conserved exactly and the radial action is adiabatically conserved.

###### Adiabatic actions do not preserve orbital closure

↑ **Parent:** [Adiabatic invariance of an orbital action](#adiabatic-invariance-of-an-orbital-action)

[Adiabatic invariance of an orbital action](#adiabatic-invariance-of-an-orbital-action) preserves action values during slow regular changes, but frequencies $\partial H/\partial J_i$ can vary. Closure requires rational frequency ratios, which need not persist. A slowly added harmonic component in a [Kepler orbit](celestial-mechanics.md#kepler-orbit) potential produces generic apsidal precession.

##### Radial action

↑ **Parent:** [Action variable](#action-variable)

For radial motion between turning radii $r_-$ and $r_+$ in a central potential, the radial action per unit mass is

$$
J_r=\frac1\pi\int_{r_-}^{r_+}
\sqrt{2[E-\Phi(r)]-\frac{L^2}{r^2}}\,dr.
$$

It vanishes on a circular orbit and is canonically conjugate to the radial angle.

###### Radial action of a Kepler orbit

↑ **Parent:** [Radial action](#radial-action)

For a bound Kepler orbit of semimajor axis $a$ around mass $M$,

$$
J_r+L=\sqrt{GMa}.
$$

Adiabatic central-mass change therefore preserves $Ma$ and orbital eccentricity.

##### Action of the one-dimensional Kepler collision orbit

↑ **Parent:** [Action variable](#action-variable)

For $H=p^2/(2m)-1/|q|=-|E|$, collision continuation between the two turning points gives $I=\sqrt{2m/|E|}$.

<h2 id="liouville-s-theorem-hamiltonian">Liouville's theorem (Hamiltonian)</h2>

↑ **Parent:** [Hamiltonian mechanics](hamiltonian-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liouville's_theorem_(Hamiltonian))

Hamiltonian flow has zero phase-space divergence and preserves phase volume.

## ↑ Ancestors (4)

1. [Classical mechanics](classical-mechanics.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (11)

- [Classical mechanics](classical-mechanics.md)
- [Conserved quantity](#conserved-quantity)
- [Equation of motion](classical-mechanics.md#equation-of-motion)
- [Solution](past-exam-of-the-chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1.md#7/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-59.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-50.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-16.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#8e/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-2.md#5/solution)
- [Symplectic basis](bilinear-form.md#symplectic-basis)
