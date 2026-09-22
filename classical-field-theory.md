# Classical field theory

↑ **Parent:** [Quantum field theory](quantum-field-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Classical_field_theory)

**Table of contents**

- [Global symmetry in field theory](#global-symmetry-in-field-theory)
  - [Scattering charge selection rule from global gauge symmetry](#scattering-charge-selection-rule-from-global-gauge-symmetry)
- [Massive two-form field](#massive-two-form-field)
  - [Light-cone decomposition of a massive two-form](#light-cone-decomposition-of-a-massive-two-form)
- [Hamiltonian density](#hamiltonian-density)
  - [Canonical Hamiltonian density of a real scalar field](#canonical-hamiltonian-density-of-a-real-scalar-field)
- [Gauge theory](#gauge-theory)
  - [Grand unified theory](#grand-unified-theory)
    - [Pati-Salam model](#pati-salam-model)
      - [Pati-Salam charge embedding](#pati-salam-charge-embedding)
        - [Pati-Salam neutrino hypercharge cancellation](#pati-salam-neutrino-hypercharge-cancellation)
  - [Chiral gauge theory](#chiral-gauge-theory)
  - [Lattice gauge theory](#lattice-gauge-theory)
  - [Noether gauging procedure](#noether-gauging-procedure)
- [Internal symmetry of a classical field theory](#internal-symmetry-of-a-classical-field-theory)
  - [O(4) symmetry of a complex scalar doublet](#o-4-symmetry-of-a-complex-scalar-doublet)
  - [Reciprocal rescaling symmetry of two cross-coupled scalar fields](#reciprocal-rescaling-symmetry-of-two-cross-coupled-scalar-fields)
- [Variational symmetry of a Lagrangian density](#variational-symmetry-of-a-lagrangian-density)
- [Scalar field](#scalar-field)
  - [Minimally coupled scalar field](#minimally-coupled-scalar-field)
    - [Scalar stress-energy divergence identity](#scalar-stress-energy-divergence-identity)
  - [Scalar mass](#scalar-mass)
  - [Adjoint scalar field](#adjoint-scalar-field)
  - [Sextic scalar field theory](#sextic-scalar-field-theory)
  - [Zero-dimensional scalar field theory](#zero-dimensional-scalar-field-theory)
    - [Zero-dimensional quartic perturbation series](#zero-dimensional-quartic-perturbation-series)
  - [Charged scalar field](#charged-scalar-field)
    - [Linear-in-potential charged-scalar Lagrangian](#linear-in-potential-charged-scalar-lagrangian)
      - [Global phase current of a linearly coupled complex scalar](#global-phase-current-of-a-linearly-coupled-complex-scalar)
      - [Canonical Hamiltonian of a linearly coupled complex scalar](#canonical-hamiltonian-of-a-linearly-coupled-complex-scalar)
    - [Gauge-covariant derivative of a charged scalar field](#gauge-covariant-derivative-of-a-charged-scalar-field)
    - [Gauge-covariant wave equation for a charged scalar field](#gauge-covariant-wave-equation-for-a-charged-scalar-field)
  - [Scalar potential](#scalar-potential)
    - [Flat direction of a scalar potential](#flat-direction-of-a-scalar-potential)
  - [Scalar-field shift symmetry](#scalar-field-shift-symmetry)
- [Lagrangian (field theory)](#lagrangian-field-theory)
  - [Lagrangian density](#lagrangian-density)
    - [Kinetic term](#kinetic-term)
      - [Gauge-covariant kinetic term](#gauge-covariant-kinetic-term)
    - [Mass term](#mass-term)
    - [Field interaction term](#field-interaction-term)
    - [Euler-Lagrange field equation](#euler-lagrange-field-equation)
      - [Damped and antidamped fields from an antisymmetric velocity coupling](#damped-and-antidamped-fields-from-an-antisymmetric-velocity-coupling)
      - [Euler-Lagrange field equation with second derivatives](#euler-lagrange-field-equation-with-second-derivatives)
      - [On shell](#on-shell)
- [Noether current](#noether-current)
  - [Axial angular-momentum current of an elastic string](#axial-angular-momentum-current-of-an-elastic-string)
  - [Transverse momentum current of an elastic string](#transverse-momentum-current-of-an-elastic-string)
  - [Unitary scalar multiplet current](#unitary-scalar-multiplet-current)
  - [Shift current of an elastic rod](#shift-current-of-an-elastic-rod)
  - [Noether current for a constant shift with second derivatives](#noether-current-for-a-constant-shift-with-second-derivatives)
  - [Conformal current](#conformal-current)
  - [Virial current](#virial-current)
  - [Noether current for a spacetime symmetry](#noether-current-for-a-spacetime-symmetry)
  - [Noether current for a first-derivative scalar field](#noether-current-for-a-first-derivative-scalar-field)
  - [Conserved current](#conserved-current)
    - [Conserved charge](#conserved-charge)
    - [Conserved-current two-point function](#conserved-current-two-point-function)
  - [Noether charge](#noether-charge)
  - [Dilatation current](#dilatation-current)
    - [On-shell divergence of a quartic scalar dilation current](#on-shell-divergence-of-a-quartic-scalar-dilation-current)
    - [Scale-breaking sources in derivative field theories](#scale-breaking-sources-in-derivative-field-theories)
    - [Dilatation charge of a one-dimensional elastic wave](#dilatation-charge-of-a-one-dimensional-elastic-wave)
  - [Canonical stress-energy tensor](#canonical-stress-energy-tensor)
    - [Scalar-field momentum flux](#scalar-field-momentum-flux)
    - [Four-momentum of a free real scalar field](#four-momentum-of-a-free-real-scalar-field)
      - [Normal-ordered free scalar four-momentum](#normal-ordered-free-scalar-four-momentum)
        - [Translation of a scalar creation operator](#translation-of-a-scalar-creation-operator)
    - [Canonical stress-energy tensor of the Maxwell field](#canonical-stress-energy-tensor-of-the-maxwell-field)
      - [Gauge-invariant Maxwell stress-energy tensor](#gauge-invariant-maxwell-stress-energy-tensor)
    - [Antisymmetric superpotential improvement](#antisymmetric-superpotential-improvement)
    - [Belinfante-Rosenfeld stress-energy tensor](#belinfante-rosenfeld-stress-energy-tensor)
    - [Lorentz current](#lorentz-current)
      - [Boost charge of a one-dimensional scalar field](#boost-charge-of-a-one-dimensional-scalar-field)
  - [Dirac current](#dirac-current)
    - [Causal Dirac spinor current](#causal-dirac-spinor-current)
      - [Null current of a commuting Majorana spinor](#null-current-of-a-commuting-majorana-spinor)
    - [Gordon identity](#gordon-identity)
    - [Dirac electromagnetic current](#dirac-electromagnetic-current)
    - [Derivative coupling to a conserved current](#derivative-coupling-to-a-conserved-current)

## Global symmetry in field theory

↑ **Parent:** [Classical field theory](classical-field-theory.md)

A global symmetry has transformation parameters constant across spacetime and preserves the action. It can relate physically distinct states. Continuous global symmetries give [Noether currents](#noether-current) and conserved charges when boundary fluxes vanish; discrete symmetries do not receive currents from the same infinitesimal theorem. A [gauge redundancy](relativistic-quantum-field.md#gauge-redundancy) instead uses local parameters to relate descriptions of the same physical state, except that nontrivial boundary transformations may carry physical charges. The [global phase symmetry of a complex scalar field](scalar-field-theory.md#global-phase-symmetry-of-a-complex-scalar-field) is an important internal example.

### Scattering charge selection rule from global gauge symmetry

↑ **Parent:** [Global symmetry in field theory](#global-symmetry-in-field-theory)

For a conserved charge $Q$ and invariant vacuum, its global symmetry commutes with the [S-matrix](quantum-scattering.md#s-matrix). Matrix elements between charge eigenstates give the displayed selection rule. Constant electromagnetic phases cancel at every QED vertex, and nonzero physical amplitudes conserve total charge. Local [gauge invariance](relativistic-quantum-field.md#gauge-invariance) strengthens this global rule to the [Ward-Takahashi identity](perturbative-quantum-field-theory.md#ward-identity).

## Massive two-form field

↑ **Parent:** [Classical field theory](classical-field-theory.md)

An antisymmetric tensor $A_{mn}$ with $F=dA$ obeys $\partial^mF_{mnp}=\mu^2A_{np}$ for $\mu\ne0$. Taking a divergence yields $\partial^mA_{mn}=0$, and the remaining equation is the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) for each component. The physical [particle polarizations](special-relativity.md#particle-polarization) form the [exterior square](multilinear-algebra.md#exterior-square) of the massive [little group](special-relativity.md#little-group) vector representation, of dimension $(D-1)(D-2)/2$. Unlike a [two-form gauge field](relativistic-quantum-field.md#two-form-gauge-field), it has physical longitudinal polarizations.

### Light-cone decomposition of a massive two-form

↑ **Parent:** [Massive two-form field](#massive-two-form-field)

If $\partial_-$ is invertible, the divergence constraint of a [massive two-form field](#massive-two-form-field) makes $A_{-i}$ and $A_{ij}$ independent. It gives $A_{+-}=-\partial_-^{-1}\partial_iA_{-i}$ and $A_{+i}=\partial_-^{-1}(-\partial_+A_{-i}+\partial_jA_{ji})$. All independent components obey the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation). Their count is $(D-2)+\binom{D-2}{2}=\binom{D-1}{2}$.

## Hamiltonian density

↑ **Parent:** [Classical field theory](classical-field-theory.md)

A [Hamiltonian density](#hamiltonian-density) is a local integrand for the field-theory [Hamiltonian](hamiltonian-mechanics.md#hamiltonian). For canonical fields with invertible velocity-momentum relation it is the [Legendre transform in mechanics](classical-mechanics.md#legendre-transform-in-mechanics) of the [Lagrangian density](#lagrangian-density), summing over all conjugate field components. [Gauge theories](#gauge-theory) require constraints and multiplier terms as well.

### Canonical Hamiltonian density of a real scalar field

↑ **Parent:** [Hamiltonian density](#hamiltonian-density)

For a [real scalar field](scalar-field-theory.md#real-scalar-field) with [Lagrangian density](#lagrangian-density) $\mathcal L=\dot\phi^2/2-|\nabla\phi|^2/2-V(\phi)$, the [canonical momentum](hamiltonian-mechanics.md#canonical-momentum) is $\pi=\dot\phi$. Its [Hamiltonian density](#hamiltonian-density) is the sum of momentum energy, gradient energy and potential energy. Hamilton's equations recover the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation).

## Gauge theory

↑ **Parent:** [Classical field theory](classical-field-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauge_theory)

A [classical field theory](classical-field-theory.md) is a gauge theory when its description has a local redundancy represented by [gauge transformations](electromagnetism.md#gauge-transformation). A [gauge field](relativistic-quantum-field.md#gauge-field) defines the [covariant derivative](general-relativity.md#covariant-derivative) that compares matter fields at different points, and its [gauge field strength](relativistic-quantum-field.md#gauge-field-strength) measures the curvature of that comparison. [Electromagnetism](electromagnetism.md) is the familiar Abelian example; [Yang-Mills theory](relativistic-quantum-field.md#yang-mills-theory) generalizes it to a non-Abelian internal group. Both classical equations and their [quantum field theory](quantum-field-theory.md) can have this structure. Physically equivalent gauge descriptions must give the same observables, even though the [gauge potential](relativistic-quantum-field.md#gauge-field) changes.

### Grand unified theory

↑ **Parent:** [Gauge theory](#gauge-theory)

A theory embedding the [Standard Model](standard-model.md) gauge factors in a larger gauge group. Particular embeddings can relate couplings and matter multiplets or predict [proton decay](standard-model.md#proton-decay). The unification hypothesis alone does not specify a unique [mass](classical-mechanics.md#mass) spectrum or an experimentally established extension.

#### Pati-Salam model

↑ **Parent:** [Grand unified theory](#grand-unified-theory)

A quark-lepton unification framework with conventional minimal [gauge group](relativistic-quantum-field.md#gauge-group) $SU(4)_C\times SU(2)_L\times SU(2)_R$. [leptons](standard-model.md#lepton) supply a fourth [color charge](standard-model.md#color-charge), and a [right-handed neutrino](standard-model.md#right-handed-neutrino) completes each family. [fermion](tensor-product-of-quantum-systems.md#fermion) [masses](classical-mechanics.md#mass) additionally depend on symmetry breaking and [Yukawa couplings](standard-model.md#yukawa-interaction).

##### Pati-Salam charge embedding

↑ **Parent:** [Pati-Salam model](#pati-salam-model)

The charge relation combines left and right weak [isospin](standard-model.md#isospin) with the generator distinguishing [quarks](standard-model.md#quark) from [leptons](standard-model.md#lepton) inside the extended [color charge](standard-model.md#color-charge) group.

###### Pati-Salam neutrino hypercharge cancellation

↑ **Parent:** [Pati-Salam charge embedding](#pati-salam-charge-embedding)

For the right-handed neutrino, $T_{3R}=1/2$ and $B-L=-1$, so $Y=T_{3R}+(B-L)/2=0$. Its colour-singlet and left-weak-singlet assignments make it sterile under the Standard Model after symmetry breaking.

### Chiral gauge theory

↑ **Parent:** [Gauge theory](#gauge-theory)

A [gauge theory](#gauge-theory) whose left- and right-chiral [fermions](tensor-product-of-quantum-systems.md#fermion) transform differently under its [gauge group](relativistic-quantum-field.md#gauge-group). The [weak charged current](standard-model.md#charged-current) gives a physical example. A chiral representation assignment must satisfy the relevant [gauge anomaly](relativistic-quantum-field.md#gauge-anomaly) cancellation conditions to define a consistent quantum theory.

### Lattice gauge theory

↑ **Parent:** [Gauge theory](#gauge-theory)

A formulation of a [gauge theory](#gauge-theory) with discretized [spacetime](special-relativity.md#spacetime). Matter fields are assigned to sites and gauge-group elements to links between nearby sites. Products of link variables around closed paths provide gauge-invariant quantities. This structure preserves the local [gauge symmetry](relativistic-quantum-field.md#gauge-invariance) while making nonperturbative numerical calculations possible. Physical predictions require control of finite spacing, finite volume and statistical errors rather than treating one finite grid as the continuum theory.

### Noether gauging procedure

↑ **Parent:** [Gauge theory](#gauge-theory)

Localizing a parameter of a global [symmetry](physics.md#symmetry-physics) produces its [Noether current](#noether-current) times a derivative of that parameter. Introduce a [gauge field](relativistic-quantum-field.md#gauge-field) with an inhomogeneous transformation and couple it to the [Noether current](#noether-current) to cancel this variation. Recompute the remaining variation and add the required interaction and transformation terms. Closure of the local [symmetry](physics.md#symmetry-physics) algebra constrains the completion. For [supersymmetry](supersymmetry.md), its [supercurrent](supersymmetry.md#supercurrent) couples to the [gravitino](supersymmetry.md#gravitino), and the translation in the [supersymmetry](supersymmetry.md) algebra requires a [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime).

## Internal symmetry of a classical field theory

↑ **Parent:** [Classical field theory](classical-field-theory.md)

An internal symmetry changes field values while leaving spacetime coordinates fixed, preserving the [action](lagrangian-mechanics.md#action). A constant phase rotation of a [complex scalar field](scalar-field-theory.md#complex-scalar-field) is an example. This distinguishes internal charges from the spacetime translation charges in the [canonical stress-energy tensor](#canonical-stress-energy-tensor). Localizing the parameter generally requires gauge fields; a global internal symmetry is not automatically a gauge symmetry.

<h3 id="o-4-symmetry-of-a-complex-scalar-doublet">O(4) symmetry of a complex scalar doublet</h3>

↑ **Parent:** [Internal symmetry of a classical field theory](#internal-symmetry-of-a-classical-field-theory)

Two canonically normalized [complex scalar fields](scalar-field-theory.md#complex-scalar-field) with potential $V=m^2\Phi^\dagger\Phi+\lambda(\Phi^\dagger\Phi)^2$ are four real fields with a radial potential. Consequently the isolated action is invariant under the [orthogonal group](linear-algebra.md#orthogonal-group) $O(4)$, not only under complex-linear $U(2)$ transformations. Writing $\phi_1=(q_1+iq_2)/\sqrt2$ and $\phi_2=(q_3+iq_4)/\sqrt2$ makes the kinetic term $\sum_A(\partial q_A)^2/2$ and the potential a function of $\sum_Aq_A^2$. The six real-plane rotations give currents $j_{AB}^\mu=q_B\partial^\mu q_A-q_A\partial^\mu q_B$. Gauge or Yukawa couplings can break this larger symmetry, so it should not be asserted for an arbitrary interacting doublet.

### Reciprocal rescaling symmetry of two cross-coupled scalar fields

↑ **Parent:** [Internal symmetry of a classical field theory](#internal-symmetry-of-a-classical-field-theory)

For $\mathcal L=\phi_{1,t}\phi_{2,t}-c^2\phi_{1,x}\phi_{2,x}$, the real linear internal transformations preserving the density are $\operatorname{diag}(r,r^{-1})$ and $\begin{pmatrix}0&r\\r^{-1}&0\end{pmatrix}$ with $r\ne0$. There are four [connected components](geometry-and-topology.md#connected-component); the [identity component](geometry-and-topology.md#identity-component) is the displayed reciprocal rescaling with $r=e^s>0$. In the sum-and-difference basis it preserves a [bilinear form](bilinear-form.md) of signature $(1,1)$, with the identity component isomorphic to that of the [One-dimensional Lorentz group](special-relativity.md#one-dimensional-lorentz-group). Its [Noether current](#noether-current) in coordinates $(t,x)$ is $j^0=\phi_1\phi_{2,t}-\phi_2\phi_{1,t}$ and $j^x=c^2(\phi_2\phi_{1,x}-\phi_1\phi_{2,x})$. The two wave equations give $\partial_tj^0+\partial_xj^x=0$. The energy quadratic form is indefinite: the fields $\phi_\pm=(\phi_1\pm\phi_2)/\sqrt2$ have equal and opposite kinetic signs.

## Variational symmetry of a Lagrangian density

↑ **Parent:** [Classical field theory](classical-field-theory.md)

A differentiable infinitesimal transformation is a variational symmetry when its change of the [Lagrangian density](#lagrangian-density) is a divergence, $\delta\mathcal L=\varepsilon\partial_\mu K^\mu$. Under suitable [boundary conditions](differential-equation.md#boundary-condition) the [action](lagrangian-mechanics.md#action) is invariant, so exact pointwise invariance is unnecessary. The off-shell variation identity gives the [Noether current for a first-derivative scalar field](#noether-current-for-a-first-derivative-scalar-field). This definition is for a constant transformation parameter; a spacetime-dependent parameter is a different, gauge-symmetry problem.

## Scalar field

↑ **Parent:** [Classical field theory](classical-field-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scalar_field)

A [scalar field](#scalar-field) assigns one scalar to each point of a specified space, such as [Euclidean space](normed-vector-space.md#euclidean-norm) or [spacetime](special-relativity.md#spacetime). For example, $F(x,y)=x^2+2y^2$ is a [real-valued function](function.md#real-valued-function) on a plane, and its change along a moving observation is given by the [derivative along a curve](calculus.md#derivative-along-a-curve). Under a change of coordinates, a scalar field's value at the same physical point is unchanged.

### Minimally coupled scalar field

↑ **Parent:** [Scalar field](#scalar-field)

A real [scalar field](#scalar-field) is minimally coupled to a [metric tensor](general-relativity.md#metric-tensor) when its kinetic term uses the metric contraction of first derivatives and its [scalar potential](#scalar-potential) depends only on the field, without an explicit [scalar curvature](second-fundamental-form.md#scalar-curvature) coupling. For [metric signature](topological-manifold.md#metric-signature) $(-,+,+,+)$ the displayed [Lagrangian](calculus-of-variations.md#lagrangian) and volume density $\sqrt{-g}$ give $\Box\phi-V'(\phi)=0$. Its [stress-energy tensor](stress-energy-tensor.md) is $T_{ab}=\nabla_a\phi\nabla_b\phi-g_{ab}[\tfrac12(\nabla\phi)^2+V]$. The [scalar stress-energy divergence identity](#scalar-stress-energy-divergence-identity) explains its conservation on the field equation.

#### Scalar stress-energy divergence identity

↑ **Parent:** [Minimally coupled scalar field](#minimally-coupled-scalar-field)

For a [minimally coupled scalar field](#minimally-coupled-scalar-field) with a [Levi-Civita connection](general-relativity.md#levi-civita-connection), [metric compatibility](vector-bundle.md#metric-compatibility) and the [symmetric Hessian of a scalar field](riemann-curvature-tensor.md#symmetric-hessian-of-a-scalar-field) give the displayed off-shell identity. It is a special case of the [diffeomorphism Noether identity for a scalar field](stress-energy-tensor.md#diffeomorphism-noether-identity-for-a-scalar-field), and gives [stress-energy conservation](stress-energy-tensor.md#stress-energy-conservation) when the scalar equation is satisfied. No gravitational field equation is needed.

### Scalar mass

↑ **Parent:** [Scalar field](#scalar-field)

The mass of a canonically normalized [scalar field](#scalar-field) is determined by its quadratic fluctuation potential at a stationary vacuum. With several real fields, physical squared masses are the [eigenvalues](linear-operator-theory.md#eigenvalue) of the [scalar mass matrix](quantum-field-theory.md#scalar-mass-matrix). A negative squared mass signals an unstable direction rather than a stable massive particle.

### Adjoint scalar field

↑ **Parent:** [Scalar field](#scalar-field)

A [scalar field](#scalar-field) transforming in the [Adjoint representation of a Lie algebra](lie-algebra.md#adjoint-representation-of-a-lie-algebra) transforms by a [Lie bracket](lie-algebra.md#lie-bracket) with the infinitesimal gauge parameter.

### Sextic scalar field theory

↑ **Parent:** [Scalar field](#scalar-field)

### Zero-dimensional scalar field theory

↑ **Parent:** [Scalar field](#scalar-field)

A [scalar field](#scalar-field) with no spacetime coordinates reduces its [path integral](quantum-field-theory.md#path-integral) to an ordinary integral. It preserves [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) and [Feynman-diagram symmetry factors](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor), making it a useful model of [perturbative quantum field theory](perturbative-quantum-field-theory.md).

#### Zero-dimensional quartic perturbation series

↑ **Parent:** [Zero-dimensional scalar field theory](#zero-dimensional-scalar-field-theory)

For $m^2>0$, the [zero-dimensional scalar field theory](#zero-dimensional-scalar-field-theory) with [Euclidean action](perturbative-quantum-field-theory.md#euclidean-action) $m^2x^2/2+\lambda x^4/4!$ has a [Gaussian integral](integral.md#gaussian-integral) normalization $I(0)=\sqrt{2\pi/m^2}$. Its [Feynman rules](perturbative-quantum-field-theory.md#feynman-rules) assign $1/m^2$ to each [propagator](quantum-field-theory.md#propagator), $-\lambda$ to each quartic vertex, and the reciprocal [Feynman-diagram symmetry factor](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) to each [vacuum diagram](perturbative-quantum-field-theory.md#vacuum-feynman-diagram). The integral itself includes disconnected [vacuum diagrams](perturbative-quantum-field-theory.md#vacuum-feynman-diagram); its logarithm selects connected ones. At second order the three possible numbers of edges joining the two vertices are zero, two and four, with [Feynman-diagram symmetry factors](perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) $128,16,48$ respectively. Their weights add to $35\lambda^2/(384m^8)$.

The [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) give the general coefficient $I(0)(-1)^v(4v-1)!!/[v!(4!)^v m^{4v}]$. Successive absolute coefficients have ratio $(4v+3)(4v+1)/[24(v+1)m^4]$, which tends to infinity. Thus this is an [asymptotic expansion](asymptotic-expansion.md) as $\lambda\downarrow0$, rather than a convergent [power series](sequence-and-series.md#power-series). For every fixed truncation the [Taylor theorem](calculus.md#taylor-s-theorem) remainder estimate for $e^{-u}$, $u\geq0$, can be integrated against the [Gaussian distribution](probability-distribution.md#normal-distribution) to justify the corresponding remainder bound.

### Charged scalar field

↑ **Parent:** [Scalar field](#scalar-field)

A charged scalar field is a complex [scalar field](#scalar-field) transforming nontrivially under a gauge symmetry. For an electromagnetic potential $A_a$, its gauge-covariant derivative is $\mathcal D_a=\nabla_a-iqA_a$.

#### Linear-in-potential charged-scalar Lagrangian

↑ **Parent:** [Charged scalar field](#charged-scalar-field)

The density

$$
\mathcal L=\partial_\mu\phi^*\partial^\mu\phi-m^2|\phi|^2
+ieA_\mu(\phi\partial^\mu\phi^*-\phi^*\partial^\mu\phi)
$$

contains the term linear in the potential from minimal coupling, but omits $e^2A_\mu A^\mu|\phi|^2$. It has exact global phase symmetry, not exact arbitrary local phase symmetry. For a prescribed background its field equation is $(\Box+m^2)\phi+ie(\partial\cdot A)\phi+2ieA\cdot\partial\phi=0$, together with its [complex conjugate](complex-analysis.md#complex-conjugate). The omitted quadratic interaction must not be added silently when solving this specified theory.

##### Global phase current of a linearly coupled complex scalar

↑ **Parent:** [Linear-in-potential charged-scalar Lagrangian](#linear-in-potential-charged-scalar-lagrangian)

For $\delta\phi=-i\epsilon\phi$, the conserved current is $J^\mu=i(\phi^*\partial^\mu\phi-\phi\partial^\mu\phi^*)-2eA^\mu|\phi|^2$. The conjugate field equations imply

$$
\phi^*\Box\phi-\phi\Box\phi^*
=-2ie\,\partial_\mu(A^\mu|\phi|^2),
$$

which directly cancels the [divergence](multivariable-calculus.md#divergence) of the explicit background term. Conservation requires no [Lorenz gauge condition](relativistic-electromagnetism.md#lorenz-gauge-condition); constancy of total charge additionally requires vanishing boundary flux.

##### Canonical Hamiltonian of a linearly coupled complex scalar

↑ **Parent:** [Linear-in-potential charged-scalar Lagrangian](#linear-in-potential-charged-scalar-lagrangian)

For the [linear-in-potential charged-scalar Lagrangian](#linear-in-potential-charged-scalar-lagrangian), $\pi=\dot\phi^*-ieA_0\phi^*$ and $\pi^*=\dot\phi+ieA_0\phi$. With $A_\mu=(A_0,-\mathbf A)$, the [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) density is

$$
\mathcal H=(\pi+ieA_0\phi^*)(\pi^*-ieA_0\phi)
+|\boldsymbol\nabla\phi|^2+m^2|\phi|^2
-ie\mathbf A\cdot(\phi\boldsymbol\nabla\phi^*-\phi^*\boldsymbol\nabla\phi).
$$

The first product includes $+e^2A_0^2|\phi|^2$ after the [Legendre transform](convex-optimization.md#convex-conjugate); that term can arise in [canonical variables](hamiltonian-mechanics.md#canonical-variables) even though the original [Lagrangian](calculus-of-variations.md#lagrangian) has no interaction quadratic in $A$.

#### Gauge-covariant derivative of a charged scalar field

↑ **Parent:** [Charged scalar field](#charged-scalar-field)

For electric charge $q$ and [electromagnetic four-potential](relativistic-electromagnetism.md#electromagnetic-four-potential) $A_a$, the derivative $\mathcal D_a=\nabla_a-iqA_a$ transforms covariantly under an electromagnetic [gauge transformation](electromagnetism.md#gauge-transformation).

#### Gauge-covariant wave equation for a charged scalar field

↑ **Parent:** [Charged scalar field](#charged-scalar-field)

The massless gauge-covariant wave equation is $\mathcal D_a\mathcal D^a\Phi=0$. In a stationary charged background, the electrostatic potential shifts the local frequency from $\omega$ to $\omega+qA_t$.

### Scalar potential

↑ **Parent:** [Scalar field](#scalar-field)

A scalar potential is the derivative-free energy density $V(\phi)$ of a [scalar field](#scalar-field). Its derivative supplies the force term in the field equation, and its local minima describe candidate vacuum field values.

#### Flat direction of a scalar potential

↑ **Parent:** [Scalar potential](#scalar-potential)

In vacuum analysis, an exact [flat direction of a scalar potential](#flat-direction-of-a-scalar-potential) is a nonconstant continuous family of degenerate stationary vacua. The [scalar potential](#scalar-potential) stays constant along this family and its [gradient](multivariable-calculus.md#gradient) vanishes there. An ordinary level set does not suffice: $V(x,y)=x^2+y^2$ is constant on every circle, but its vacuum at the origin has no flat direction. A vanishing [eigenvalue](linear-operator-theory.md#eigenvalue) of the quadratic [Hessian matrix](multivariable-calculus.md#hessian-matrix) also does not suffice: $V(x)=x^4$ has zero quadratic mass at zero but no family of nearby vacua. Exact flat directions can be lifted by corrections absent from the classical [scalar potential](#scalar-potential).

### Scalar-field shift symmetry

↑ **Parent:** [Scalar field](#scalar-field)

A scalar-field shift symmetry acts by $\phi(x)\mapsto\phi(x)+c$ for constant $c$. Its [Noether charge](#noether-charge) is the spatial integral of the canonical momentum, up to the normalization of $c$, and interactions invariant under the symmetry contain derivatives of the scalar field.

## Lagrangian (field theory)

↑ **Parent:** [Classical field theory](classical-field-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrangian_(field_theory))

Lagrangian field theory specifies an [action](lagrangian-mechanics.md#action) by integrating a Lagrangian density $\mathcal L(\phi,\partial\phi,x)$ over spacetime. Requiring its [first variation](calculus-of-variations.md#first-variation) to vanish for compactly supported field variations yields the field [Euler-Lagrange equations](analysis.md#euler-lagrange-equation). The variational [Lagrangian](calculus-of-variations.md#lagrangian) is the integrand, whereas this field-theoretic formalism specifies the continuum fields and their dynamics.

### Lagrangian density

↑ **Parent:** [Lagrangian (field theory)](#lagrangian-field-theory)

A [Lagrangian density](#lagrangian-density) is integrated over spacetime to give the [action](lagrangian-mechanics.md#action) $S=\int d^dx\,\mathcal L$ in [Lagrangian](#lagrangian-field-theory).

#### Kinetic term

↑ **Parent:** [Lagrangian density](#lagrangian-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kinetic_term)

A kinetic term contains derivatives of a field and determines its free propagation. Its quadratic differential operator becomes the inverse [quantum field theory propagator](quantum-field-theory.md#propagator).

##### Gauge-covariant kinetic term

↑ **Parent:** [Kinetic term](#kinetic-term)

A gauge-covariant kinetic term replaces ordinary derivatives by covariant derivatives. Expanding it generates interactions between the matter field and one or more gauge fields, including contact vertices with two gauge bosons.

#### Mass term

↑ **Parent:** [Lagrangian density](#lagrangian-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mass_term)

A mass term is a quadratic term without derivatives whose coefficient sets the mass scale of a free field.

#### Field interaction term

↑ **Parent:** [Lagrangian density](#lagrangian-density)

A field interaction term is nonlinear in the fields and produces the interaction vertices of perturbation theory.

#### Euler-Lagrange field equation

↑ **Parent:** [Lagrangian density](#lagrangian-density)

For a field $\Phi$,

$$
\frac{\partial\mathcal L}{\partial\Phi}
-\partial_\mu\frac{\partial\mathcal L}{\partial(\partial_\mu\Phi)}=0.
$$

##### Damped and antidamped fields from an antisymmetric velocity coupling

↑ **Parent:** [Euler-Lagrange field equation](#euler-lagrange-field-equation)

Adding $(\phi_1\phi_{2,t}-\phi_2\phi_{1,t})/(2\tau)$ to the cross-coupled scalar [Lagrangian density](#lagrangian-density) produces independent equations $\phi_{1,tt}-c^2\phi_{1,xx}+\phi_{1,t}/\tau=0$ and $\phi_{2,tt}-c^2\phi_{2,xx}-\phi_{2,t}/\tau=0$. For the convention $e^{i(kx-\omega t)}$, their frequencies are respectively $-i/(2\tau)\pm\sqrt{c^2k^2-1/(4\tau^2)}$ and $+i/(2\tau)\pm\sqrt{c^2k^2-1/(4\tau^2)}$. Above the threshold they oscillate with decaying or growing envelopes; below it they have nonoscillatory real temporal exponents. At equality the repeated temporal root supplies $(A+Bt)e^{\mp t/(2\tau)}$. At $k=0$ each equation also has a constant solution. The full system is generically unstable because of the amplified second field, even though it arises from an autonomous variational system with conserved, indefinite total energy.

##### Euler-Lagrange field equation with second derivatives

↑ **Parent:** [Euler-Lagrange field equation](#euler-lagrange-field-equation)

For an [action](lagrangian-mechanics.md#action) $S=\int\mathcal L(\phi,\partial\phi,\partial^2\phi)d^{d+1}x$, vary the field with compact support, or fix both $\delta\phi$ and its first derivatives on the boundary. One [integration by parts](calculus.md#integration-by-parts) on the first-derivative term and two on the second-derivative term give the displayed [Euler-Lagrange field equation](#euler-lagrange-field-equation). With ordered repeated indices, define the second-derivative coefficient symmetrically so that $\delta\mathcal L=\mathcal L_\phi\delta\phi+\mathcal L_{\phi_{,\mu}}\partial_\mu\delta\phi+\mathcal L_{\phi_{,\mu\nu}}\partial_\mu\partial_\nu\delta\phi$. This convention avoids an unintended factor of two in mixed derivative terms. Higher spatial derivatives alone do not require higher time derivatives.

##### On shell

↑ **Parent:** [Euler-Lagrange field equation](#euler-lagrange-field-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/On_shell)

A field configuration or identity is on shell when the [equations of motion](#euler-lagrange-field-equation) hold.

## Noether current

↑ **Parent:** [Classical field theory](classical-field-theory.md)

A continuous variational symmetry gives a current satisfying $\partial_\mu j^\mu=0$ [on shell](#on-shell). Integrating $j^0$ over space gives a conserved charge when boundary flux vanishes.

### Axial angular-momentum current of an elastic string

↑ **Parent:** [Noether current](#noether-current)

Rotating the two transverse displacement components around the string axis gives density $\ell_x=\rho(\psi_y\dot\psi_z-\psi_z\dot\psi_y)$ and flux $\mathcal J_x=-F(\psi_y\psi_z'-\psi_z\psi_y')$. The pair of [wave equations](wave-equation.md) yields $\partial_t\ell_x+\partial_x\mathcal J_x=0$. The total charge is physical [angular momentum](momentum.md#angular-momentum) about the axis; it is conserved only when the net endpoint [torque](momentum.md#torque) flux vanishes.

### Transverse momentum current of an elastic string

↑ **Parent:** [Noether current](#noether-current)

For $\mathcal L=\rho(\dot\psi_y^2+\dot\psi_z^2)/2-F((\psi_y')^2+(\psi_z')^2)/2$, constant displacement symmetry in $y$ gives $j^0=\rho\dot\psi_y$ and $j^x=-F\psi_y'$. The [wave equation](wave-equation.md) implies $\partial_tj^0+\partial_xj^x=0$. Its integrated charge is physical transverse momentum; endpoint forces can change that charge on a finite segment.

### Unitary scalar multiplet current

↑ **Parent:** [Noether current](#noether-current)

For a [complex scalar field](scalar-field-theory.md#complex-scalar-field) multiplet with canonical kinetic term and [scalar potential](#scalar-potential) invariant under $\Phi\mapsto e^{i\varepsilon T}\Phi$, a constant [Hermitian matrix](hilbert-space.md#hermitian-operator) $T$ gives the displayed [Noether current](#noether-current). Vary the field and its conjugate independently in the [Noether current for a first-derivative scalar field](#noether-current-for-a-first-derivative-scalar-field). A common alternative convention reverses both the parameter and current sign. Its divergence vanishes [on shell](#on-shell).

### Shift current of an elastic rod

↑ **Parent:** [Noether current](#noether-current)

For a longitudinal displacement field $\psi(z,t)$ and [Lagrangian density](#lagrangian-density) $\mathcal L=A[\rho\dot\psi^2-K\psi'^2]/2$, uniform field shifts give [Noether current](#noether-current) $j^0=A\rho\dot\psi$, $j^z=-AK\psi'$. Its spatial integral is the rod's longitudinal mechanical [momentum](momentum.md). A prescribed position-dependent [mass density](fluid-mechanics.md#density) changes $j^0$ to $A\rho(z)\dot\psi$ but does not break this internal shift symmetry. Boundary traction can carry momentum into or out of a finite rod, so action symmetry alone does not guarantee conservation of the integrated charge.

### Noether current for a constant shift with second derivatives

↑ **Parent:** [Noether current](#noether-current)

If a [Lagrangian density](#lagrangian-density) depending on first and second derivatives has no undifferentiated field, the [scalar-field shift symmetry](#scalar-field-shift-symmetry) $\delta\phi=\epsilon$ gives the displayed [Noether current](#noether-current). Its [divergence](multivariable-calculus.md#divergence) is minus the [Euler-Lagrange field equation with second derivatives](#euler-lagrange-field-equation-with-second-derivatives), so it is conserved [on shell](#on-shell). The spatial integral of $j^0$ is constant only if the boundary current vanishes. For $\mathcal L=\rho\phi_t^2/2+\alpha\phi_x^2/2-\beta\phi_{xx}^2/2$, it gives $j^0=\rho\phi_t$, $j^x=\alpha\phi_x+\beta\phi_{xxx}$. Fixed transverse endpoint positions break the global shift symmetry of the boundary problem; support forces can then change the total transverse momentum even though the bulk continuity equation still holds.

### Conformal current

↑ **Parent:** [Noether current](#noether-current)

For a symmetric conserved [stress-energy tensor](stress-energy-tensor.md) $\Theta$ and a [Conformal Killing vector field](general-relativity.md#conformal-killing-vector-field) $\omega$ in dimension $d$, the displayed [conformal current](#conformal-current) has divergence $(\partial\cdot\omega)\Theta^\mu{}_{\mu}/d$. This follows by contracting the [Conformal Killing equation](general-relativity.md#conformal-killing-equation) with $\Theta$. A traceless tensor therefore gives a conserved current for every conformal generator.

### Virial current

↑ **Parent:** [Noether current](#noether-current)

A [virial current](#virial-current) $V^\mu$ represents the [trace](linear-algebra.md#matrix-trace) of a conserved [stress-energy tensor](stress-energy-tensor.md) as a divergence. Then the dilation [Noether current](#noether-current) $D^\mu=x_\nu T^{\mu\nu}-V^\mu$ is conserved, since its divergence is $T^\mu{}_{\mu}-\partial_\mu V^\mu$. This establishes [scale invariance](mathematics.md#scale-invariance); a traceless [stress-energy tensor improvement](stress-energy-tensor.md#stress-energy-tensor-improvement) is the extra condition needed for [conformal currents](#conformal-current).

### Noether current for a spacetime symmetry

↑ **Parent:** [Noether current](#noether-current)

For $x'^\mu=x^\mu+\varepsilon\xi^\mu$ and $\phi'_a(x')=\phi_a(x)+\varepsilon\Delta_a$, the fixed-coordinate field variation is $Q_a=\Delta_a-\xi^\nu\partial_\nu\phi_a$. Suppose action invariance is expressed as $\delta_0\mathcal L/\varepsilon+\partial_\mu(\mathcal L\xi^\mu)=\partial_\mu K^\mu$. Writing $\Pi_a^\mu=\partial\mathcal L/\partial(\partial_\mu\phi_a)$ and $E_a=\mathcal L_{\phi_a}-\partial_\mu\Pi_a^\mu$, the product rule gives $\partial_\mu j^\mu=-\sum_a E_aQ_a$. Thus $j^\mu$ is a [conserved current](#conserved-current) [on shell](#on-shell). A vanishing spatial boundary flux is additionally required for its [Noether charge](#noether-charge) to be conserved. This formula includes internal transformations, translations and [Lorentz transformations](special-relativity.md#lorentz-transformation).

### Noether current for a first-derivative scalar field

↑ **Parent:** [Noether current](#noether-current)

For $\delta\phi=\varepsilon X$ and a [variational symmetry of a Lagrangian density](#variational-symmetry-of-a-lagrangian-density), write $\Pi^\mu=\partial\mathcal L/\partial(\partial_\mu\phi)$ and $\mathcal E=\mathcal L_\phi-\partial_\mu\Pi^\mu$. The product rule gives $\delta\mathcal L/\varepsilon=\mathcal E X+\partial_\mu(\Pi^\mu X)$. Therefore $j^\mu=\Pi^\mu X-K^\mu$ obeys $\partial_\mu j^\mu=-\mathcal E X$, so it is a [conserved current](#conserved-current) [on shell](#on-shell). Spatial integration gives a conserved [Noether charge](#noether-charge) only when the boundary flux vanishes. The formula extends to several components by summation.

### Conserved current

↑ **Parent:** [Noether current](#noether-current)

A conserved current is a vector field $j^\mu$ satisfying the continuity equation $\partial_\mu j^\mu=0$. Its spatial integral is constant in time when no current crosses the boundary.

#### Conserved charge

↑ **Parent:** [Conserved current](#conserved-current)

An integral of the time component of a [conserved current](#conserved-current) is a [conserved charge](#conserved-charge) when the spatial boundary flux vanishes. Charges need not come from an immediately apparent elementary symmetry; a field theory can have an infinite higher-derivative current hierarchy. A [Noether charge](#noether-charge) is obtained from the symmetry current supplied by the [Noether theorem](calculus-of-variations.md#noether-theorem).

#### Conserved-current two-point function

↑ **Parent:** [Conserved current](#conserved-current)

In a massless four-dimensional theory, current conservation gives a transverse tensor structure, $\int d^4x\,e^{-ikx}\langle J_\mu(x)J_\nu(0)\rangle=(k_\mu k_\nu-\delta_{\mu\nu}k^2)G(k^2)$. With current [mass dimension](perturbative-quantum-field-theory.md#mass-dimension) three, the scalar coefficient has dimension zero.

### Noether charge

↑ **Parent:** [Noether current](#noether-current)

A Noether charge is the spatial integral $Q=\int j^0d^3x$ of a [Noether current](#noether-current). It is time-independent when the current has vanishing flux through the spatial boundary, and in a Hamiltonian formulation it generates the associated continuous symmetry.

### Dilatation current

↑ **Parent:** [Noether current](#noether-current)

The dilatation current associated with scale transformations is $D^\mu=x_\nu T^{\mu\nu}$ up to improvement terms. Its divergence is the trace of the stress-energy tensor, so classical scale invariance requires a traceless improved tensor on shell.

#### On-shell divergence of a quartic scalar dilation current

↑ **Parent:** [Dilatation current](#dilatation-current)

For $\mathcal L=(\partial\phi)^2/2-\lambda\phi^4$ and the displayed-weight dilation variation $\delta\phi=\phi+x\cdot\partial\phi$, the full divergence identity is $(4-n)\mathcal L+\delta\phi(\Box\phi+4\lambda\phi^3)$. The field equation removes the second term. In four [spacetime](special-relativity.md#spacetime) dimensions the [density](fluid-mechanics.md#density) changes by a total divergence, so the [Noether current](#noether-current) includes the subtraction $-x^\mu\mathcal L$. This is a classical statement about generic solutions and this particular current.

#### Scale-breaking sources in derivative field theories

↑ **Parent:** [Dilatation current](#dilatation-current)

For a first-derivative real [scalar field](#scalar-field) in one space and one time dimension, put $j_D^\mu=\mathcal L_{\partial_\mu\psi}(z\psi'+t\dot\psi)-x^\mu\mathcal L$. Its on-shell divergence is

$$
\partial_\mu j_D^\mu=\mathcal L_{\partial_\mu\psi}\partial_\mu\psi-2\mathcal L-z\left.\frac{\partial\mathcal L}{\partial z}\right|_{\psi,\partial\psi}-t\left.\frac{\partial\mathcal L}{\partial t}\right|_{\psi,\partial\psi}.
$$

A quadratic derivative density with arbitrary field-dependent coefficients has zero derivative-homogeneity term. An extra term $-\alpha\psi'^4$ instead gives $-2\alpha\psi'^4$. A position-dependent kinetic coefficient $A\rho(z)/2$ gives $-Az\rho'(z)\dot\psi^2/2$. These source terms distinguish [scale invariance](mathematics.md#scale-invariance) from internal field-shift symmetry.

#### Dilatation charge of a one-dimensional elastic wave

↑ **Parent:** [Dilatation current](#dilatation-current)

For constant $A,\rho,K$ on all space and time, the active waveform transformation $\psi_b(z,t)=\psi(bz,bt)$ leaves the [action](lagrangian-mechanics.md#action) of $\mathcal L=A(\rho\dot\psi^2-K\psi'^2)/2$ invariant: the density gains $b^2$ and the integration measure gains $b^{-2}$. With [canonical momentum](hamiltonian-mechanics.md#canonical-momentum) $\Pi=A\rho\dot\psi$, its [Noether current](#noether-current) can be chosen as

$$
j_D^0=t\mathcal H+z\Pi\psi',\qquad
j_D^z=-tAK\dot\psi\psi'-z\mathcal H.
$$

The integrated charge $D=\int j_D^0dz$ is conserved if its boundary flux vanishes and the weighted integral exists. For a rightgoing [wave packet](dispersion-relation.md#wave-packet) $\psi=f(z-ct)$, $c=\sqrt{K/\rho}$, it becomes $D=-A\rho c\int\xi[f'(\xi)]^2d\xi$. A fixed finite interval generally breaks this scale symmetry unless its boundaries and boundary data are transformed too.

### Canonical stress-energy tensor

↑ **Parent:** [Noether current](#noether-current)

Spacetime translations give the canonical stress-energy tensor

$$
T^\mu{}_{\nu}=\sum_a
\frac{\partial\mathcal L}{\partial(\partial_\mu\Phi_a)}
\partial_\nu\Phi_a-\delta^\mu_\nu\mathcal L.
$$

#### Scalar-field momentum flux

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)

For a real [scalar field](#scalar-field) in one spatial dimension with metric signature $(+,-)$ and potential $V$, the [stress-energy conservation](stress-energy-tensor.md#stress-energy-conservation) law is $\partial_tT^{01}+\partial_xT^{11}=0$. The force on the field to the left of a fixed cut is $-T^{11}$ at the cut when the far-left boundary flux vanishes. [Finite-energy field configurations](classical-field-theory-soliton.md#finite-energy-field-configuration) also permit this conclusion by spatial cutoffs, without assuming pointwise decay of all derivatives.

#### Four-momentum of a free real scalar field

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)

For the free [real scalar field](scalar-field-theory.md#real-scalar-field) with signature $(+,-,-,-)$,

$$
E=\frac12\int(\dot\phi^2+|\nabla\phi|^2+m^2\phi^2)d^3x,
\qquad \mathbf P=-\int\dot\phi\,\nabla\phi\,d^3x.
$$

The [canonical stress-energy tensor](#canonical-stress-energy-tensor) is $T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L$. Its divergence vanishes by the [Klein-Gordon equation](wave-equation.md#klein-gordon-equation), giving constant integrated charges when integrals and boundary flux are well behaved. The minus sign in contravariant spatial [momentum](momentum.md) is from $\partial^i=-\partial_i$; lower-index spatial charges have the opposite sign. A [plane wave](wave-function.md#plane-wave) $\cos(Et-\mathbf k\cdot\mathbf x)$ has [momentum](momentum.md) density pointing along $\mathbf k$.

##### Normal-ordered free scalar four-momentum

↑ **Parent:** [Four-momentum of a free real scalar field](#four-momentum-of-a-free-real-scalar-field)

For a canonically quantized [real scalar field](scalar-field-theory.md#real-scalar-field), the quadratic Hamiltonian contains $\frac12\sum_{\mathbf p}E_{\mathbf p}$ in a regulated box. [Normal ordering](perturbative-quantum-field-theory.md#normal-ordering) subtracts this [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy), leaving

$$
P^\mu=\int\frac{d^3p}{(2\pi)^3}p^\mu a_{\mathbf p}^\dagger a_{\mathbf p}.
$$

The vacuum momentum is zero with an inversion-symmetric regulator. The [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) then gives $[P^\mu,a_{\mathbf p}^\dagger]=p^\mu a_{\mathbf p}^\dagger$, identifying the momentum and energy added by one particle. The un-subtracted energy differs by a constant and is not literally the same operator.

###### Translation of a scalar creation operator

↑ **Parent:** [Normal-ordered free scalar four-momentum](#normal-ordered-free-scalar-four-momentum)

The [canonical commutation relation](quantum-mechanics.md#canonical-commutation-relation) gives $[P^\mu,a_p^\dagger]=p^\mu a_p^\dagger$ for a free [real scalar field](scalar-field-theory.md#real-scalar-field). Differentiate the exponential conjugation: its derivative is a scalar multiple of the same operator, yielding the displayed phase. The [annihilation operator](quantum-harmonic-oscillator.md#annihilation-operator) receives the opposite phase, so at equal time $e^{-i\mathbf P\cdot\mathbf y}\phi(\mathbf x)e^{i\mathbf P\cdot\mathbf y}=\phi(\mathbf x+\mathbf y)$. The [spatial translation operator](quantum-mechanics.md#spatial-translation-operator) translates a state's position wavefunction in the opposite argument direction.

#### Canonical stress-energy tensor of the Maxwell field

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)

For signature $(+,-,-,-)$, translation invariance of the [Maxwell Lagrangian](relativistic-electromagnetism.md#maxwell-lagrangian) gives this tensor. It is generally neither symmetric nor gauge invariant. The [antisymmetric superpotential improvement](#antisymmetric-superpotential-improvement) $-\partial_\rho(F^{\rho\mu}A^\nu)$ produces, on the source-free equations of motion, the symmetric [electromagnetic stress-energy tensor](relativistic-electromagnetism.md#electromagnetic-stress-energy-tensor) $\Theta^{\mu\nu}=-F^{\mu\rho}F^\nu{}_{\rho}+\eta^{\mu\nu}F^2/4$, which is traceless in four spacetime dimensions.

##### Gauge-invariant Maxwell stress-energy tensor

↑ **Parent:** [Canonical stress-energy tensor of the Maxwell field](#canonical-stress-energy-tensor-of-the-maxwell-field)

In signature $+---$, the [Maxwell Lagrangian](relativistic-electromagnetism.md#maxwell-lagrangian) yields

$$
\Theta^\mu{}_{\nu}=-F^{\mu\rho}F_{\nu\rho}+\tfrac14\delta^\mu{}_{\nu}F_{\rho\sigma}F^{\rho\sigma}.
$$

It is symmetric after raising its second index, [gauge-invariant](relativistic-quantum-field.md#gauge-invariance), and conserved on the source-free [Maxwell equations](maxwell-equations.md). Its energy density is $\frac12(\mathbf E^2+\mathbf B^2)$ and its energy flux is the [Poynting vector](electromagnetic-wave.md#poynting-vector). Its difference from the [canonical stress-energy tensor](#canonical-stress-energy-tensor) is an antisymmetric superpotential divergence plus an equation-of-motion term, so integrated charges coincide when the constraints and vanishing boundary terms are imposed.

#### Antisymmetric superpotential improvement

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)

If $B^{\rho\mu\nu}=-B^{\mu\rho\nu}$, commuting partial derivatives gives $\partial_\mu\partial_\rho B^{\rho\mu\nu}=0$. Such an improvement preserves conservation of a [stress-energy tensor](stress-energy-tensor.md) and changes integrated charges only by a spatial boundary term. The [Belinfante-Rosenfeld stress-energy tensor](#belinfante-rosenfeld-stress-energy-tensor) is obtained through this type of improvement.

#### Belinfante-Rosenfeld stress-energy tensor

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Belinfante–Rosenfeld_stress–energy_tensor)

The Belinfante-Rosenfeld construction adds the divergence of a spin-current superpotential to the [canonical stress-energy tensor](#canonical-stress-energy-tensor), producing a symmetric conserved tensor with the same integrated four-momentum under suitable boundary conditions.

#### Lorentz current

↑ **Parent:** [Canonical stress-energy tensor](#canonical-stress-energy-tensor)

For a symmetric conserved stress-energy tensor, the Lorentz current is $J^{\mu\rho\sigma}=x^\rho T^{\mu\sigma}-x^\sigma T^{\mu\rho}$. Its spatial integrals generate rotations and boosts.

##### Boost charge of a one-dimensional scalar field

↑ **Parent:** [Lorentz current](#lorentz-current)

For a free massless real [scalar field](#scalar-field) with [wave speed](wave-equation.md#wave-speed) set to one and metric $(+,-)$, define $\mathcal E=(\phi_t^2+\phi_x^2)/2$ and $p=-\phi_t\phi_x$. Its symmetric [stress-energy tensor](stress-energy-tensor.md) is $T^{\mu\nu}=\left(\begin{smallmatrix}\mathcal E&p\\p&\mathcal E\end{smallmatrix}\right)$. The [Lorentz current](#lorentz-current) has density $t p-x\mathcal E$ and flux $t\mathcal E-xp$. Its conserved charge is the displayed expression when boundary flux vanishes. In one spatial dimension it generates boosts, not spatial rotations; there is no independent purely spatial angular-momentum component. Its conservation says that the center of energy moves uniformly. This is a symmetry of the wave-field model and need not survive boundaries or additional material effects.

### Dirac current

↑ **Parent:** [Noether current](#noether-current)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_current)

The global phase symmetry of a [Dirac field](relativistic-quantum-field.md#dirac-field) gives the conserved Dirac current $j^\mu=\bar\psi\gamma^\mu\psi$.

#### Causal Dirac spinor current

↑ **Parent:** [Dirac current](#dirac-current)

For a commuting spinor in mostly-plus signature, orient its [Dirac current](#dirac-current) to the future and write $V^i=\epsilon^\dagger\alpha^i\epsilon$, with Hermitian $\alpha^i=-\gamma^0\gamma^i$. For every spatial [unit vector](vector-space.md#unit-vector) $u$, $(u\cdot\alpha)^2=1$ implies $|u\cdot V|\le\epsilon^\dagger\epsilon=V^0$. Choosing $u$ along the spatial current proves $V^2\le0$. Thus spinor bilinears supply causal [vectors](vector-space.md#vector) suitable for energy-condition estimates. A Grassmann-valued spinor does not have this ordinary positivity interpretation.

##### Null current of a commuting Majorana spinor

↑ **Parent:** [Causal Dirac spinor current](#causal-dirac-spinor-current)

In four dimensions a single commuting [Majorana spinor](relativistic-quantum-field.md#majorana-spinor) is specified by a two-component complex spinor $\xi$. Its future [Dirac current](#dirac-current) is proportional to $(\xi^\dagger\xi,\xi^\dagger\boldsymbol\sigma\xi)$, and the [Pauli matrix multiplication law](algebra.md#pauli-matrix-multiplication-law) implies $|\xi^\dagger\boldsymbol\sigma\xi|^2=(\xi^\dagger\xi)^2$. Thus it is null. A Dirac spinor or a sum of independent Majorana currents can be timelike. This distinction matters when applying a timelike-current classification to minimal real supersymmetry.

#### Gordon identity

↑ **Parent:** [Dirac current](#dirac-current)

The [Gordon identity](#gordon-identity) rewrites a vector-current matrix element between equal-mass on-shell [Dirac spinors](relativistic-quantum-field.md#dirac-spinor) using a momentum term and an antisymmetric spin term. In the mostly-minus convention $\{\Gamma^a,\Gamma^b\}=2\eta^{ab}$, $(\not p-m)u=0$, and $\Gamma^{ab}=[\Gamma^a,\Gamma^b]/2$, it reads $2m\bar u'\Gamma^au=\bar u'[(p'+p)^a-\Gamma^{ab}(p'_b-p_b)]u$. Derive it by adding the two external [Dirac equation](relativistic-quantum-field.md#dirac-equation) identities. The equivalent formula in the [mostly-plus Dirac convention](relativistic-quantum-field.md#mostly-plus-dirac-convention) is $\bar u'[\gamma^{ab}(p'_b-p_b)+2m\gamma^a+p^a+p'^a]u=0$. The identity before division by $m$ remains valid for massless equal-mass states.

#### Dirac electromagnetic current

↑ **Parent:** [Dirac current](#dirac-current)

The Dirac electromagnetic current is the electric charge times the [Dirac current](#dirac-current). Its coupling $-ej^\mu A_\mu$ to the [electromagnetic four-potential](relativistic-electromagnetism.md#electromagnetic-four-potential) is the matter interaction of [quantum electrodynamics](perturbative-quantum-field-theory.md#quantum-electrodynamics).

#### Derivative coupling to a conserved current

↑ **Parent:** [Dirac current](#dirac-current)

An interaction $-\lambda j^\mu\partial_\mu\phi$ with an exactly [conserved current](#conserved-current) is redundant: integration by parts gives $\lambda\phi\,\partial_\mu j^\mu$ up to a boundary term. For the [Dirac current](#dirac-current), the local phase redefinition $\psi=e^{-i\lambda\phi}\chi$ removes the coupling, so its on-shell scattering amplitudes vanish.

## ↑ Ancestors (4)

1. [Quantum field theory](quantum-field-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Gauge theory](#gauge-theory)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-48.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-41.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56.md#4/solution)
