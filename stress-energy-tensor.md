# Stress-energy tensor

↑ **Parent:** [General relativity](general-relativity.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stress-energy_tensor)

The stress-energy tensor describes local energy density, momentum density, and stress. Compatibility with the [Einstein field equations](einstein-field-equations.md) requires covariant conservation $\nabla^\mu T_{\mu\nu}=0$.

**Table of contents**

- [Hilbert stress-energy tensor](#hilbert-stress-energy-tensor)
- [Stress-energy tensor of a canonical scalar field](#stress-energy-tensor-of-a-canonical-scalar-field)
- [Stress-energy tensor improvement](#stress-energy-tensor-improvement)
  - [Improved stress-energy tensor of a free massless scalar](#improved-stress-energy-tensor-of-a-free-massless-scalar)
  - [Stress-energy superpotential](#stress-energy-superpotential)
- [Dust stress-energy tensor](#dust-stress-energy-tensor)
  - [Null dust](#null-dust)
- [Momentum density](#momentum-density)
- [Anisotropic stress](#anisotropic-stress)
- [Stress-energy tensor of a nonminimally coupled scalar field](#stress-energy-tensor-of-a-nonminimally-coupled-scalar-field)
- [Stress-energy conservation](#stress-energy-conservation)
  - [Noether identity](#noether-identity)
    - [Diffeomorphism identity for a metric action](#diffeomorphism-identity-for-a-metric-action)
    - [Diffeomorphism Noether identity for a scalar field](#diffeomorphism-noether-identity-for-a-scalar-field)
- [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)
  - [Relativistic dust](#relativistic-dust)
    - [Geodesic motion of uncharged dust](#geodesic-motion-of-uncharged-dust)
    - [Charged relativistic dust](#charged-relativistic-dust)
  - [Canonical scalar stress as a perfect fluid](#canonical-scalar-stress-as-a-perfect-fluid)
    - [Conformal density of a canonical scalar field](#conformal-density-of-a-canonical-scalar-field)
  - [Canonical vorticity of a relativistic fluid](#canonical-vorticity-of-a-relativistic-fluid)
  - [Variational action for relativistic potential flow](#variational-action-for-relativistic-potential-flow)
  - [Particle number conservation in a relativistic fluid](#particle-number-conservation-in-a-relativistic-fluid)
  - [Specific enthalpy per particle](#specific-enthalpy-per-particle)
    - [Barotropic relativistic sound speed](#barotropic-relativistic-sound-speed)
  - [Perfect-fluid alignment in a static spacetime](#perfect-fluid-alignment-in-a-static-spacetime)
  - [Stiff fluid](#stiff-fluid)
    - [Homogeneous free scalar as a stiff fluid](#homogeneous-free-scalar-as-a-stiff-fluid)
      - [Cosmological contraction with a free homogeneous scalar](#cosmological-contraction-with-a-free-homogeneous-scalar)
        - [Newtonian-potential Hankel modes in stiff contraction](#newtonian-potential-hankel-modes-in-stiff-contraction)
          - [Vacuum-normalized Newtonian spectrum in stiff contraction](#vacuum-normalized-newtonian-spectrum-in-stiff-contraction)
  - [Relativistic perfect-fluid energy equation](#relativistic-perfect-fluid-energy-equation)
  - [Relativistic Euler equation](#relativistic-euler-equation)
    - [Weak-field slow-motion equations for a relativistic fluid](#weak-field-slow-motion-equations-for-a-relativistic-fluid)
    - [Hydrostatic equilibrium along a Killing vector](#hydrostatic-equilibrium-along-a-killing-vector)
      - [Stationary radiation density](#stationary-radiation-density)
        - [Radiation fluid has no regular free surface](#radiation-fluid-has-no-regular-free-surface)
      - [Barotropic hydrostatic first integral](#barotropic-hydrostatic-first-integral)
  - [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation)
    - [Stellar compactness](#stellar-compactness)
    - [Regular central expansion of the TOV equations](#regular-central-expansion-of-the-tov-equations)
    - [Interior Schwarzschild metric](#interior-schwarzschild-metric)
      - [Central pressure of a constant-density relativistic star](#central-pressure-of-a-constant-density-relativistic-star)
        - [Dominant-energy compactness bound for an incompressible star](#dominant-energy-compactness-bound-for-an-incompressible-star)
    - [Buchdahl's theorem](#buchdahl-s-theorem)
      - [High-density core bound from TOV compactness](#high-density-core-bound-from-tov-compactness)
- [Null energy condition](#null-energy-condition)
  - [Perfect-fluid null energy condition](#perfect-fluid-null-energy-condition)
  - [Null energy condition for a canonical scalar field](#null-energy-condition-for-a-canonical-scalar-field)
  - [Null energy condition for a planar warped spacetime](#null-energy-condition-for-a-planar-warped-spacetime)
  - [Null convergence condition](#null-convergence-condition)
    - [Cosmological constant preserves null convergence](#cosmological-constant-preserves-null-convergence)
  - [Averaged null energy condition](#averaged-null-energy-condition)
    - [Averaged null energy condition for a nonminimally coupled scalar](#averaged-null-energy-condition-for-a-nonminimally-coupled-scalar)
- [Conserved Klein-Gordon scalar stress-energy ansatz](#conserved-klein-gordon-scalar-stress-energy-ansatz)
- [Klein-Gordon scalar stress-energy tensor](#klein-gordon-scalar-stress-energy-tensor)
- [Weak energy condition](#weak-energy-condition)
  - [Weak energy condition for a quadratic scalar stress-energy ansatz](#weak-energy-condition-for-a-quadratic-scalar-stress-energy-ansatz)
- [Strong energy condition](#strong-energy-condition)
- [Dominant energy condition](#dominant-energy-condition)
  - [Dominant energy condition for a kinetic scalar field](#dominant-energy-condition-for-a-kinetic-scalar-field)

## Hilbert stress-energy tensor

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

The metric variational stress tensor is defined by the matter action's response to a metric change. With signature $(+---)$ and the corresponding usual matter-action signs, the displayed convention means $\delta S_m=\tfrac12\int\sqrt{-g}\,T_{ab}\delta g^{ab}=-\tfrac12\int\sqrt{-g}\,T^{ab}\delta g_{ab}$. Fix the independent matter variables while varying the metric. Sign conventions must be matched to the action; copying a mostly-plus stress formula into this convention can reverse its energy density.

## Stress-energy tensor of a canonical scalar field

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

For signature $(+---)$ and $S_\phi=\int\sqrt{-g}[(\nabla\phi)^2/2-V(\phi)]$, the convention $T_{\mu\nu}=2(\delta S_\phi/\delta g^{\mu\nu})/\sqrt{-g}$ gives the displayed tensor. Varying the inverse metric yields the derivative product, while varying the volume element yields the term proportional to $g_{\mu\nu}$. A homogeneous field has energy density $\dot\phi^2/2+V$ and pressure $\dot\phi^2/2-V$.

## Stress-energy tensor improvement

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

Adding $\partial_\rho B^{\rho\mu\nu}$ with $B^{\rho\mu\nu}=-B^{\mu\rho\nu}$ to a [stress-energy tensor](stress-energy-tensor.md) preserves its divergence identically, since commuting partial derivatives annihilates the antisymmetric pair. The total [four-momentum](special-relativity.md#four-momentum) changes only by a spatial boundary term. Improvements can make local densities symmetric or [gauge-invariant](relativistic-quantum-field.md#gauge-invariance); equality of integrated charges requires the chosen [boundary conditions](differential-equation.md#boundary-condition). Equation-of-motion terms can also relate representatives [on shell](classical-field-theory.md#on-shell).

### Improved stress-energy tensor of a free massless scalar

↑ **Parent:** [Stress-energy tensor improvement](#stress-energy-tensor-improvement)

For $d>1$, the displayed [stress-energy tensor](stress-energy-tensor.md) is symmetric and conserved on the free massless [scalar field](classical-field-theory.md#scalar-field) equation $\Box\phi=0$. Its improvement is identically divergence-free. Since $\Box\phi^2=2(\partial\phi)^2$ on shell, its trace vanishes. Contracting it with a [Conformal Killing vector field](general-relativity.md#conformal-killing-vector-field) therefore produces a conserved conformal current. In $d=2$ the improvement coefficient is zero: the canonical tensor already has zero trace.

### Stress-energy superpotential

↑ **Parent:** [Stress-energy tensor improvement](#stress-energy-tensor-improvement)

A [stress-energy superpotential](#stress-energy-superpotential) is an antisymmetric tensor $B^{\rho\mu\nu}=-B^{\mu\rho\nu}$ whose divergence supplies a [stress-energy tensor improvement](#stress-energy-tensor-improvement). In the [Maxwell field](electromagnetism.md#electromagnetic-field), the potential-dependent expression $B^{\rho\mu}{}_{\nu}=F^{\mu\rho}A_\nu$ produces the difference between canonical and gauge-invariant [stress-energy tensors](stress-energy-tensor.md) [on shell](classical-field-theory.md#on-shell). Antisymmetry ensures identically conserved improvement terms.

## Dust stress-energy tensor

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

A pressureless fluid with proper number density $n_0$, rest mass $m$ and [four-velocity](special-relativity.md#four-velocity) $u$ has tensor $mn_0u^\mu u^\nu$. In its local rest frame there is energy density but no spatial stress. Particle-number conservation and the Lorentz force make its divergence the electromagnetic force density.

### Null dust

↑ **Parent:** [Dust stress-energy tensor](#dust-stress-energy-tensor)

Null dust is matter with a [stress-energy tensor](stress-energy-tensor.md) $T_{ab}=\varepsilon k_ak_b$ for a future-directed [null vector](special-relativity.md#null-vector) $k$. For every future-directed [timelike vector](general-relativity.md#timelike-vector) $t$, the energy current is $-T^a{}_bt^b=\varepsilon(-k\cdot t)k^a$. Therefore its [dominant energy condition](#dominant-energy-condition) holds exactly when $\varepsilon\geq0$, allowing the zero current. Rescaling $k$ rescales $\varepsilon$ inversely by the square and leaves the [stress-energy tensor](stress-energy-tensor.md) unchanged. Ingoing [Vaidya metric](general-relativity.md#vaidya-metric) matter has $k=-\partial_r$, $k_a=-(dv)_a$, and $\varepsilon=\dot m/(4\pi r^2)$.

## Momentum density

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

[Momentum density](#momentum-density) is [momentum](momentum.md) per unit physical volume. In a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime) of the measuring observer it is $q^{\hat i}=T^{\hat0\hat i}$. A [perfect fluid in general relativity](#perfect-fluid-in-general-relativity) moving at a small velocity relative to that observer has $q^{\hat i}=(\rho+P)v^{\hat i}$ to first order. For isotropic background [photons](quantum-mechanics.md#photon), $P=\rho/3$, so the factor is $4\rho/3$ rather than $\rho$. Integrating the [kinetic stress-energy tensor](boltzmann-equation.md#kinetic-stress-energy-tensor) gives $q^{\hat i}=\int f p^{\hat i}\,d^3p$.

## Anisotropic stress

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

In a local [orthonormal tetrad](general-relativity.md#orthonormal-frame-in-spacetime), [anisotropic stress](#anisotropic-stress) is the trace-free spatial part of the [stress-energy tensor](stress-energy-tensor.md), conventionally denoted $\pi^{ij}$. Some [linear cosmological perturbation theory](linear-cosmological-perturbation-theory.md) conventions instead use $\Pi^{ij}=-\pi^{ij}$ and write $T^{ij}=P\delta^{ij}-\Pi^{ij}$. The sign must be specified before using a [photon Euler equation](cosmic-microwave-background-anisotropy.md#photon-euler-equation). The [photon quadrupole](cosmic-microwave-background-anisotropy.md#photon-quadrupole) determines the linear [photon](quantum-mechanics.md#photon) [anisotropic stress](#anisotropic-stress).

## Stress-energy tensor of a nonminimally coupled scalar field

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

For action $S=\int\sqrt{-g}[-\frac12(\nabla\Phi)^2-\xi R\Phi^2]d^4x$, [metric variation](einstein-field-equations.md#metric-variation) defines $\delta S=\frac12\int\sqrt{-g}T^{ab}\delta g_{ab}d^4x$ and gives the displayed tensor. The [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) and the scalar derivative commutator yield $\nabla^aT_{ab}=(\Box\Phi-2\xi R\Phi)\nabla_b\Phi$, so the [stress-energy tensor](stress-energy-tensor.md) is conserved on the field equation.

## Stress-energy conservation

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

Local energy-momentum conservation is the covariant equation $\nabla_\mu T^{\mu\nu}=0$. Its normal and spatial projections give energy and momentum evolution equations in a spacetime foliation.

### Noether identity

↑ **Parent:** [Stress-energy conservation](#stress-energy-conservation)

A Noether identity is an off-shell differential relation among Euler-Lagrange expressions implied by a local gauge symmetry. Diffeomorphism invariance relates the divergence of the stress-energy tensor to the matter field equations.

#### Diffeomorphism identity for a metric action

↑ **Parent:** [Noether identity](#noether-identity)

For a diffeomorphism-invariant pure metric action, write $\delta S=-\int\sqrt{-g}E^{ab}\delta g_{ab}$. Substitute $\delta g_{ab}=\nabla_a\xi_b+\nabla_b\xi_a$ for an arbitrary compactly supported [vector field](multivariable-calculus.md#vector-field) and integrate by parts. Symmetry of $E^{ab}$ gives $\nabla_aE^{ab}=0$ without using field equations. This [Noether identity](#noether-identity) concerns the gravitational variational tensor alone.

#### Diffeomorphism Noether identity for a scalar field

↑ **Parent:** [Noether identity](#noether-identity)

Simultaneously varying a [metric tensor](general-relativity.md#metric-tensor) and a [scalar field](classical-field-theory.md#scalar-field) by the [Lie derivative](differential-form.md#lie-derivative-of-a-differential-form) along a compactly supported [vector field](multivariable-calculus.md#vector-field) leaves a covariant matter action invariant. [Integration by parts](calculus.md#integration-by-parts) gives the displayed [Noether identity](#noether-identity). It implies [stress-energy conservation](#stress-energy-conservation) when the scalar equation holds without needing to impose the metric field equation.

## Perfect fluid in general relativity

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

A relativistic perfect fluid has energy density $\rho$, isotropic pressure $p$ and unit timelike four-velocity $u$. Projecting $\nabla_aT^{ab}=0$ along and orthogonally to $u$ gives its energy and Euler equations.

For a [perfect fluid](general-relativity.md#perfect-fluid), the relativistic stress tensor is $T_{ab}=(\rho+p)u_au_b+pg_{ab}$ in signature $(-,+,+,+)$ with $u^au_a=-1$.

### Relativistic dust

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

[Relativistic dust](#relativistic-dust) is a continuum of noninteracting massive particles with one local [four-velocity](special-relativity.md#four-velocity) $u^\mu$ and negligible [pressure](pressure.md). With signature $(+---)$, $u^\mu u_\mu=c^2$ and rest [mass density](fluid-mechanics.md#density) $\rho$, its [stress-energy tensor](stress-energy-tensor.md) has the displayed form. Contracting [stress-energy conservation](#stress-energy-conservation) with $u_\nu$ and using [metric compatibility](vector-bundle.md#metric-compatibility) gives $c^2\nabla_\mu(\rho u^\mu)=0$. Substituting back yields $u^\mu\nabla_\mu u^\nu=0$ wherever $\rho>0$: each particle follows a [geodesic](riemannian-geometry.md#geodesic). The cosmological [pressureless matter](cosmology.md#pressureless-matter) model is a homogeneous application.

#### Geodesic motion of uncharged dust

↑ **Parent:** [Relativistic dust](#relativistic-dust)

For $T^{\mu\nu}=\rho u^\mu u^\nu$ and constant normalized $u_\mu u^\mu=c^2$, contraction of $\nabla_\mu T^{\mu\nu}=0$ with $u_\nu$ gives $\nabla_\mu(\rho u^\mu)=0$. At nonzero [density](fluid-mechanics.md#density) the remaining projection gives $u^\mu\nabla_\mu u^\nu=0$.

#### Charged relativistic dust

↑ **Parent:** [Relativistic dust](#relativistic-dust)

For identical particles of [rest mass](special-relativity.md#invariant-mass) $m$ and [electric charge](electric-charge.md) $q$, the [four-current](electric-charge.md#four-current) is $j^\mu=(q/m)\rho u^\mu$. The matter [stress-energy tensor](stress-energy-tensor.md) obeys $\nabla_\mu T_{\rm m}^{\mu\nu}=F^{\nu\alpha}j_\alpha$, with the opposite force density in the electromagnetic [stress-energy tensor](stress-energy-tensor.md). Antisymmetry of the [electromagnetic field tensor](relativistic-electromagnetism.md#electromagnetic-field-tensor) makes its contraction with two [four-velocities](special-relativity.md#four-velocity) vanish, so mass continuity still holds. Removing that term leaves the displayed covariant [Lorentz force](relativistic-electromagnetism.md#lorentz-force) law. The matter tensor alone is not divergence-free when an electromagnetic force acts.

### Canonical scalar stress as a perfect fluid

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

For a canonical scalar with timelike gradient, its [stress-energy tensor](stress-energy-tensor.md) has perfect-fluid form. In a homogeneous background, $\rho=\dot\phi^2/2+V$ and $p=\dot\phi^2/2-V$. Potential domination gives negative pressure, while the scalar's physical rest-frame [sound speed](compressible-flow.md#speed-of-sound) is one. A constant negative background $w$ therefore does not force its perturbations to obey the adiabatic barotropic closure $\delta p=w\delta\rho$.

// Target: cosmology.bigb

#### Conformal density of a canonical scalar field

↑ **Parent:** [Canonical scalar stress as a perfect fluid](#canonical-scalar-stress-as-a-perfect-fluid)

For $ds^2=a^2(d\tau^2-d\mathbf x^2)$ and a homogeneous canonical scalar, $\rho=\phi'^2/(2a^2)+V$ is the physical density, whereas $T_{00}=a^2\rho$. At $w=-1/3$, the kinetic and potential energies are $K=\rho/3$ and $V=2\rho/3$, so $\phi'^2=2a^2\rho/3=2T_{00}/3$. A single power of $\phi'$ cannot replace the square in this energy identity.

// Target: cosmology.bigb

### Canonical vorticity of a relativistic fluid

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

The canonical vorticity two-form is $\omega_{ab}=\nabla_a(\epsilon u_b)-\nabla_b(\epsilon u_a)$, with [specific enthalpy per particle](#specific-enthalpy-per-particle) $\epsilon$. Potential flow $\epsilon u_a=\nabla_a\chi$ has $\omega=0$ for a [torsion-free connection](vector-bundle.md#torsion-free-connection). Contracting this identity with $u^a$ yields $\epsilon u^a\nabla_au_b=\nabla_b\epsilon-u_bu^a\nabla_a\epsilon$, the isentropic [relativistic Euler equation](#relativistic-euler-equation) in signature $(+---)$. This canonical condition does not mean the unweighted four-velocity one-form is closed.

### Variational action for relativistic potential flow

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

In signature $(+---)$, the matter action $S=\int\sqrt{-g}[p(\epsilon)+n((\nabla\chi)^2-\epsilon^2)/(2\epsilon)]$ uses independent $n,\epsilon,\chi$. Variations of $n,\epsilon,\chi$ give $(\nabla\chi)^2=\epsilon^2$, $p'(\epsilon)=n$, and [particle number conservation in a relativistic fluid](#particle-number-conservation-in-a-relativistic-fluid) for $u_a=\nabla_a\chi/\epsilon$. Its [Hilbert stress-energy tensor](#hilbert-stress-energy-tensor) is $T_{ab}=(\rho+p)u_au_b-pg_{ab}$. The action describes isentropic potential flow, with vanishing [canonical vorticity of a relativistic fluid](#canonical-vorticity-of-a-relativistic-fluid), rather than every vortical perfect-fluid solution.

### Particle number conservation in a relativistic fluid

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

The number current is $J^a=nu^a$, where $n$ is the rest-frame [number density](statistical-physics.md#number-density) and $u^a$ the unit [four-velocity](special-relativity.md#four-velocity). Its covariant continuity equation is $\nabla_aJ^a=0$, equivalently $u^a\nabla_an+n\nabla_au^a=0$. Integration over a spacetime volume and the [divergence theorem](multivariable-calculus.md#divergence-theorem) equate the particle numbers crossing its boundary. This conservation law is separate from [stress-energy conservation](#stress-energy-conservation).

### Specific enthalpy per particle

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

For [number density](statistical-physics.md#number-density) $n$, rest-frame [energy density](statistical-physics.md#energy-density) $\rho$ and [pressure](pressure.md) $p$, the enthalpy per particle is $\epsilon=(\rho+p)/n$. In an isentropic [barotropic fluid](fluid-mechanics.md#barotropic-fluid), $d\rho=\epsilon\,dn$ and $dp=n\,d\epsilon$. It differs from enthalpy per unit mass by the particle mass when that mass is fixed. Using $\epsilon$ as thermodynamic variable gives $n=p'(\epsilon)$ and $\rho=\epsilon p'(\epsilon)-p(\epsilon)$.

#### Barotropic relativistic sound speed

↑ **Parent:** [Specific enthalpy per particle](#specific-enthalpy-per-particle)

In units $c=1$, an isentropic [perfect fluid in general relativity](#perfect-fluid-in-general-relativity) has sound speed $c_s^2=dp/d\rho$. Writing $n=p'(\epsilon)$ gives $d\rho=\epsilon\,dn$ and $c_s^2=n/(\epsilon p''(\epsilon))$. Linearized [particle number conservation in a relativistic fluid](#particle-number-conservation-in-a-relativistic-fluid) and the [relativistic Euler equation](#relativistic-euler-equation) then yield acoustic waves with this speed. Positive $c_s^2$ is needed for ordinary acoustic stability; a causal fluid model additionally requires $c_s^2\le1$.

### Perfect-fluid alignment in a static spacetime

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

For [metric signature](topological-manifold.md#metric-signature) $(+---)$, a [perfect fluid](general-relativity.md#perfect-fluid) has $T_{ab}=(\rho+p)u_au_b-pg_{ab}$. The [Einstein field equations](einstein-field-equations.md) and [static Killing field is a Ricci eigenvector](general-relativity.md#static-killing-field-is-a-ricci-eigenvector) imply $(\rho+p)(k\cdot u)u_{[a}k_{b]}=0$. Two nonzero timelike vectors cannot be orthogonal, so $k\cdot u\ne0$. If $\rho+p\ne0$, the [four-velocity](special-relativity.md#four-velocity) is parallel to the static [Killing vector](killing-vector-field.md). Choosing both future-directed gives the displayed normalization. For $\rho+p=0$, the [stress-energy tensor](stress-energy-tensor.md) is proportional to the [metric tensor](general-relativity.md#metric-tensor) and does not determine a preferred fluid velocity; the strict enthalpy hypothesis is therefore material.

### Stiff fluid

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

A [perfect fluid](general-relativity.md#perfect-fluid) with [equation of state](pressure.md#equation-of-state) $P=\rho$ is called a stiff fluid. For positive [energy density](statistical-physics.md#energy-density), its constant equation-of-state parameter is $w=1$. The [cosmological continuity equation](cosmology.md#cosmological-continuity-equation) gives $\rho\propto a^{-6}$. In a flat universe dominated by this fluid, the [Friedmann equation](cosmology.md#friedmann-equations) then gives $a(t)\propto(t-t_B)^{1/3}$. This statement assumes a nonzero fluid density and negligible other components.

#### Homogeneous free scalar as a stiff fluid

↑ **Parent:** [Stiff fluid](#stiff-fluid)

For a spatially homogeneous [minimally coupled scalar field](classical-field-theory.md#minimally-coupled-scalar-field) with zero [scalar potential](classical-field-theory.md#scalar-potential), the [stress-energy tensor](stress-energy-tensor.md) has $\rho=P=\dot\phi^2/2$. Its field equation is $\ddot\phi+3H\dot\phi=0$, so $a^3\dot\phi$ is constant and its [energy density](statistical-physics.md#energy-density) decreases as $a^{-6}$. Thus its homogeneous stress is precisely that of a [stiff fluid](#stiff-fluid). Spatial gradients would introduce directional stresses, so this equivalence requires homogeneity.

##### Cosmological contraction with a free homogeneous scalar

↑ **Parent:** [Homogeneous free scalar as a stiff fluid](#homogeneous-free-scalar-as-a-stiff-fluid)

In units $8\pi G=1$, a free homogeneous scalar has $\rho=P=\dot\phi_0^2/2$ and therefore a stiff equation of state. Its equation gives $a^2\phi_0'=\text{constant}$, while the [Friedmann equation](cosmology.md#friedmann-equations) gives $3\mathcal H^2=\phi_0'^2/2$. The displayed contracting branch satisfies both equations for negative [conformal time](cosmology.md#conformal-time). Constant normalizations and an additive scalar shift can be restored.

###### Newtonian-potential Hankel modes in stiff contraction

↑ **Parent:** [Cosmological contraction with a free homogeneous scalar](#cosmological-contraction-with-a-free-homogeneous-scalar)

In [conformal Newtonian gauge](linear-cosmological-perturbation-theory.md#newtonian-gauge), a free scalar has no linear anisotropic stress. Eliminating its perturbation with the momentum constraint gives $\Phi_k''+3\Phi_k'/\tau+k^2\Phi_k=0$. Substitution of $\Phi_k=(-\tau)^{-1}y(-k\tau)$ gives the order-one [Bessel equation](bessel-function.md#bessel-differential-equation). The displayed [Hankel function](bessel-function.md#hankel-function) has positive incoming frequency $e^{-ik\tau}$ at early times.

###### Vacuum-normalized Newtonian spectrum in stiff contraction

↑ **Parent:** [Newtonian-potential Hankel modes in stiff contraction](#newtonian-potential-hankel-modes-in-stiff-contraction)

The momentum constraint relates the incoming scalar mode $a^{-1}\sqrt{\hbar/(2k)}e^{-ik\tau}$ to the [Newtonian-potential Hankel modes in stiff contraction](#newtonian-potential-hankel-modes-in-stiff-contraction). Large-argument Hankel asymptotics give $|N_k|^2=3\pi\hbar/(32k^2)$. The small-argument behavior $H_1^{(1)}(z)\sim-2i/(\pi z)$ then gives the displayed spectrum. Its dimensional power is $k^{-4}$ and its power per logarithmic interval is proportional to $k^{-1}$. These are Newtonian-potential spectra; a curvature-perturbation spectrum need not have the same exponent.

### Relativistic perfect-fluid energy equation

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

The timelike projection of stress-energy conservation is $u^a\nabla_a\rho+(\rho+p)\nabla_au^a=0$. It is the local adiabatic first law for a perfect fluid.

### Relativistic Euler equation

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)

The spatial projection of stress-energy conservation is $(\rho+p)u^b\nabla_bu^a=-(g^{ab}+u^au^b)\nabla_bp$.

#### Weak-field slow-motion equations for a relativistic fluid

↑ **Parent:** [Relativistic Euler equation](#relativistic-euler-equation)

For $ds^2=(1+2\phi)dt^2-d\mathbf x^2$ with static weak $\phi$, normalization gives $u^0=1-\phi+O(\phi^2,v^2)$ and $\Gamma^i{}_{00}=\partial_i\phi$. Around a homogeneous state, the first-order equations are $\partial_t\delta n+n_0\nabla\cdot\mathbf v=0$, $\partial_t\delta\rho+(\rho_0+p_0)\nabla\cdot\mathbf v=0$, and $(\rho_0+p_0)\partial_t\mathbf v=-\nabla\delta p-(\rho_0+p_0)\nabla\phi$. The inertial density is enthalpy density even though the flow is slow. Only a further nonrelativistic equation of state, $p\ll\rho\simeq mn$, replaces it by mass density.

#### Hydrostatic equilibrium along a Killing vector

↑ **Parent:** [Relativistic Euler equation](#relativistic-euler-equation)

For [metric signature](topological-manifold.md#metric-signature) $(+---)$, a stationary [perfect fluid](general-relativity.md#perfect-fluid) follows a timelike [Killing vector field](killing-vector-field.md) $K$ with [four-velocity](special-relativity.md#four-velocity) $U=K/N$. Its [Killing-flow four-acceleration](killing-vector-field.md#killing-flow-four-acceleration) is $U^b\nabla_bU_a=-\nabla_a\log N$. The [relativistic Euler equation](#relativistic-euler-equation) and stationarity of the [pressure](pressure.md) give the displayed [hydrostatic equilibrium](statistical-physics.md#hydrostatic-equilibrium) equation. This uses stationarity along $K$ and does not require hypersurface orthogonality.

##### Stationary radiation density

↑ **Parent:** [Hydrostatic equilibrium along a Killing vector](#hydrostatic-equilibrium-along-a-killing-vector)

The [equation of state](pressure.md#equation-of-state) of isotropic [blackbody radiation](statistical-physics.md#black-body-radiation) is $p=\rho/3$. The [barotropic hydrostatic first integral](#barotropic-hydrostatic-first-integral) gives $\rho N^4=C$. The [Stefan–Boltzmann law](heat.md#stefan-boltzmann-law) $\rho\propto T^4$ then yields the [Tolman–Ehrenfest relation](thermal-equilibrium.md#tolman-ehrenfest-relation) $TN=\mathrm{constant}$. Here $N=\sqrt{|K^aK_a|}$ for the stationary timelike [Killing vector field](killing-vector-field.md); its normalization only changes the constants.

###### Radiation fluid has no regular free surface

↑ **Parent:** [Stationary radiation density](#stationary-radiation-density)

A connected nonvacuum [perfect fluid](general-relativity.md#perfect-fluid) with [equation of state](pressure.md#equation-of-state) $p=\rho/3$ obeys the [stationary radiation density](#stationary-radiation-density) law $\rho=C/N^4$ with $C>0$. On a compact region of a regular [spacetime](special-relativity.md#spacetime), a smooth [Killing vector field](killing-vector-field.md) has bounded norm. Consequently $\rho$ cannot tend to zero at a finite regular [free surface](fluid-mechanics.md#free-surface). A vanishing timelike norm instead makes the density diverge. A radiation-filled cavity can have a material wall with nonzero boundary [pressure](pressure.md); this is a different boundary condition.

##### Barotropic hydrostatic first integral

↑ **Parent:** [Hydrostatic equilibrium along a Killing vector](#hydrostatic-equilibrium-along-a-killing-vector)

For a [barotropic fluid](fluid-mechanics.md#barotropic-fluid) in [hydrostatic equilibrium along a Killing vector](#hydrostatic-equilibrium-along-a-killing-vector), assume $\rho+p>0$. Integrating $dp/(\rho+p)=-d\log N$ gives the displayed [first integral](differential-equation.md#first-integral), constant on each connected fluid region. For the [equation of state](pressure.md#equation-of-state) $p=w\rho$ with constant $w>0$, it gives $\rho N^{(1+w)/w}=C_1$.

<h3 id="tolman-oppenheimer-volkoff-equation">Tolman–Oppenheimer–Volkoff equation</h3>

↑ **Parent:** [Perfect fluid in general relativity](#perfect-fluid-in-general-relativity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tolman–Oppenheimer–Volkoff_equation)

The Tolman–Oppenheimer–Volkoff equation governs a static, spherically symmetric [perfect fluid in general relativity](#perfect-fluid-in-general-relativity). In geometrized units, if $m(r)$ is the mass inside areal radius $r$, then

$$
\frac{dm}{dr}=4\pi r^2\rho,
\qquad
\frac{dp}{dr}=-\frac{(\rho+p)(m+4\pi r^3p)}{r(r-2m)}.
$$

#### Stellar compactness

↑ **Parent:** [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation)

The ratio of enclosed gravitational mass to areal radius in units $G=c=1$. In a spherical star the local value is $m(r)/r$, and the surface value is $M/R$. Bounds on this ratio constrain relativistic stellar models; it is unrelated to topological compactness.

#### Regular central expansion of the TOV equations

↑ **Parent:** [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation)

For a smooth centre with density $\rho_c$ and pressure $p_c$, the [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation) gives $m(r)=4\pi\rho_cr^3/3+O(r^5)$ and $p(r)=p_c-2\pi(\rho_c+p_c)(\rho_c/3+p_c)r^2+O(r^4)$. A fixed [barotropic stellar equation of state](pressure.md#barotropic-stellar-equation-of-state) leaves one physical central parameter; the additive lapse constant fixes time normalization.

#### Interior Schwarzschild metric

↑ **Parent:** [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interior_Schwarzschild_metric)

The interior Schwarzschild metric is the exact static solution for a spherical fluid of constant density. If the star has mass $M$ and radius $R$, its pressure is

$$
p(r)=\rho
\frac{\sqrt{1-2Mr^2/R^3}-\sqrt{1-2M/R}}
{3\sqrt{1-2M/R}-\sqrt{1-2Mr^2/R^3}}.
$$

##### Central pressure of a constant-density relativistic star

↑ **Parent:** [Interior Schwarzschild metric](#interior-schwarzschild-metric)

The [Interior Schwarzschild metric](#interior-schwarzschild-metric) has central pressure

$$
p(0)=\rho
\frac{1-\sqrt{1-2M/R}}
{3\sqrt{1-2M/R}-1}.
$$

It diverges when $M/R=4/9$, the limiting compactness in [Buchdahl's theorem](#buchdahl-s-theorem).

###### Dominant-energy compactness bound for an incompressible star

↑ **Parent:** [Central pressure of a constant-density relativistic star](#central-pressure-of-a-constant-density-relativistic-star)

The [dominant energy condition](#dominant-energy-condition) for the [Interior Schwarzschild metric](#interior-schwarzschild-metric) reduces to its largest pressure satisfying $p_c\leq\rho$. Substitution of the exact central pressure gives $\sqrt{1-2M/R}\geq1/2$, hence $M/R\leq3/8$. Equality has finite central pressure and is allowed by the non-strict condition.

<h4 id="buchdahl-s-theorem">Buchdahl's theorem</h4>

↑ **Parent:** [Tolman–Oppenheimer–Volkoff equation](#tolman-oppenheimer-volkoff-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Buchdahl's_theorem)

Buchdahl's theorem gives $2M/R\leq8/9$ for a static spherical perfect-fluid star whose density is nonincreasing outwards, subject to its regularity assumptions. Equality would require divergent central pressure, so every regular such star satisfies $M/R<4/9$.

##### High-density core bound from TOV compactness

↑ **Parent:** [Buchdahl's theorem](#buchdahl-s-theorem)

Let $\rho_0>0$ be a density threshold and let $a,\mu$ be the radius and enclosed mass where a monotonically decreasing stellar density reaches that threshold. Then $\mu\geq4\pi\rho_0a^3/3$. A local compactness bound $\mu/a<4/9$ implies $a<(3\pi\rho_0)^{-1/2}$ and $\mu<4/(9\sqrt{3\pi\rho_0})$, independently of the [equation of state](pressure.md#equation-of-state) above the threshold. A total-mass bound also requires suitable control of the known low-density envelope.

## Null energy condition

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Null_energy_condition)

The null energy condition requires $T_{\mu\nu}k^\mu k^\nu\geq0$ for every null vector $k$. Through the Einstein field equations this is equivalent to $R_{\mu\nu}k^\mu k^\nu\geq0$ when the cosmological term is absent.

### Perfect-fluid null energy condition

↑ **Parent:** [Null energy condition](#null-energy-condition)

For $T_{ab}=(\rho+p)u_au_b+pg_{ab}$ and nonzero null $k$, contraction gives $T_{ab}k^ak^b=(\rho+p)(u\cdot k)^2$. A timelike fluid velocity has nonzero scalar product with every nonzero null vector, so the [null energy condition](#null-energy-condition) is exactly the displayed inequality. Individual nonnegativity of pressure or density is unnecessary for null focusing. A [cosmological constant](cosmology.md#cosmological-constant) term has zero null contraction.

### Null energy condition for a canonical scalar field

↑ **Parent:** [Null energy condition](#null-energy-condition)

The classical [stress-energy tensor of a canonical scalar field](#stress-energy-tensor-of-a-canonical-scalar-field) has a gradient-product term and a metric-proportional term. Contracting with a real [null vector](special-relativity.md#null-vector) removes the latter, leaving the displayed square for a real field. This proves the [null energy condition](#null-energy-condition) for a minimally coupled canonical scalar, including the massless case. It is not a statement about arbitrary curvature couplings, wrong-sign kinetic terms or a renormalized quantum [stress-energy tensor](stress-energy-tensor.md).

### Null energy condition for a planar warped spacetime

↑ **Parent:** [Null energy condition](#null-energy-condition)

In a [planar warped spacetime](general-relativity.md#planar-warped-spacetime), contraction of the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) with a [null vector](special-relativity.md#null-vector) in an [orthonormal frame](general-relativity.md#orthonormal-frame-in-spacetime) gives $R_{ab}k^ak^b=-2(\log A)''(k^3)^2$. The [Einstein field equations](einstein-field-equations.md) identify this with $8\pi T_{ab}k^ak^b$; metric terms, including a cosmological constant, vanish in a null contraction. Thus the [null energy condition](#null-energy-condition) is equivalent to concavity of $\log A$ in the proper transverse coordinate $z$. Null directions confined to a planar slice saturate the condition.

### Null convergence condition

↑ **Parent:** [Null energy condition](#null-energy-condition)

The [null convergence condition](#null-convergence-condition) requires $R_{ab}k^ak^b\geq0$ for every [null vector](special-relativity.md#null-vector). Through the [Einstein field equations](einstein-field-equations.md), it follows from the [null energy condition](#null-energy-condition), since all terms proportional to the [metric tensor](general-relativity.md#metric-tensor) vanish on a [null vector](special-relativity.md#null-vector).

#### Cosmological constant preserves null convergence

↑ **Parent:** [Null convergence condition](#null-convergence-condition)

Contract the [Einstein field equations](einstein-field-equations.md) with a [null vector](special-relativity.md#null-vector). Both the trace term and the [cosmological constant](cosmology.md#cosmological-constant) term multiply $g_{ab}\ell^a\ell^b=0$ and disappear. The [null energy condition](#null-energy-condition) therefore still implies the [null convergence condition](#null-convergence-condition), independently of the sign of the [cosmological constant](cosmology.md#cosmological-constant). A [black-hole area theorem](black-hole.md#hawking-s-area-theorem) still needs the appropriate global horizon assumptions as well as this local focusing condition.

### Averaged null energy condition

↑ **Parent:** [Null energy condition](#null-energy-condition)

The averaged null energy condition requires

$$
\int_{-\infty}^{\infty}T_{ab}k^ak^b\,d\lambda\geq0
$$

along every complete affinely parametrized null geodesic. It is weaker than the pointwise null energy condition.

#### Averaged null energy condition for a nonminimally coupled scalar

↑ **Parent:** [Averaged null energy condition](#averaged-null-energy-condition)

For the curvature-coupled scalar equation considered here, contraction with an affine null tangent and integration by parts gives, for $\xi<0$,

$$
\int T_{ab}k^ak^b\,d\lambda
=\int\frac{1+\xi(4\xi-1)\Phi^2}{(1-\xi\Phi^2)^2}(\Phi')^2\,d\lambda\geq0
$$

when $\Phi\Phi'/(1-\xi\Phi^2)$ vanishes at the endpoints.

## Conserved Klein-Gordon scalar stress-energy ansatz

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

For $\nabla_\alpha\nabla^\alpha\phi=m^2\phi$, consider

$$
T_{\mu\nu}=\frac12\left[
\nabla_\mu\phi\nabla_\nu\phi
+g_{\mu\nu}\left(A\nabla_\rho\phi\nabla^\rho\phi+B\phi^2\right)
\right].
$$

Covariant conservation for all solutions holds exactly when

$$
A=-\frac12,
\qquad
B=-\frac{m^2}{2}.
$$

## Klein-Gordon scalar stress-energy tensor

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)

For a real scalar satisfying $\nabla_a\nabla^a\psi-\mu^2\psi=0$,

$$
T_{ab}=\nabla_a\psi\nabla_b\psi-\frac12g_{ab}\left(\nabla_c\psi\nabla^c\psi+\mu^2\psi^2\right)
$$

is symmetric and covariantly conserved.

## Weak energy condition

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_energy_condition)

The weak energy condition requires

$$
T_{\mu\nu}X^\mu X^\nu\geq0
$$

for every timelike vector $X$, so every observer measures nonnegative energy density.

### Weak energy condition for a quadratic scalar stress-energy ansatz

↑ **Parent:** [Weak energy condition](#weak-energy-condition)

For the general scalar ansatz in [Conserved Klein-Gordon scalar stress-energy ansatz](#conserved-klein-gordon-scalar-stress-energy-ansatz), work in a unit timelike frame. Then

$$
2T_{00}=(1+A)(\partial_0\phi)^2
-A|\nabla_{\rm s}\phi|^2-B\phi^2.
$$

The weak energy condition for arbitrary local field data is therefore equivalent to

$$
-1\leq A\leq0,
\qquad B\leq0.
$$

## Strong energy condition

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_energy_condition)

The strong energy condition requires $(T_{ab}-Tg_{ab}/2)u^au^b\geq0$ for every timelike vector $u$ in four spacetime dimensions. Through the [Einstein field equations](einstein-field-equations.md), it implies the timelike convergence condition $R_{ab}u^au^b\geq0$ when the cosmological constant vanishes.

## Dominant energy condition

↑ **Parent:** [Stress-energy tensor](stress-energy-tensor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dominant_energy_condition)

The dominant energy condition requires the energy flux measured by every future-directed timelike observer to be future-directed and causal. Equivalently, $T_{ab}u^av^b\geq0$ for every pair of future-directed causal vectors $u$ and $v$ under the $(-,+,+,+)$ convention.

### Dominant energy condition for a kinetic scalar field

↑ **Parent:** [Dominant energy condition](#dominant-energy-condition)

For a [scalar field](classical-field-theory.md#scalar-field) with $X=-q^2/2$, Lagrangian $F(X)$ and [stress-energy tensor](stress-energy-tensor.md) $T_{ab}=F\prime q_aq_b+Fg_{ab}$, the inequalities $A=F\prime\ge0$ and $Y=XF\prime-F\ge0$ imply the [dominant energy condition](#dominant-energy-condition) for any gradient type. In a local [Lorentz frame](general-relativity.md#lorentz-frame), $\rho=A(q_0^2+\sum_iq_i^2)/2+Y\ge0$ and $\rho^2-\sum_iT_{0i}^2=A^2X^2+A(q_0^2+\sum_iq_i^2)Y+Y^2\ge0$.

## ↑ Ancestors (4)

1. [General relativity](general-relativity.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (106)

- [Abelian Chern-Simons five-form field equation](relativistic-quantum-field.md#abelian-chern-simons-five-form-field-equation)
- [Absence of a local gravitational stress-energy tensor](general-relativity.md#absence-of-a-local-gravitational-stress-energy-tensor)
- [Anisotropic stress](#anisotropic-stress)
- [Antisymmetric superpotential improvement](classical-field-theory.md#antisymmetric-superpotential-improvement)
- [Averaged stress-energy of transverse gravitational waves](gravitational-wave.md#averaged-stress-energy-of-transverse-gravitational-waves)
- [Boost charge of a one-dimensional scalar field](classical-field-theory.md#boost-charge-of-a-one-dimensional-scalar-field)
- [Canonical scalar stress as a perfect fluid](#canonical-scalar-stress-as-a-perfect-fluid)
- [Charged relativistic dust](#charged-relativistic-dust)
- [Chern-Simons source stress convention](topological-quantum-matter.md#chern-simons-source-stress-convention)
- [Conformal current](classical-field-theory.md#conformal-current)
- [Dominant energy condition for a kinetic scalar field](#dominant-energy-condition-for-a-kinetic-scalar-field)
- [Einstein-equation coupling under reversed curvature](einstein-field-equations.md#einstein-equation-coupling-under-reversed-curvature)
- [Einstein field equations](einstein-field-equations.md)
- [Gravitational mass](classical-mechanics.md#gravitational-mass)
- [Hadamard condition](quantum-field-theory.md#hadamard-condition)
- [Homogeneous free scalar as a stiff fluid](#homogeneous-free-scalar-as-a-stiff-fluid)
- [Improved stress-energy tensor of a free massless scalar](#improved-stress-energy-tensor-of-a-free-massless-scalar)
- [Inverse metric volume variation](general-relativity.md#inverse-metric-volume-variation)
- [Israel junction conditions](general-relativity.md#israel-junction-conditions)
- [Kinetic stress-energy tensor](boltzmann-equation.md#kinetic-stress-energy-tensor)
- [Kink–antikink attraction from the stress tensor](classical-field-theory-soliton.md#kink-antikink-attraction-from-the-stress-tensor)
- [Komar angular momentum with inner boundaries](killing-vector-field.md#komar-angular-momentum-with-inner-boundaries)
- [Minimally coupled scalar field](classical-field-theory.md#minimally-coupled-scalar-field)
- [Neutrino tensor anisotropic stress](linear-cosmological-perturbation-theory.md#neutrino-tensor-anisotropic-stress)
- [Normalization of the metric f(R) field equation](einstein-field-equations.md#normalization-of-the-metric-f-r-field-equation)
- [Null dust](#null-dust)
- [Null energy condition for a canonical scalar field](#null-energy-condition-for-a-canonical-scalar-field)
- [One-particle distribution function](boltzmann-equation.md#one-particle-distribution-function)
- [Papapetrou electromagnetic field](killing-vector-field.md#papapetrou-electromagnetic-field)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-68.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-70.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-70.md#4/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-70.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-51.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-54.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-60.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-62.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-63.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-64.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-64.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-61.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-63.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-64.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-61.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-62.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-63.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-66.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-56.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-54.md#2/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#3/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-56.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-57.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-41.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-49.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#2/b/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-52.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-53.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-53.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#34a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#34a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309.md#4/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#2/d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#3/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-311.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-308.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-311.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-312.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#4/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-309.md#4/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-310.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-312.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-306.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#37b/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-306.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-354.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-306.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-354.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-301.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-325.md#3/a/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2016/paper-1.md#3/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2017.md#1/b/solution)
- [Solution](past-exam-of-the-relativity-course-of-the-university-of-cambridge/2019.md#section-b/b4/solution)
- [Solution](past-exam-of-the-theoretical-physics-i-course-of-the-university-of-cambridge/2016/paper-1.md#2/b/solution)
- [Perfect-fluid alignment in a static spacetime](#perfect-fluid-alignment-in-a-static-spacetime)
- [Photon energy density](boltzmann-equation.md#photon-energy-density)
- [Quadratic gravitational effective stress-energy tensor](linearized-gravity.md#quadratic-gravitational-effective-stress-energy-tensor)
- [Relativistic dust](#relativistic-dust)
- [Relativistic energy and momentum of a phi-four kink](classical-field-theory-soliton.md#relativistic-energy-and-momentum-of-a-phi-four-kink)
- [Scalar-field stress projections](numerical-relativity.md#scalar-field-stress-projections)
- [Semiclassical gravity](quantum-theory.md#semiclassical-gravity)
- [Stress-energy quadrupole identity](gravitational-wave.md#stress-energy-quadrupole-identity)
- [Stress-energy superpotential](#stress-energy-superpotential)
- [Stress-energy tensor improvement](#stress-energy-tensor-improvement)
- [Stress-energy tensor of a nonminimally coupled scalar field](#stress-energy-tensor-of-a-nonminimally-coupled-scalar-field)
- [Vacuum Einstein equations](einstein-field-equations.md#vacuum-einstein-equations)
- [Vacuum spacetime](einstein-field-equations.md#vacuum-spacetime)
- [Virial current](classical-field-theory.md#virial-current)
