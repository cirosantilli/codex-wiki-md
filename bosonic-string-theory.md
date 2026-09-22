# Bosonic string theory

↑ **Parent:** [String theory](string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bosonic_string_theory)

Bosonic string theory quantizes a relativistic string using only bosonic worldsheet fields. Lorentz-invariant quantization requires 26-dimensional target spacetime and contains a tachyonic ground state.

**Table of contents**

- [Internal free fermions in a four-dimensional bosonic string](#internal-free-fermions-in-a-four-dimensional-bosonic-string)
  - [Zero- and two-fermion vertices of an internally fermionized bosonic string](#zero-and-two-fermion-vertices-of-an-internally-fermionized-bosonic-string)
- [Open string](#open-string)
  - [Open-string oscillator degeneracy](#open-string-oscillator-degeneracy)
    - [Large-level degeneracy of an open bosonic string](#large-level-degeneracy-of-an-open-bosonic-string)
  - [Open-string endpoint momentum flux](#open-string-endpoint-momentum-flux)
    - [Variational open-string boundary conditions](#variational-open-string-boundary-conditions)
    - [Free-end string boundary condition](#free-end-string-boundary-condition)
      - [Null motion of a free string endpoint](#null-motion-of-a-free-string-endpoint)
  - [Open-string mode expansion](#open-string-mode-expansion)
    - [Integer-mode expansion with parallel D-brane endpoints](#integer-mode-expansion-with-parallel-d-brane-endpoints)
    - [Oscillator symplectic form of an open string](#oscillator-symplectic-form-of-an-open-string)
    - [Neumann-Dirichlet open-string boundary condition](#neumann-dirichlet-open-string-boundary-condition)
      - [Bosonic ND boundary-changing conformal weight](#bosonic-nd-boundary-changing-conformal-weight)
- [Closed string](#closed-string)
  - [Large-level degeneracy of a closed bosonic string](#large-level-degeneracy-of-a-closed-bosonic-string)
  - [Closed-string mode expansion](#closed-string-mode-expansion)
- [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)
  - [No-ghost theorem below the critical bosonic dimension](#no-ghost-theorem-below-the-critical-bosonic-dimension)
  - [DDF operator](#ddf-operator)
  - [No-ghost theorem for the critical bosonic string](#no-ghost-theorem-for-the-critical-bosonic-string)
  - [Level-two open-string polarization decomposition](#level-two-open-string-polarization-decomposition)
  - [Negative-norm string state](#negative-norm-string-state)
  - [Old covariant string quantization](#old-covariant-string-quantization)
    - [Level-two scalar in covariant string quantization](#level-two-scalar-in-covariant-string-quantization)
    - [Level-one intercept bound in covariant string quantization](#level-one-intercept-bound-in-covariant-string-quantization)
  - [Physical string state](#physical-string-state)
  - [Spurious string state](#spurious-string-state)
    - [Null string state](#null-string-state)
      - [Null-state quotient of a string](#null-state-quotient-of-a-string)
      - [Level-two scalar Virasoro null state](#level-two-scalar-virasoro-null-state)
- [String tension](#string-tension)
  - [String length](#string-length)
  - [Regge trajectory](#regge-trajectory)
    - [Regge limit](#regge-limit)
- [Polyakov action](#polyakov-action)
  - [String sigma model in a spacetime metric](#string-sigma-model-in-a-spacetime-metric)
    - [String sigma model in an isotropic plane wave](#string-sigma-model-in-an-isotropic-plane-wave)
      - [Plane-wave string mode Hamiltonian](#plane-wave-string-mode-hamiltonian)
      - [Plane-wave string mode frequency](#plane-wave-string-mode-frequency)
  - [Classical equivalence of Polyakov and Nambu–Goto actions](#classical-equivalence-of-polyakov-and-nambu-goto-actions)
  - [Worldsheet stress-energy tensor](#worldsheet-stress-energy-tensor)
  - [Phase-space identification of the Polyakov metric](#phase-space-identification-of-the-polyakov-metric)
  - [Polyakov path integral](#polyakov-path-integral)
    - [Two-dimensional quantum-gravity interpretation of strings](#two-dimensional-quantum-gravity-interpretation-of-strings)
    - [Worldsheet moduli](#worldsheet-moduli)
      - [Worldsheet conformal Killing group](#worldsheet-conformal-killing-group)
      - [Infinitesimal worldsheet modulus](#infinitesimal-worldsheet-modulus)
      - [Torus modular invariance](#torus-modular-invariance)
    - [Closed-string scattering amplitude](#closed-string-scattering-amplitude)
      - [Worldsheet integration count after conformal gauge fixing](#worldsheet-integration-count-after-conformal-gauge-fixing)
      - [Sphere tachyon position integral](#sphere-tachyon-position-integral)
      - [Sphere gauge fixing for four string vertices](#sphere-gauge-fixing-for-four-string-vertices)
      - [String dual resonance](#string-dual-resonance)
    - [Worldsheet Green function](#worldsheet-green-function)
    - [String vertex operator](#string-vertex-operator)
      - [Integrated string vertex operator](#integrated-string-vertex-operator)
        - [Massless closed-string vertex operator](#massless-closed-string-vertex-operator)
          - [Polarization tensor](#polarization-tensor)
          - [String-state gauge redundancy](#string-state-gauge-redundancy)
      - [String mass-shell condition](#string-mass-shell-condition)
      - [Tachyon vertex operator](#tachyon-vertex-operator)
  - [Worldsheet diffeomorphism](#worldsheet-diffeomorphism)
    - [Temporal gauge for a string](#temporal-gauge-for-a-string)
    - [Static gauge](#static-gauge)
      - [Monge gauge](#monge-gauge)
        - [Physical transverse velocity of a tilted string](#physical-transverse-velocity-of-a-tilted-string)
        - [Monge-gauge Hamiltonian of a three-dimensional string](#monge-gauge-hamiltonian-of-a-three-dimensional-string)
  - [Weyl transformation](#weyl-transformation)
  - [Conformal gauge](#conformal-gauge)
    - [Residual conformal transformation](#residual-conformal-transformation)
      - [Light-cone gauge in string theory](#light-cone-gauge-in-string-theory)
        - [Light-cone super-Virasoro constraints](#light-cone-super-virasoro-constraints)
        - [Residual mass-shell action in light-cone string gauge](#residual-mass-shell-action-in-light-cone-string-gauge)
    - [Virasoro constraint](#virasoro-constraint)
      - [Closed-string physical-state Virasoro conditions](#closed-string-physical-state-virasoro-conditions)
      - [Physical-state Virasoro conditions for an open string](#physical-state-virasoro-conditions-for-an-open-string)
      - [Classical Virasoro constraint algebra](#classical-virasoro-constraint-algebra)
  - [String nonlinear sigma model](#string-nonlinear-sigma-model)
    - [String-frame massless effective action](#string-frame-massless-effective-action)
    - [String-frame metric](#string-frame-metric)
      - [Einstein-frame metric](#einstein-frame-metric)
    - [Background field expansion of a string sigma model](#background-field-expansion-of-a-string-sigma-model)
    - [Kalb–Ramond field](#kalb-ramond-field)
      - [Light-cone gauge for a two-form](#light-cone-gauge-for-a-two-form)
      - [Kalb-Ramond field strength](#kalb-ramond-field-strength)
      - [H-field](#h-field)
    - [Sigma-model beta function](#sigma-model-beta-function)
      - [One-loop metric beta function of a string sigma model](#one-loop-metric-beta-function-of-a-string-sigma-model)
      - [Leading dilaton Weyl anomaly coefficient](#leading-dilaton-weyl-anomaly-coefficient)
      - [Leading metric-dilaton Weyl condition](#leading-metric-dilaton-weyl-condition)
        - [Dilaton equation from contracted Bianchi identity](#dilaton-equation-from-contracted-bianchi-identity)
          - [Linear dilaton counterexample to zero integration constant](#linear-dilaton-counterexample-to-zero-integration-constant)
          - [Exponentiated dilaton wave equation](#exponentiated-dilaton-wave-equation)
      - [Worldsheet Weyl anomaly](#worldsheet-weyl-anomaly)
        - [Bosonic sigma-model Weyl anomaly coefficients](#bosonic-sigma-model-weyl-anomaly-coefficients)
  - [Worldsheet ghost field](#worldsheet-ghost-field)
    - [Three-point worldsheet ghost correlator](#three-point-worldsheet-ghost-correlator)
    - [Ghost oscillator Virasoro generators](#ghost-oscillator-virasoro-generators)
    - [Ghost Virasoro zero-mode convention](#ghost-virasoro-zero-mode-convention)
    - [Ghost oscillator vacuum](#ghost-oscillator-vacuum)
      - [Ghost zero-mode pairing](#ghost-zero-mode-pairing)
    - [BRST operator](#brst-operator)
      - [Virasoro closure from BRST nilpotence](#virasoro-closure-from-brst-nilpotence)
      - [BRST physical-state constraints of an open string](#brst-physical-state-constraints-of-an-open-string)
      - [BRST current](#brst-current)
    - [Worldsheet ghost action](#worldsheet-ghost-action)
      - [Chiral conformal-gauge BRST nilpotence is on shell](#chiral-conformal-gauge-brst-nilpotence-is-on-shell)
      - [Trace elimination in string Faddeev-Popov gauge fixing](#trace-elimination-in-string-faddeev-popov-gauge-fixing)
      - [Worldsheet diffeomorphism ghost operator](#worldsheet-diffeomorphism-ghost-operator)
        - [Formal adjoint of the worldsheet conformal Killing operator](#formal-adjoint-of-the-worldsheet-conformal-killing-operator)
- [Worldsheet](#worldsheet)
  - [Winding-supported circular string](#winding-supported-circular-string)
  - [Proper length of a string](#proper-length-of-a-string)
  - [Worldsheet metric](#worldsheet-metric)
  - [Worldsheet area](#worldsheet-area)
  - [String embedding map](#string-embedding-map)
    - [Worldsheet zero mode](#worldsheet-zero-mode)
    - [Induced worldsheet metric](#induced-worldsheet-metric)
      - [Nambu–Goto action](#nambu-goto-action)
        - [Pulsating circular string](#pulsating-circular-string)
        - [Nambu–Goto equations of motion](#nambu-goto-equations-of-motion)
        - [Nambu-Goto phase-space action](#nambu-goto-phase-space-action)
          - [Target-space Noether charges of a string](#target-space-noether-charges-of-a-string)
          - [Nambu–Goto phase-space constraints](#nambu-goto-phase-space-constraints)
            - [Chiral constraint algebra of a closed string](#chiral-constraint-algebra-of-a-closed-string)
        - [Rotating Nambu–Goto string](#rotating-nambu-goto-string)
          - [Free-ended straight-string Regge relation](#free-ended-straight-string-regge-relation)
          - [Rigid circular string in four spatial dimensions](#rigid-circular-string-in-four-spatial-dimensions)
          - [Straight rotating string with one fixed endpoint](#straight-rotating-string-with-one-fixed-endpoint)
  - [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)
    - [Global conformal Ward identities for chiral correlators](#global-conformal-ward-identities-for-chiral-correlators)
    - [Liouville field theory](#liouville-field-theory)
    - [Radial quantization](#radial-quantization)
    - [Quasi-primary operator](#quasi-primary-operator)
    - [Free chiral Majorana fermion conformal field theory](#free-chiral-majorana-fermion-conformal-field-theory)
      - [Ising Virasoro modules from a Majorana fermion](#ising-virasoro-modules-from-a-majorana-fermion)
    - [Beta-gamma system](#beta-gamma-system)
      - [Stress tensor of a commuting beta-gamma system](#stress-tensor-of-a-commuting-beta-gamma-system)
      - [Radial-ordering sign in commuting beta-gamma contractions](#radial-ordering-sign-in-commuting-beta-gamma-contractions)
    - [bc system](#bc-system)
      - [Central charge of reparameterization ghosts](#central-charge-of-reparameterization-ghosts)
      - [bc ghost operator-product expansion](#bc-ghost-operator-product-expansion)
    - [Primary field](#primary-field)
      - [Primary state](#primary-state)
      - [Transversality of derivative-exponential primary vertices](#transversality-of-derivative-exponential-primary-vertices)
      - [Conformal weight](#conformal-weight)
      - [Virasoro descendant](#virasoro-descendant)
    - [Operator product expansion](#operator-product-expansion)
    - [Holomorphic stress-energy tensor](#holomorphic-stress-energy-tensor)
      - [Stress-tensor operator-product expansion](#stress-tensor-operator-product-expansion)
      - [Virasoro algebra](#virasoro-algebra)
        - [Virasoro character](#virasoro-character)
        - [Virasoro Verma module](#virasoro-verma-module)
          - [Level-two Virasoro descendant Gram matrix](#level-two-virasoro-descendant-gram-matrix)
        - [Unitary highest-weight Virasoro module](#unitary-highest-weight-virasoro-module)
        - [Sugawara construction](#sugawara-construction)
          - [Coset construction](#coset-construction)
        - [Unitary Virasoro discrete series](#unitary-virasoro-discrete-series)
        - [Virasoro generator](#virasoro-generator)
        - [Virasoro zero-mode shift](#virasoro-zero-mode-shift)
        - [Virasoro central extension](#virasoro-central-extension)
          - [Free-boson Virasoro central term](#free-boson-virasoro-central-term)
      - [Central charge](#central-charge)
        - [Superconformal current](#superconformal-current)
          - [Canonical supercurrent bracket of free RNS matter](#canonical-supercurrent-bracket-of-free-rns-matter)
          - [N=1 super-Virasoro algebra](#n-1-super-virasoro-algebra)
            - [Ramond supercurrent zero-mode square](#ramond-supercurrent-zero-mode-square)
    - [Free boson conformal field theory](#free-boson-conformal-field-theory)
      - [Free-boson worldsheet propagator](#free-boson-worldsheet-propagator)
      - [Linear dilaton conformal field theory](#linear-dilaton-conformal-field-theory)
        - [Background-charge scalar field](#background-charge-scalar-field)
      - [Torus partition function of a free boson](#torus-partition-function-of-a-free-boson)
        - [Dedekind eta function](#dedekind-eta-function)
          - [Eta-quotient](#eta-quotient)
      - [Compact boson](#compact-boson)
        - [Momentum and winding modes](#momentum-and-winding-modes)
          - [Exceptional massless ground states of a bosonic circle](#exceptional-massless-ground-states-of-a-bosonic-circle)
          - [Compact-circle closed-string level matching](#compact-circle-closed-string-level-matching)
          - [Massless spectrum at the bosonic self-dual circle](#massless-spectrum-at-the-bosonic-self-dual-circle)
          - [T-duality](#t-duality)
            - [T-duality of D-brane boundary conditions](#t-duality-of-d-brane-boundary-conditions)
              - [Brane separation becomes a Wilson line](#brane-separation-becomes-a-wilson-line)
            - [Global qualifications of Abelian T-duality](#global-qualifications-of-abelian-t-duality)
            - [Self-dual circle compactification](#self-dual-circle-compactification)
              - [Self-dual circle current algebra](#self-dual-circle-current-algebra)
              - [Radius deformation as a Higgs mechanism](#radius-deformation-as-a-higgs-mechanism)
            - [Buscher procedure](#buscher-procedure)
              - [First-order action for Abelian worldsheet duality](#first-order-action-for-abelian-worldsheet-duality)
              - [Buscher dilaton shift](#buscher-dilaton-shift)
                - [Polar-coordinate T-dual background](#polar-coordinate-t-dual-background)
              - [Buscher rules](#buscher-rules)
                - [Buscher dual of a metric with vanishing two-form](#buscher-dual-of-a-metric-with-vanishing-two-form)
- [String oscillator](#string-oscillator)
  - [Oscillator vacuum](#oscillator-vacuum)
  - [Half-integer open-string oscillator](#half-integer-open-string-oscillator)
  - [String level operator](#string-level-operator)
    - [Integer string oscillator level](#integer-string-oscillator-level)
  - [Closed-string level matching](#closed-string-level-matching)
  - [Normal-ordering constant of a string](#normal-ordering-constant-of-a-string)
    - [Critical-vector assumption in the string intercept argument](#critical-vector-assumption-in-the-string-intercept-argument)
    - [Neumann-Dirichlet string zero-point energy](#neumann-dirichlet-string-zero-point-energy)
      - [Lowest levels of a fully transverse ND bosonic string](#lowest-levels-of-a-fully-transverse-nd-bosonic-string)
  - [Bosonic string mass spectrum](#bosonic-string-mass-spectrum)
    - [Closed-bosonic-string mass shell from primary weights](#closed-bosonic-string-mass-shell-from-primary-weights)
    - [Massive two-form at closed-string level two](#massive-two-form-at-closed-string-level-two)
    - [Massless first closed-string level](#massless-first-closed-string-level)
    - [Open bosonic string mass spectrum](#open-bosonic-string-mass-spectrum)
      - [Lowest light-cone levels of an open bosonic string](#lowest-light-cone-levels-of-an-open-bosonic-string)
- [Critical dimension of string theory](#critical-dimension-of-string-theory)
  - [Bosonic-string critical dimension from ghost descendants](#bosonic-string-critical-dimension-from-ghost-descendants)
  - [Critical dimension of the RNS superstring](#critical-dimension-of-the-rns-superstring)
    - [Massless chiral RNS spectrum after GSO projection](#massless-chiral-rns-spectrum-after-gso-projection)
- [Koba-Nielsen factor](#koba-nielsen-factor)
  - [Möbius invariance of on-shell closed-string vertex integrals](#mobius-invariance-of-on-shell-closed-string-vertex-integrals)
  - [Virasoro–Shapiro amplitude](#virasoro-shapiro-amplitude)
    - [Fixed-angle softness of the closed-string amplitude](#fixed-angle-softness-of-the-closed-string-amplitude)
    - [Virasoro–Shapiro amplitude pole residue](#virasoro-shapiro-amplitude-pole-residue)
  - [CHY formalism](#chy-formalism)
    - [Scattering equation](#scattering-equation)

## Internal free fermions in a four-dimensional bosonic string

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)

Keeping the ordinary reparameterization [bc ghost system](#bc-system), four embedding bosons require 44 additional real chiral fermions in each chirality to cancel the [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly). These are internal matter fields, not an assumed locally supersymmetric RNS construction. Their bilinear currents generate the chiral $\mathfrak{so}(44)$ current algebra, with $\binom{44}{2}=946$ currents. A full closed fermionic model also requires consistent spin-structure and modular projections; the central-charge count alone does not determine these choices.

<h3 id="zero-and-two-fermion-vertices-of-an-internally-fermionized-bosonic-string">Zero- and two-fermion vertices of an internally fermionized bosonic string</h3>

↑ **Parent:** [Internal free fermions in a four-dimensional bosonic string](#internal-free-fermions-in-a-four-dimensional-bosonic-string)

In the unprojected polynomial Neveu–Schwarz vertex sector, zero fermion insertions give the usual closed-string tachyon and the massless graviton, two-form and dilaton. Two insertions split into a left-right pair $\psi^i\bar\psi^j e^{ipX}$ of internal weights $(1/2,1/2)$ and a same-chirality current pair of weight one. The first has $M^2=-2/\alpha'$ and 44-squared scalar components. The second requires a bosonic derivative on the opposite side for level matching and gives the two sets of 946 massless gauge vectors. Four-fermion scalar-current products belong to a different insertion count. A chosen global projection may retain a subset, so these operators do not by themselves specify a projected string spectrum.

## Open string

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Open_string)

An open string has a worldsheet with boundary. Its endpoint conditions may be [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition), or mixtures selected independently in target-space directions.

### Open-string oscillator degeneracy

↑ **Parent:** [Open string](#open-string)

For an ordinary critical [open string](#open-string) with all [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition), there are 24 independent transverse creation oscillators at each positive mode number $n$. Summing their nonnegative occupation numbers gives one factor $(1-w^n)^{-24}$. The coefficient $d_p=[w^p]F(w)$ counts oscillator polarizations at level $p$, excluding continuous center-of-mass momentum and additional endpoint multiplicities. [Cauchy coefficient formula](analysis.md#cauchy-coefficient-formula) gives $d_p=(2\pi i)^{-1}\oint F(w)w^{-p-1}dw$.

#### Large-level degeneracy of an open bosonic string

↑ **Parent:** [Open-string oscillator degeneracy](#open-string-oscillator-degeneracy)

The [Dedekind eta function](#dedekind-eta-function) modular transformation gives $F(e^{-t})\sim(t/2\pi)^{12}\exp(4\pi^2/t-t)$. The [saddle-point approximation](analysis.md#saddle-point-approximation) for coefficient extraction has $t_0=2\pi/\sqrt{p-1}$, phase $4\pi\sqrt{p-1}$ and curvature $(p-1)^{3/2}/\pi$. Its prefactor $t_0^{12}$ supplies $(p-1)^{-6}$ and the Gaussian width supplies $(p-1)^{-3/4}/\sqrt2$. This explains both the exponential growth and the power $-27/4$.

### Open-string endpoint momentum flux

↑ **Parent:** [Open string](#open-string)

For the [Nambu-Goto phase-space action](#nambu-goto-phase-space-action), $\dot P_m=\partial_\sigma J_m$ with $J_m=eT^2X'_m+uP_m$. Thus $\dot{\mathcal P}_m=J_m(\pi)-J_m(0)$. Free endpoint variations force $J_m=0$ individually. A [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) allows an external support or [D-brane](string-theory.md#d-brane) to absorb momentum in the fixed direction.

#### Variational open-string boundary conditions

↑ **Parent:** [Open-string endpoint momentum flux](#open-string-endpoint-momentum-flux)

The spatial integration-by-parts term in the [Nambu-Goto phase-space action](#nambu-goto-phase-space-action) pairs endpoint displacement with momentum flux $J_m=eT^2X'_m+uP_m$. Free endpoint displacements require zero flux. Fixed normal coordinates instead set those variations to zero, while tangential variations retain a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition). Boundary conditions must also be preserved by the equations of motion. In a boundary-preserving gauge with $u=0$, mixed [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) and [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) implement a planar [D-brane](string-theory.md#d-brane).

#### Free-end string boundary condition

↑ **Parent:** [Open-string endpoint momentum flux](#open-string-endpoint-momentum-flux)

Free endpoint variations set the [open string](#open-string) flux $eT^2X'_m+uP_m$ to zero. In a boundary-adapted temporal gauge, freedom to vary time forces $u=0$ at the end. Nonzero lapse then gives $X'^m=0$, a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition).

##### Null motion of a free string endpoint

↑ **Parent:** [Free-end string boundary condition](#free-end-string-boundary-condition)

In a boundary-adapted [temporal gauge](relativistic-quantum-field.md#temporal-gauge), a free [open string](#open-string) endpoint has $X'^m=0$. The [Nambu–Goto phase-space constraints](#nambu-goto-phase-space-constraints) then imply $P^2=0$, while $\dot X=eP$ implies $\dot X^2=0$. For $X^0=t$, its spatial speed is one. This null boundary is compatible with a timelike interior [worldsheet](#worldsheet).

### Open-string mode expansion

↑ **Parent:** [Open string](#open-string)

In [conformal gauge](#conformal-gauge), a free open-string coordinate with [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) has a cosine expansion. Canonical quantization turns its nonzero Fourier coefficients into [string oscillators](#string-oscillator).

#### Integer-mode expansion with parallel D-brane endpoints

↑ **Parent:** [Open-string mode expansion](#open-string-mode-expansion)

On $0\le\sigma\le\pi$, a coordinate with [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition) at both ends has a constant position, linear time [zero mode](linear-operator-theory.md#zero-mode) and cosine oscillators. A coordinate with [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) at both ends has a linear spatial interpolation between endpoint positions and sine oscillators, with no [momentum](momentum.md) [zero mode](linear-operator-theory.md#zero-mode). Both have [integer](integer.md) frequencies. This differs from an [ND boundary condition](#neumann-dirichlet-open-string-boundary-condition), which applies different conditions at the two ends of the same coordinate and gives half-integer frequencies.

#### Oscillator symplectic form of an open string

↑ **Parent:** [Open-string mode expansion](#open-string-mode-expansion)

The Fourier kinetic term $\sum_{k>0}i\alpha_{-k}\cdot\dot\alpha_k/k$ supplies conjugate pairs, with $\alpha_{-k}=\alpha_k^*$. Inverting its [symplectic form](symplectic-geometry.md#symplectic-form) yields the displayed [Poisson brackets](hamiltonian-mechanics.md#poisson-bracket). Nonzero modes are independent of the center-of-mass pair, while $\alpha_0=\sqrt{2\alpha'}p$ is the momentum zero mode. The imaginary factors are compatible with a real action up to a total derivative.

#### Neumann-Dirichlet open-string boundary condition

↑ **Parent:** [Open-string mode expansion](#open-string-mode-expansion)

A transverse [open string](#open-string) coordinate has an ND boundary condition when one endpoint obeys a [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) and the other a [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition). On a strip of width $\pi$, its nonconstant spatial [eigenfunctions](linear-operator-theory.md#eigenfunction) are $\cos((n+1/2)\sigma)$ when the free endpoint is at zero. They solve the endpoint equations because their derivatives vanish at zero and their values vanish at $\pi$. Reversing the endpoints gives sine [eigenfunctions](linear-operator-theory.md#eigenfunction) with the same frequencies. The fixed endpoint removes the dynamical [worldsheet zero mode](#worldsheet-zero-mode).

##### Bosonic ND boundary-changing conformal weight

↑ **Parent:** [Neumann-Dirichlet open-string boundary condition](#neumann-dirichlet-open-string-boundary-condition)

For one free boson, the mixed ND open-string sector has strip vacuum energy $E_0=1/48$. The strip-to-plane transformation relates this energy to the plane [Virasoro algebra](#virasoro-algebra) zero mode by $E_0=h-c/24$, with [central charge](#central-charge) $c=1$. Hence its ground [conformal weight](#conformal-weight) is $h=1/48+1/24=1/16$. For $d$ independent ND coordinates the weights add to $d/16$. At $d=24$, the plane matter ground weight is $3/2$, while the strip oscillator vacuum energy is $1/2$. The plane physical condition $L_0^{\mathrm{plane}}-1=0$ is therefore equivalent to $\alpha'p_\parallel^2+N+1/2=0$. The apparent different constants are coordinate/constraint conventions, not different mass spectra.

## Closed string

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Closed_string)

A closed string has a cylindrical worldsheet without boundary. Periodicity permits independent left- and right-moving oscillator sectors and, in a compact target direction, winding modes.

### Large-level degeneracy of a closed bosonic string

↑ **Parent:** [Closed string](#closed-string)

The left and right transverse oscillator sectors each have [generating function](sequence-and-series.md#generating-function) $\prod_{m\ge1}(1-q^m)^{-24}$. Its coefficient satisfies $d_N\sim2^{-1/2}(N-1)^{-27/4}e^{4\pi\sqrt{N-1}}$. [Closed-string level matching](#closed-string-level-matching) requires equal levels but leaves their polarizations independent, so $g_N=d_N^2$. With $\alpha'M^2=4(N-1)$, the exponential is $e^{\beta_H M}$ with $\beta_H=4\pi\sqrt{\alpha'}$. The smooth rest-mass density is proportional to $M^{-26}e^{\beta_H M}$, since $dN/dM=\alpha'M/2$. This distinguishes degeneracy per level from density per unit mass. The [polynomial](polynomial.md) prefactor matters at the boundary of canonical convergence.

### Closed-string mode expansion

↑ **Parent:** [Closed string](#closed-string)

A free closed-string embedding coordinate is the sum of center-of-mass zero modes and independent periodic left- and right-moving oscillator expansions.

## Covariant quantization of the bosonic string

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)

Covariant quantization keeps target-spacetime Lorentz covariance manifest, imposes canonical commutation relations on every embedding coordinate and removes unphysical states with the [Virasoro constraints](#virasoro-constraint).

### No-ghost theorem below the critical bosonic dimension

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

For integer target dimension $2\le d\le26$, intercept $a=1$ and ordinary nonzero momentum, the [old covariant string quantization](#old-covariant-string-quantization) conditions leave a positive-semidefinite physical inner product. Quotienting its physical [null string states](#null-string-state) removes gauge degeneracy. A [DDF operator](#ddf-operator) basis displays $d-2$ positive transverse oscillators; below dimension 26 the remaining physical longitudinal sector can be organized as a unitary [Virasoro algebra](#virasoro-algebra) sector with central charge $26-d$ and highest weight zero. At $d=26$ this extra sector becomes null and the quotient reduces to the 24 transverse oscillators. The result concerns negative-norm states, not the removal of the bosonic [tachyon](physics.md#tachyon), and it does not itself cancel the [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) of a subcritical matter theory.

### DDF operator

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

DDF operators are transverse physical [string oscillators](#string-oscillator) constructed as contour integrals of weight-one [string vertex operators](#string-vertex-operator). Choose a null reference momentum $q$ and transverse polarizations $\epsilon_i$ orthogonal to it and to a reference on-shell momentum. The integrand is proportional to $\epsilon_i\cdot\partial X\,e^{inq\cdot X}$; its normalization and $q\cdot p$ are fixed so the operators obey the oscillator algebra in the title and commute with the positive-mode [Virasoro constraints](#virasoro-constraint). For an open-string tachyon seed, one can use $2\alpha' q\cdot p=1$. Acting with negative modes shifts momentum and raises oscillator level while preserving the physical mass-shell condition. Their transverse [Fock space](quantum-field-theory.md#fock-space) has positive norm and makes the physical content of the [no-ghost theorem for the critical bosonic string](#no-ghost-theorem-for-the-critical-bosonic-string) explicit.

### No-ghost theorem for the critical bosonic string

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

In flat 26-dimensional [bosonic string theory](bosonic-string-theory.md), at ordinary nonzero momentum, take [physical string states](#physical-string-state) satisfying $L_{n>0}|\psi\rangle=0$ and $(L_0-1)|\psi\rangle=0$. The [inner product](inner-product.md) restricted to these states is positive semidefinite. Quotienting by physical [null string states](#null-string-state) removes the degeneracy; the resulting [Hilbert space](hilbert-space.md) is represented by the 24 transverse [string oscillators](#string-oscillator). This is a statement about negative-norm matter states, not about removing the auxiliary [Faddeev-Popov ghosts](relativistic-quantum-field.md#faddeev-popov-ghost). It does not remove the bosonic [tachyon](physics.md#tachyon).

### Level-two open-string polarization decomposition

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

For $d=26$, $q^2=-2$ and the [physical string state](#physical-string-state) $[\zeta_{\mu\nu}\alpha_{-1}^\mu\alpha_{-1}^\nu+b_\mu\alpha_{-2}^\mu]|p\rangle$, the [Virasoro constraints](#virasoro-constraint) give $b_\nu=-q^\mu\zeta_{\mu\nu}$ and $t=\zeta^\mu{}_{\mu}=-2q\cdot b$. Every solution has the displayed decomposition, where $q\cdot A=0$ and $c$ is symmetric, traceless and transverse to $q$. The vector piece is $L_{-1}(2A\cdot\alpha_{-1}|p\rangle)$; the scalar piece is $t(L_{-2}+3L_{-1}^2/2)|p\rangle/10$. These are [null string states](#null-string-state), leaving the transverse traceless massive tensor as the physical polarization.

### Negative-norm string state

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

Time-coordinate oscillators produce negative norms in the covariant indefinite [Fock space](quantum-field-theory.md#fock-space). A physical negative-norm state would violate probabilistic unitarity. Such ghosts differ from the anticommuting [worldsheet ghost fields](#worldsheet-ghost-field) introduced by [gauge fixing](relativistic-quantum-field.md#gauge-fixing).

### Old covariant string quantization

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

Old covariant quantization retains all target-space [string oscillators](#string-oscillator) and imposes $(L_0-a)|\psi\rangle=0$ and $L_n|\psi\rangle=0$ for $n>0$. Negative-mode constraints are adjoints, not further annihilation conditions. Quotienting physical [null string states](#null-string-state) removes redundant polarizations.

#### Level-two scalar in covariant string quantization

↑ **Parent:** [Old covariant string quantization](#old-covariant-string-quantization)

At $a=1$, let $k=\sqrt{2\alpha'}p$, $k^2=-2$. The physical scalar $[\alpha_{-1}\cdot\alpha_{-1}+(D+4)(k\cdot\alpha_{-1})^2/10+(D-1)k\cdot\alpha_{-2}/5]|p\rangle$ has norm $2(D-1)(26-D)/25$. It is positive below 26, null at 26, and a [string ghost state](#negative-norm-string-state) above 26. Matching the ordinary transverse spectrum removes this extra scalar at 26.

#### Level-one intercept bound in covariant string quantization

↑ **Parent:** [Old covariant string quantization](#old-covariant-string-quantization)

A polarization obeys $p\cdot\epsilon=0$ and $p^2=(a-1)/\alpha'$. If $a>1$, spacelike momentum allows a negative-norm timelike polarization. Thus ghost absence requires $a\leq1$. At $a=1$ the [null string state](#null-string-state) identification $\epsilon\sim\epsilon+\lambda p$ leaves $D-2$ polarizations.

### Physical string state

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

A physical string state obeys the Virasoro mass-shell and positive-mode constraints. States differing by a null state represent the same physical polarization.

### Spurious string state

↑ **Parent:** [Covariant quantization of the bosonic string](#covariant-quantization-of-the-bosonic-string)

A spurious string state is a positive-level Virasoro descendant orthogonal to all physical string states.

#### Null string state

↑ **Parent:** [Spurious string state](#spurious-string-state)

A null string state is both physical and spurious. It has zero norm and is quotiented from the physical state space.

##### Null-state quotient of a string

↑ **Parent:** [Null string state](#null-string-state)

The physical state space of [old covariant quantization](#old-covariant-string-quantization) is quotiented by its physical spurious states, which are orthogonal to all physical states. In a ghost-free sector these form the radical of the semidefinite inner product. The quotient retains positive physical polarizations.

##### Level-two scalar Virasoro null state

↑ **Parent:** [Null string state](#null-string-state)

For $L_0|p\rangle=-|p\rangle$, the descendant $Z=(L_{-2}+\tfrac32L_{-1}^2)|p\rangle$ obeys $L_1Z=0$ and $L_2Z=(D-26)|p\rangle/2$. It becomes physical and null at 26 and supplies the scalar quotient needed for the massive spin-two [light-cone gauge in string theory](#light-cone-gauge-in-string-theory) spectrum.

## String tension

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/String_tension)

String tension is energy per unit length. The Regge-slope parameter $\alpha'$ is conventionally defined by $T=(2\pi\alpha')^{-1}$.

### String length

↑ **Parent:** [String tension](#string-tension)

The characteristic string length is $\ell_s=\sqrt{\alpha'}$, with $T=1/(2\pi\alpha')$. Excited string states have masses of order $1/\ell_s$ and higher-derivative corrections become important at that scale.

### Regge trajectory

↑ **Parent:** [String tension](#string-tension)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Regge_trajectory)

A Regge trajectory is an approximately linear relation between angular momentum and squared mass. A classical rotating open string obeys $J=\alpha'M^2$, with quantum effects adding an intercept.

#### Regge limit

↑ **Parent:** [Regge trajectory](#regge-trajectory)

The Regge limit of a scattering amplitude takes the center-of-mass energy invariant $s$ large at fixed momentum-transfer invariant $t$. A leading trajectory produces a power $s^{\alpha(t)}$, with signature and residue factors. For the bosonic [Virasoro–Shapiro amplitude](#virasoro-shapiro-amplitude) in dimensionless string variables, $\alpha(t)=2+2t$. This differs from fixed-angle high-energy scattering.

## Polyakov action

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polyakov_action)

The Polyakov action introduces an independent worldsheet metric $g_{\alpha\beta}$:

$$
S_{\rm P}=-\frac T2\int_\Sigma d^2\sigma\,\sqrt{-g}\,
g^{\alpha\beta}\partial_\alpha X\mathbin\cdot\partial_\beta X.
$$

Its metric equation makes $g_{\alpha\beta}$ conformal to the [induced worldsheet metric](#induced-worldsheet-metric), reducing it classically to the [Nambu–Goto action](#nambu-goto-action).

### String sigma model in a spacetime metric

↑ **Parent:** [Polyakov action](#polyakov-action)

Replacing the flat target metric in the [Polyakov action](#polyakov-action) by a [spacetime metric](general-relativity.md#spacetime-metric) $g_{\mu\nu}(X)$ gives the displayed string sigma model. The embedding fields $X^\mu$ map the [worldsheet](#worldsheet) into target spacetime, while $h_{ab}$ is an independent [worldsheet metric](#worldsheet-metric). Classical [worldsheet diffeomorphisms](#worldsheet-diffeomorphism) and [Weyl transformations](#weyl-transformation) permit [conformal gauge](#conformal-gauge); quantum consistency additionally requires vanishing [sigma-model beta functions](#sigma-model-beta-function).

#### String sigma model in an isotropic plane wave

↑ **Parent:** [String sigma model in a spacetime metric](#string-sigma-model-in-a-spacetime-metric)

In [conformal gauge](#conformal-gauge) and [light-cone gauge in string theory](#light-cone-gauge-in-string-theory) $X^+=\kappa\tau$, the transverse part of the [string sigma model in a spacetime metric](#string-sigma-model-in-a-spacetime-metric) reduces to

$$
S_\perp=\frac T2\int d\tau d\sigma\,\left(\dot X^I\dot X^I-X'^IX'^I-m^2\kappa^2X^IX^I\right).
$$

The omitted longitudinal term is a total time derivative. Each transverse coordinate obeys a massive [wave equation](wave-equation.md). If the spatial period is $L$, the longitudinal momentum is $p^+=T\kappa L$ in this normalization. Keeping the gauge slope explicit prevents missing a factor of $p^+$ when changing conventions.

##### Plane-wave string mode Hamiltonian

↑ **Parent:** [String sigma model in an isotropic plane wave](#string-sigma-model-in-an-isotropic-plane-wave)

Expand every transverse [closed string](#closed-string) coordinate in a real orthonormal [Fourier basis](fourier-series.md#fourier-basis) of the spatial circle. The [canonical momenta](hamiltonian-mechanics.md#canonical-momentum) are $p_{Ia}=T\dot q_{Ia}$, and spatial orthogonality reduces the field [Hamiltonian](hamiltonian-mechanics.md#hamiltonian) to the displayed independent [harmonic oscillators](classical-mechanics.md#simple-harmonic-motion). Canonical quantization gives $\omega_a(a_{Ia}^\dagger a_{Ia}+1/2)$ for each nonzero-frequency mode; a zero-frequency mode retains the free particle term $p_{Ia}^2/(2T)$. The formal [zero-point energy](quantum-harmonic-oscillator.md#zero-point-energy) requires a regulator; it is not automatically the massless flat-background intercept. Opposite travelling-wave oscillator combinations diagonalize the translation generator and satisfy [closed-string level matching](#closed-string-level-matching).

##### Plane-wave string mode frequency

↑ **Parent:** [String sigma model in an isotropic plane wave](#string-sigma-model-in-an-isotropic-plane-wave)

For a [closed string](#closed-string) in a [string sigma model in an isotropic plane wave](#string-sigma-model-in-an-isotropic-plane-wave), insert $e^{-i\omega_n\tau+2\pi in\sigma/L}$ into the transverse [wave equation](wave-equation.md). Periodicity requires integer $n$, giving the displayed [dispersion relation](dispersion-relation.md). The zero spatial mode is an oscillator of frequency $|m\kappa|$; when this mass vanishes it becomes a free particle mode and needs the position-plus-linear-time expansion.

<h3 id="classical-equivalence-of-polyakov-and-nambu-goto-actions">Classical equivalence of Polyakov and Nambu–Goto actions</h3>

↑ **Parent:** [Polyakov action](#polyakov-action)

Varying the independent metric in the [Polyakov action](#polyakov-action) sets the [worldsheet stress tensor](#worldsheet-stress-energy-tensor) to zero. For a nondegenerate timelike embedding in two [worldsheet](#worldsheet) dimensions, the metric is proportional to the [induced worldsheet metric](#induced-worldsheet-metric). The conformal factor cancels from the action, which becomes the [Nambu–Goto action](#nambu-goto-action). This elimination is classical; the quantum measure and [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) require separate treatment.

### Worldsheet stress-energy tensor

↑ **Parent:** [Polyakov action](#polyakov-action)

Varying the independent [worldsheet metric](#worldsheet-metric) gives $T_{ab}=T[\partial_aX\cdot\partial_bX-\tfrac12\gamma_{ab}\gamma^{cd}\partial_cX\cdot\partial_dX]$. Its classical vanishing is the metric equation and produces the [Virasoro constraints](#virasoro-constraint).

### Phase-space identification of the Polyakov metric

↑ **Parent:** [Polyakov action](#polyakov-action)

For positive lapse, eliminating momentum gives $(\dot X-uX')^2/(2e)-eT^2X'^2/2$. This is the [Polyakov action](#polyakov-action) for $\gamma_{ab}=\bigl(\begin{smallmatrix}u^2-e^2T^2&u\\u&1\end{smallmatrix}\bigr)$, up to a [Weyl transformation](#weyl-transformation). Thus $e=1/T,u=0$ is [conformal gauge](#conformal-gauge).

### Polyakov path integral

↑ **Parent:** [Polyakov action](#polyakov-action)

The Polyakov path integral integrates over string embeddings and worldsheet metrics, divided by worldsheet diffeomorphisms and Weyl transformations. Gauge fixing introduces worldsheet ghosts and moduli integrals.

#### Two-dimensional quantum-gravity interpretation of strings

↑ **Parent:** [Polyakov path integral](#polyakov-path-integral)

The [Polyakov path integral](#polyakov-path-integral) integrates over [string worldsheet](#worldsheet) metrics as well as embedding fields, modulo [worldsheet diffeomorphisms](#worldsheet-diffeomorphism) and [Weyl transformations](#weyl-transformation). Summing surface topologies gives perturbative [two-dimensional quantum gravity](quantum-theory.md#two-dimensional-quantum-gravity) coupled to the coordinate matter fields. Gauge fixing retains [worldsheet moduli](#worldsheet-moduli) and introduces ghosts; a conformal gauge is locally flat, not a global flat metric on every genus. Cancellation of the [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) makes the critical bosonic version consistent.

#### Worldsheet moduli

↑ **Parent:** [Polyakov path integral](#polyakov-path-integral)

Worldsheet moduli parameterize inequivalent conformal structures and marked insertion points after [worldsheet diffeomorphisms](#worldsheet-diffeomorphism) and [Weyl invariance](#weyl-transformation) are fixed. At each [genus](topological-surface.md#genus-of-a-surface), [string perturbation theory](string-theory.md#string-perturbation-theory) integrates over the corresponding moduli space.

##### Worldsheet conformal Killing group

↑ **Parent:** [Worldsheet moduli](#worldsheet-moduli)

The worldsheet conformal Killing group is the connected residual group of conformal automorphisms of the chosen compact [Riemann surface](riemann-surfaces.md). Its infinitesimal vectors satisfy the [Conformal Killing equation](general-relativity.md#conformal-killing-equation), or $P_1v=0$ for the [worldsheet diffeomorphism ghost operator](#worldsheet-diffeomorphism-ghost-operator). Its complex dimensions are three on a sphere, one on a torus, and zero for [genus](topological-surface.md#genus-of-a-surface) at least two. The sphere group consists of [Möbius transformations](group-theory.md#mobius-transformation), while the torus's connected group is translation. Additional discrete automorphisms are handled by the moduli quotient rather than counted as continuous zero modes.

##### Infinitesimal worldsheet modulus

↑ **Parent:** [Worldsheet moduli](#worldsheet-moduli)

After quotienting infinitesimal [worldsheet diffeomorphisms](#worldsheet-diffeomorphism) and [Weyl transformations](#weyl-transformation), choose a metric variation orthogonal to the gauge directions. Orthogonality to Weyl scaling makes its trace zero; the [formal adjoint of the worldsheet conformal Killing operator](#formal-adjoint-of-the-worldsheet-conformal-killing-operator) makes its divergence zero. These are transverse-traceless variations of the two-dimensional metric. In a local conformal complex coordinate, their nonzero components satisfy $\partial_{\bar z}t_{zz}=0$ and its conjugate, linking them to [holomorphic quadratic differentials](complex-geometry.md#holomorphic-quadratic-differential).

##### Torus modular invariance

↑ **Parent:** [Worldsheet moduli](#worldsheet-moduli)

The torus worldsheet path integral is invariant under the [modular group](modular-function.md#modular-group) acting on its complex parameter $\tau$. Integrating over the [standard fundamental domain of the modular group](modular-function.md#standard-fundamental-domain-of-the-modular-group) counts each inequivalent torus once and excludes the short-proper-time ultraviolet region.

#### Closed-string scattering amplitude

↑ **Parent:** [Polyakov path integral](#polyakov-path-integral)

A closed-string [scattering amplitude](quantum-scattering.md#scattering-amplitude) is a worldsheet correlation function of external [string vertex operators](#string-vertex-operator), integrated over their unfixed positions and [worldsheet moduli](#worldsheet-moduli), with the necessary [worldsheet ghost fields](#worldsheet-ghost-field).

##### Worldsheet integration count after conformal gauge fixing

↑ **Parent:** [Closed-string scattering amplitude](#closed-string-scattering-amplitude)

For a stable $n$-point [closed-string scattering amplitude](#closed-string-scattering-amplitude) on a [genus](topological-surface.md#genus-of-a-surface)-$g$ surface, let $d_g$ count complex unmarked [worldsheet moduli](#worldsheet-moduli) and $k_g$ count complex dimensions of the [worldsheet conformal Killing group](#worldsheet-conformal-killing-group). Integrating the $n$ vertex positions and moduli, then fixing $k_g$ positions, leaves $d_g+n-k_g$ complex integrations. The [punctured Riemann surface moduli dimension](geometry-and-topology.md#punctured-riemann-surface-moduli-dimension) identifies this as $3g-3+n$. [Faddeev-Popov ghost fields](relativistic-quantum-field.md#faddeev-popov-ghost) and antighost insertions implement the removed zero modes and the surviving modulus measure; they do not add independently integrated worldsheet coordinates.

##### Sphere tachyon position integral

↑ **Parent:** [Closed-string scattering amplitude](#closed-string-scattering-amplitude)

The tree-level [Polyakov path integral](#polyakov-path-integral) for closed-string [tachyons](physics.md#tachyon) reduces in [conformal gauge](#conformal-gauge) to their vertex-position integral on the [Riemann sphere](riemann-surfaces.md#riemann-sphere). Three positions are fixed by the residual [Möbius group](group-theory.md#mobius-group); the other $N-3$ complex positions are integrated. The embedding-field Gaussian integral produces [momentum conservation](momentum.md#momentum-conservation) and the [Koba-Nielsen factor](#koba-nielsen-factor).

##### Sphere gauge fixing for four string vertices

↑ **Parent:** [Closed-string scattering amplitude](#closed-string-scattering-amplitude)

At genus zero the residual [Möbius transformation](group-theory.md#mobius-transformation) group fixes three marked insertion points, leaving one complex position to integrate. The corresponding [worldsheet ghost fields](#worldsheet-ghost-field) give $|z_{ij}z_{jk}z_{ki}|^2$ for the three fixed points. For on-shell weight-$(1,1)$ [string vertex operators](#string-vertex-operator), these ghost factors cancel the coordinate dependence of the fixed-point normalization, including the limit at infinity. The remaining [Koba-Nielsen factor](#koba-nielsen-factor) for four tachyons is the integrand of the [complex beta integral](complex-analysis.md#complex-beta-integral), producing the [Virasoro–Shapiro amplitude](#virasoro-shapiro-amplitude).

##### String dual resonance

↑ **Parent:** [Closed-string scattering amplitude](#closed-string-scattering-amplitude)

A single [crossing-symmetric scattering amplitude](quantum-scattering.md#crossing-symmetry) has equivalent pole expansions in different exchange channels. Its [scattering-amplitude factorization](quantum-scattering.md#scattering-amplitude-factorization) reproduces the string spectrum and couplings in each channel without adding the channel expansions again.

#### Worldsheet Green function

↑ **Parent:** [Polyakov path integral](#polyakov-path-integral)

A worldsheet Green function inverts the scalar kinetic operator after its zero modes have been removed. In a locally flat complex coordinate it satisfies $-(\pi\alpha')^{-1}\partial\bar\partial G(z,w)=\delta^{(2)}(z-w)$ and is $G(z,w)=-(\alpha'/2)\log|z-w|^2$ up to harmonic and constant terms.

#### String vertex operator

↑ **Parent:** [Polyakov path integral](#polyakov-path-integral)

A string vertex operator inserts an asymptotic string state at a point of the worldsheet. Its conformal weights encode the physical-state and mass-shell conditions.

These insertions are described by the state-field correspondence of a [vertex operator algebra](algebra.md#vertex-operator-algebra); an individual insertion is not the whole algebra.

##### Integrated string vertex operator

↑ **Parent:** [String vertex operator](#string-vertex-operator)

An integrated closed-string vertex is inserted as $\int d^2z\,V(z,\bar z)$. In conformal gauge its matter operator must have [conformal weights](#conformal-weight) $(1,1)$ so that the insertion is invariant under worldsheet coordinate changes.

###### Massless closed-string vertex operator

↑ **Parent:** [Integrated string vertex operator](#integrated-string-vertex-operator)

At the first massless closed-string level, the matter vertex has the form $\epsilon_{\mu\nu}:\!\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}\!:$, with null momentum and a polarization tensor transverse in both indices. Its symmetric trace-free, antisymmetric and trace sectors describe the graviton, [Kalb–Ramond field](#kalb-ramond-field) and [dilaton](string-theory.md#dilaton).

###### Polarization tensor

↑ **Parent:** [Massless closed-string vertex operator](#massless-closed-string-vertex-operator)

A closed-string polarization tensor specifies the target-spacetime tensor state multiplying $\partial X^\mu\bar\partial X^\nu e^{ik\cdot X}$. Its decomposition into symmetric trace-free, antisymmetric and trace parts separates the graviton, [Kalb–Ramond field](#kalb-ramond-field) and [dilaton](string-theory.md#dilaton) polarizations.

###### String-state gauge redundancy

↑ **Parent:** [Massless closed-string vertex operator](#massless-closed-string-vertex-operator)

Changing a massless closed-string polarization by a momentum-longitudinal tensor changes the integrated vertex by a worldsheet total derivative, equivalently by a BRST-exact state. The corresponding target-space transformations are linearized diffeomorphisms and two-form gauge transformations.

##### String mass-shell condition

↑ **Parent:** [String vertex operator](#string-vertex-operator)

A string mass-shell condition relates the target momentum of a vertex operator to its oscillator level. Together with polarization constraints, it makes the matter vertex have the conformal weights required for an integrated insertion.

##### Tachyon vertex operator

↑ **Parent:** [String vertex operator](#string-vertex-operator)

The bosonic closed-string tachyon vertex is the normal-ordered exponential ${}:e^{ip\cdot X}:$ integrated over its worldsheet position. Pairwise contractions of such exponentials generate the [Koba-Nielsen factor](#koba-nielsen-factor).

### Worldsheet diffeomorphism

↑ **Parent:** [Polyakov action](#polyakov-action)

A worldsheet diffeomorphism is a smooth reparameterization of the worldsheet coordinates under which $X^\mu$ is a scalar and $g_{\alpha\beta}$ is a rank-two tensor.

#### Temporal gauge for a string

↑ **Parent:** [Worldsheet diffeomorphism](#worldsheet-diffeomorphism)

On a future-directed patch, choose target time as worldsheet time, $X^0=t$. The momentum equation then gives $P^0=1/e$ and $X'^0=0$. Freedom to vary target time at an open-string endpoint sets its shift to zero, simplifying the endpoint momentum-flux condition.

#### Static gauge

↑ **Parent:** [Worldsheet diffeomorphism](#worldsheet-diffeomorphism)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Static_gauge)

Static gauge identifies selected target-space coordinates with worldvolume coordinates, such as $X^0=\tau$ for a string.

##### Monge gauge

↑ **Parent:** [Static gauge](#static-gauge)

For a string, this local [static gauge](#static-gauge) identifies two embedding coordinates with the worldsheet coordinates, $X^0=t$ and $X^1=\sigma$. The remaining coordinates describe a graph over that coordinate plane. Folded embeddings may require more than one patch.

###### Physical transverse velocity of a tilted string

↑ **Parent:** [Monge gauge](#monge-gauge)

For $X=(t,\sigma,k(\sigma+t))$, the vertical coordinate velocity is $k$, but its normal projection has magnitude $|k|/\sqrt{1+k^2}<1$. Tangential motion merely changes string labels. The [induced worldsheet metric](#induced-worldsheet-metric) has determinant $-1$ even when constant-label curves become spacelike for $|k|>1$.

###### Monge-gauge Hamiltonian of a three-dimensional string

↑ **Parent:** [Monge gauge](#monge-gauge)

With unit tension and $X^0=t$, $X^1=\sigma$, the [Virasoro constraints](#virasoro-constraint) give $P_1=-\Pi\Phi'$ and $P_0=-\sqrt{(1+\Phi'^2)(1+\Pi^2)}$. The reduced energy density is $\mathcal H=-P_0$. On the chiral branch $\Pi=\Phi'$, the [Hamiltonian field equation](hamiltonian-mechanics.md#hamiltonian-field-equation) becomes $\dot\Phi=\Phi'$.

### Weyl transformation

↑ **Parent:** [Polyakov action](#polyakov-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weyl_transformation)

A [Weyl transformation](#weyl-transformation) locally rescales a [metric tensor](general-relativity.md#metric-tensor), $g\mapsto e^{2\omega}g$, while retaining the same points and coordinates. Applied to a worldsheet metric, it leaves the embedding $X^\mu$ unchanged, and the classical [Polyakov action](#polyakov-action) is invariant under these [Weyl transformations](#weyl-transformation). Applied to a spacetime metric, a [Weyl rescaling](#weyl-transformation) can relate different frame conventions, such as a string metric and an Einstein metric; the accompanying field normalizations must be transformed as well. It is not itself a coordinate transformation.

### Conformal gauge

↑ **Parent:** [Polyakov action](#polyakov-action)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conformal_gauge)

Conformal gauge uses worldsheet diffeomorphisms and Weyl transformations to set $g_{\alpha\beta}=e^{2\phi}\eta_{\alpha\beta}$ locally.

#### Residual conformal transformation

↑ **Parent:** [Conformal gauge](#conformal-gauge)

After conformal gauge fixing, independent reparameterizations $\sigma^+\mapsto f(\sigma^+)$ and $\sigma^-\mapsto\widetilde f(\sigma^-)$ remain, accompanied by a compensating Weyl transformation.

##### Light-cone gauge in string theory

↑ **Parent:** [Residual conformal transformation](#residual-conformal-transformation)

Light-cone gauge uses residual conformal transformations to make the target-space coordinate $X^+$ linear in worldsheet time. The Virasoro constraints then determine $X^-$ from the transverse fields.

This is the string-worldsheet realization of [light cone gauge](relativistic-quantum-field.md#light-cone-gauge).

###### Light-cone super-Virasoro constraints

↑ **Parent:** [Light-cone gauge in string theory](#light-cone-gauge-in-string-theory)

On a patch with $\alpha_0^+\ne0$, use [worldsheet diffeomorphisms](#worldsheet-diffeomorphism) and [worldsheet supersymmetry](string-theory.md#worldsheet-supersymmetry) to fix $\alpha_{n\ne0}^+=0$ and $\psi_r^+=0$. The [Virasoro constraints](#virasoro-constraint) and [superconformal current](#superconformal-current) constraints then determine the longitudinal modes by the displayed transverse bilinears. In the [Ramond sector](string-theory.md#ramond-sector), reduction of the fermionic zero modes includes the zero-mode Dirac constraint; fixing only nonzero modes does not complete the reduction. Eight transverse bosons and eight transverse fermions remain in the critical ten-dimensional [RNS string](string-theory.md#spinning-string).

###### Residual mass-shell action in light-cone string gauge

↑ **Parent:** [Light-cone gauge in string theory](#light-cone-gauge-in-string-theory)

Fixing nonzero longitudinal oscillators leaves the center-of-mass symplectic term, transverse oscillator terms, and a zero-mode multiplier imposing the [mass-shell condition](#string-mass-shell-condition). On a patch with $p^+\ne0$, further choosing $x^+$ as time solves that [constraint](classical-mechanics.md#constraint-mechanics) for $p^-=[p_\perp^2+(N-a)/\alpha']/(2p^+)$. This distinguishes partial oscillator gauge fixing from the subsequent time choice.

#### Virasoro constraint

↑ **Parent:** [Conformal gauge](#conformal-gauge)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virasoro_constraint)

The worldsheet metric equation in conformal gauge sets the stress tensor to zero, $T_{++}=T_{--}=0$. In oscillator language these are the Virasoro constraints.

##### Closed-string physical-state Virasoro conditions

↑ **Parent:** [Virasoro constraint](#virasoro-constraint)

Critical [closed bosonic strings](#closed-string) have independent left- and right-moving [Virasoro constraints](#virasoro-constraint). Positive modes in both sectors annihilate physical kets, while both zero-mode conditions impose the mass shell and [closed-string level matching](#closed-string-level-matching). Quotient by physical [null string states](#null-string-state), equivalently use the appropriate [BRST cohomology](relativistic-quantum-field.md#brst-cohomology). With $L_0=\alpha'k^2/4+N$, the result is $N=\widetilde N$ and $M^2=4(N-1)/\alpha'$. Negative matter modes are adjoints rather than additional ket-annihilation constraints.

##### Physical-state Virasoro conditions for an open string

↑ **Parent:** [Virasoro constraint](#virasoro-constraint)

The covariant physical-state conditions impose positive-mode [Virasoro constraints](#virasoro-constraint) on kets and the adjoint conditions on bras, with intercept $a$ in the zero mode. They are a string version of [Gupta-Bleuler quantization](relativistic-quantum-field.md#gupta-bleuler-formalism). Imposing every positive and negative matter mode on the same state would conflict with the [Virasoro central extension](#virasoro-central-extension). In critical [bosonic string theory](bosonic-string-theory.md), $a=1$ and the matter [central charge](#central-charge) is $26$, canceled by the reparameterization ghosts.

##### Classical Virasoro constraint algebra

↑ **Parent:** [Virasoro constraint](#virasoro-constraint)

With the [oscillator symplectic form of an open string](#oscillator-symplectic-form-of-an-open-string), the quadratic generators $L_n=\sum_k\alpha_k\cdot\alpha_{n-k}/2$ obey $\{\alpha_k,L_n\}=-ik\alpha_{k+n}$. Their [Poisson brackets](hamiltonian-mechanics.md#poisson-bracket) close without a central term, so they are [first-class constraints](classical-mechanics.md#first-class-constraint). Quantization requires [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) and can produce the [Virasoro central extension](#virasoro-central-extension).

### String nonlinear sigma model

↑ **Parent:** [Polyakov action](#polyakov-action)

The string nonlinear sigma model couples the worldsheet embedding fields to target-space backgrounds such as a metric, a [Kalb–Ramond field](#kalb-ramond-field) and a [dilaton](string-theory.md#dilaton). Quantum Weyl invariance requires its beta functions to vanish.

#### String-frame massless effective action

↑ **Parent:** [String nonlinear sigma model](#string-nonlinear-sigma-model)

The leading massless-sector spacetime action is proportional to $\int\sqrt{-G}e^{-2\Phi}[R+4(\nabla\Phi)^2-H^2/12]$, with $H=dB$. The backgrounds are the [string-frame metric](#string-frame-metric), [dilaton](string-theory.md#dilaton), and [Kalb–Ramond field](#kalb-ramond-field). Massive string exchange generates higher-derivative corrections ordered by $\alpha'$. This perturbative bosonic massless-sector truncation does not remove the [tachyon](physics.md#tachyon) instability.

#### String-frame metric

↑ **Parent:** [String nonlinear sigma model](#string-nonlinear-sigma-model)

The string-frame metric is the target metric appearing directly in the kinetic term of the [string nonlinear sigma model](#string-nonlinear-sigma-model). With conventional Euclidean [dilaton](string-theory.md#dilaton) $\varphi$, its leading spacetime gravitational action contains $\sqrt{-g^{(s)}}e^{-2\varphi}(R+4|\nabla\varphi|^2)$. The dilaton-dependent Ricci coefficient distinguishes it from the [Einstein-frame metric](#einstein-frame-metric). Frame changes are local field redefinitions where the conformal factor is finite and nonzero; the [Lorentzian dilaton coupling sign convention](string-theory.md#lorentzian-dilaton-coupling-sign-convention) fixes which named field is $\varphi$.

##### Einstein-frame metric

↑ **Parent:** [String-frame metric](#string-frame-metric)

For $D>2$, rescale the [string-frame metric](#string-frame-metric) by $g^{(E)}=e^{-4\varphi/(D-2)}g^{(s)}$. The [Weyl transformation](#weyl-transformation) of the [Ricci scalar](general-relativity.md#ricci-scalar) makes the coefficient of the Einstein-frame Ricci term independent of the [dilaton](string-theory.md#dilaton). Indeed $g^{(s)}=e^{4\varphi/(D-2)}g^{(E)}$ contributes factors $e^{2D\varphi/(D-2)}$ from the volume, $e^{-2\varphi}$ from the original coupling and $e^{-4\varphi/(D-2)}$ from the Ricci term; their product is one. Derivative terms supply the transformed dilaton kinetic term. The two-dimensional case is excluded from this particular rescaling.

#### Background field expansion of a string sigma model

↑ **Parent:** [String nonlinear sigma model](#string-nonlinear-sigma-model)

Expand the [string embedding map](#string-embedding-map) along target geodesics as $X=\exp_{\bar X}Y$. The quadratic Euclidean fluctuation action has a [covariant derivative](general-relativity.md#covariant-derivative) term and a curvature term $-R_{acbd}Y^aY^b\partial\bar X^c\partial\bar X^d$. The logarithmically divergent coincident contraction is proportional to $\alpha'g^{ab}$; its curvature contraction is the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor). A compensating metric [counterterm](perturbative-quantum-field-theory.md#counterterm) gives $\beta^g_{ab}=\alpha'R_{ab}+O(\alpha'^2)$. This is why the target gravitational equation arises from quantum [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) cancellation, rather than from the classical worldsheet metric variation. Infrared regulation and removal of equation-of-motion terms by field redefinitions specify the usual one-loop scheme.

<h4 id="kalb-ramond-field">Kalb–Ramond field</h4>

↑ **Parent:** [String nonlinear sigma model](#string-nonlinear-sigma-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kalb–Ramond_field)

The Kalb–Ramond field is an antisymmetric two-form background coupled to the oriented worldsheet area element. Its gauge-invariant field strength is the three-form $H=dB$.

##### Light-cone gauge for a two-form

↑ **Parent:** [Kalb–Ramond field](#kalb-ramond-field)

When $\partial_-$ is invertible, choose $B_{-m}=0$. Residual gauge parameters are exact one-forms and act trivially on $B$. The remaining independent modes are antisymmetric transverse components $B_{IJ}$, satisfying $\square B_{IJ}=0$; longitudinal components obey $B_{+I}=\partial_-^{-1}\partial^JB_{IJ}$. There are $(D-2)(D-3)/2$ physical polarizations.

##### Kalb-Ramond field strength

↑ **Parent:** [Kalb–Ramond field](#kalb-ramond-field)

The three-form field strength of the [Kalb–Ramond field](#kalb-ramond-field) is $H=dB$. Its components are $H_{mnp}=\partial_mB_{np}+\partial_nB_{pm}+\partial_pB_{mn}$. In flat spacetime the free equation is $\partial^mH_{mnp}=0$.

##### H-field

↑ **Parent:** [Kalb–Ramond field](#kalb-ramond-field)

The H-field is the three-form field strength of a [Kalb–Ramond field](#kalb-ramond-field). It obeys the Bianchi identity $dH=0$ and contributes quadratically to the leading string background equations.

#### Sigma-model beta function

↑ **Parent:** [String nonlinear sigma model](#string-nonlinear-sigma-model)

A sigma-model beta function measures the failure of a worldsheet background coupling to remain scale invariant. Vanishing metric, B-field and dilaton beta functions gives the spacetime field equations order by order in $\alpha'$.

##### One-loop metric beta function of a string sigma model

↑ **Parent:** [Sigma-model beta function](#sigma-model-beta-function)

For the Euclidean kinetic normalization $(4\pi\alpha')^{-1}\int g_{ab}(X)\partial X^a\partial X^b$, vanishing two-form and constant [dilaton](string-theory.md#dilaton), the leading beta function is $\beta^g_{ab}=\alpha'R_{ab}$. The covariant Gaussian fluctuation operator contains a curvature vertex whose one-loop trace contracts to the [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor). Its logarithmic divergence renormalizes the metric. The scale convention is $\beta=\mu\,dg/d\mu$; Weyl consistency requires vanishing of this beta function as well as the other anomaly coefficients.

##### Leading dilaton Weyl anomaly coefficient

↑ **Parent:** [Sigma-model beta function](#sigma-model-beta-function)

For the conventional positive Euclidean [dilaton](string-theory.md#dilaton) curvature coupling, with no antisymmetric background field, the leading scalar Weyl coefficient is the displayed expression. The matter/ghost [central charge](#central-charge) gives $(D-26)/6$. In a geodesic [background field expansion of a string sigma model](#background-field-expansion-of-a-string-sigma-model), contracting $\tfrac12\nabla_a\nabla_b\varphi\,Y^aY^b$ in the curvature coupling produces the [counterterm](perturbative-quantum-field-theory.md#counterterm) $\delta\varphi=-\alpha'\Box\varphi/(2\varepsilon)$ and hence the Laplacian term. The full embedding equation $\Box_hX^a+\Gamma^a{}_{bc}\partial X^b\partial X^c=(\alpha'/2)R^{(2)}\nabla^a\varphi$ supplies the gradient-square improvement in the dilaton Weyl variation. Setting this coefficient to zero fixes the constant in the [dilaton equation from contracted Bianchi identity](#dilaton-equation-from-contracted-bianchi-identity); the metric equation alone does not. The [Lorentzian dilaton coupling sign convention](string-theory.md#lorentzian-dilaton-coupling-sign-convention) determines the named-field translation.

The noncritical coefficient is also given in [Tong's string theory notes, Section 7.4.4](https://davidtong.org/pdfs/teaching/string-theory/string7.pdf).

##### Leading metric-dilaton Weyl condition

↑ **Parent:** [Sigma-model beta function](#sigma-model-beta-function)

For the conventional Euclidean [dilaton](string-theory.md#dilaton) coupling $+(4\pi)^{-1}\int\sqrt h\,R\varphi$ and no antisymmetric background, the metric [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) vanishes at first order in $\alpha'$ when $R_{ab}+2\nabla_a\nabla_b\varphi=0$. The one-loop Ricci term follows from the [background field expansion of a string sigma model](#background-field-expansion-of-a-string-sigma-model). Under a [Weyl transformation](#weyl-transformation), the dilaton coupling varies as $-(2\pi)^{-1}\int\sqrt h\,\omega\Box_h\varphi$; the embedding equations replace this by the target Hessian contribution. Full Weyl invariance also requires the dilaton curvature coefficient, including the central-charge deficit, to vanish. See the [Lorentzian dilaton coupling sign convention](string-theory.md#lorentzian-dilaton-coupling-sign-convention) when translating an action with a specified Lorentzian sign.

The conventional coefficient agrees with the background equations in [Tong's string theory notes, Section 7.2.3](https://davidtong.org/pdfs/teaching/string-theory/string7.pdf).

###### Dilaton equation from contracted Bianchi identity

↑ **Parent:** [Leading metric-dilaton Weyl condition](#leading-metric-dilaton-weyl-condition)

Diverging $R_{ab}+2\nabla_a\nabla_b\varphi=0$ and using the [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity) and [Ricci identity](riemann-curvature-tensor.md#curvature-commutator-on-a-covariant-tensor) gives $\nabla_b(R+4\Box_g\varphi-4|\nabla\varphi|^2)=0$. The trace equation $R+2\Box_g\varphi=0$ then gives $\Box_g\varphi-2|\nabla\varphi|^2=C$, with $C$ constant on each connected component. Zero does not follow from the tensor equation alone. The additional dilaton anomaly coefficient fixes $C=(D-26)/(3\alpha')$ at leading order for the bosonic string without an antisymmetric background. In critical dimension it is zero; noncritical backgrounds have a central-charge-deficit term.

###### Linear dilaton counterexample to zero integration constant

↑ **Parent:** [Dilaton equation from contracted Bianchi identity](#dilaton-equation-from-contracted-bianchi-identity)

In flat target space, $\varphi=q_aX^a$ has zero Hessian and therefore solves the [leading metric-dilaton Weyl condition](#leading-metric-dilaton-weyl-condition) for every constant covector $q$. But $\Box\varphi-2|\nabla\varphi|^2=-2q^2$, which need not vanish. This demonstrates the integration constant left by the [contracted Bianchi identity](riemann-curvature-tensor.md#contracted-bianchi-identity). Full quantum Weyl invariance fixes the allowed $q^2$ through the [central charge](#central-charge), as in a [linear dilaton conformal field theory](#linear-dilaton-conformal-field-theory); the metric equation alone does not.

###### Exponentiated dilaton wave equation

↑ **Parent:** [Dilaton equation from contracted Bianchi identity](#dilaton-equation-from-contracted-bianchi-identity)

For the [dilaton equation from contracted Bianchi identity](#dilaton-equation-from-contracted-bianchi-identity), put $F=e^{-2\varphi}$. The chain rule gives $\Box_gF=F(-2\Box_g\varphi+4|\nabla\varphi|^2)=-2CF$. Thus the exponential obeys a linear [Klein-Gordon equation](wave-equation.md#klein-gordon-equation) on the given background, although the original [dilaton](string-theory.md#dilaton) equation is nonlinear and the [string-frame metric](#string-frame-metric) remains coupled to the [dilaton](string-theory.md#dilaton). With the opposite named-field convention $\varphi=-\Phi$, this variable is $F=e^{2\Phi}$.

##### Worldsheet Weyl anomaly

↑ **Parent:** [Sigma-model beta function](#sigma-model-beta-function)

A worldsheet Weyl anomaly is the quantum failure of the gauge-fixed string path integral to remain invariant under a [Weyl transformation](#weyl-transformation). Its local coefficients are the [sigma-model beta functions](#sigma-model-beta-function), while its constant part is controlled by the total [central charge](#central-charge).

###### Bosonic sigma-model Weyl anomaly coefficients

↑ **Parent:** [Worldsheet Weyl anomaly](#worldsheet-weyl-anomaly)

To first order in $\alpha'$, the conventional Euclidean [dilaton](string-theory.md#dilaton) coupling gives $\overline\beta^G_{\mu\nu}=\alpha'[R_{\mu\nu}-H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}/4+2\nabla_\mu\nabla_\nu\Phi]$ and $\overline\beta^B_{\mu\nu}=\alpha'[-\nabla^\rho H_{\rho\mu\nu}/2+(\nabla^\rho\Phi)H_{\rho\mu\nu}]$. The scalar coefficient is $(d-26)/6+\alpha'[(\nabla\Phi)^2-\nabla^2\Phi/2-H^2/24]$. Here $H$ is the [Kalb-Ramond field strength](#kalb-ramond-field-strength). Vanishing of these coefficients, including higher-order corrections, is the background-field condition for quantum [Weyl transformations](#weyl-transformation) to remain a gauge symmetry. The scalar coefficient includes the [central charge](#central-charge) deficit and is not implied by the metric equation alone.

### Worldsheet ghost field

↑ **Parent:** [Polyakov action](#polyakov-action)

Gauge fixing worldsheet diffeomorphism and Weyl symmetry introduces an anticommuting vector ghost $c^\alpha$ and a symmetric traceless antighost $b_{\alpha\beta}$. In complex coordinates they form holomorphic and antiholomorphic $bc$ systems.

#### Three-point worldsheet ghost correlator

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

On the [Riemann sphere](riemann-surfaces.md#riemann-sphere), three holomorphic reparameterization ghost zero modes correspond to the three infinitesimal [Möbius transformations](group-theory.md#mobius-transformation). Three $c$ insertions saturate their [Grassmann integral](supersymmetric-quantum-mechanics.md#berezin-integral). In a basis $1,z,z^2$, their integral is the Vandermonde determinant, giving $z_{12}z_{13}z_{23}$ up to an ordering-dependent sign. Including the antiholomorphic factor gives $|z_{12}z_{13}z_{23}|^2$, the Jacobian in [sphere gauge fixing for four string vertices](#sphere-gauge-fixing-for-four-string-vertices).

#### Ghost oscillator Virasoro generators

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

Contracting an antighost with the cubic [FP ghost](relativistic-quantum-field.md#faddeev-popov-ghost) term of the [BRST operator](#brst-operator) produces the bilinear generators. They give $[L_m,b_n]=(m-n)b_{m+n}$ and $[L_m,c_n]=-(2m+n)c_{m+n}$. Their zero-mode additive constant depends on the vacuum and [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) convention; it must agree with the corresponding $c_0$ term in the charge.

#### Ghost Virasoro zero-mode convention

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

With the [ghost oscillator vacuum](#ghost-oscillator-vacuum), one can define $L_0^{\mathrm{gh}}=\sum_{k>0}k(b_{-k}c_k+c_{-k}b_k)$ with vacuum eigenvalue zero. The corresponding [Virasoro algebra](#virasoro-algebra) contains a linear shift: $[L_m^{\mathrm{gh}},L_n^{\mathrm{gh}}]=(m-n)(L_{m+n}^{\mathrm{gh}}-\delta_{m+n,0})-\tfrac{26}{12}(m^3-m)\delta_{m+n,0}$. Shifting the zero mode by minus one removes the linear term but changes the stated vacuum eigenvalue. A [BRST charge](relativistic-quantum-field.md#brst-charge) must use a consistent choice throughout.

#### Ghost oscillator vacuum

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

For the anticommuting [bc system](#bc-system), $\{b_m,c_n\}=\delta_{m+n,0}$. A useful oscillator vacuum obeys $b_n|0\rangle=c_n|0\rangle=0$ for $n>0$ and $b_0|0\rangle=0$. Its partner $c_0|0\rangle$ is nonzero. This specifies a ghost zero-mode doublet and differs from imposing annihilation by both zero modes.

##### Ghost zero-mode pairing

↑ **Parent:** [Ghost oscillator vacuum](#ghost-oscillator-vacuum)

With Hermitian $b_0,c_0$ and $\{b_0,c_0\}=1$, a ket annihilated by $b_0$ has zero bare full-ghost norm. Nonzero amplitudes need [FP ghost](relativistic-quantum-field.md#faddeev-popov-ghost) zero-mode saturation. Low-level [Virasoro descendant](#virasoro-descendant) calculations can instead normalize the highest-weight coefficient and compute $L_nL_{-n}|\Omega\rangle$ algebraically. Such normalized contravariant coefficients are not positive-definite Hilbert norms. The pairing convention must be stated before using [FP ghost](relativistic-quantum-field.md#faddeev-popov-ghost) descendants in a norm argument.

#### BRST operator

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

The BRST operator is the Grassmann-odd conserved charge that combines a gauge transformation with its ghost field. Quantum gauge consistency requires $Q_B^2=0$, and physical states are its cohomology classes.

##### Virasoro closure from BRST nilpotence

↑ **Parent:** [BRST operator](#brst-operator)

If $L_m=\{b_m,Q\}$, nilpotence gives $[L_m,Q]=0$. The [graded Jacobi identity](lie-algebra.md#graded-jacobi-identity) and $[b_m,L_n]=(m-n)b_{m+n}$ then imply the displayed algebra. Thus a quantum central extension in the total generators obstructs [BRST nilpotence](relativistic-quantum-field.md#brst-nilpotence).

##### BRST physical-state constraints of an open string

↑ **Parent:** [BRST operator](#brst-operator)

For a matter state tensored with the [ghost oscillator vacuum](#ghost-oscillator-vacuum), the [BRST charge](relativistic-quantum-field.md#brst-charge) produces the independent ghost states $c_0|0\rangle$ and $c_{-m}|0\rangle$ with coefficients $(L_0-1)|\Psi\rangle$ and $L_m|\Psi\rangle$. Thus BRST closure is equivalent to $(L_0-1)|\Psi\rangle=0$ and $L_{m>0}|\Psi\rangle=0$ in this sector. It reproduces [old covariant string quantization](#old-covariant-string-quantization) and the [open bosonic string mass spectrum](#open-bosonic-string-mass-spectrum).

##### BRST current

↑ **Parent:** [BRST operator](#brst-operator)

The BRST current is the conserved worldsheet current whose contour integral is the [BRST operator](#brst-operator). For the bosonic string it is built from the reparameterization ghost and the matter and ghost stress tensors; its self-OPE is nonsingular only when the total central charge vanishes.

#### Worldsheet ghost action

↑ **Parent:** [Worldsheet ghost field](#worldsheet-ghost-field)

For the traceless diffeomorphism operator

$$
(P_1c)_{\alpha\beta}=\nabla_\alpha c_\beta+\nabla_\beta c_\alpha-g_{\alpha\beta}\nabla_\gamma c^\gamma,
$$

the ghost action is

$$
S_{\rm gh}=\frac1{2\pi}\int d^2\sigma\,\sqrt g\,
b^{\alpha\beta}(P_1c)_{\alpha\beta}.
$$

##### Chiral conformal-gauge BRST nilpotence is on shell

↑ **Parent:** [Worldsheet ghost action](#worldsheet-ghost-action)

In [conformal gauge](#conformal-gauge), let the odd [left-acting BRST differential](relativistic-quantum-field.md#left-acting-brst-differential) act by $sX=c^+\partial_+X+c^-\partial_-X$ and $sc^\pm=c^\pm\partial_\pm c^\pm$. The [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) gives the displayed expression for $s^2X$. It vanishes using the ghost [equations of motion](classical-mechanics.md#equation-of-motion) $\partial_-c^+=\partial_+c^-=0$, but it is not zero for arbitrary off-shell fields. For independent [Grassmann variables](multilinear-algebra.md#grassmann-variable) $\xi,\rho$, take $c^+=\xi$, $c^-=\rho\sigma^+$ and $X=\sigma^-$; then $s^2X=-\xi\rho\ne0$. Each ghost itself satisfies $s^2c^\pm=0$ algebraically. With the eliminated-antighost transformation $sb_{\pm\pm}=i\theta_{\pm\pm}/\alpha'$ and $s\theta_{\pm\pm}=0$ on the solution space, the antighosts are nilpotent too. This on-shell closure is compatible with an off-shell total-derivative variation of the gauge-fixed action. A full off-shell [BRST quantization](relativistic-quantum-field.md#brst-quantization) uses the complete gauge transformation and, where required, auxiliary fields rather than silently dropping mixed ghost derivatives.

##### Trace elimination in string Faddeev-Popov gauge fixing

↑ **Parent:** [Worldsheet ghost action](#worldsheet-ghost-action)

In two dimensions the metric variation splits into a scalar trace and the trace-free diffeomorphism operator $(P_1v)_{ab}=\nabla_av_b+\nabla_bv_a-g_{ab}\nabla\cdot v$. Integrating the Weyl parameter in the inverse [Faddeev-Popov determinant](relativistic-quantum-field.md#faddeev-popov-determinant) removes the trace delta function. The remaining determinant is exponentiated by an anticommuting vector ghost and symmetric trace-free antighost, yielding the two chiral $b\bar\partial c$ terms. Conformal Killing vectors and moduli are zero modes treated separately from this local determinant.

##### Worldsheet diffeomorphism ghost operator

↑ **Parent:** [Worldsheet ghost action](#worldsheet-ghost-action)

The [trace](linear-algebra.md#matrix-trace)-free metric variation is $(P_1c)_{ab}=\nabla_ac_b+\nabla_bc_a-\gamma_{ab}\nabla_dc^d$. A symmetric [trace](linear-algebra.md#matrix-trace)-free antighost exponentiates the [Faddeev-Popov determinant](relativistic-quantum-field.md#faddeev-popov-determinant). In light-cone worldsheet coordinates its two chiral kinetic terms are $b_{++}\partial_-c^+$ and $b_{--}\partial_+c^-$.

###### Formal adjoint of the worldsheet conformal Killing operator

↑ **Parent:** [Worldsheet diffeomorphism ghost operator](#worldsheet-diffeomorphism-ghost-operator)

Use the half-normalized operator $(P_1v)_{ab}=(\nabla_av_b+\nabla_bv_a-h_{ab}\nabla_cv^c)/2$. On a closed [worldsheet](#worldsheet), a symmetric trace-free tensor obeys

$$
\int\sqrt h\,t^{ab}(P_1v)_{ab}=-\int\sqrt h\,(\nabla_at^{ab})v_b.
$$

This [integration by parts](calculus.md#integration-by-parts) identifies the displayed formal [adjoint operator](hilbert-space.md#adjoint-operator). A convention with twice $P_1$ has twice this adjoint, with identical kernels. The [worldsheet conformal Killing group](#worldsheet-conformal-killing-group) corresponds to the kernel of $P_1$, while [infinitesimal worldsheet moduli](#infinitesimal-worldsheet-modulus) correspond to the trace-free kernel of its adjoint.

## Worldsheet

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Worldsheet)

A string worldsheet $\Sigma$ is the two-dimensional surface swept out by a string in spacetime. Local coordinates are commonly denoted $\sigma^\alpha=(\tau,\sigma)$.

### Winding-supported circular string

↑ **Parent:** [Worldsheet](#worldsheet)

In flat noncompact spacetime a fixed circular loop's cylindrical worldsheet is not a stationary point of the [Nambu–Goto action](#nambu-goto-action). A compact coordinate changes the possibilities. The displayed embedding in $\mathbb R^{2,1}\times S^1_R$ has unit winding, satisfies the [wave equation](wave-equation.md), and obeys $\dot X\cdot X'=0$ and $\dot X^2+X'^2=0$. Its projection is a circle with static shape, while its motion in the compact direction supplies the second chiral null tangent. The [induced worldsheet metric](#induced-worldsheet-metric) is $2R^2\operatorname{diag}(-1,1)$, so the full worldsheet is nondegenerate.

### Proper length of a string

↑ **Parent:** [Worldsheet](#worldsheet)

On a spacelike constant-target-time slice, integrate the induced spatial line element to obtain the geometric string length. It depends on the embedding and is distinct from the fundamental [string length](#string-length) $\ell_s=\sqrt{\alpha'}$. For transverse local motion, energy additionally includes the local Lorentz factor; the geometric length alone does not determine the total energy.

### Worldsheet metric

↑ **Parent:** [Worldsheet](#worldsheet)

The intrinsic Lorentzian metric in the [Polyakov action](#polyakov-action) is independent of the [string embedding map](#string-embedding-map). Its equation relates it conformally to the [induced worldsheet metric](#induced-worldsheet-metric). A [Weyl transformation](#weyl-transformation) changes the intrinsic metric without changing the classical action.

### Worldsheet area

↑ **Parent:** [Worldsheet](#worldsheet)

The area of a [string worldsheet](#worldsheet) is computed from its [induced worldsheet metric](#induced-worldsheet-metric). The [Nambu–Goto action](#nambu-goto-action) is minus [string tension](#string-tension) times Lorentzian worldsheet area.

### String embedding map

↑ **Parent:** [Worldsheet](#worldsheet)

The string embedding map $X:\Sigma\to\mathcal M$ assigns each worldsheet point its position in target spacetime.

#### Worldsheet zero mode

↑ **Parent:** [String embedding map](#string-embedding-map)

A worldsheet zero mode is a field component annihilated by the worldsheet kinetic operator. For a noncompact string embedding coordinate, its constant zero mode is the target-space center-of-mass position; integrating over it enforces target-space momentum conservation.

#### Induced worldsheet metric

↑ **Parent:** [String embedding map](#string-embedding-map)

The induced worldsheet metric is the pullback of the target-space metric:

$$
\gamma_{\alpha\beta}=\partial_\alpha X^\mu\partial_\beta X^\nu\eta_{\mu\nu}.
$$

<h5 id="nambu-goto-action">Nambu–Goto action</h5>

↑ **Parent:** [Induced worldsheet metric](#induced-worldsheet-metric)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nambu–Goto_action)

The Nambu–Goto action

$$
S_{\rm NG}=-T\int_\Sigma d^2\sigma\,\sqrt{-\det\gamma}
$$

is minus the string tension times the Lorentzian area of the worldsheet.

###### Pulsating circular string

↑ **Parent:** [Nambu–Goto action](#nambu-goto-action)

A circular [closed string](#closed-string) contracts and re-expands with $X^0=Rt$ and $X^1+iX^2=R\cos t\,e^{i\sigma}$. Its [proper length](special-relativity.md#proper-length) is $2\pi R|\cos t|$, while its [energy](energy.md) remains $2\pi TR$. At collapse the [induced worldsheet metric](#induced-worldsheet-metric) degenerates, but the [Nambu-Goto phase-space action](#nambu-goto-phase-space-action) supplies a regular continuation.

<h6 id="nambu-goto-equations-of-motion">Nambu–Goto equations of motion</h6>

↑ **Parent:** [Nambu–Goto action](#nambu-goto-action)

For a nondegenerate [induced worldsheet metric](#induced-worldsheet-metric) $g_{ab}=\partial_aX\cdot\partial_bX$, variation gives $\partial_a(\sqrt{-g}\,g^{ab}\partial_bX^m)=0$. In [conformal gauge](#conformal-gauge) this is the two-dimensional [wave equation](wave-equation.md), supplemented by the [Virasoro constraints](#virasoro-constraint).

###### Nambu-Goto phase-space action

↑ **Parent:** [Nambu–Goto action](#nambu-goto-action)

The first-order string action is

$$
I=\int dt\,d\sigma\left[\dot X\cdot P-\frac e2(P^2+T^2X'^2)-uX'\cdot P\right].
$$

The multipliers impose the two [Virasoro constraints](#virasoro-constraint). The canonical equations give a spatial momentum flux $J_m=eT^2X'_m+uP_m$.

###### Target-space Noether charges of a string

↑ **Parent:** [Nambu-Goto phase-space action](#nambu-goto-phase-space-action)

Translations and [Lorentz transformations](special-relativity.md#lorentz-transformation) give [Noether charges](classical-field-theory.md#noether-charge) $\mathcal P_m=\int P_m\,d\sigma$ and $\mathcal J_{mn}=\int(X_mP_n-X_nP_m)\,d\sigma$. Their time derivatives are boundary fluxes, which vanish for a [closed string](#closed-string) or a free-ended [open string](#open-string).

<h6 id="nambu-goto-phase-space-constraints">Nambu–Goto phase-space constraints</h6>

↑ **Parent:** [Nambu-Goto phase-space action](#nambu-goto-phase-space-action)

The two constraints are $P^2+T^2X'^2=0$ and $P\cdot X'=0$. They are [first-class constraints](classical-mechanics.md#first-class-constraint) associated with [worldsheet diffeomorphisms](#worldsheet-diffeomorphism). Their [Lagrange multipliers](mathematical-optimization.md#lagrange-multiplier) are arbitrary gauge functions rather than propagating fields.

###### Chiral constraint algebra of a closed string

↑ **Parent:** [Nambu–Goto phase-space constraints](#nambu-goto-phase-space-constraints)

For a [closed string](#closed-string), the currents $J_\pm=P\pm TX'$ have vanishing mixed [Poisson brackets](hamiltonian-mechanics.md#poisson-bracket). The densities $\mathcal H_\pm=J_\pm^2/(4T)$ therefore generate commuting constraint algebras. With opposite Fourier orientations their modes satisfy $\{L_m,L_n\}=-i(m-n)L_{m+n}$ and the identical relation for $\widetilde L_n$. This is a [direct sum of Lie algebras](lie-algebra.md#direct-sum-of-lie-algebras) consisting of two [Witt algebras](lie-algebra.md#witt-algebra).

<h6 id="rotating-nambu-goto-string">Rotating Nambu–Goto string</h6>

↑ **Parent:** [Nambu–Goto action](#nambu-goto-action)

A straight rigidly rotating classical string has [speed of light](special-relativity.md#speed-of-light) at a free endpoint. Its [energy](energy.md) and [angular momentum](momentum.md#angular-momentum) satisfy a [Regge trajectory](#regge-trajectory). A segment with one anchored and one free end has $J=E^2/(\pi T)$, twice the slope of the string with two free ends.

###### Free-ended straight-string Regge relation

↑ **Parent:** [Rotating Nambu–Goto string](#rotating-nambu-goto-string)

With [string tension](#string-tension) $T=1/(2\pi\alpha')$, the free-ended [open string](#open-string) $X^0=a\tau$, $X^1+iX^2=a\cos\sigma\,e^{i\tau}$, $0\leq\sigma\leq\pi$, is straight at every target time. Its [Nambu–Goto equations of motion](#nambu-goto-equations-of-motion) and [Virasoro constraints](#virasoro-constraint) hold, and its ends move at light speed. Integrating the [target-space Noether charges of a string](#target-space-noether-charges-of-a-string) gives $M=\pi Ta$ and $J=\pi Ta^2/2$. Thus $J=\alpha'M^2$. Extending the same map to $0\leq\sigma\leq2\pi$ describes a double-covered folded [closed string](#closed-string), with twice the mass and twice the [angular momentum](momentum.md#angular-momentum), hence $J=\alpha'M^2/2$. The different slopes record the different boundary topology.

###### Rigid circular string in four spatial dimensions

↑ **Parent:** [Rotating Nambu–Goto string](#rotating-nambu-goto-string)

If $A(t)$ and $B(t)$ are perpendicular four-dimensional spatial vectors of equal fixed magnitude, every constant-time slice is a planar circle. Opposite rotations in two orthogonal coordinate planes can produce a [Nambu–Goto action](#nambu-goto-action) solution with constant radius and a rotating plane. The [induced worldsheet metric](#induced-worldsheet-metric) can be constant even though the embedding moves. Rotating Cartesian axes clarify its shape without removing its kinetic target-space energy.

###### Straight rotating string with one fixed endpoint

↑ **Parent:** [Rotating Nambu–Goto string](#rotating-nambu-goto-string)

A [Nambu–Goto action](#nambu-goto-action) solution with $X^0=t$ is $\boldsymbol X=L\sin(\sigma/L)(\cos(t/L),\sin(t/L))$, for $0\leq\sigma\leq\pi L/2$. It solves the [wave equation](wave-equation.md), has a fixed endpoint at the origin, and obeys the [free-end string boundary condition](#free-end-string-boundary-condition) at the other end. Its [proper length](special-relativity.md#proper-length) is $L$ and its free endpoint has angular speed $1/L$ and spatial speed one.

### Two-dimensional conformal field theory

↑ **Parent:** [Worldsheet](#worldsheet)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Two-dimensional_conformal_field_theory)

A two-dimensional conformal field theory is invariant under local holomorphic and antiholomorphic conformal transformations.

#### Global conformal Ward identities for chiral correlators

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

For [primary operators](#primary-field) of holomorphic weights $h_i$ and a [Möbius transformation](group-theory.md#mobius-transformation) invariant vacuum, infinitesimal translations, dilations and special conformal transformations give $\sum_i\partial_iG=0$, $\sum_i(z_i\partial_i+h_i)G=0$, and $\sum_i(z_i^2\partial_i+2h_i z_i)G=0$. Solving gives a constant one-point function only at $h=0$, a two-point function $Cz_{12}^{-2h}$ only for equal weights, and a three-point function $Cz_{12}^{h_3-h_1-h_2}z_{13}^{h_2-h_1-h_3}z_{23}^{h_1-h_2-h_3}$. Three-point covariance imposes no further equality of weights; dynamical selection rules may still force $C=0$. For more points, arbitrary functions of [conformal cross-ratios](string-theory.md#conformal-cross-ratio) remain.

#### Liouville field theory

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Liouville_field_theory)

[Liouville field theory](#liouville-field-theory) is a two-dimensional scalar theory with a curvature background charge and an exponential interaction. In the usual spacelike normalization, quantum conformal invariance gives $Q=b+b^{-1}$ and [central charge](#central-charge) $c_L=1+6Q^2$. When a noncritical [string worldsheet](#worldsheet) conformal factor is retained as a dynamical field, its effective action has this form and its [central charge](#central-charge) combines with the matter and [worldsheet ghost field](#worldsheet-ghost-field) charges. It is closely related to a [background-charge scalar field](#background-charge-scalar-field), but its exponential potential supplies an additional interaction.

#### Radial quantization

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

[Radial quantization](#radial-quantization) treats circles around the origin as equal-time slices and logarithmic radius as Euclidean time. A local insertion at the origin prepares a state on a surrounding circle. Contours of the stress tensor act on that insertion, turning its singular [operator product expansion](#operator-product-expansion) into the [Virasoro algebra](#virasoro-algebra) action on the corresponding state.

#### Quasi-primary operator

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

A [quasi-primary operator](#quasi-primary-operator) transforms with weights $(h,\widetilde h)$ under global conformal, or Möbius, transformations. A [primary operator](#primary-field) has this covariance under every locally invertible holomorphic and antiholomorphic coordinate change. In [radial quantization](#radial-quantization), quasi-primary states are annihilated by $L_1,\widetilde L_1$, whereas [primary states](#primary-state) are annihilated by every positive Virasoro mode. The stress tensor at nonzero [central charge](#central-charge) is quasi-primary but not primary because its transformation under a general coordinate change includes a Schwarzian term.

#### Free chiral Majorana fermion conformal field theory

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

A real chiral [Majorana fermion](relativistic-quantum-field.md#majorana-spinor) with contraction $\psi(z)\psi(w)\sim1/(z-w)$ has stress tensor $T=-:\psi\partial\psi:/2$. Fermionic [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) give $T(z)\psi(w)\sim\psi(w)/(2(z-w)^2)+\partial\psi(w)/(z-w)$. Double contractions in $TT$ give $1/(4(z-w)^4)$, so the [central charge](#central-charge) is $1/2$. Fermion bilinears of different species are weight-one currents; equal-species undifferentiated bilinears vanish by antisymmetry.

##### Ising Virasoro modules from a Majorana fermion

↑ **Parent:** [Free chiral Majorana fermion conformal field theory](#free-chiral-majorana-fermion-conformal-field-theory)

A chiral [Majorana fermion](relativistic-quantum-field.md#majorana-spinor) with modes $\{b_r,b_s\}=\delta_{r+s,0}$ and $b_r^\dagger=b_{-r}$ has $T=-:\psi\partial\psi:/2$ and [central charge](#central-charge) $1/2$. The even and odd fermion-number parts of its [Neveu–Schwarz sector](string-theory.md#neveu-schwarz-sector) give unitary modules with lowest weights $0$ and $1/2$. In its [Ramond sector](string-theory.md#ramond-sector), a choice of ground-state zero-mode eigenvalue gives the module of weight $1/16$; the other choice gives an isomorphic [Virasoro algebra](#virasoro-algebra) module. Their cyclic highest-weight submodules are irreducible: a positive-energy invariant proper submodule would have a lowest vector orthogonal to every descendant of the original highest vector, which is impossible in a positive inner-product cyclic module.

#### Beta-gamma system

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

A beta-gamma system is a pair of commuting chiral fields with first-order action $\int\beta\bar\partial\gamma$. If $\gamma$ has weight $h$ and $\beta$ has weight $1-h$, its central charge is $2(6h^2-6h+1)$.

##### Stress tensor of a commuting beta-gamma system

↑ **Parent:** [Beta-gamma system](#beta-gamma-system)

Using the [radial-ordering sign in commuting beta-gamma contractions](#radial-ordering-sign-in-commuting-beta-gamma-contractions), single contractions give $T(z)\beta(w)\sim\lambda\beta(w)/(z-w)^2+\partial\beta(w)/(z-w)$ and the corresponding weight $1-\lambda$ for $\gamma$. Put $A=:\partial\beta\,\gamma:$ and $B=:\beta\,\partial\gamma:$. Their double-contraction coefficients in $AA,BB,AB,BA$ are respectively $1,1,2,2$. The fourth-order pole of $TT$ is therefore $(1-\lambda)^2+\lambda^2-4\lambda(1-\lambda)=6\lambda^2-6\lambda+1$, which equals $c/2$. There is no anticommuting Wick sign.

##### Radial-ordering sign in commuting beta-gamma contractions

↑ **Parent:** [Beta-gamma system](#beta-gamma-system)

Commutation allows exchanging the factors at their existing arguments; it does not allow exchanging their arguments while retaining the same pole sign. With the displayed convention, differentiation produces $\partial\beta(z)\gamma(w)\sim(z-w)^{-2}$ and $\partial\gamma(z)\beta(w)\sim-(z-w)^{-2}$. These signs are essential for the [conformal weights](#conformal-weight) and [central charge](#central-charge) of a commuting [beta-gamma system](#beta-gamma-system).

#### bc system

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

A bc system is the anticommuting counterpart of a [beta-gamma system](#beta-gamma-system). For weights $h$ and $1-h$, its central charge is $-2(6h^2-6h+1)$.

##### Central charge of reparameterization ghosts

↑ **Parent:** [bc system](#bc-system)

The [worldsheet ghost fields](#worldsheet-ghost-field) form a [bc system](#bc-system) with [conformal weights](#conformal-weight) $2$ and $-1$. Setting $J=2$ in $c=-2(6J^2-6J+1)$ gives [central charge](#central-charge) $-26$ in each chirality. The [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) of $D$ free embedding bosons cancels at $D=26$.

##### bc ghost operator-product expansion

↑ **Parent:** [bc system](#bc-system)

For reparameterization ghosts of weights two and minus one, the canonical anticommutators imply $b(z)c(w)\sim1/(z-w)$. This operator-product expansion fixes the ghost contractions and the ghost stress tensor.

#### Primary field

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primary_field)

A primary operator of weights $(h,\widetilde h)$ transforms covariantly under local conformal maps and has a universal operator-product expansion with the stress-energy tensor.

##### Primary state

↑ **Parent:** [Primary field](#primary-field)

A [primary state](#primary-state) is a simultaneous eigenvector of $L_0,\widetilde L_0$ with eigenvalues $h,\widetilde h$ that is annihilated by all positive modes of both [Virasoro algebras](#virasoro-algebra). Negative modes generate descendants. The [state–operator correspondence](string-theory.md#state-operator-correspondence) identifies it with a [primary operator](#primary-field) inserted at the origin.

##### Transversality of derivative-exponential primary vertices

↑ **Parent:** [Primary field](#primary-field)

For free embedding bosons, the [operator product expansion](#operator-product-expansion) of the stress tensor with $\zeta_\mu:\partial X^\mu e^{ipX}:$ has a cubic pole $-i\alpha'(p\cdot\zeta):e^{ipX}:/2$. Its vanishing is precisely the primary condition, with weight $1+\alpha'p^2/4$. The two-derivative closed-string vertex has the two displayed transversality conditions from its holomorphic and antiholomorphic cubic poles. Being primary does not require $p^2=0$; that extra condition follows when a physical integrated vertex must have [conformal weights](#conformal-weight) $(1,1)$.

##### Conformal weight

↑ **Parent:** [Primary field](#primary-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conformal_weight)

The conformal weights determine the response of a primary operator to holomorphic and antiholomorphic coordinate rescaling. Its scaling dimension is $\Delta=h+\widetilde h$ and its spin is $h-\widetilde h$.

##### Virasoro descendant

↑ **Parent:** [Primary field](#primary-field)

A Virasoro descendant is obtained by applying negative Virasoro modes $L_{-n}$ to a primary state or operator. Its level is the sum of the mode numbers.

#### Operator product expansion

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operator_product_expansion)

An operator product expansion expresses the short-distance product of local operators as a sum of local operators multiplied by singular coefficient functions.

#### Holomorphic stress-energy tensor

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

The holomorphic stress-energy tensor generates infinitesimal holomorphic conformal transformations through its operator product expansions.

##### Stress-tensor operator-product expansion

↑ **Parent:** [Holomorphic stress-energy tensor](#holomorphic-stress-energy-tensor)

In a two-dimensional conformal field theory,

$$
T(z)T(w)\sim\frac{c/2}{(z-w)^4}+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}.
$$

The fourth-order pole is the central extension, while the remaining poles express that $T$ has conformal weight two.

##### Virasoro algebra

↑ **Parent:** [Holomorphic stress-energy tensor](#holomorphic-stress-energy-tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virasoro_algebra)

The Virasoro algebra is the central extension of the algebra of holomorphic vector fields on a circle. Its generators are the Laurent modes of the holomorphic stress-energy tensor, and its central term is controlled by the [central charge](#central-charge) $c$.

###### Virasoro character

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

A [Virasoro character](#virasoro-character) records the graded dimensions of a positive-energy [Virasoro algebra](#virasoro-algebra) module. A state of weight $h+N$ contributes $q^{h+N-c/24}$, and its multiplicity is the dimension of that energy eigenspace. The shift accounts for the [Casimir energy of a two-dimensional conformal field theory](string-theory.md#casimir-energy-of-a-two-dimensional-conformal-field-theory). For a [Virasoro Verma module](#virasoro-verma-module), the character is $q^{h-c/24}\prod_{n\ge1}(1-q^n)^{-1}$, by counting the ordered descendant basis.

###### Virasoro Verma module

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

The [Virasoro Verma module](#virasoro-verma-module) $M(c,h)$ is the universal [highest-weight representation](semisimple-lie-algebra.md#highest-weight-representation) with [central charge](#central-charge) $c$ and ground weight $h$. The [Poincaré-Birkhoff-Witt theorem](lie-algebra.md#poincare-birkhoff-witt-theorem) gives a basis $L_{-n_1}\cdots L_{-n_s}|h\rangle$ with $n_1\ge\cdots\ge n_s>0$. Its invariant Hermitian form is fixed by $L_n^\dagger=L_{-n}$ and the norm of the ground vector. Quotienting by its maximal proper submodule produces the irreducible highest-weight module; in the unitary cases this removes the null vectors.

###### Level-two Virasoro descendant Gram matrix

↑ **Parent:** [Virasoro Verma module](#virasoro-verma-module)

For a normalized [highest-weight vector](semisimple-lie-algebra.md#highest-weight-vector) with $L_0|h\rangle=h|h\rangle$, $L_{n>0}|h\rangle=0$ and $L_n^\dagger=L_{-n}$, the level-two descendants $L_{-2}|h\rangle,L_{-1}^2|h\rangle$ have the displayed [Gram matrix](inner-product.md#gram-matrix). It follows from the [Virasoro algebra](#virasoro-algebra): $\langle L_2L_{-2}\rangle=4h+c/2$, $\langle L_2L_{-1}^2\rangle=6h$ and $\langle L_1^2L_{-1}^2\rangle=4h(2h+1)$. At $h=-1,c=26$ its null direction is $(1,3/2)$, giving the [level-two scalar Virasoro null state](#level-two-scalar-virasoro-null-state). Nullity of a descendant is a metric statement; satisfying all physical constraints must be checked separately.

###### Unitary highest-weight Virasoro module

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

A [unitary highest-weight Virasoro module](#unitary-highest-weight-virasoro-module) is generated by a normalized vector satisfying the displayed relations, with a positive-definite [inner product](inner-product.md) and $L_n^\dagger=L_{-n}$. Its [Virasoro descendants](#virasoro-descendant) have $L_0$ eigenvalues $h+N$ for nonnegative integral levels $N$. The commutator gives $\|L_{-1}|h\rangle\|^2=2h$, so unitarity requires $h\ge0$. Such a module is a quotient of a [Virasoro Verma module](#virasoro-verma-module); its [Unitary Virasoro discrete series](#unitary-virasoro-discrete-series) describes the cases with [central charge](#central-charge) below one.

###### Sugawara construction

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sugawara_construction)

For a restricted representation of an affine current algebra with $[J_m^a,J_n^b]=if^{abc}J_{m+n}^c+km\delta^{ab}\delta_{m+n,0}$ and $f^{abc}f^{abd}=Q\delta^{cd}$, the displayed [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) construction is defined when $2k+Q\ne0$. Moving the currents past each other gives $[L_m,J_n^a]=-nJ_{m+n}^a$; the additional $Q$ in the denominator is the adjoint-Casimir reordering term. The resulting [Virasoro algebra](#virasoro-algebra) has [central charge](#central-charge) $c=k\dim\mathfrak g/(k+Q/2)$. On a compact unitary positive-energy module, $L_m^\dagger=L_{-m}$.

###### Coset construction

↑ **Parent:** [Sugawara construction](#sugawara-construction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset_construction)

For a current subalgebra $\mathfrak h\subset\mathfrak g$, its currents have conformal weight one under both [Sugawara construction](#sugawara-construction) stress tensors. Their difference therefore commutes with all $\mathfrak h$ currents and with the $\mathfrak h$ stress tensor. It obeys the [Virasoro algebra](#virasoro-algebra) with [central charge](#central-charge) $c_{\mathfrak g}-c_{\mathfrak h}$. For a positive-level compact unitary vacuum representation, $\|L_{-2}^{\mathfrak g/\mathfrak h}|0\rangle\|^2=(c_{\mathfrak g}-c_{\mathfrak h})/2\ge0$. A [Cartan subalgebra](semisimple-lie-algebra.md#cartan-subalgebra) has $c_{\mathfrak h}=\operatorname{rank}\mathfrak g$, giving the lower bound on $c_{\mathfrak g}$ under these hypotheses.

###### Unitary Virasoro discrete series

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

An irreducible unitary [highest weight](semisimple-lie-algebra.md#highest-weight-of-a-representation) module of the [Virasoro algebra](#virasoro-algebra) with $c<1$ has integer $m\ge2$, $1\le r\le m-1$, $1\le s\le m$, and the displayed weights. Labels $(r,s)$ and $(m-r,m+1-s)$ represent the same module. It is obtained from the [Verma module](semisimple-lie-algebra.md#verma-module) by quotienting its zero-norm submodules; the two generating singular-vector levels are $rs$ and $(m-r)(m+1-s)$. For $m=2$ this is the trivial $c=h=0$ module. For $m=3$, the three weights are $0$, $1/2$, $1/16$.

###### Virasoro generator

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

[Virasoro generators](#virasoro-generator) are the contour modes of the holomorphic stress tensor in a [two-dimensional conformal field theory](#two-dimensional-conformal-field-theory). Their commutators are $[L_m,L_n]=(m-n)L_{m+n}+c(m^3-m)\delta_{m+n,0}/12$. A contour around an operator insertion extracts the corresponding coefficient of its stress-tensor [operator product expansion](#operator-product-expansion). $L_{-1}$ generates translations, $L_0$ measures holomorphic weight, and all positive generators annihilate a [primary state](#primary-state). An independent antiholomorphic copy acts on the other weight.

###### Virasoro zero-mode shift

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

Shifting the zero mode changes the algebra's central representative:

$$
[\mathcal L_m,\mathcal L_n]=(m-n)\mathcal L_{m+n}
+\left(\frac c{12}m(m^2-1)+2am\right)\delta_{m+n,0}.
$$

The linear term follows from replacing $L_{m+n}$ by $\mathcal L_{m+n}+a\delta_{m+n,0}$. It changes the zero-mode convention, not the cubic coefficient or [central charge](#central-charge). This distinction separates the intercept from the [Virasoro central extension](#virasoro-central-extension).

###### Virasoro central extension

↑ **Parent:** [Virasoro algebra](#virasoro-algebra)

The Virasoro central extension is the term $c(m^3-m)\delta_{m+n,0}/12$ in $[L_m,L_n]$. It records the conformal anomaly and commutes with every Virasoro generator.

###### Free-boson Virasoro central term

↑ **Parent:** [Virasoro central extension](#virasoro-central-extension)

For $d$ free target coordinates, [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) of $L_m=\sum_n:\alpha_{m-n}\cdot\alpha_n:/2$ gives a matter [central charge](#central-charge) $d$. On the formal zero-momentum vacuum, the double contractions yield $\langle L_mL_{-m}\rangle=(d/2)\sum_{r=1}^{m-1}r(m-r)=d(m^3-m)/12$. Two target-metric contractions give $\eta_{ab}\eta^{ab}=d$, so timelike target coordinates do not subtract from this [central charge](#central-charge). Transverse-only and covariant generators must not be confused.

##### Central charge

↑ **Parent:** [Holomorphic stress-energy tensor](#holomorphic-stress-energy-tensor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_charge)

The central charge is the coefficient of the fourth-order pole in the stress-tensor operator-product expansion, $T(z)T(w)\sim c/[2(z-w)^4]+\cdots$. A free real boson contributes one and a free real chiral fermion contributes one half.

###### Superconformal current

↑ **Parent:** [Central charge](#central-charge)

In a two-dimensional supersymmetric conformal field theory, the superconformal current has weight $3/2$ and its self-OPE closes on the stress tensor and the [central charge](#central-charge).

###### Canonical supercurrent bracket of free RNS matter

↑ **Parent:** [Superconformal current](#superconformal-current)

For [RNS string](string-theory.md#spinning-string) matter normalized by $[\dot X^\mu(\sigma),X^\nu(\sigma')]=-i\pi\eta^{\mu\nu}\delta(\sigma-\sigma')$ and $\{\psi_1^\mu(\sigma),\psi_1^\nu(\sigma')\}=\pi\eta^{\mu\nu}\delta(\sigma-\sigma')$, put $A=\partial_+X$ and $J=\psi_1\cdot A$. Then $[A^\mu(\sigma),A^\nu(\sigma')]=(i\pi/2)\eta^{\mu\nu}\partial_\sigma\delta(\sigma-\sigma')$. The noncentral part of $\{J(\sigma),J(\sigma')\}$ is $\pi\delta A^2+(i\pi/2)\partial_\sigma\delta\,\psi_1(\sigma)\cdot\psi_1(\sigma')$. The [distributional derivative](distribution-theory.md#distributional-derivative) identity $f(\sigma,\sigma')\delta'=f(\sigma,\sigma)\delta'+(\partial_{\sigma'}f)(\sigma,\sigma)\delta$, with a vanishing coincident Grassmann bilinear, converts this to $\pi\delta\theta_{++}$. Use the chiral [equation of motion](classical-mechanics.md#equation-of-motion) to identify $\partial_\sigma\psi_1=\partial_+\psi_1$. Quantum [normal ordering](perturbative-quantum-field-theory.md#normal-ordering) adds a central contact term proportional to $\delta''$, the local form of the [N=1 super-Virasoro algebra](#n-1-super-virasoro-algebra) central extension.

<h6 id="n-1-super-virasoro-algebra">N=1 super-Virasoro algebra</h6>

↑ **Parent:** [Superconformal current](#superconformal-current)

The holomorphic N=1 super-Virasoro algebra extends the Virasoro algebra by fermionic modes $G_r$ satisfying $\{G_r,G_s\}=2L_{r+s}+(c/12)(4r^2-1)\delta_{r,-s}$.

###### Ramond supercurrent zero-mode square

↑ **Parent:** [N=1 super-Virasoro algebra](#n-1-super-virasoro-algebra)

With the standard [string oscillator](#string-oscillator) algebra and $G_0=\sum_m\alpha_m\cdot\psi_{-m}$, pairing positive and negative modes gives $G_0^2=\alpha_0^2/2+\sum_{m>0}(\alpha_{-m}\cdot\alpha_m+m\psi_{-m}\cdot\psi_m)$. This is the vacuum-normal-ordered [Ramond sector](string-theory.md#ramond-sector) generator $L_0^R$, so $\{G_0,G_0\}=2L_0^R$. Rescaling the [superconformal current](#superconformal-current) rescales its square quadratically; its normalization cannot be ignored when comparing it with a fixed [Virasoro generator](#virasoro-generator).

#### Free boson conformal field theory

↑ **Parent:** [Two-dimensional conformal field theory](#two-dimensional-conformal-field-theory)

The free boson conformal field theory has action quadratic in a scalar $X$ and central charge one. Its oscillator partition function is expressed through the [Dedekind eta function](#dedekind-eta-function).

##### Free-boson worldsheet propagator

↑ **Parent:** [Free boson conformal field theory](#free-boson-conformal-field-theory)

For the normalization $S=(2\pi\alpha')^{-1}\int d^2z\,\partial X\bar\partial X$, the free-boson worldsheet propagator has singular part

$$
X^\mu(z,\bar z)X^\nu(w,\bar w)\sim-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2.
$$

Differentiation gives the singular operator-product expansions of the embedding currents.

##### Linear dilaton conformal field theory

↑ **Parent:** [Free boson conformal field theory](#free-boson-conformal-field-theory)

A linear dilaton conformal field theory improves the free-boson stress tensor by a second derivative, $T=-\alpha'^{-1}:\!\partial X\partial X\!:-q\partial^2X$. The improvement shifts the [central charge](#central-charge) to $c=1+6\alpha'q^2$ and corresponds to a dilaton linear in the target coordinate $X$.

###### Background-charge scalar field

↑ **Parent:** [Linear dilaton conformal field theory](#linear-dilaton-conformal-field-theory)

A background-charge scalar field is a free scalar coupled linearly to the worldsheet Ricci scalar. This curvature coupling produces the improved stress tensor of a [linear dilaton conformal field theory](#linear-dilaton-conformal-field-theory).

##### Torus partition function of a free boson

↑ **Parent:** [Free boson conformal field theory](#free-boson-conformal-field-theory)

For a noncompact free boson with target volume $V$, the torus partition function is $Z=V[2\pi\sqrt{\operatorname{Im}\tau}]^{-1}|\eta(\tau)|^{-2}$ in the normalization where the zero-mode Hamiltonian is $p^2/2$.

###### Dedekind eta function

↑ **Parent:** [Torus partition function of a free boson](#torus-partition-function-of-a-free-boson)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dedekind_eta_function)

The Dedekind eta function is

$$
\eta(\tau)=q^{1/24}\prod_{n=1}^{\infty}(1-q^n),
\qquad q=e^{2\pi i\tau}.
$$

It packages the oscillator contribution of a chiral free boson.

###### Eta-quotient

↑ **Parent:** [Dedekind eta function](#dedekind-eta-function)

##### Compact boson

↑ **Parent:** [Free boson conformal field theory](#free-boson-conformal-field-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Compact_boson)

A compact boson takes values on a circle, $X\sim X+2\pi R$. Its states carry quantized momentum $n/R$ and integer winding $wR$.

###### Momentum and winding modes

↑ **Parent:** [Compact boson](#compact-boson)

For a compact boson of radius $R$, momentum number $n$ and winding number $w$ combine into left- and right-moving zero-mode momenta $p_L=n/R+wR$ and $p_R=n/R-wR$ in a common normalization.

###### Exceptional massless ground states of a bosonic circle

↑ **Parent:** [Momentum and winding modes](#momentum-and-winding-modes)

In the critical [closed bosonic string](#closed-string), compactification of one coordinate gives $M^2=n^2/R^2+w^2R^2/\alpha'^2+2(N+\widetilde N-2)/\alpha'$ and $\widetilde N-N+nw=0$. At oscillator level zero, level matching forces $nw=0$. Thus a pure [momentum](momentum.md) [ground state](quantum-mechanics.md#ground-state) becomes a massless [scalar field](classical-field-theory.md#scalar-field) at $R=|n|\sqrt{\alpha'}/2$, while a pure winding [ground state](quantum-mechanics.md#ground-state) does so at $R=2\sqrt{\alpha'}/|w|$. These are threshold states descended from the bosonic [tachyon](physics.md#tachyon); they are additional to the neutral [graviton](quantum-theory.md#graviton), two-form, vectors, [dilaton](string-theory.md#dilaton) and radius modulus. At the [self-dual circle](#self-dual-circle-compactification), the four charges $(\pm2,0),(0,\pm2)$ contribute to the enhanced massless [scalar field](classical-field-theory.md#scalar-field) spectrum.

###### Compact-circle closed-string level matching

↑ **Parent:** [Momentum and winding modes](#momentum-and-winding-modes)

For a compact string coordinate of radius $R$, choose $p_L=n/R+wR/\alpha'$ and $p_R=n/R-wR/\alpha'$, where the left-moving oscillators are denoted by tildes. The two classical zero-mode [Virasoro constraints](#virasoro-constraint) give $M^2=p_L^2+4\widetilde N/\alpha'=p_R^2+4N/\alpha'$. Their difference yields the displayed shifted [closed-string level matching](#closed-string-level-matching) condition. Their average is $M^2=(n/R)^2+(wR/\alpha')^2+2(N+\widetilde N)/\alpha'$. Classically the center-of-mass momentum can be continuous; the integer momentum number belongs to compact-coordinate quantization. Quantum intercepts shift the mass formula but cancel out of level matching.

###### Massless spectrum at the bosonic self-dual circle

↑ **Parent:** [Momentum and winding modes](#momentum-and-winding-modes)

The [self-dual circle](#self-dual-circle-compactification) mass equation and [closed-string level matching](#closed-string-level-matching) exhaust the possibilities at level sum zero, one or two. Besides the usual neutral $(N,\widetilde N)=(1,1)$ states, charges $(n,w)=(\pm1,\pm1)$ supply singly excited chiral states, with the sector fixed by level matching. Ground-state charges $(\pm2,0)$ and $(0,\pm2)$ also become massless. Their compact energy cancels the uncompactified [tachyon](physics.md#tachyon) mass. With $d$ physical transverse components, these families have $d^2+4d+4$ independent polarizations.

###### T-duality

↑ **Parent:** [Momentum and winding modes](#momentum-and-winding-modes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/T-duality)

T-duality identifies a compact boson of radius $R$ with one of reciprocal radius by exchanging momentum and winding numbers. Factors of $\alpha'$ restore the dimensional relation $R\leftrightarrow\alpha'/R$.

###### T-duality of D-brane boundary conditions

↑ **Parent:** [T-duality](#t-duality)

For a compact [string embedding map](#string-embedding-map) coordinate, [T-duality](#t-duality) preserves its left-moving part and reverses its right-moving part. Consequently $\partial_\tau\widetilde X=\partial_\sigma X$ and $\partial_\sigma\widetilde X=\partial_\tau X$. A [Neumann boundary condition](differential-equation.md#neumann-boundary-condition) becomes a [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) and conversely. A [D-brane](string-theory.md#d-brane) wrapping the circle loses one spatial worldvolume dimension; a [D-brane](string-theory.md#d-brane) transverse to it gains one in the dual description.

###### Brane separation becomes a Wilson line

↑ **Parent:** [T-duality of D-brane boundary conditions](#t-duality-of-d-brane-boundary-conditions)

Under [T-duality](#t-duality), the positions $y_i$ of [D-branes](string-theory.md#d-brane) transverse to a circle of radius $R$ become diagonal [Wilson lines](relativistic-quantum-field.md#wilson-line) on branes wrapping the dual circle $R'=\alpha'/R$. Their holonomies are $\exp(i2\pi R'A_i)=\exp(iy_i/R)$. An [Open string stretched between D-branes](string-theory.md#open-string-stretched-between-d-branes) with displacement $y_j-y_i+2\pi Rw$ becomes a string with shifted compact momentum $w/R'+A_j-A_i$. The stretching contribution and the shifted-momentum contribution to its squared mass are identical.

###### Global qualifications of Abelian T-duality

↑ **Parent:** [T-duality](#t-duality)

A local [Buscher procedure](#buscher-procedure) sets a flat auxiliary connection equal to a coordinate derivative only on a simply connected patch. A full compact-circle [Polyakov path integral](#polyakov-path-integral) must also sum flat-connection holonomies, match the period of the dual multiplier, and include [momentum and winding modes](#momentum-and-winding-modes). A free circle isometry then gives the radius relation $R'=\alpha'/R$. Fixed points, noncompact orbits and global identifications require additional analysis; a local spacelike [Killing vector](killing-vector-field.md) does not specify these data.

###### Self-dual circle compactification

↑ **Parent:** [T-duality](#t-duality)

A circle compactification is self-dual when the radius is unchanged by the [T-duality](#t-duality) map $R\mapsto\alpha'/R$. Momentum and winding then enter the [bosonic string mass spectrum](#bosonic-string-mass-spectrum) with equal weights. Special charge sectors can become massless at this radius.

###### Self-dual circle current algebra

↑ **Parent:** [Self-dual circle compactification](#self-dual-circle-compactification)

At $R=\sqrt{\alpha'}$, a chiral [compact boson](#compact-boson) has [operator product expansion](#operator-product-expansion) $Y_L(z)Y_L(w)\sim-\alpha'\log(z-w)/2$. The currents $J^3=i\partial Y_L/\sqrt{\alpha'}$ and $J^\pm=:\!e^{\pm2iY_L/\sqrt{\alpha'}}\!:$ have [conformal weight](#conformal-weight) one. Contractions give $J^3(z)J^3(w)\sim1/[2(z-w)^2]$, $J^3(z)J^\pm(w)\sim\pm J^\pm(w)/(z-w)$ and $J^+(z)J^-(w)\sim1/(z-w)^2+2J^3(w)/(z-w)$. These are the level-one [SU(2) Lie algebra](semisimple-lie-algebra.md#su-2-lie-algebra) currents. The right-moving copy supplies a second factor. Combining a current with a noncompact coordinate derivative gives a massless [string vertex operator](#string-vertex-operator) for each of the six vectors; four are additional to the generic two Cartan vectors.

###### Radius deformation as a Higgs mechanism

↑ **Parent:** [Self-dual circle compactification](#self-dual-circle-compactification)

At the [self-dual circle](#self-dual-circle-compactification), left and right dimension-one currents generate $SU(2)_L\times SU(2)_R$. The compact-coordinate vertex $\partial Y_L\bar\partial Y_R$ is a Cartan–Cartan component of a [scalar field](classical-field-theory.md#scalar-field) in the $(3,3)$ representation. Its [expectation value](quantum-system.md#expectation-value) changes the circle radius and leaves $U(1)_L\times U(1)_R$ unbroken. The four extra charged vectors acquire the displayed mass, and four [scalar field](classical-field-theory.md#scalar-field) polarizations become their longitudinal modes. This realizes the [Higgs mechanism](standard-model.md#higgs-mechanism) geometrically. In a bosonic string the ever-present [tachyon](physics.md#tachyon) and additional [scalar field](classical-field-theory.md#scalar-field) instabilities prevent interpreting the whole family as a stable vacuum.

###### Buscher procedure

↑ **Parent:** [T-duality](#t-duality)

The Buscher procedure derives T-dual backgrounds by replacing the derivative of an isometric target coordinate with an independent worldsheet one-form and imposing its flatness with a Lagrange multiplier. Integrating out either field yields the original or dual sigma model.

###### First-order action for Abelian worldsheet duality

↑ **Parent:** [Buscher procedure](#buscher-procedure)

Replace the derivative of an isometric coordinate by an independent one-form $A$ and impose $dA=0$ with a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier). In signature $(-,+)$ with $\epsilon^{\tau\sigma}=1$, its equation is $VA^\nu=\epsilon^{\mu\nu}\partial_\mu\widetilde z$. Eliminating $A$ from the full action, including the multiplier term, gives $\tfrac12V^{-1}\partial_\mu\widetilde z\partial^\mu\widetilde z$. Omitting the multiplier term during substitution would give the wrong sign. This derives the block-diagonal metric inversion in the [Buscher rules](#buscher-rules).

###### Buscher dilaton shift

↑ **Parent:** [Buscher procedure](#buscher-procedure)

The quantum measure in abelian [T-duality](#t-duality) changes the conventional [dilaton](string-theory.md#dilaton) by $\varphi'=\varphi-\frac12\log g_{yy}$ in alpha-prime-one units for a spacelike isometry. The regulated Gaussian integration over the auxiliary gauge field produces this curvature coupling. It is consistent with invariance of the string-frame density $e^{-2\varphi}\sqrt{\det g}$ under the local Buscher rules.

###### Polar-coordinate T-dual background

↑ **Parent:** [Buscher dilaton shift](#buscher-dilaton-shift)

The flat polar metric $dr^2+r^2dz^2$ has a circle isometry away from $r=0$. Its local [Buscher rules](#buscher-rules) give the displayed dual metric and [dilaton](string-theory.md#dilaton). The dual [Ricci tensor](riemann-curvature-tensor.md#ricci-tensor) has components $R_{rr}=-2/r^2$ and $R_{\widetilde z\widetilde z}=-2/r^4$, while the dilaton Hessian has components $1/r^2$ and $1/r^4$. Thus the [leading metric-dilaton Weyl condition](#leading-metric-dilaton-weyl-condition) $R_{ab}+2\nabla_a\nabla_b\Phi=0$ holds despite nonzero curvature. Flat spectators complete a critical target; the scalar anomaly condition also holds because $|\nabla\Phi|^2=1/r^2$, $\Box\Phi=2/r^2$ and $R=-4/r^2$. The construction is local on $r>0$, excluding the degenerating circle.

###### Buscher rules

↑ **Parent:** [Buscher procedure](#buscher-procedure)

The Buscher rules invert the metric component along an Abelian isometry and transform the other metric and B-field components. The Gaussian functional determinant also shifts the dilaton; when the metric is block diagonal with $G_{zz}=V$, $\widetilde\Phi=\Phi-\tfrac12\log V$.

###### Buscher dual of a metric with vanishing two-form

↑ **Parent:** [Buscher rules](#buscher-rules)

For a nondegenerate isometry direction $y$ and initially zero two-form, the local T-dual fields in alpha-prime-one units are $g'_{yy}=1/g_{yy}$, $g'_{yi}=0$, $g'_{ij}=g_{ij}-g_{yi}g_{yj}/g_{yy}$, $B'_{yi}=g_{yi}/g_{yy}$ and $B'_{ij}=0$. Gauging the isometry and eliminating its auxiliary connection derives these rules. The spectator metric is a [Schur complement](linear-algebra.md#schur-complement). The sign of the mixed two-form follows the multiplier and dual-coordinate orientation convention.

## String oscillator

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)

The Fourier modes $\alpha_n^i$ and $\widetilde\alpha_n^i$ of the transverse closed-string coordinates obey harmonic-oscillator commutation relations. Modes with negative index create string excitations.

### Oscillator vacuum

↑ **Parent:** [String oscillator](#string-oscillator)

An oscillator vacuum is annihilated by all positive-frequency oscillator annihilation operators. For a [Ramond sector](string-theory.md#ramond-sector) string this leaves a degenerate space on which the fermionic zero modes act through the [Ramond zero-mode Clifford algebra](string-theory.md#ramond-zero-mode-clifford-algebra). Vacuum annihilation therefore does not select a unique spinor state.

### Half-integer open-string oscillator

↑ **Parent:** [String oscillator](#string-oscillator)

For a [Neumann-Dirichlet open-string boundary condition](#neumann-dirichlet-open-string-boundary-condition), the transverse modes have frequencies $r\in\mathbb Z+1/2$. The [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) give $[\alpha_r^i,\alpha_s^j]=r\delta^{ij}\delta_{r+s,0}$ and $\alpha_r^\dagger=\alpha_{-r}$. One derivation expands $X-y=\sum_{r>0}q_r\cos(r\sigma)$: spatial [orthogonality](inner-product.md#orthogonal-vectors) reduces the [Polyakov action](#polyakov-action) to $(8\alpha')^{-1}\int\sum_r(\dot q_r^2-r^2q_r^2)d\tau$. These are [harmonic oscillators](classical-mechanics.md#simple-harmonic-motion) of [mass](classical-mechanics.md#mass) $1/(4\alpha')$, whose normalized [creation operators](quantum-harmonic-oscillator.md#creation-operator) satisfy $\alpha_{-r}=i\sqrt r\,a_r^\dagger$ in the conventional phased expansion.

### String level operator

↑ **Parent:** [String oscillator](#string-oscillator)

The string level operator is the weighted oscillator number $N=\sum_{n>0}\alpha_{-n}\mathbin\cdot\alpha_n$. A closed string has independent operators $N$ and $\widetilde N$ for its two chiral sectors.

#### Integer string oscillator level

↑ **Parent:** [String level operator](#string-level-operator)

The [canonical commutation relations](quantum-mechanics.md#canonical-commutation-relation) imply $[N,\alpha_{-k}^i]=k\alpha_{-k}^i$ for $N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k$. With zero level assigned to the [oscillator vacuum](#oscillator-vacuum), a [Fock space](quantum-field-theory.md#fock-space) basis state containing $r_{ki}$ [creation operators](quantum-harmonic-oscillator.md#creation-operator) of each mode has level $\sum_{k,i}kr_{ki}$. The level is therefore a nonnegative integer; it counts oscillator excitation weighted by frequency, not simply the number of creation operators.

### Closed-string level matching

↑ **Parent:** [String oscillator](#string-oscillator)

Closed-string periodicity and the residual spatial constraint require equal left- and right-moving excitation levels, $N=\widetilde N$.

### Normal-ordering constant of a string

↑ **Parent:** [String oscillator](#string-oscillator)

The normal-ordering constant is the zero-point shift in the quantum Virasoro generator. Closure of the target-space Lorentz algebra fixes $a=1$ and the spacetime dimension $D=26$ for the bosonic string.

#### Critical-vector assumption in the string intercept argument

↑ **Parent:** [Normal-ordering constant of a string](#normal-ordering-constant-of-a-string)

In the usual critical Lorentz-invariant bosonic string, level-one transverse vector polarizations fit a massless representation, whereas a massive vector would require an extra polarization. This fixes the intercept to one. Polarization counting alone does not establish that conclusion in every dimension: in three dimensions the one transverse polarization transforms trivially under the transverse rotation group and can be interpreted as a scalar. The quantum consistency assumptions must accompany an argument that the first level must be massless.

#### Neumann-Dirichlet string zero-point energy

↑ **Parent:** [Normal-ordering constant of a string](#normal-ordering-constant-of-a-string)

Each of $d$ physical transverse [bosons](tensor-product-of-quantum-systems.md#boson) with a [Neumann-Dirichlet open-string boundary condition](#neumann-dirichlet-open-string-boundary-condition) contributes $\tfrac12\sum_{r>0}r=1/48$ by the [half-integer zeta-regularized mode sum](holomorphic-function.md#half-integer-zeta-regularized-mode-sum). Thus $L_0^\perp=N+d/48$ and the convention $L_0=\alpha'p^2+N-a$ has $a=-d/48$. For $d=24$, the vacuum shift is $+1/2$. The ordinary integer-moded open-string shift is instead $-d/24$; these endpoint sectors have different normal-ordering constants.

##### Lowest levels of a fully transverse ND bosonic string

↑ **Parent:** [Neumann-Dirichlet string zero-point energy](#neumann-dirichlet-string-zero-point-energy)

With 24 physical [half-integer open-string oscillators](#half-integer-open-string-oscillator), the first three [string level operator](#string-level-operator) [eigenvalues](linear-operator-theory.md#eigenvalue) are $0,1/2,1$. Their states are the vacuum, $a_{1/2}^{i\dagger}|0\rangle$, and $a_{1/2}^{i\dagger}a_{1/2}^{j\dagger}|0\rangle$. The [creation operators](quantum-harmonic-oscillator.md#creation-operator) commute, so the third level is the [symmetric square](multilinear-algebra.md#symmetric-square) of the 24-dimensional transverse vector, of dimension $24\cdot25/2=300$. Its trace is a scalar and its trace-free part has dimension 299. Including the vacuum shift gives $\alpha'M^2=1/2,1,3/2$ when the two longitudinal directions are common directions with [Neumann boundary conditions](differential-equation.md#neumann-boundary-condition). The representation labels refer to the surviving ND rotation group, not full unbroken target Lorentz symmetry.

### Bosonic string mass spectrum

↑ **Parent:** [String oscillator](#string-oscillator)

For a closed bosonic string,

$$
M^2=\frac4{\alpha'}(N-a)=\frac4{\alpha'}(\widetilde N-a),
\qquad N=\widetilde N.
$$

#### Closed-bosonic-string mass shell from primary weights

↑ **Parent:** [Bosonic string mass spectrum](#bosonic-string-mass-spectrum)

A matter vertex with left and right oscillator levels $N,\widetilde N$ and momentum $k$ has weights $N+\alpha'k^2/4,\widetilde N+\alpha'k^2/4$. An [integrated string vertex operator](#integrated-string-vertex-operator) must have weights $(1,1)$, giving the displayed mass shell and level matching with $M^2=-k^2$. Physical states are further identified modulo [null string states](#null-string-state), equivalently through [BRST cohomology](relativistic-quantum-field.md#brst-cohomology); merely counting all weight-one primaries would include gauge redundancies.

#### Massive two-form at closed-string level two

↑ **Parent:** [Bosonic string mass spectrum](#bosonic-string-mass-spectrum)

Each level-two chiral sector of the critical [closed string](#closed-string) is the [symmetric traceless square](multilinear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation) $S^2_0V$ of the massive [little group](special-relativity.md#little-group) vector space. The [tensor product](multilinear-algebra.md#tensor-product) of its two sectors contains the [exterior square](multilinear-algebra.md#exterior-square) $\Lambda^2V$: the equivariant map $(S,T)\mapsto ST-TS$ is onto the antisymmetric matrices. Compact-group complete reducibility realizes this quotient as a subrepresentation. It describes a [massive two-form field](classical-field-theory.md#massive-two-form-field) with $M^2=8\pi T=4/\alpha'$.

#### Massless first closed-string level

↑ **Parent:** [Bosonic string mass spectrum](#bosonic-string-mass-spectrum)

In the critical [bosonic string theory](bosonic-string-theory.md), the states $\alpha_{-1}^i\widetilde\alpha_{-1}^j|0;p\rangle$ have $M^2=0$. Their coefficient matrix decomposes into a symmetric trace-free tensor, an antisymmetric tensor, and a scalar trace, representing the [graviton](quantum-theory.md#graviton), [Kalb–Ramond field](#kalb-ramond-field), and [dilaton](string-theory.md#dilaton). Their transverse [particle polarization](special-relativity.md#particle-polarization) counts add to $(D-2)^2$. The [normal-ordering constant of a string](#normal-ordering-constant-of-a-string) is one.

#### Open bosonic string mass spectrum

↑ **Parent:** [Bosonic string mass spectrum](#bosonic-string-mass-spectrum)

The [string level operator](#string-level-operator) for a free-ended [open string](#open-string) is $N=\sum_{k>0}\alpha_{-k}\cdot\alpha_k$. The quantum condition is $\alpha'M^2=N-a$, where $a$ is the [normal-ordering constant of a string](#normal-ordering-constant-of-a-string). Lorentz-consistent [bosonic string theory](bosonic-string-theory.md) has $a=1$.

##### Lowest light-cone levels of an open bosonic string

↑ **Parent:** [Open bosonic string mass spectrum](#open-bosonic-string-mass-spectrum)

The first levels are the [oscillator vacuum](#oscillator-vacuum), $\alpha_{-1}^I|0\rangle$, and $\alpha_{-2}^I|0\rangle,\alpha_{-1}^I\alpha_{-1}^J|0\rangle$. At level two the transverse [vector representation](representation-theory.md#vector-representation) and [symmetric square](multilinear-algebra.md#symmetric-square) assemble into the massive [symmetric traceless square](multilinear-algebra.md#symmetric-trace-free-square-of-the-defining-orthogonal-representation) of one extra rotation dimension.

## Critical dimension of string theory

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)

The critical dimension is the target-spacetime dimension in which quantum anomalies obstructing Lorentz or Weyl symmetry cancel. It is 26 for the bosonic string.

Here critical means cancellation of the string’s quantum anomalies; it does not mean the upper or lower critical dimension of a phase transition.

### Bosonic-string critical dimension from ghost descendants

↑ **Parent:** [Critical dimension of string theory](#critical-dimension-of-string-theory)

For the [FP ghost](relativistic-quantum-field.md#faddeev-popov-ghost) vacuum annihilated by $b_{n\ge0}$ and $c_{n>0}$, the [FP ghost](relativistic-quantum-field.md#faddeev-popov-ghost) level-one and level-two descendant coefficients are $-2$ and $-17$. Matter contributes $\alpha_0^2$ and $2\alpha_0^2+D/2$. [Virasoro closure from BRST nilpotence](#virasoro-closure-from-brst-nilpotence) at level one fixes the total highest weight to $\alpha_0^2/2-1$; level two then requires $D=26$. Imposing ground-state BRST closure gives $\alpha_0^2=2$ and the open bosonic [tachyon](physics.md#tachyon). Interpret the coefficients with the stated [ghost zero-mode pairing](#ghost-zero-mode-pairing).

### Critical dimension of the RNS superstring

↑ **Parent:** [Critical dimension of string theory](#critical-dimension-of-string-theory)

Each of $D$ embedding [bosons](tensor-product-of-quantum-systems.md#boson) contributes one to the chiral [central charge](#central-charge), and each real [worldsheet Majorana fermion](string-theory.md#worldsheet-majorana-fermion) contributes one half. The reparameterization [bc system](#bc-system) contributes $-26$, and the [superconformal ghosts](string-theory.md#superconformal-ghost) contribute $+11$. Vanishing total [worldsheet Weyl anomaly](#worldsheet-weyl-anomaly) therefore requires $3D/2-26+11=0$, or $D=10$. This differs from the critical dimension 26 of the bosonic string, which has no worldsheet [fermions](tensor-product-of-quantum-systems.md#fermion) or superconformal ghosts.

#### Massless chiral RNS spectrum after GSO projection

↑ **Parent:** [Critical dimension of the RNS superstring](#critical-dimension-of-the-rns-superstring)

In one critical chiral [RNS string](string-theory.md#spinning-string) sector, [light-cone gauge in string theory](#light-cone-gauge-in-string-theory) leaves eight transverse directions. The [Neveu–Schwarz sector](string-theory.md#neveu-schwarz-sector) massless states $b_{-1/2}^i|0;k\rangle$ give eight spacetime bosonic polarizations. The [Ramond zero-mode Clifford algebra](string-theory.md#ramond-zero-mode-clifford-algebra) gives sixteen ground-state polarizations, split into two eight-dimensional spinor chiralities. The supersymmetric [GSO projection](string-theory.md#gso-projection) keeps one chirality, giving eight spacetime fermionic polarizations. Without that projection the massless counts do not agree. Counting a chiral sector is distinct from tensoring left and right sectors into closed-string states.

## Koba-Nielsen factor

↑ **Parent:** [Bosonic string theory](bosonic-string-theory.md)

The Koba-Nielsen factor is the product of powers of pairwise worldsheet insertion-point distances produced by contractions of string vertex operators.

<h3 id="mobius-invariance-of-on-shell-closed-string-vertex-integrals">Möbius invariance of on-shell closed-string vertex integrals</h3>

↑ **Parent:** [Koba-Nielsen factor](#koba-nielsen-factor)

Under $z\mapsto(az+b)/(cz+d)$ with $ad-bc=1$, the coordinate measure contributes $|cz_i+d|^{-4}$ at insertion $i$. The [Koba-Nielsen factor](#koba-nielsen-factor) contributes $|cz_i+d|^{-\alpha'\sum_{j\ne i}p_i\cdot p_j}$. [Four-momentum conservation](special-relativity.md#four-momentum-conservation) makes this exponent $\alpha'p_i^2$, so the factors cancel precisely on the displayed [tachyon](physics.md#tachyon) mass shell. The correlator alone is covariant; its product with all the coordinate measures is invariant.

<h3 id="virasoro-shapiro-amplitude">Virasoro–Shapiro amplitude</h3>

↑ **Parent:** [Koba-Nielsen factor](#koba-nielsen-factor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Virasoro–Shapiro_amplitude)

The Virasoro–Shapiro amplitude is the crossing-symmetric tree-level four-point amplitude of closed-string tachyons. Its worldsheet integral is a complex beta integral, and its poles display the closed-string spectrum.

#### Fixed-angle softness of the closed-string amplitude

↑ **Parent:** [Virasoro–Shapiro amplitude](#virasoro-shapiro-amplitude)

For $t\simeq-as$, $u\simeq-(1-a)s$ with $0<a<1$, the smooth high-energy envelope satisfies $\log|A|\simeq-2s[-a\log a-(1-a)\log(1-a)]$. The [Gamma function](complex-analysis.md#gamma-function) asymptotics cancel the leading $s\log s$ terms, leaving exponential suppression. Exact real-axis resonance poles must be excluded or treated by analytic continuation.

<h4 id="virasoro-shapiro-amplitude-pole-residue">Virasoro–Shapiro amplitude pole residue</h4>

↑ **Parent:** [Virasoro–Shapiro amplitude](#virasoro-shapiro-amplitude)

For $a=-1-\alpha's/4$, $b=-1-\alpha't/4$ and $a+b+c=1$, the amplitude has generic [simple poles](isolated-singularity.md#simple-pole) at $a=-n$. The [gamma function](complex-analysis.md#gamma-function) [residue](analysis.md#residue) and recurrence give

$$
\operatorname*{Res}_{s=s_n}A^{(4)}=-\frac{8\pi g_s^2}{\alpha'(n!)^2}\prod_{j=1}^n(b-j)^2.
$$

The [residue](analysis.md#residue) polynomial has degree $2n$, consistent with closed-string exchange up to spin $2n$. When $a=-n+\delta_a$ and $b=-m+\delta_b$, the reciprocal factor $1/\Gamma(a+b)$ removes a putative double pole: the leading ratio is $\binom{n+m}{n}^2(1/\delta_a+1/\delta_b)$. Thus channel singularities must be counted using the kinematic constraint, not by multiplying independent numerator poles.

### CHY formalism

↑ **Parent:** [Koba-Nielsen factor](#koba-nielsen-factor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CHY_formalism)

The Cachazo-He-Yuan formalism expresses tree-level scattering amplitudes as integrals localized on scattering equations.

#### Scattering equation

↑ **Parent:** [CHY formalism](#chy-formalism)

For null or hard external momenta, the scattering equations are

$$
\sum_{j\ne i}\frac{p_i\cdot p_j}{z_i-z_j}=0.
$$

They arise as stationary-point equations for the Koba-Nielsen exponent and are covariant under projective transformations of the insertion points.

## ↑ Ancestors (4)

1. [String theory](string-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (19)

- [Bosonic D3-brane low-energy field content](string-theory.md#bosonic-d3-brane-low-energy-field-content)
- [BRST nilpotence](relativistic-quantum-field.md#brst-nilpotence)
- [Massless first closed-string level](#massless-first-closed-string-level)
- [No-ghost theorem for the critical bosonic string](#no-ghost-theorem-for-the-critical-bosonic-string)
- [Open bosonic string mass spectrum](#open-bosonic-string-mass-spectrum)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-66.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-67.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-53.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-53.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-54.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-54.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-51.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-51.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-46.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-46.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-306.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306.md#4/solution)
- [Physical-state Virasoro conditions for an open string](#physical-state-virasoro-conditions-for-an-open-string)
