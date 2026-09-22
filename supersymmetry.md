# Supersymmetry

↑ **Parent:** [Branches of physics](physics.md#branches-of-physics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetry)

Supersymmetry extends spacetime symmetry by odd [supercharges](#supersymmetry-generator) that interchange [boson](quantum-mechanics.md#boson) and [fermion](quantum-mechanics.md#fermion) states. Their [Super-Poincaré algebra](#super-poincare-algebra) pairs positive-energy states into [supermultiplets](#supermultiplet) and gives [energy positivity in global supersymmetry](#energy-positivity-in-global-supersymmetry). [Superspace](#superspace) and [superfields](#superfield) package the component fields into representations of this symmetry.

**Table of contents**

- [Supersymmetric action](#supersymmetric-action)
  - [Two-derivative global supersymmetric gauge action](#two-derivative-global-supersymmetric-gauge-action)
  - [Gauge kinetic function](#gauge-kinetic-function)
    - [Holomorphic gauge coupling](#holomorphic-gauge-coupling)
  - [Grassmann-valued classical supersymmetric mechanics](#grassmann-valued-classical-supersymmetric-mechanics)
    - [First-order zero-energy solution in Grassmann supersymmetric mechanics](#first-order-zero-energy-solution-in-grassmann-supersymmetric-mechanics)
  - [Renormalizable chiral-superfield action](#renormalizable-chiral-superfield-action)
- [Worldline supersymmetry algebra](#worldline-supersymmetry-algebra)
- [Supersymmetric localization](#supersymmetric-localization)
  - [Localization of a zero-dimensional polynomial model](#localization-of-a-zero-dimensional-polynomial-model)
- [Supersymmetric Ward identity](#supersymmetric-ward-identity)
- [Zero-dimensional supersymmetric field theory](#zero-dimensional-supersymmetric-field-theory)
  - [Odd symmetries of a zero-dimensional polynomial model](#odd-symmetries-of-a-zero-dimensional-polynomial-model)
- [Extended supersymmetry](#extended-supersymmetry)
  - [Chirality constraint on extended supersymmetry](#chirality-constraint-on-extended-supersymmetry)
  - [Hypermultiplet](#hypermultiplet)
- [Two-dimensional N=(2,2) supersymmetry](#two-dimensional-n-2-2-supersymmetry)
  - [Twisted chiral superfield](#twisted-chiral-superfield)
    - [Twisted superpotential](#twisted-superpotential)
- [Two-dimensional N=(0,2) supersymmetry](#two-dimensional-n-0-2-supersymmetry)
  - [Fermi superfield](#fermi-superfield)
- [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)
  - [Super-Poincaré group](#super-poincare-group)
  - [Supercurrent](#supercurrent)
  - [Super-Poincaré algebra](#super-poincare-algebra)
    - [Domain-wall charge in N=1 supersymmetry](#domain-wall-charge-in-n-1-supersymmetry)
    - [Supertranslation](#supertranslation)
    - [Superspace differential realization of N=1 supercharges](#superspace-differential-realization-of-n-1-supercharges)
    - [Supercharges commute with translations](#supercharges-commute-with-translations)
    - [Energy positivity in global supersymmetry](#energy-positivity-in-global-supersymmetry)
      - [Nullity of real N=1 supercharges](#nullity-of-real-n-1-supercharges)
    - [Central charge in supersymmetry](#central-charge-in-supersymmetry)
      - [BPS bound in supersymmetry](#bps-bound-in-supersymmetry)
        - [BPS state](#bps-state)
          - [Wall of marginal stability](#wall-of-marginal-stability)
    - [Supersymmetry generator](#supersymmetry-generator)
      - [Supersymmetry transformation](#supersymmetry-transformation)
      - [Jacobi sign test for supercharge components](#jacobi-sign-test-for-supercharge-components)
    - [Coleman–Mandula theorem](#coleman-mandula-theorem)
      - [Haag–Łopuszański–Sohnius theorem](#haag-lopuszanski-sohnius-theorem)
    - [Superspin Casimir](#superspin-casimir)
  - [Supermultiplet](#supermultiplet)
    - [Chiral multiplet](#chiral-multiplet)
    - [Massive supermultiplet](#massive-supermultiplet)
      - [Superspin](#superspin)
      - [Spin-zero massive N=1 supermultiplet](#spin-zero-massive-n-1-supermultiplet)
      - [Shortened massive supermultiplet](#shortened-massive-supermultiplet)
    - [Supersymmetric vector multiplet](#supersymmetric-vector-multiplet)
      - [Massive N=1 vector multiplet](#massive-n-1-vector-multiplet)
        - [Massless limit of a massive N=1 vector multiplet](#massless-limit-of-a-massive-n-1-vector-multiplet)
    - [CPT completion of a supermultiplet](#cpt-completion-of-a-supermultiplet)
    - [Massless supermultiplet](#massless-supermultiplet)
      - [Superhelicity](#superhelicity)
      - [Helicity spectrum of a massless supermultiplet](#helicity-spectrum-of-a-massless-supermultiplet)
        - [Spin bound for massless supermultiplets](#spin-bound-for-massless-supermultiplets)
    - [Boson-fermion degeneracy in a supermultiplet](#boson-fermion-degeneracy-in-a-supermultiplet)
      - [Supertrace pairing at positive energy](#supertrace-pairing-at-positive-energy)
      - [Odd involution pairing bosonic and fermionic states](#odd-involution-pairing-bosonic-and-fermionic-states)
      - [Supersymmetric mass degeneracy](#supersymmetric-mass-degeneracy)
        - [Complex scalar mass at a supersymmetric critical point](#complex-scalar-mass-at-a-supersymmetric-critical-point)
  - [Superspace](#superspace)
    - [Supertranslation-invariant superspace coframe](#supertranslation-invariant-superspace-coframe)
      - [Closed three-form on four-dimensional superspace](#closed-three-form-on-four-dimensional-superspace)
    - [Supervielbein](#supervielbein)
    - [Kappa symmetry](#kappa-symmetry)
      - [Kappa symmetry projector](#kappa-symmetry-projector)
    - [Two-dimensional N=(1,1) superspace](#two-dimensional-n-1-1-superspace)
      - [Supersymmetric Liouville equation](#supersymmetric-liouville-equation)
    - [Two-component superspace contraction signs](#two-component-superspace-contraction-signs)
    - [Superspace integration](#superspace-integration)
    - [Superfield](#superfield)
      - [Superfield covariance is not Grassmann dependence alone](#superfield-covariance-is-not-grassmann-dependence-alone)
      - [Scalar superfield transformation](#scalar-superfield-transformation)
        - [Partial derivatives and superfield covariance](#partial-derivatives-and-superfield-covariance)
        - [Pure-scalar truncation of a superfield](#pure-scalar-truncation-of-a-superfield)
        - [Product of scalar superfields](#product-of-scalar-superfields)
      - [Vector superfield](#vector-superfield)
        - [Superspace gauge connection](#superspace-gauge-connection)
        - [Wess-Zumino gauge](#wess-zumino-gauge)
        - [Gauge-transformation superfield](#gauge-transformation-superfield)
          - [Supergauge transformation](#supergauge-transformation)
        - [D-term scalar potential](#d-term-scalar-potential)
          - [Single charged-field D-term breaking](#single-charged-field-d-term-breaking)
            - [Mass spectrum of single charged-field D-term breaking](#mass-spectrum-of-single-charged-field-d-term-breaking)
          - [D-term vacuum branches of a cubic superpotential](#d-term-vacuum-branches-of-a-cubic-superpotential)
          - [Fayet–Iliopoulos term](#fayet-iliopoulos-term)
            - [Constant Fayet–Iliopoulos terms in conventional N=1 supergravity](#constant-fayet-iliopoulos-terms-in-conventional-n-1-supergravity)
            - [Perturbative renormalization of a Fayet–Iliopoulos term](#perturbative-renormalization-of-a-fayet-iliopoulos-term)
            - [Fayet–Iliopoulos terms require an Abelian gauge factor](#fayet-iliopoulos-terms-require-an-abelian-gauge-factor)
        - [Chiral field-strength superfield](#chiral-field-strength-superfield)
          - [Superspace Yang-Mills Bianchi identity](#superspace-yang-mills-bianchi-identity)
          - [Abelian field-strength chiral projection](#abelian-field-strength-chiral-projection)
          - [Supersymmetric Yang-Mills action](#supersymmetric-yang-mills-action)
      - [Chiral superfield](#chiral-superfield)
        - [Chiral spinor superfield](#chiral-spinor-superfield)
        - [Holomorphic closure of chiral superfields](#holomorphic-closure-of-chiral-superfields)
        - [Nilpotent chiral superfield](#nilpotent-chiral-superfield)
          - [Chiral superfield constrained by a nilpotent superfield](#chiral-superfield-constrained-by-a-nilpotent-superfield)
            - [Cubic nilpotency from a mixed chiral constraint](#cubic-nilpotency-from-a-mixed-chiral-constraint)
        - [Antichiral superfield](#antichiral-superfield)
        - [Supersymmetric covariant derivative](#supersymmetric-covariant-derivative)
          - [Chiral projection by squared supercovariant derivatives](#chiral-projection-by-squared-supercovariant-derivatives)
          - [Supersymmetric derivatives in chiral coordinates](#supersymmetric-derivatives-in-chiral-coordinates)
          - [Supercovariant derivative algebra with left derivatives](#supercovariant-derivative-algebra-with-left-derivatives)
        - [Chiral-superfield component expansion](#chiral-superfield-component-expansion)
        - [Auxiliary field](#auxiliary-field)
        - [Superpotential](#superpotential)
          - [Constant superpotential in global supersymmetry](#constant-superpotential-in-global-supersymmetry)
          - [Superpotential critical-point shift](#superpotential-critical-point-shift)
          - [Chiral-superfield fermion mass matrix](#chiral-superfield-fermion-mass-matrix)
          - [F-term](#f-term)
          - [F-term scalar potential](#f-term-scalar-potential)
            - [Real-slice diagnosis of chiral-scalar vacua](#real-slice-diagnosis-of-chiral-scalar-vacua)
            - [Tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule)
              - [Gauge contributions to the F-term supertrace](#gauge-contributions-to-the-f-term-supertrace)
          - [Non-renormalization theorem](#non-renormalization-theorem)
            - [One-loop exactness of the holomorphic gauge kinetic function](#one-loop-exactness-of-the-holomorphic-gauge-kinetic-function)
            - [Holomorphic and canonically normalized superpotential couplings](#holomorphic-and-canonically-normalized-superpotential-couplings)
            - [Holomorphy argument for superpotential non-renormalization](#holomorphy-argument-for-superpotential-non-renormalization)
              - [Wess–Zumino spurion charge assignment](#wess-zumino-spurion-charge-assignment)
              - [Spurion selection rule for perturbative non-renormalization](#spurion-selection-rule-for-perturbative-non-renormalization)
                - [Perturbative gauge-coupling independence of the Wilsonian superpotential](#perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential)
        - [Kähler potential](#kahler-potential)
          - [Kähler transformation](#kahler-transformation)
          - [D-term](#d-term)
  - [Wess–Zumino model](#wess-zumino-model)
    - [Supersymmetric domain wall](#supersymmetric-domain-wall)
    - [Wess-Zumino chiral multiplet coupled to supergravity](#wess-zumino-chiral-multiplet-coupled-to-supergravity)
    - [Trilinear scalar vertices in the Wess–Zumino model](#trilinear-scalar-vertices-in-the-wess-zumino-model)
    - [Discriminant mass invariant of a cubic superpotential](#discriminant-mass-invariant-of-a-cubic-superpotential)
    - [Supersymmetric relation between quartic and Yukawa couplings](#supersymmetric-relation-between-quartic-and-yukawa-couplings)
      - [Quartic complex-scalar vertex in the Wess–Zumino model](#quartic-complex-scalar-vertex-in-the-wess-zumino-model)
    - [Supersymmetric cancellation of quadratic divergences](#supersymmetric-cancellation-of-quadratic-divergences)
- [Supersymmetry breaking](#supersymmetry-breaking)
  - [Dynamical supersymmetry breaking](#dynamical-supersymmetry-breaking)
  - [Flat F-term breaking with a linear superpotential](#flat-f-term-breaking-with-a-linear-superpotential)
  - [Explicit versus spontaneous supersymmetry breaking](#explicit-versus-spontaneous-supersymmetry-breaking)
  - [Hidden supersymmetry-breaking sector](#hidden-supersymmetry-breaking-sector)
  - [Goldstino](#goldstino)
    - [Goldstino null vector with F-term and D-term breaking](#goldstino-null-vector-with-f-term-and-d-term-breaking)
    - [Goldstino zero mode from vacuum stationarity](#goldstino-zero-mode-from-vacuum-stationarity)
  - [Soft supersymmetry breaking](#soft-supersymmetry-breaking)
    - [Soft scalar-mass sensitivity](#soft-scalar-mass-sensitivity)
    - [Sparticle](#sparticle)
      - [Neutralino](#neutralino)
      - [Lightest supersymmetric particle](#lightest-supersymmetric-particle)
      - [Slepton](#slepton)
      - [Higgsino](#higgsino)
      - [Gaugino](#gaugino)
        - [Bino](#bino)
        - [Wino](#wino)
        - [Gluino](#gluino)
      - [Squark](#squark)
        - [Top squark](#top-squark)
  - [O'Raifeartaigh model](#o-raifeartaigh-model)
    - [Mass spectrum of the quadratic-cubic O'Raifeartaigh model](#mass-spectrum-of-the-quadratic-cubic-o-raifeartaigh-model)
    - [Pseudomodulus](#pseudomodulus)
- [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)
  - [MSSM superpotential](#mssm-superpotential)
    - [Cubic superpotential with right-handed-neutrino superfields](#cubic-superpotential-with-right-handed-neutrino-superfields)
    - [Supersymmetric mu problem](#supersymmetric-mu-problem)
  - [Holomorphic need for two Higgs chiral doublets](#holomorphic-need-for-two-higgs-chiral-doublets)
  - [Higgsino anomaly cancellation](#higgsino-anomaly-cancellation)
  - [Higgs chiral doublet](#higgs-chiral-doublet)
  - [MSSM superfield representations](#mssm-superfield-representations)
  - [MSSM tree-level sfermion mass constraint](#mssm-tree-level-sfermion-mass-constraint)
  - [R-parity](#r-parity)
    - [Matter parity](#matter-parity)
      - [Matter parity allows Majorana neutrino masses](#matter-parity-allows-majorana-neutrino-masses)
    - [R-parity violation](#r-parity-violation)
      - [Squark-mediated proton decay](#squark-mediated-proton-decay)
        - [Four-fermion matching for squark-mediated proton decay](#four-fermion-matching-for-squark-mediated-proton-decay)
        - [Proton-lifetime bound on a product of R-parity-violating couplings](#proton-lifetime-bound-on-a-product-of-r-parity-violating-couplings)
  - [Supersymmetric gauge coupling unification](#supersymmetric-gauge-coupling-unification)
- [Supersymmetric gauge theory](#supersymmetric-gauge-theory)
  - [Ten-dimensional super Yang-Mills theory](#ten-dimensional-super-yang-mills-theory)
  - [Seiberg–Witten theory](#seiberg-witten-theory)
  - [Supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism)
  - [Four-dimensional N=4 super Yang-Mills theory](#four-dimensional-n-4-super-yang-mills-theory)
    - [Commuting-scalar vacua of four-dimensional N=4 Yang-Mills theory](#commuting-scalar-vacua-of-four-dimensional-n-4-yang-mills-theory)
  - [R-symmetry](#r-symmetry)
    - [R-charge](#r-charge)
      - [Chiral primary operator in four-dimensional N=1 supersymmetry](#chiral-primary-operator-in-four-dimensional-n-1-supersymmetry)
    - [Vector R-symmetry](#vector-r-symmetry)
    - [Axial R-symmetry](#axial-r-symmetry)
  - [Supersymmetric vacuum](#supersymmetric-vacuum)
    - [F-flatness](#f-flatness)
    - [D-flatness](#d-flatness)
    - [Vacuum moduli space of a supersymmetric gauge theory](#vacuum-moduli-space-of-a-supersymmetric-gauge-theory)
      - [Neutral flat direction with oppositely charged chiral fields](#neutral-flat-direction-with-oppositely-charged-chiral-fields)
      - [Higgs branch](#higgs-branch)
      - [Coulomb branch](#coulomb-branch)
  - [Supersymmetric quantum electrodynamics](#supersymmetric-quantum-electrodynamics)
  - [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)
    - [Supersymmetric conformal window](#supersymmetric-conformal-window)
    - [Chiral ring of a supersymmetric gauge theory](#chiral-ring-of-a-supersymmetric-gauge-theory)
      - [Meson operator in supersymmetric quantum chromodynamics](#meson-operator-in-supersymmetric-quantum-chromodynamics)
      - [Baryon operator in supersymmetric quantum chromodynamics](#baryon-operator-in-supersymmetric-quantum-chromodynamics)
    - [Holomorphic strong-coupling scale](#holomorphic-strong-coupling-scale)
      - [Affleck–Dine–Seiberg superpotential](#affleck-dine-seiberg-superpotential)
    - [Quantum-deformed moduli space](#quantum-deformed-moduli-space)
    - [s-confinement](#s-confinement)
    - [Seiberg duality](#seiberg-duality)
  - [One-loop beta function of a supersymmetric gauge theory](#one-loop-beta-function-of-a-supersymmetric-gauge-theory)
- [Supergravity](#supergravity)
  - [Composite Kähler connection](#composite-kahler-connection)
  - [Eleven-dimensional supergravity](#eleven-dimensional-supergravity)
    - [Freund-Rubin compactification](#freund-rubin-compactification)
      - [Maximal supersymmetry of AdS4 times S7](#maximal-supersymmetry-of-ads4-times-s7)
    - [Toroidal reduction of eleven-dimensional supergravity](#toroidal-reduction-of-eleven-dimensional-supergravity)
      - [Circle reduction of eleven-dimensional supergravity](#circle-reduction-of-eleven-dimensional-supergravity)
        - [Reduction of the eleven-dimensional Chern-Simons term](#reduction-of-the-eleven-dimensional-chern-simons-term)
  - [Killing spinor](#killing-spinor)
    - [Anti-de Sitter Killing-spinor connection](#anti-de-sitter-killing-spinor-connection)
    - [Parallel-spinor classification of vacuum four-geometries](#parallel-spinor-classification-of-vacuum-four-geometries)
  - [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)
    - [Old-minimal supergravity](#old-minimal-supergravity)
    - [Off-shell component count of minimal supergravity](#off-shell-component-count-of-minimal-supergravity)
    - [Gravitino-induced torsion](#gravitino-induced-torsion)
    - [Supergravity coupling of an Abelian vector multiplet](#supergravity-coupling-of-an-abelian-vector-multiplet)
    - [Anti-de Sitter deformation of minimal supergravity](#anti-de-sitter-deformation-of-minimal-supergravity)
  - [Maximal nine-dimensional supergravity](#maximal-nine-dimensional-supergravity)
  - [Type IIB supergravity](#type-iib-supergravity)
  - [Type IIA supergravity](#type-iia-supergravity)
    - [Massive type IIA supergravity](#massive-type-iia-supergravity)
      - [Romans mass](#romans-mass)
  - [Dilatino](#dilatino)
  - [Super-Higgs mechanism](#super-higgs-mechanism)
  - [Gravitino](#gravitino)
  - [No-scale supergravity](#no-scale-supergravity)
    - [Matter-logarithm no-scale potential](#matter-logarithm-no-scale-potential)
      - [No-scale volume runaway criterion](#no-scale-volume-runaway-criterion)
      - [Cubic-matter no-scale vacuum with an exponential dilaton](#cubic-matter-no-scale-vacuum-with-an-exponential-dilaton)
        - [Quartic stabilization at a double no-scale root](#quartic-stabilization-at-a-double-no-scale-root)
    - [No-scale vacuum with a cubic matter superpotential](#no-scale-vacuum-with-a-cubic-matter-superpotential)
    - [Finite zero-energy vacuum for a single exponential superpotential](#finite-zero-energy-vacuum-for-a-single-exponential-superpotential)
    - [No-scale identity from degree-one homogeneity](#no-scale-identity-from-degree-one-homogeneity)
  - [Supergravity auxiliary field](#supergravity-auxiliary-field)
  - [Four-dimensional N=8 supergravity](#four-dimensional-n-8-supergravity)
  - [Supergravity multiplet](#supergravity-multiplet)
  - [Supergravity F-term potential](#supergravity-f-term-potential)
    - [Supergravity moment-map constraint on D-term breaking](#supergravity-moment-map-constraint-on-d-term-breaking)
    - [Gravitino mass from a superpotential](#gravitino-mass-from-a-superpotential)
    - [Kähler covariant derivative of a superpotential](#kahler-covariant-derivative-of-a-superpotential)
    - [Polonyi model](#polonyi-model)
      - [Stable zero-energy Polonyi vacuum](#stable-zero-energy-polonyi-vacuum)
      - [Polonyi supersymmetry branches](#polonyi-supersymmetry-branches)
- [Spurion](#spurion)

## Supersymmetric action

↑ **Parent:** [Supersymmetry](supersymmetry.md)

A supersymmetric action is invariant under [supersymmetry](supersymmetry.md) up to boundary terms. For ordinary four-dimensional [chiral superfields](#chiral-superfield), a full [superspace integration](#superspace-integration) of a real [Kähler potential](#kahler-potential) and a chiral [superspace integration](#superspace-integration) of a [superpotential](#superpotential) provide the two-derivative ungauged action.

### Two-derivative global supersymmetric gauge action

↑ **Parent:** [Supersymmetric action](#supersymmetric-action)

A two-derivative four-dimensional $\mathcal N=1$ gauge action is specified by a real gauge-invariant [Kähler potential](#kahler-potential), a gauge-invariant holomorphic [superpotential](#superpotential), and a holomorphic symmetric [gauge kinetic function](#gauge-kinetic-function). A constant [Fayet–Iliopoulos term](#fayet-iliopoulos-term) is additionally allowed for an Abelian gauge factor. Renormalizability restricts the matter kinetic function to a quadratic form, the superpotential to degree at most three, and the gauge kinetic function to a constant invariant tensor.

### Gauge kinetic function

↑ **Parent:** [Supersymmetric action](#supersymmetric-action)

The gauge kinetic function is a symmetric [holomorphic function](complex-analysis.md#holomorphic-function) of [chiral superfields](#chiral-superfield) multiplying the gauge field-strength [F-term](#f-term). Its real part controls gauge kinetic coefficients and its imaginary part controls topological-angle terms. Its Wilsonian perturbative correction is constrained by [one-loop exactness of the holomorphic gauge kinetic function](#one-loop-exactness-of-the-holomorphic-gauge-kinetic-function); canonical and one-particle-irreducible gauge couplings require separate normalization and infrared analysis.

// Target: supersymmetry.bigb

#### Holomorphic gauge coupling

↑ **Parent:** [Gauge kinetic function](#gauge-kinetic-function)

A holomorphic gauge coupling is the coefficient of the gauge kinetic [F-term](#f-term) in a local [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action) written in holomorphic variables. In a common normalization its real part is $1/g_h^2$. The continuous perturbative shift of its topological angle, together with holomorphy, restricts its beta function to one-loop order. [Wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) and anomalous canonical field rescalings distinguish it from the physical gauge coupling.

// Target: supersymmetry.bigb

### Grassmann-valued classical supersymmetric mechanics

↑ **Parent:** [Supersymmetric action](#supersymmetric-action)

A classical supersymmetric mechanical model takes its coordinates in a [Grassmann algebra](linear-algebra.md#grassmann-algebra): the position is even and the fermionic coordinates are odd. Time differentiation is even, while variation with respect to an odd coordinate uses [Grassmann derivatives](linear-algebra.md#grassmann-derivative). For example, moving an odd variation to the left and integrating by parts gives $\delta\int\psi\dot\psi\,dt=2\int\delta\psi\dot\psi\,dt$.

For the real variant $L=\dot x^2/2+U^2/2-\psi_1\dot\psi_1/2+\psi_2\dot\psi_2/2+U'\psi_1\psi_2$, the [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) are

$$
\ddot x=UU'+U''\psi_1\psi_2,\qquad \dot\psi_1=U'\psi_2,\qquad \dot\psi_2=U'\psi_1.
$$

The conserved even energy is $E=\dot x^2/2-U^2/2-U'\psi_1\psi_2$ and the odd [supercharges](#supersymmetry-generator) are $Q_1=\dot x\psi_1-U\psi_2$, $Q_2=\dot x\psi_2-U\psi_1$. For example, $\dot Q_i=U''\psi_1\psi_2\psi_i=0$, since each odd element squares to zero. Also $d(\psi_1\psi_2)/dt=U'(\psi_2^2+\psi_1^2)=0$, which proves $\dot E=0$.

#### First-order zero-energy solution in Grassmann supersymmetric mechanics

↑ **Parent:** [Grassmann-valued classical supersymmetric mechanics](#grassmann-valued-classical-supersymmetric-mechanics)

In the real [Grassmann-valued classical supersymmetric mechanics](#grassmann-valued-classical-supersymmetric-mechanics) variant, impose $\dot x=U(x)$ and $\psi_2=-\psi_1$. Then $\psi_1\psi_2=0$, and differentiating the first-order equation gives $\ddot x=UU'$. The remaining [Euler-Lagrange equations](analysis.md#euler-lagrange-equation) reduce to $\dot\psi_1=-U'\psi_1$. These solutions have $E=0$ but $Q_1=2U\psi_1=-Q_2$, which need not vanish: $d(U\psi_1)/dt=U'U\psi_1-UU'\psi_1=0$.

For $U=1+cx$, one obtains $x(t)=e^{ct}x_0+(e^{ct}-1)/c$ and $\psi_1(t)=e^{-ct}\psi_{10}$ when $c\ne0$. At $c=0$, the limiting solution is $x(t)=x_0+t$, $\psi_1(t)=\psi_{10}$. In either case $Q_1=2(1+cx_0)\psi_{10}$.

### Renormalizable chiral-superfield action

↑ **Parent:** [Supersymmetric action](#supersymmetric-action)

In four spacetime dimensions, power-counting [renormalizability](perturbative-quantum-field-theory.md#renormalizable-quantum-field-theory) restricts an ungauged chiral action to a canonical quadratic [Kähler potential](#kahler-potential), up to transformations, and a [superpotential](#superpotential) of degree at most three. Terms of larger degree belong to an [effective field theory](quantum-field-theory.md#effective-field-theory).

## Worldline supersymmetry algebra

↑ **Parent:** [Supersymmetry](supersymmetry.md)

The spinning particle constraints $\mathcal Q=\psi^mp_m$ and $\mathcal H=p^2/2$ obey $\{\mathcal Q,\mathcal Q\}_D=-2i\mathcal H$ and $\{\mathcal Q,\mathcal H\}_D=0$. In the quantum theory $\widehat{\mathcal Q}^{\,2}=\widehat{\mathcal H}$, so the fermionic physical-state equation implies the mass-shell equation.

## Supersymmetric localization

↑ **Parent:** [Supersymmetry](supersymmetry.md)

A symmetry-preserving deformation can leave protected observables unchanged while concentrating their integral on a smaller critical locus. [Supersymmetric Ward identities](#supersymmetric-ward-identity) justify the deformation; convergence and boundary terms must be controlled.

### Localization of a zero-dimensional polynomial model

↑ **Parent:** [Supersymmetric localization](#supersymmetric-localization)

With $P=W^{\prime}$ a nonconstant polynomial, positive area measure and [Berezin integration](quantum-mechanics.md#berezin-integral) oriented positively, a holomorphic polynomial insertion in $S=|P|^2-P^{\prime}\theta_1\theta_2-\overline{P^{\prime}}\bar\theta_1\bar\theta_2$ equals $\pi\sum_a m_a f(z_a)$, where $P(z_a)=0$ and $m_a$ is the [multiplicity of a root](polynomial.md#multiplicity-of-a-root). Rescaling $P$ by $t>0$ leaves the insertion fixed and localizes it as $t\to\infty$.

## Supersymmetric Ward identity

↑ **Parent:** [Supersymmetry](supersymmetry.md)

If an odd [graded derivation](commutative-algebra.md#graded-derivation) $Q$ preserves the action and integration measure, then $\langle QX\rangle=0$ whenever boundary contributions and anomalies vanish. This applies to finite-dimensional [zero-dimensional supersymmetric field theories](#zero-dimensional-supersymmetric-field-theory) as well as suitably regulated field integrals.

## Zero-dimensional supersymmetric field theory

↑ **Parent:** [Supersymmetry](supersymmetry.md)

A zero-dimensional model is a finite-dimensional integral with bosonic and [Grassmann variables](linear-algebra.md#grassmann-variable), rather than a field depending on spacetime. Odd [graded derivations](commutative-algebra.md#graded-derivation) preserve its action and integration measure. Such models expose [supersymmetric Ward identities](#supersymmetric-ward-identity) and [supersymmetric localization](#supersymmetric-localization) without spacetime dynamics.

### Odd symmetries of a zero-dimensional polynomial model

↑ **Parent:** [Zero-dimensional supersymmetric field theory](#zero-dimensional-supersymmetric-field-theory)

For $P=W^{\prime}$ and $S=|P|^2-P^{\prime}\theta_1\theta_2-\overline{P^{\prime}}\bar\theta_1\bar\theta_2$, four odd [graded derivations](commutative-algebra.md#graded-derivation) preserve $S$: $\theta_1\partial_z-\bar P\partial_{\theta_2}$, $\theta_2\partial_z+\bar P\partial_{\theta_1}$ and their barred counterparts. [Left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative) fix the signs.

## Extended supersymmetry

↑ **Parent:** [Supersymmetry](supersymmetry.md)

In four-dimensional [Minkowski spacetime](special-relativity.md#minkowski-spacetime), extended [supersymmetry](supersymmetry.md) has more than one independent [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) [supercharge](#supersymmetry-generator), together with their adjoints. The index $A=1,\ldots,\mathcal N$ distinguishes these [supercharges](#supersymmetry-generator).

### Chirality constraint on extended supersymmetry

↑ **Parent:** [Extended supersymmetry](#extended-supersymmetry)

In a four-dimensional theory with unbroken $\mathcal N\ge2$ [supersymmetry](supersymmetry.md), a full charged [hypermultiplet](#hypermultiplet) contains $\mathcal N=1$ [chiral superfields](#chiral-superfield) in $R$ and $\overline R$. Their net complex [chiral gauge spectrum](relativistic-quantum-field.md#chiral-gauge-spectrum) vanishes. The [vector multiplet](#supersymmetric-vector-multiplet) is in the real adjoint [gauge group representation](relativistic-quantum-field.md#gauge-group-representation). Half-[hypermultiplets](#hypermultiplet) in [pseudoreal representations](representation-theory.md#pseudoreal-representation) do not supply genuinely complex gauge chirality. Thus the chiral matter of the [Standard Model](standard-model.md) can have at most unbroken $\mathcal N=1$ [supersymmetry](supersymmetry.md) in four dimensions.

### Hypermultiplet

↑ **Parent:** [Extended supersymmetry](#extended-supersymmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypermultiplet)

A full four-dimensional $\mathcal N=2$ hypermultiplet is a matter [supermultiplet](#supermultiplet) equivalent to two $\mathcal N=1$ [chiral superfields](#chiral-superfield) in conjugate [gauge group representations](relativistic-quantum-field.md#gauge-group-representation). [Pseudoreal representations](representation-theory.md#pseudoreal-representation) can admit half-hypermultiplets; these do not provide genuinely complex [chiral gauge spectra](relativistic-quantum-field.md#chiral-gauge-spectrum).

<h2 id="two-dimensional-n-2-2-supersymmetry">Two-dimensional N=(2,2) supersymmetry</h2>

↑ **Parent:** [Supersymmetry](supersymmetry.md)

Two-dimensional $\mathcal N=(2,2)$ supersymmetry has independent left- and right-moving complex supercharges. Its superspace uses $\theta^\pm,\bar\theta^\pm$ and supports both chiral and twisted chiral superfields.

### Twisted chiral superfield

↑ **Parent:** [Two-dimensional N=(2,2) supersymmetry](#two-dimensional-n-2-2-supersymmetry)

A twisted chiral superfield obeys $\bar D_+\Sigma=D_-\Sigma=0$. In an Abelian gauge theory the field-strength multiplet $\Sigma=\bar D_+D_-V$ is gauge invariant and twisted chiral.

#### Twisted superpotential

↑ **Parent:** [Twisted chiral superfield](#twisted-chiral-superfield)

A twisted superpotential is a holomorphic function of twisted chiral superfields integrated over $d\theta^+d\bar\theta^-$ superspace. Its highest component varies by a spacetime total derivative under two-dimensional N=(2,2) supersymmetry.

<h2 id="two-dimensional-n-0-2-supersymmetry">Two-dimensional N=(0,2) supersymmetry</h2>

↑ **Parent:** [Supersymmetry](supersymmetry.md)

Two-dimensional $\mathcal N=(0,2)$ supersymmetry retains one complex right-moving supercharge. Its basic matter multiplets are chiral superfields containing a scalar and right-moving fermion, and Fermi superfields containing a left-moving fermion and an auxiliary scalar.

### Fermi superfield

↑ **Parent:** [Two-dimensional N=(0,2) supersymmetry](#two-dimensional-n-0-2-supersymmetry)

A Fermi superfield $\Lambda_-^a$ obeys $\bar D_+\Lambda_-^a=f_a(\Phi)$. A supersymmetric $J$-type coupling $\int d\theta^+\Lambda_-^aJ^a(\Phi)$ requires $\sum_af_aJ^a=0$.

<h2 id="four-dimensional-n-1-supersymmetry">Four-dimensional N=1 supersymmetry</h2>

↑ **Parent:** [Supersymmetry](supersymmetry.md)

Four-dimensional $\mathcal N=1$ supersymmetry has one Weyl-spinor supercharge and four real supercharges.

<h3 id="super-poincare-group">Super-Poincaré group</h3>

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)

The [Super-Poincaré group](#super-poincare-group) combines [Lorentz transformations](special-relativity.md#lorentz-transformation) and [supertranslations](#supertranslation). Its even part acts by spin-group transformations and ordinary spacetime translations; odd parameters generate the [supercharges](#supersymmetry-generator). Their graded commutator closes on translations through the [Super-Poincaré algebra](#super-poincare-algebra). A superspace tensor built from invariant coframes and Lorentz-invariant contractions is invariant under the full group.

### Supercurrent

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)

The supercurrent is the spinor-valued [Noether current](quantum-field-theory.md#noether-current) of rigid [supersymmetry](supersymmetry.md). Its spatial integral is a [supercharge](#supersymmetry-generator). Localizing the [supersymmetry](supersymmetry.md) parameter produces $\partial_\mu\bar\epsilon\,S^\mu$ in the variation of the [action](classical-mechanics.md#action); a [gravitino](#gravitino) coupling cancels this term and starts the [Noether gauging procedure](quantum-field-theory.md#noether-gauging-procedure).

<h3 id="super-poincare-algebra">Super-Poincaré algebra</h3>

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Super-Poincaré_algebra)

The super-Poincaré algebra extends the Poincare algebra by odd spinor generators. In four-dimensional $\mathcal N=1$ supersymmetry, $\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu$ and the equal-chirality anticommutators vanish.

<h4 id="domain-wall-charge-in-n-1-supersymmetry">Domain-wall charge in N=1 supersymmetry</h4>

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

A [supersymmetric domain wall](#supersymmetric-domain-wall) contributes a boundary or tensorial charge to the extended [anticommutator](vector-space.md#anticommutator) of [supercharges](#supersymmetry-generator). It is not the Lorentz-scalar central charge of an extended particle algebra. The wall's energy per unit area can cancel this charge in half the real charge combinations, giving the BPS tension bound and half-supersymmetry preservation. This does not contradict the rank classification for the ordinary algebra without wall charges.

#### Supertranslation

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

A [supertranslation](#supertranslation) is generated by translations and [supercharges](#supersymmetry-generator), excluding the [Lorentz transformations](special-relativity.md#lorentz-transformation). For flat Majorana [superspace](#superspace) with $\Pi^m=dX^m+i\bar\theta\gamma^m d\theta$, the rigid odd transformation $\delta\theta=\epsilon$, $\delta X^m=-i\bar\epsilon\gamma^m\theta$ leaves $\Pi^m$ invariant. Its commutator gives an ordinary translation.

<h4 id="superspace-differential-realization-of-n-1-supercharges">Superspace differential realization of N=1 supercharges</h4>

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

With left [Grassmann derivatives](linear-algebra.md#grassmann-derivative), define $\mathcal P_\mu=-i\partial_\mu$, $\mathcal Q_\alpha=-i\partial_{\theta^\alpha}-\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu$ and $\bar{\mathcal Q}_{\dot\beta}=i\partial_{\bar\theta^{\dot\beta}}+\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu$. The anticommutators of the derivative parts and of the coordinate parts vanish. Each mixed derivative/coordinate pair contributes $-i\sigma^\mu\partial_\mu$ by the graded product rule, giving the displayed mixed [anticommutator](vector-space.md#anticommutator). Equal-chirality anticommutators vanish, and all these operators commute with translations. Under [Lorentz transformations](special-relativity.md#lorentz-transformation) their spinor indices transform in conjugate [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) representations, completing the minimal [Super-Poincaré algebra](#super-poincare-algebra). A convention for left derivatives is essential to the signs.

#### Supercharges commute with translations

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

In the minimal [Super-Poincaré algebra](#super-poincare-algebra), [Lorentz covariance](special-relativity.md#lorentz-covariance) allows $[P^\mu,Q_\alpha]=A\sigma^\mu_{\alpha\dot\beta}\bar Q^{\dot\beta}$. The [graded Jacobi identity](lie-algebra.md#graded-jacobi-identity) with $P^\mu,Q_\alpha,Q_\beta$ forces $A=0$. Thus each [supercharge](#supersymmetry-generator) preserves [four-momentum](special-relativity.md#four-momentum) and its mass Casimir, giving [supersymmetric mass degeneracy](#supersymmetric-mass-degeneracy) in an unbroken physical [supermultiplet](#supermultiplet).

#### Energy positivity in global supersymmetry

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

For $\{Q_\alpha,Q_\beta^\dagger\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu$, summing diagonal components gives $4H$. The expectation of each [anticommutator](vector-space.md#anticommutator) is $\|Q_\alpha v\|^2+\|Q_\alpha^\dagger v\|^2$, so $H$ is a [positive semidefinite operator](hilbert-space.md#positive-operator). A vacuum has zero energy exactly when every [supercharge](#supersymmetry-generator) annihilates it. Spontaneously broken global [supersymmetry](supersymmetry.md) with an existing vacuum therefore gives positive [vacuum energy](perturbative-quantum-field-theory.md#vacuum-energy) density. This statement fixes the energy zero through the algebra and does not apply to the general [supergravity F-term potential](#supergravity-f-term-potential).

<h5 id="nullity-of-real-n-1-supercharges">Nullity of real N=1 supercharges</h5>

↑ **Parent:** [Energy positivity in global supersymmetry](#energy-positivity-in-global-supersymmetry)

For a normalized state in a [unitary representation](representation-theory.md#unitary-representation) of the ordinary four-dimensional [Super-Poincaré algebra](#super-poincare-algebra), define $M_{ab}=\langle\{Q_a,Q_b\}\rangle/2$ in a real Hermitian charge basis. Then $\|u\cdot Q\,\psi\|^2=u^TMu$, so its annihilator is precisely the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) represented by the positive matrix $M$. In a suitable real basis its [eigenvalues](linear-operator-theory.md#eigenvalue) are the two [eigenvalues](linear-operator-theory.md#eigenvalue) of $\langle P^0\rangle I+\langle\mathbf P\rangle\cdot\boldsymbol\sigma$, each repeated twice. A nonzero kernel therefore has dimension two at nonzero null momentum expectation or four at zero expectation. Complex non-Hermitian lowering operators and algebras with domain-wall extensions are not covered by this argument.

#### Central charge in supersymmetry

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

A central charge in four-dimensional [extended supersymmetry](#extended-supersymmetry) is a [Lorentz scalar](special-relativity.md#lorentz-scalar) even generator appearing in $\{Q_\alpha^A,Q_\beta^B\}=\epsilon_{\alpha\beta}Z^{AB}$. It commutes with the displayed translation, [Lorentz algebra](semisimple-lie-algebra.md#lorentz-algebra), and [supercharge](#supersymmetry-generator) generators. An added [R-symmetry](#r-symmetry) automorphism can act on the central charges.

##### BPS bound in supersymmetry

↑ **Parent:** [Central charge in supersymmetry](#central-charge-in-supersymmetry)

Use $\{Q^A_\alpha,Q^B_\beta\}=\epsilon_{\alpha\beta}Z^{AB}$. [Unitary skew-diagonalization of an antisymmetric matrix](linear-algebra.md#unitary-skew-diagonalization-of-an-antisymmetric-matrix) gives two-by-two blocks with entries $Z_r=2z_r$. At rest, the paired [supercharges](#supersymmetry-generator) have [anticommutators](vector-space.md#anticommutator) $2(M\pm|z_r|)$. The squared [norms](functional-analysis.md#norm) of an operator and its adjoint sum to the expectation of their [anticommutator](vector-space.md#anticommutator), so positive [norm](functional-analysis.md#norm) requires $M\ge|z_r|$ for every block. A convention with $2Z$ in the algebra instead writes $M\ge\max|Z_r|$.

###### BPS state

↑ **Parent:** [BPS bound in supersymmetry](#bps-bound-in-supersymmetry)

A [BPS state](#bps-state) saturates a [BPS bound in supersymmetry](#bps-bound-in-supersymmetry). The zero-norm combinations of [supercharges](#supersymmetry-generator) and their adjoints annihilate its entire irreducible [supermultiplet](#supermultiplet). Thus part of the [supersymmetry](supersymmetry.md) is preserved. For a positive-mass representation, its [massive supermultiplet](#massive-supermultiplet) is shortened; [massless supermultiplets](#massless-supermultiplet) require the separate null-momentum construction. Charge conjugation can require a separate conjugate multiplet in the physical spectrum.

###### Wall of marginal stability

↑ **Parent:** [BPS state](#bps-state)

A wall of marginal stability is a locus in the parameter or vacuum space where the complex [central charges in supersymmetry](#central-charge-in-supersymmetry) of possible decay products align in phase. The [triangle inequality](topological-analysis.md#triangle-inequality) then becomes an equality, $|Z_1+Z_2|=|Z_1|+|Z_2|$, permitting a [BPS state](#bps-state) to reach the threshold for decay into other [BPS states](#bps-state). Away from such alignment, the strict triangle inequality can prohibit the decay. Supersymmetry protects the mass-charge relation of an existing short state; it does not guarantee that the state exists or remains stable everywhere in parameter space.

#### Supersymmetry generator

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

A supersymmetry generator is an odd [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) generator of the [Super-Poincaré algebra](#super-poincare-algebra). Acting on a physical state reverses [fermion parity](topological-quantum-matter.md#fermion-parity) while preserving its [four-momentum](special-relativity.md#four-momentum).

##### Supersymmetry transformation

↑ **Parent:** [Supersymmetry generator](#supersymmetry-generator)

A [supersymmetry transformation](#supersymmetry-transformation) is the infinitesimal action generated by an odd [supercharge](#supersymmetry-generator), with constant anticommuting spinor parameter in a global theory. In [superspace](#superspace) it acts as $\delta\mathcal S=(\epsilon Q+\bar\epsilon\bar Q)\mathcal S$, with possible conventional overall factors of $i$. On the fermion of a [chiral superfield](#chiral-superfield), the transformation includes $\delta\psi=\sqrt2\epsilon F_{\mathrm{aux}}+i\sqrt2\sigma^\mu\bar\epsilon\,\partial_\mu\phi$. A nonzero vacuum [auxiliary field](#auxiliary-field) therefore gives an inhomogeneous fermion shift, identifying the [Goldstino](#goldstino) direction when global [supersymmetry](supersymmetry.md) is spontaneously broken.

##### Jacobi sign test for supercharge components

↑ **Parent:** [Supersymmetry generator](#supersymmetry-generator)

Let $[J_i,q_a]=(R_i)_{ab}q_b$, with numerical coefficient matrices and $[J_i,J_j]=i\epsilon_{ijk}J_k$. The [Jacobi identity](lie-algebra.md#jacobi-identity) then gives $(R_jR_i-R_iR_j)q=i\epsilon_{ijk}R_kq$, so component coefficient matrices obey the opposite bracket to state-representation matrices. Thus $R_i=-\sigma_i/2$ is consistent for an upper-column spinor, whereas $+\sigma_i/2$ in that same component prescription is not. Inverse adjoint actions and dual row conventions must be compared with their index contractions intact.

<h4 id="coleman-mandula-theorem">Coleman–Mandula theorem</h4>

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coleman–Mandula_theorem)

Under standard assumptions on a nontrivial analytic relativistic S-matrix, the Coleman–Mandula theorem says that every continuous bosonic symmetry algebra is a direct sum of the Poincare algebra and an internal symmetry algebra.

<h5 id="haag-lopuszanski-sohnius-theorem">Haag–Łopuszański–Sohnius theorem</h5>

↑ **Parent:** [Coleman–Mandula theorem](#coleman-mandula-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Haag–Łopuszański–Sohnius_theorem)

The Haag–Łopuszański–Sohnius theorem allows a Z2-graded Lie superalgebra and shows that supersymmetry, including possible central charges and R-symmetries, is the nontrivial fermionic extension compatible with an interacting relativistic S-matrix.

#### Superspin Casimir

↑ **Parent:** [Super-Poincaré algebra](#super-poincare-algebra)

The superspin Casimir classifies massive supermultiplets analogously to the Pauli-Lubanski Casimir for Poincare representations. One construction contracts the tensor $C_{\mu\nu}=B_\mu P_\nu-B_\nu P_\mu$, where $B_\mu$ is the supersymmetric correction of the Pauli-Lubanski pseudovector.

### Supermultiplet

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supermultiplet)

A supermultiplet is an irreducible representation of the [Super-Poincaré algebra](#super-poincare-algebra). Conserved supercharges pair its bosonic and fermionic states at equal four-momentum.

#### Chiral multiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

A four-dimensional N=1 [chiral multiplet](#chiral-multiplet) consists off shell of a [complex scalar](scalar-field-theory.md#complex-scalar-field) $\phi$, a Weyl [fermion](quantum-mechanics.md#fermion) $\psi_\alpha$, and a complex auxiliary scalar $F$. A [chiral superfield](#chiral-superfield) packages their [supersymmetry](supersymmetry.md) transformations. Eliminating the auxiliary scalar leaves two bosonic and two fermionic physical polarizations; an allowed supersymmetric mass gives equal scalar and [fermion](quantum-mechanics.md#fermion) masses.

#### Massive supermultiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

A [massive supermultiplet](#massive-supermultiplet) is a [unitary irreducible representation](representation-theory.md#unitary-irreducible-representation) of the [Super-Poincaré algebra](#super-poincare-algebra) with positive timelike momentum. At rest, its nonzero [supercharges](#supersymmetry-generator) become [fermionic creation operators](relativistic-quantum-field.md#fermionic-creation-operator) and [fermionic annihilation operators](relativistic-quantum-field.md#fermionic-annihilation-operator). Without [central charges in supersymmetry](#central-charge-in-supersymmetry), four-dimensional extended [supersymmetry](supersymmetry.md) has $2\mathcal N$ complex oscillators; a spin-$j$ [Clifford vacuum](quantum-mechanics.md#clifford-vacuum) gives $(2j+1)2^{2\mathcal N}$ states.

##### Superspin

↑ **Parent:** [Massive supermultiplet](#massive-supermultiplet)

For a massive four-dimensional N=1 [supermultiplet](#supermultiplet), [superspin](#superspin) $j$ is the [spin](quantum-mechanics.md#spin) of its [Clifford vacuum](quantum-mechanics.md#clifford-vacuum), the state annihilated by the two lowering [supercharges](#supersymmetry-generator). The creation operators produce spins $j,j,j+1/2,j-1/2$, omitting the last when $j=0$. The corresponding [superspin](#superspin) Casimir has an [eigenvalue](linear-operator-theory.md#eigenvalue) proportional to $j(j+1)$; this representation label is distinct from the [spin](quantum-mechanics.md#spin) of any one constituent.

<h5 id="spin-zero-massive-n-1-supermultiplet">Spin-zero massive N=1 supermultiplet</h5>

↑ **Parent:** [Massive supermultiplet](#massive-supermultiplet)

At rest the two complex [supercharges](#supersymmetry-generator) have [anticommutators](vector-space.md#anticommutator) $2m\delta_{ab}$. A normalized scalar [Clifford vacuum](quantum-mechanics.md#clifford-vacuum) generates four states at occupation levels $0,1,2$: two spin-zero bosonic states and one spin-half pair. Products of three creation charges vanish. The one-creation normalization is $(2m)^{-1/2}$ and the two-creation normalization is $(2m)^{-1}$. The resulting on-shell content is a [complex scalar](scalar-field-theory.md#complex-scalar-field) and a massive [fermion](quantum-mechanics.md#fermion) with equal masses.

##### Shortened massive supermultiplet

↑ **Parent:** [Massive supermultiplet](#massive-supermultiplet)

For $\mathcal N$ supersymmetries and $k$ saturated two-by-two central-charge blocks, $2k$ complex oscillators act trivially. A spin-$j$ [Clifford vacuum](quantum-mechanics.md#clifford-vacuum) therefore gives $(2j+1)2^{2\mathcal N-2k}$ states and preserves $4k$ of the $4\mathcal N$ real [supercharges](#supersymmetry-generator). With $\mathcal N=2$ and a scalar vacuum, the shortened multiplet has two [boson](quantum-mechanics.md#boson) states and two [fermion](quantum-mechanics.md#fermion) states, before any [CPT completion of a supermultiplet](#cpt-completion-of-a-supermultiplet).

#### Supersymmetric vector multiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

A supersymmetric vector multiplet contains a [gauge boson](relativistic-quantum-field.md#gauge-boson) and its [gaugino](#gaugino) partners, with additional [scalar fields](quantum-field-theory.md#scalar-field) for [extended supersymmetry](#extended-supersymmetry). Its [gauge group representation](relativistic-quantum-field.md#gauge-group-representation) is the adjoint [group representation](representation-theory.md#group-representation).

<h5 id="massive-n-1-vector-multiplet">Massive N=1 vector multiplet</h5>

↑ **Parent:** [Supersymmetric vector multiplet](#supersymmetric-vector-multiplet)

A four-dimensional massive $\mathcal N=1$ [vector multiplet](#supersymmetric-vector-multiplet) contains one spin-one particle, two spin-one-half particles and one real spin-zero particle. Its on-shell state counts are $3+1=4$ bosonic and $2+2=4$ fermionic. These masses agree in an unbroken [supersymmetric vacuum](#supersymmetric-vacuum). The [supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism) assembles it from a massless [vector multiplet](#supersymmetric-vector-multiplet) and one [chiral superfield](#chiral-superfield) per broken gauge generator.

<h6 id="massless-limit-of-a-massive-n-1-vector-multiplet">Massless limit of a massive N=1 vector multiplet</h6>

↑ **Parent:** [Massive N=1 vector multiplet](#massive-n-1-vector-multiplet)

The [massive N=1 vector multiplet](#massive-n-1-vector-multiplet) contains [spins](quantum-mechanics.md#spin) $1,1/2,1/2,0$. Its massless [helicity](special-relativity.md#helicity) content splits into a CPT-complete [vector multiplet](#supersymmetric-vector-multiplet) with helicities $(1,1/2)$ and $(-1/2,-1)$, and a CPT-complete [chiral multiplet](#chiral-multiplet) with helicities $(1/2,0)$ and $(0,-1/2)$. The longitudinal vector polarization becomes one of the two scalar polarizations; the other comes from the original real scalar. This is the representation-theoretic inverse of the [supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism).

#### CPT completion of a supermultiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

The [CPT theorem](quantum-field-theory.md#cpt-theorem) reverses [helicity](special-relativity.md#helicity) and conjugates internal charges. If a [supermultiplet](#supermultiplet) is not mapped into itself, a physical spectrum must also include its conjugate [supermultiplet](#supermultiplet); this can double the irreducible state count.

#### Massless supermultiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

A massless [supermultiplet](#supermultiplet) is a positive-energy [unitary irreducible representation](representation-theory.md#unitary-irreducible-representation) of the [Super-Poincaré algebra](#super-poincare-algebra) with null [four-momentum](special-relativity.md#four-momentum). For finite [helicity](special-relativity.md#helicity) states in four dimensions, half the [supercharges](#supersymmetry-generator) act trivially and the others form a [fermionic Fock space](quantum-mechanics.md#fermionic-fock-space).

##### Superhelicity

↑ **Parent:** [Massless supermultiplet](#massless-supermultiplet)

For a four-dimensional $\mathcal N=1$ finite-helicity [massless supermultiplet](#massless-supermultiplet), one complex oscillator changes [helicity](special-relativity.md#helicity) by one-half. A lower-helicity labelling convention assigns $\kappa$ to the pair $(\kappa,\kappa+1/2)$. A symmetric midpoint convention instead uses $\kappa+1/4$; report the [helicity](special-relativity.md#helicity) pair when comparing conventions. [CPT completion of a supermultiplet](#cpt-completion-of-a-supermultiplet) pairs $\kappa$ with $-\kappa-1/2$.

##### Helicity spectrum of a massless supermultiplet

↑ **Parent:** [Massless supermultiplet](#massless-supermultiplet)

For a four-dimensional [massless supermultiplet](#massless-supermultiplet) with $\mathcal N$ independent [supercharges](#supersymmetry-generator) and highest [helicity](special-relativity.md#helicity) $\lambda$, level $k$ has [helicity](special-relativity.md#helicity) $\lambda-k/2$ and multiplicity $\binom{\mathcal N}{k}$. The total is $2^{\mathcal N}$ states and the [helicity](special-relativity.md#helicity) range has width $\mathcal N/2$, before any necessary [CPT completion of a supermultiplet](#cpt-completion-of-a-supermultiplet).

###### Spin bound for massless supermultiplets

↑ **Parent:** [Helicity spectrum of a massless supermultiplet](#helicity-spectrum-of-a-massless-supermultiplet)

In four-dimensional [supersymmetry](supersymmetry.md), a finite-[helicity](special-relativity.md#helicity) [massless supermultiplet](#massless-supermultiplet) has [helicity](special-relativity.md#helicity) interval of width $\mathcal N/2$. If every state obeys $|h|\le s$, that interval fits inside one of width $2s$, giving $\mathcal N\le4s$. The bounds $4$ for $s=1$ and $8$ for $s=2$ are attained by the [four-dimensional N=4 super Yang-Mills theory](#four-dimensional-n-4-super-yang-mills-theory) [vector multiplet](#supersymmetric-vector-multiplet) and the [four-dimensional N=8 supergravity](#four-dimensional-n-8-supergravity) [supergravity multiplet](#supergravity-multiplet). Spin bounds alone do not prove that an arbitrary action is renormalizable.

#### Boson-fermion degeneracy in a supermultiplet

↑ **Parent:** [Supermultiplet](#supermultiplet)

Every positive-energy supermultiplet contains equally many bosonic and fermionic states. A supertrace of a positive supercharge anticommutator proves the equality, provided supersymmetry is exact and the representation is finite-dimensional at fixed momentum.

##### Supertrace pairing at positive energy

↑ **Parent:** [Boson-fermion degeneracy in a supermultiplet](#boson-fermion-degeneracy-in-a-supermultiplet)

For a finite physical [supermultiplet](#supermultiplet) at fixed positive energy, [fermion parity](topological-quantum-matter.md#fermion-parity) anticommutes with each odd [supercharge](#supersymmetry-generator). Trace cyclicity makes $\operatorname{Tr}[(-1)^F\{Q,Q^\dagger\}]=0$. Summing the [Super-Poincaré algebra](#super-poincare-algebra) diagonal entries replaces the anticommutator by $4E$, giving equal bosonic and fermionic state counts. A zero-energy vacuum is an exception to the division by $E$, so it need not have a partner. The argument requires an invariant fixed-momentum representation, which is the step lost under explicit supersymmetry breaking.

##### Odd involution pairing bosonic and fermionic states

↑ **Parent:** [Boson-fermion degeneracy in a supermultiplet](#boson-fermion-degeneracy-in-a-supermultiplet)

An odd [involution](group-theory.md#involution) $A$ reverses [fermion parity](topological-quantum-matter.md#fermion-parity) and is its own inverse, so it identifies the bosonic and fermionic subspaces. They have equal dimension in a finite-dimensional representation. For a [supercharge](#supersymmetry-generator) $q$ with $q^2=0$ and $\{q,q^\dagger\}=cI$, $c>0$, use $A=(q+q^\dagger)/\sqrt c$. This gives a direct proof of [boson-fermion degeneracy in a supermultiplet](#boson-fermion-degeneracy-in-a-supermultiplet) at positive energy. A zero-energy supersymmetric vacuum need not have an accompanying fermionic vacuum.

##### Supersymmetric mass degeneracy

↑ **Parent:** [Boson-fermion degeneracy in a supermultiplet](#boson-fermion-degeneracy-in-a-supermultiplet)

In an unbroken [supersymmetric vacuum](#supersymmetric-vacuum), physical [boson](quantum-mechanics.md#boson) and [fermion](quantum-mechanics.md#fermion) partners have equal masses because [supercharges](#supersymmetry-generator) commute with [four-momentum](special-relativity.md#four-momentum). For one canonical [chiral superfield](#chiral-superfield), fluctuations about $W'(v)=0$ have mass $|W''(v)|$ for both the [complex scalar field](scalar-field-theory.md#complex-scalar-field) and [Weyl spinor](relativistic-quantum-field.md#weyl-spinor).

###### Complex scalar mass at a supersymmetric critical point

↑ **Parent:** [Supersymmetric mass degeneracy](#supersymmetric-mass-degeneracy)

For one canonical chiral field at $W'(v)=0$, the quadratic [scalar potential](quantum-field-theory.md#scalar-potential) is $|W''(v)|^2|\delta\varphi|^2$. Writing $\delta\varphi=(a+ib)/\sqrt2$ gives two canonically normalized real scalars with squared mass $|W''(v)|^2$. The [chiral-superfield fermion mass matrix](#chiral-superfield-fermion-mass-matrix) has the same physical mass. A complex bilinear coefficient or its algebraic square is not itself a signed physical squared mass.

### Superspace

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superspace)

Superspace extends spacetime coordinates $x^\mu$ by anticommuting spinor coordinates $\theta^\alpha$ and $\bar\theta^{\dot\alpha}$.

#### Supertranslation-invariant superspace coframe

↑ **Parent:** [Superspace](#superspace)

The displayed one-forms give an invertible triangular change from the coordinate coframe on flat Majorana [superspace](#superspace). A rigid [supertranslation](#supertranslation) has $d\epsilon=0$, and the variation of $dX^m$ cancels that of $i\bar\theta\gamma^m d\theta$. Their [Maurer-Cartan equation](lie-theory.md#maurer-cartan-equation) is $d\Pi^m=i\,d\bar\theta\gamma^m d\theta$. The bosonic frame transforms as a Lorentz vector and the odd frame as a [Majorana spinor](relativistic-quantum-field.md#majorana-spinor).

##### Closed three-form on four-dimensional superspace

↑ **Parent:** [Supertranslation-invariant superspace coframe](#supertranslation-invariant-superspace-coframe)

The contraction of invariant vector and spinor frames makes $H_3$ invariant under the [Super-Poincaré group](#super-poincare-group). Odd-coordinate differentials commute in the graded exterior algebra. The four-dimensional [Fierz rearrangement](quantum-field-theory.md#fierz-identity) identity $(C\gamma^m)_{(\alpha\beta}(C\gamma_m)_{\gamma\delta)}=0$ consequently gives $dH_3=i(d\bar\theta\gamma^m d\theta)(d\bar\theta\gamma_m d\theta)=0$. Its three-form degree is distinct from the four-form needed in the [four-dimensional supermembrane](string-theory.md#four-dimensional-supermembrane) Wess-Zumino coupling.

#### Supervielbein

↑ **Parent:** [Superspace](#superspace)

The supervielbein is the local frame of a superspace geometry. Pulling its bosonic-frame components back along a brane embedding gives $\Pi_i^a=\partial_iZ^{\mathcal M}E_{\mathcal M}{}^a$, and hence the [induced worldvolume metric](string-theory.md#induced-worldvolume-metric) $h_{ij}=\Pi_i^a\Pi_j^b\eta_{ab}$. Fermionic coordinates remain present through their dependence on $Z$.

// Target: string-theory.bigb

#### Kappa symmetry

↑ **Parent:** [Superspace](#superspace)

A local fermionic gauge symmetry of supersymmetric [brane](string-theory.md#brane) actions. Since the [kappa symmetry projector](#kappa-symmetry-projector) has half rank, the symmetry removes half the embedding fermions. The remaining physical fermions pair with the bosonic worldvolume degrees of freedom.

##### Kappa symmetry projector

↑ **Parent:** [Kappa symmetry](#kappa-symmetry)

With $\Gamma_\kappa^2=1$, the two complementary [linear projections](vector-space.md#projection-linear-algebra) select its two eigenspaces. A bosonic brane preserves a background [Killing spinor](#killing-spinor) precisely when its target-space supersymmetry variation can be compensated by [kappa symmetry](#kappa-symmetry), giving $\Gamma_\kappa\epsilon=\epsilon$. This condition must hold at every worldvolume point; several branes require a common solution. The full superspace construction is described in [Superspace Geometry for Supermembrane Backgrounds](https://arxiv.org/abs/hep-th/9803209).

<h4 id="two-dimensional-n-1-1-superspace">Two-dimensional N=(1,1) superspace</h4>

↑ **Parent:** [Superspace](#superspace)

In [light-cone coordinates](special-relativity.md#light-cone-coordinates) $x^\pm$ on two-dimensional [Minkowski spacetime](special-relativity.md#minkowski-spacetime), add two real odd [Grassmann variables](linear-algebra.md#grassmann-variable) $\theta^\pm$. With [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), the [supercharges](#supersymmetry-generator) and [supersymmetric covariant derivatives](#supersymmetric-covariant-derivative) can be represented as

$$
Q_\pm=\partial_{\theta^\pm}+i\theta^\pm\partial_\pm,\qquad D_\pm=\partial_{\theta^\pm}-i\theta^\pm\partial_\pm.
$$

The identity $\{\partial_\theta,\theta\}=1$ gives $Q_\pm^2=i\partial_\pm$, $D_\pm^2=-i\partial_\pm$, $\{Q_+,Q_-\}=\{D_+,D_-\}=0$, and $\{Q_s,D_t\}=0$ for every $s,t$. A [Lorentz boost](special-relativity.md#lorentz-boost) acts as $x^\pm\mapsto e^{\pm\omega}x^\pm$, $\theta^\pm\mapsto e^{\pm\omega/2}\theta^\pm$. Thus $D_\pm$ have boost weights $\mp1/2$, and $D_-D_+$ is a [Lorentz scalar](special-relativity.md#lorentz-scalar). Since it commutes with both [supercharges](#supersymmetry-generator), an equation $iD_-D_+\Phi=W(\Phi)$ for an even scalar [superfield](#superfield) is [Lorentz invariant](special-relativity.md#lorentz-invariance) and [supersymmetry](supersymmetry.md) covariant.

##### Supersymmetric Liouville equation

↑ **Parent:** [Two-dimensional N=(1,1) superspace](#two-dimensional-n-1-1-superspace)

In [two-dimensional N=(1,1) superspace](#two-dimensional-n-1-1-superspace), one convention for the supersymmetric Liouville equation is $iD_-D_+\Phi=e^\Phi$. With the ordered expansion $\Phi=\phi+i\theta^-\psi_++i\theta^+\psi_-+i\theta^-\theta^+F$ and [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), its left side is

$$
F+i\theta^-\partial_-\psi_- -i\theta^+\partial_+\psi_+ -i\theta^-\theta^+\partial_-\partial_+\phi.
$$

Writing $N=\Phi-\phi$, [Grassmann parity](linear-algebra.md#grassmann-parity) gives $N^2=2\theta^-\theta^+\psi_+\psi_-$ and $N^3=0$. Hence

$$
e^\Phi=e^\phi[1+i\theta^-\psi_++i\theta^+\psi_-+\theta^-\theta^+(iF+\psi_+\psi_-)].
$$

Comparing coefficients eliminates the [auxiliary field](#auxiliary-field) as $F=e^\phi$ and gives $\partial_-\psi_-=e^\phi\psi_+$, $\partial_+\psi_+=-e^\phi\psi_-$, $\partial_-\partial_+\phi=-e^{2\phi}+ie^\phi\psi_+\psi_-$. The fermion bilinear sign depends on the stated ordering and derivative convention.

#### Two-component superspace contraction signs

↑ **Parent:** [Superspace](#superspace)

For [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), $\epsilon^{12}=-\epsilon_{12}=1$, $\theta\theta=\theta^\alpha\theta_\alpha$ and $\bar\theta\bar\theta=\bar\theta_{\dot\alpha}\bar\theta^{\dot\alpha}$, the antisymmetric products are $\theta^\alpha\theta^\beta=-\epsilon^{\alpha\beta}\theta\theta/2$ and $\bar\theta^{\dot\alpha}\bar\theta^{\dot\beta}=\epsilon^{\dot\alpha\dot\beta}\bar\theta\bar\theta/2$. With contractions $\partial^2=\partial^\alpha\partial_\alpha$ and $\bar\partial^2=\bar\partial_{\dot\alpha}\bar\partial^{\dot\alpha}$, both squared derivatives give $-4$ on the matching quadratic monomial. If $\operatorname{Tr}(\sigma^\mu\bar\sigma^\nu)=2\eta^{\mu\nu}$, the mixed bilinear product is $+(\theta\theta)(\bar\theta\bar\theta)\eta^{\mu\nu}/2$. Reversing the metric-relative trace convention reverses this last sign.

#### Superspace integration

↑ **Parent:** [Superspace](#superspace)

Superspace integration uses the [Berezin integral](quantum-mechanics.md#berezin-integral) over [Grassmann variables](linear-algebra.md#grassmann-variable). A chiral $d^2\theta$ integral extracts an [F-term](#f-term), while a full $d^4\theta$ integral extracts a [D-term](#d-term).

#### Superfield

↑ **Parent:** [Superspace](#superspace)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superfield)

A superfield is a function on superspace. Its finite Taylor expansion in Grassmann coordinates packages component fields into a supersymmetry representation.

##### Superfield covariance is not Grassmann dependence alone

↑ **Parent:** [Superfield](#superfield)

A [superfield](#superfield) is a field on [superspace](#superspace) with a specified [Super-Poincaré group](#super-poincare-group) transformation law. Being a polynomial in anticommuting coordinates alone does not specify this law or make coefficients a [supermultiplet](#supermultiplet). Conversely, a suitably graded function on full [superspace](#superspace), acted on by coordinate pullback, is an unconstrained scalar superfield. A polynomial with spacetime-independent coefficients can be a special constant-component [chiral superfield](#chiral-superfield); dependence on spacetime is not itself the defining criterion. Chirality and reality impose additional conditions.

##### Scalar superfield transformation

↑ **Parent:** [Superfield](#superfield)

With [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), let $Q_\alpha=\partial_\alpha-i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu$ and $\bar Q_{\dot\alpha}=\bar\partial_{\dot\alpha}-i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu$. Left-placed odd parameters generate $\delta\theta=\epsilon$, $\delta\bar\theta=\bar\epsilon$ and $\delta x^\mu=i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta$. A scalar [superfield](#superfield) transforms by pullback under this [superspace](#superspace) translation. The parameter-weighted variation is an even [derivation](associative-algebra.md#derivation-of-an-algebra), although each [supercharge](#supersymmetry-generator) is odd.

###### Partial derivatives and superfield covariance

↑ **Parent:** [Scalar superfield transformation](#scalar-superfield-transformation)

A [supersymmetry transformation](#supersymmetry-transformation) mixes the bosonic and odd coordinates of [superspace](#superspace). A bare derivative with respect to an odd coordinate therefore acquires a spacetime-derivative term under the coordinate Jacobian and is not a covariant spinor [superfield](#superfield). [Supersymmetric covariant derivatives](#supersymmetric-covariant-derivative) add terms linear in the other odd coordinate; their graded anticommutation with the [supercharges](#supersymmetry-generator) makes their application to a scalar [superfield](#superfield) transform covariantly.

###### Pure-scalar truncation of a superfield

↑ **Parent:** [Scalar superfield transformation](#scalar-superfield-transformation)

A function $S(x,\theta,\bar\theta)=\phi(x)$ is an allowed special configuration of an unconstrained [superfield](#superfield). The subspace where all other components remain zero is not invariant: $\delta S=(i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta)\partial_\mu\phi$ produces components depending on [Grassmann variables](linear-algebra.md#grassmann-variable) whenever $\phi$ is nonconstant. Thus an isolated spacetime [scalar field](quantum-field-theory.md#scalar-field) is not closed under [supersymmetry](supersymmetry.md). A constant gauge-singlet value is a trivial invariant exception.

###### Product of scalar superfields

↑ **Parent:** [Scalar superfield transformation](#scalar-superfield-transformation)

A product of scalar [superfields](#superfield) is a scalar [superfield](#superfield): the pullback of a product is the product of the pullbacks at the same transformed [superspace](#superspace) point. Infinitesimally, the even supersymmetry variation obeys $\delta(ST)=(\delta S)T+S(\delta T)$. This follows from the [graded Leibniz rule](commutative-algebra.md#graded-leibniz-rule) for the odd [supercharges](#supersymmetry-generator), after including their odd parameters.

##### Vector superfield

↑ **Parent:** [Superfield](#superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vector_superfield)

A vector superfield is a real superfield, $V=V^\dagger$, used to describe a supersymmetric gauge multiplet. In Wess-Zumino gauge its components are a gauge field, a gaugino and a real auxiliary field.

###### Superspace gauge connection

↑ **Parent:** [Vector superfield](#vector-superfield)

A gauge connection on [superspace](#superspace) has both vector and spinor components. Subtracting the flat-frame torsion from the graded commutator of its [covariant derivatives](general-relativity.md#covariant-derivative) defines its supercurvature. The conventional four-dimensional $\mathcal N=1$ spinor-curvature constraints leave one real [vector superfield](#vector-superfield) as a prepotential. Its [chiral field-strength superfield](#chiral-field-strength-superfield) contains the ordinary gauge curvature, [gaugino](#gaugino) and real [auxiliary field](#auxiliary-field).

###### Wess-Zumino gauge

↑ **Parent:** [Vector superfield](#vector-superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wess-Zumino_gauge)

Wess-Zumino gauge uses supergauge freedom to remove the scalar and spinor components of a general vector superfield that do not belong to the physical gauge multiplet.

###### Gauge-transformation superfield

↑ **Parent:** [Vector superfield](#vector-superfield)

In four-dimensional $\mathcal N=1$ supersymmetry, a gauge-transformation superfield is a dimensionless chiral, Lie-algebra-valued parameter $\Lambda$. Its complex nature allows gauge transformations to preserve chirality.

###### Supergauge transformation

↑ **Parent:** [Gauge-transformation superfield](#gauge-transformation-superfield)

A supergauge transformation acts on a charged chiral superfield and vector superfield together. In one common convention, $\Phi'=e^{-2i\Lambda}\Phi$ and $e^{2V'}=e^{-2i\Lambda^\dagger}e^{2V}e^{2i\Lambda}$.

###### D-term scalar potential

↑ **Parent:** [Vector superfield](#vector-superfield)

Eliminating the real auxiliary field $D$ gives a nonnegative D-term scalar potential. For a $U(1)$ theory with charges $q_i$ and a Fayet–Iliopoulos parameter $\xi$, one convention gives $V_D=\tfrac12[g\sum_iq_i|\phi_i|^2+\xi]^2$.

###### Single charged-field D-term breaking

↑ **Parent:** [D-term scalar potential](#d-term-scalar-potential)

For one charged [chiral superfield](#chiral-superfield), canonical kinetic terms, no nonconstant gauge-invariant [superpotential](#superpotential), and $g>0$, the sign of $q\xi$ selects the vacuum. If $q\xi>0$, the minimum has $\phi=0$, positive vacuum energy, unbroken internal gauge symmetry and a [gaugino](#gaugino) [Goldstino](#goldstino); the scalar squared mass is $gq\xi$ while its chiral fermion is massless. If $q\xi<0$, a scalar condensate cancels the auxiliary field, preserving [supersymmetry](supersymmetry.md) while Higgsing the gauge group. These are classical statements; a consistent quantum charged spectrum must cancel its [gauge anomalies](relativistic-quantum-field.md#gauge-anomaly).

###### Mass spectrum of single charged-field D-term breaking

↑ **Parent:** [Single charged-field D-term breaking](#single-charged-field-d-term-breaking)

For canonical kinetic terms, vanishing [superpotential](#superpotential), $g>0$ and $q\xi>0$, the [D-term scalar potential](#d-term-scalar-potential) $V=\tfrac12(\xi+gq|\phi|^2)^2$ has its minimum at $\phi=0$. Both real scalar modes have squared mass $gq\xi$, while the chiral Weyl fermion, photon and [gaugino](#gaugino) are massless; the gaugino is the [goldstino](#goldstino). The scalar-to-fermion squared-mass splitting is $gq\xi$. On the other branch $q\xi<0$, $v^2=-\xi/(gq)$ cancels $D$ and preserves [supersymmetry](supersymmetry.md); the Higgsed vector, remaining real scalar and Dirac fermion have common squared mass $2g^2q^2v^2$. A single nonzero-charge chiral fermion has a [gauge anomaly](relativistic-quantum-field.md#gauge-anomaly), so a quantum realization requires an anomaly-cancelling completion; these are the stated classical vacuum spectra.

###### D-term vacuum branches of a cubic superpotential

↑ **Parent:** [D-term scalar potential](#d-term-scalar-potential)

For canonical [Kähler potential](#kahler-potential), set $a=|\phi_0|^2$, $b=|\phi_+|^2$, $c=|\phi_-|^2$. The supplied [supergravity F-term potential](#supergravity-f-term-potential) is $|\lambda|^2e^{\kappa^2(a+b+c)}[ab+ac+bc+3\kappa^2abc+\kappa^4abc(a+b+c)]$. Adding $g(b-c-\zeta)^2$ with $g>0$, $\lambda\ne0$ and $\zeta>0$ gives a [supersymmetric vacuum](#supersymmetric-vacuum) at $a=c=0$, $b=\zeta$. The branch $b=c=0$ has positive energy $g\zeta^2$, [D-term](#d-term) breaking and a [flat direction of a scalar potential](quantum-field-theory.md#flat-direction-of-a-scalar-potential) in $\phi_0$. Its charged squared masses are $|\lambda|^2ae^{\kappa^2a}\mp2g\zeta$, so it is a [local minimum](analysis.md#local-minimum) valley only when both are positive. For negative $\zeta$, exchange the charged fields. These are branches rather than two isolated minima; a conventional constant [Fayet–Iliopoulos term](#fayet-iliopoulos-term) additionally needs a consistent [supergravity](#supergravity) gauge completion.

<h6 id="fayet-iliopoulos-term">Fayet–Iliopoulos term</h6>

↑ **Parent:** [D-term scalar potential](#d-term-scalar-potential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fayet–Iliopoulos_term)

A Fayet–Iliopoulos term is a gauge-invariant term linear in the auxiliary $D$ field of an Abelian vector multiplet. Supersymmetry is broken only if no charged-scalar configuration can make the shifted D-term vanish simultaneously with every F-term.

<h6 id="constant-fayet-iliopoulos-terms-in-conventional-n-1-supergravity">Constant Fayet–Iliopoulos terms in conventional N=1 supergravity</h6>

↑ **Parent:** [Fayet–Iliopoulos term](#fayet-iliopoulos-term)

In the conventional two-derivative [supergravity](#supergravity) action described by a [Kähler potential](#kahler-potential), [superpotential](#superpotential) and [gauge kinetic function](#gauge-kinetic-function), a constant [Fayet–Iliopoulos term](#fayet-iliopoulos-term) cannot be added independently of the gauging. It makes the Abelian gauging an [R-symmetry](#r-symmetry) gauging, and the superpotential must have the corresponding gauge transformation. Thus the rigid Abelian constant is subject to extra local consistency conditions. This statement concerns the conventional matter-coupled action, not distinct nonstandard FI constructions.

<h6 id="perturbative-renormalization-of-a-fayet-iliopoulos-term">Perturbative renormalization of a Fayet–Iliopoulos term</h6>

↑ **Parent:** [Fayet–Iliopoulos term](#fayet-iliopoulos-term)

In an exactly supersymmetric Abelian theory a one-loop auxiliary-field tadpole can generate a cutoff-dependent [Fayet–Iliopoulos term](#fayet-iliopoulos-term) proportional to the trace of the matter charges. Gauge invariance with arbitrary background [spurions](#spurion) forbids a general coupling-dependent full-superspace coefficient multiplying the vector superfield. In the supersymmetry-preserving Wilsonian setting the additive perturbative correction is exhausted by the one-loop term; it vanishes for a traceless charge generator. Canonical vector normalization and soft breaking require separate treatment. For a simple non-Abelian group the term itself is forbidden.

<h6 id="fayet-iliopoulos-terms-require-an-abelian-gauge-factor">Fayet–Iliopoulos terms require an Abelian gauge factor</h6>

↑ **Parent:** [Fayet–Iliopoulos term](#fayet-iliopoulos-term)

A constant linear auxiliary-field term $\xi_aD^a$ is [gauge-invariant](relativistic-quantum-field.md#gauge-invariance) only when $\xi$ is an invariant vector in the dual adjoint representation. Equivalently, it annihilates all Lie brackets. A simple non-Abelian [Lie algebra](lie-algebra.md) equals its commutator algebra and has no such nonzero vector. Abelian factors do admit the term. Identifying a Fayet–Iliopoulos parameter in a simple non-Abelian theory therefore requires setting it to zero, rather than treating it as an arbitrary coupling.

###### Chiral field-strength superfield

↑ **Parent:** [Vector superfield](#vector-superfield)

For a non-Abelian vector superfield, the chiral field-strength superfield is

$$
W_\alpha=-\frac18\bar D^2\left(e^{-2V}D_\alpha e^{2V}\right).
$$

It obeys $\bar D_{\dot\alpha}W_\alpha=0$ and transforms covariantly under a supergauge transformation.

###### Superspace Yang-Mills Bianchi identity

↑ **Parent:** [Chiral field-strength superfield](#chiral-field-strength-superfield)

For a real Abelian [vector superfield](#vector-superfield), $W_\alpha=-\bar D^2D_\alpha V/4$ is chiral. The [supercovariant derivative algebra with left derivatives](#supercovariant-derivative-algebra-with-left-derivatives) gives $D^\alpha\bar D^2D_\alpha=\bar D_{\dot\alpha}D^2\bar D^{\dot\alpha}$, proving the displayed reality condition. Its component equations contain the ordinary [gauge-theory Bianchi identity](relativistic-quantum-field.md#gauge-theory-bianchi-identity), not the [Maxwell equations](electromagnetism.md#maxwell-equations) of motion. For a non-Abelian [gauge group](relativistic-quantum-field.md#gauge-group), replace these by gauge-covariant derivatives and compare both field strengths in the same gauge frame; the identity follows from the [graded Jacobi identity](lie-algebra.md#graded-jacobi-identity) of the superconnection.

###### Abelian field-strength chiral projection

↑ **Parent:** [Chiral field-strength superfield](#chiral-field-strength-superfield)

For an Abelian [vector superfield](#vector-superfield), the [chiral field-strength superfield](#chiral-field-strength-superfield) is $W_\alpha=-\bar D^2D_\alpha V/4$. Three barred [supersymmetric covariant derivatives](#supersymmetric-covariant-derivative) vanish, proving $\bar D_{\dot\beta}W_\alpha=0$. This is a [chiral spinor superfield](#chiral-spinor-superfield) with a [gaugino](#gaugino) as its lowest component. Phase and component signs depend on the stated [Wess-Zumino gauge](#wess-zumino-gauge) convention; the reality of $V$ alone does not fix those phase conventions.

###### Supersymmetric Yang-Mills action

↑ **Parent:** [Chiral field-strength superfield](#chiral-field-strength-superfield)

The four-dimensional supersymmetric Yang-Mills action is the chiral superspace integral of $\operatorname{Tr}(W^\alpha W_\alpha)$ plus its Hermitian conjugate. Its component fields are a Yang-Mills gauge field, a gaugino and an auxiliary field.

##### Chiral superfield

↑ **Parent:** [Superfield](#superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chiral_superfield)

A chiral superfield obeys $\bar D_{\dot\alpha}\Phi=0$. In chiral coordinates $y^\mu=x^\mu+i\bar\theta\bar\sigma^\mu\theta$ it expands as

$$
\Phi(y,\theta)=\phi(y)+\sqrt2\,\theta\psi(y)+\theta^2F(y).
$$

###### Chiral spinor superfield

↑ **Parent:** [Chiral superfield](#chiral-superfield)

A [chiral spinor superfield](#chiral-spinor-superfield) carries a [Spinor representation of the Lorentz group](relativistic-quantum-field.md#spinor-representation-of-the-lorentz-group) index and satisfies $\bar D_{\dot\alpha}\Psi_\beta=0$. The [chiral field-strength superfield](#chiral-field-strength-superfield) is a fermionic example: its lowest component is the [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) [gaugino](#gaugino). Its spinor index distinguishes it from a scalar [chiral superfield](#chiral-superfield), even though both obey the same chirality constraint.

###### Holomorphic closure of chiral superfields

↑ **Parent:** [Chiral superfield](#chiral-superfield)

A nonsingular [holomorphic function](complex-analysis.md#holomorphic-function) of [chiral superfields](#chiral-superfield) remains chiral because $\bar D_{\dot\alpha}f(\Phi)=\sum_i f_i(\Phi)\bar D_{\dot\alpha}\Phi_i=0$. Dependence on conjugate [superfields](#superfield) generally destroys the constraint. This explains the holomorphic form of a [superpotential](#superpotential).

###### Nilpotent chiral superfield

↑ **Parent:** [Chiral superfield](#chiral-superfield)

For $X=x+\sqrt2\theta G+\theta^2F$, the nilpotency condition gives $x^2=xG=0$ and $2xF=GG$. On the branch with invertible commuting part of $F$, $x=GG/(2F)$, while the [goldstino](#goldstino) $G$ and [auxiliary field](#auxiliary-field) $F$ are independent. Products of three identical two-component odd spinor entries vanish, verifying the remaining constraints. The scalar is therefore composite. The branch hypothesis matters: $X=0$ also obeys the constraint and need not break [supersymmetry](supersymmetry.md).

###### Chiral superfield constrained by a nilpotent superfield

↑ **Parent:** [Nilpotent chiral superfield](#nilpotent-chiral-superfield)

With $X^2=0$ and invertible $F_X$, the additional [chiral superfield](#chiral-superfield) $Y=y+\sqrt2\theta\chi+\theta^2F_Y$ satisfying $XY=0$ has $y=(G\chi)/F_X-(GG)F_Y/(2F_X^2)$. Its [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) $\chi$ and [auxiliary field](#auxiliary-field) $F_Y$ remain independent. This eliminates the independent scalar. It does not force $Y^2=0$.

###### Cubic nilpotency from a mixed chiral constraint

↑ **Parent:** [Chiral superfield constrained by a nilpotent superfield](#chiral-superfield-constrained-by-a-nilpotent-superfield)

On the invertible-$F_X$ branch, use $y=(G\chi)/F_X-(GG)F_Y/(2F_X^2)$ and the two-component [Grassmann algebra](linear-algebra.md#grassmann-algebra) identity $(G\chi)^2=-\tfrac12(GG)(\chi\chi)$. Then $y^2=-(GG)(\chi\chi)/(2F_X^2)$, $y^3=y^2\chi=0$ and $y^2F_Y-y\chi\chi=0$. These are the components of $Y^3=0$. Generally $y^2$ is nonzero, so cubic nilpotency must not be replaced by quadratic nilpotency. The allowed analytic holomorphic monomials are $1,X,Y,Y^2$.

###### Antichiral superfield

↑ **Parent:** [Chiral superfield](#chiral-superfield)

An antichiral superfield obeys $D_\alpha\Phi^\dagger=0$ and is the Hermitian conjugate of a chiral superfield. It depends naturally on $\bar y^\mu=x^\mu-i\theta\sigma^\mu\bar\theta$ and $\bar\theta$.

###### Supersymmetric covariant derivative

↑ **Parent:** [Chiral superfield](#chiral-superfield)

Supersymmetric covariant derivatives anticommute with the supersymmetry generators. Their antichiral member defines a chiral superfield through $\bar D_{\dot\alpha}\Phi=0$.

###### Chiral projection by squared supercovariant derivatives

↑ **Parent:** [Supersymmetric covariant derivative](#supersymmetric-covariant-derivative)

In flat [four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry), let $\bar D^2=\bar D_{\dot\alpha}\bar D^{\dot\alpha}$, contracting the two spinor indices with the antisymmetric epsilon [invariant tensor](representation-theory.md#invariant-tensor). The [supercovariant derivative algebra with left derivatives](#supercovariant-derivative-algebra-with-left-derivatives) has $\{\bar D_{\dot\alpha},\bar D_{\dot\beta}\}=0$. There are only two dotted components, so every product of three barred derivatives repeats one component and vanishes. Therefore $\bar D_{\dot\alpha}\bar D^2X=0$ for any [superfield](#superfield) $X$: $\bar D^2X$ is a [chiral superfield](#chiral-superfield). This map is called chiral projection, although $\bar D^2$ is not an idempotent projector.

If $\Phi$ is a [chiral superfield](#chiral-superfield), [holomorphic closure of chiral superfields](#holomorphic-closure-of-chiral-superfields) also makes $W'(\Phi)$ chiral. Thus an equation $\bar D^2\Phi^\dagger=4W'(\Phi)$ is consistent with the chiral constraint: applying any $\bar D_{\dot\alpha}$ gives zero on both sides. Both sides are scalar [superfields](#superfield), and the squared [supersymmetric covariant derivative](#supersymmetric-covariant-derivative) commutes with the [supercharges](#supersymmetry-generator), so the equation is [Lorentz invariant](special-relativity.md#lorentz-invariance) and [supersymmetry](supersymmetry.md) covariant.

###### Supersymmetric derivatives in chiral coordinates

↑ **Parent:** [Supersymmetric covariant derivative](#supersymmetric-covariant-derivative)

For [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative) and $D_\alpha=\partial_\alpha+i(\sigma^\mu\bar\theta)_\alpha\partial_\mu$, $\bar D_{\dot\alpha}=-\bar\partial_{\dot\alpha}-i(\theta\sigma^\mu)_{\dot\alpha}\partial_\mu$, the coordinate $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$ gives $D_\alpha=\partial_\alpha|_y+2i(\sigma^\mu\bar\theta)_\alpha\partial_{y^\mu}$ and $\bar D_{\dot\alpha}=-\bar\partial_{\dot\alpha}|_y$. The odd chain rule gives $\bar\partial_{\dot\alpha}(\theta\sigma^\mu\bar\theta)=-(\theta\sigma^\mu)_{\dot\alpha}$. A [chiral superfield](#chiral-superfield) is consequently independent of $\bar\theta$ at fixed $y$.

###### Supercovariant derivative algebra with left derivatives

↑ **Parent:** [Supersymmetric covariant derivative](#supersymmetric-covariant-derivative)

For [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), choose $D_\alpha=\partial_\alpha+i\sigma^\mu_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_\mu$ and $\bar D_{\dot\alpha}=\bar\partial_{\dot\alpha}+i\theta^\beta\sigma^\mu_{\beta\dot\alpha}\partial_\mu$. Differentiating the other operator's odd coefficient gives two equal contributions to the mixed [anticommutator](vector-space.md#anticommutator); coefficient-coefficient terms cancel by the [Grassmann algebra](linear-algebra.md#grassmann-algebra). Thus the mixed [anticommutator](vector-space.md#anticommutator) is $2i\sigma^\mu\partial_\mu$, while equal-chirality ones vanish. Also $\bar D(x+i\theta\sigma\bar\theta)=0$, giving the coordinates used in the [chiral-superfield component expansion](#chiral-superfield-component-expansion). Negating the barred derivative negates the mixed algebra.

###### Chiral-superfield component expansion

↑ **Parent:** [Chiral superfield](#chiral-superfield)

With [left Grassmann derivatives](linear-algebra.md#left-grassmann-derivative), a [chiral superfield](#chiral-superfield) is a finite expansion in chiral coordinates $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$:

$$
\Phi(y,\theta)=\phi(y)+\sqrt2\theta\psi(y)+\theta^2F(y).
$$

Here $\phi$ is a [complex scalar field](scalar-field-theory.md#complex-scalar-field), $\psi$ a [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) and $F$ an [auxiliary field](#auxiliary-field). The translation form of its ordinary-coordinate expansion is

$$
\Phi(x,\theta,\bar\theta)=\exp\bigl(i\theta\sigma^\mu\bar\theta\,\partial_\mu\bigr)\bigl(\phi(x)+\sqrt2\theta\psi(x)+\theta^2F(x)\bigr).
$$

The exponential terminates in the [Grassmann algebra](linear-algebra.md#grassmann-algebra). To reduce its contractions, choose signature $(+---)$, $\sigma^\mu=(I,\boldsymbol\sigma)$, left differentiation, and $\epsilon_{12}=1$ for both lower spinor epsilon tensors. Define $\theta^2=\theta^\alpha\theta_\alpha$ and $\bar\theta^2=\bar\theta_{\dot\alpha}\bar\theta^{\dot\alpha}$. Then $v^\mu=\theta\sigma^\mu\bar\theta$ satisfies $v^\mu v^\nu=\tfrac12\theta^2\bar\theta^2\eta^{\mu\nu}$. Expanding the translation gives

$$
\Phi=\phi+\sqrt2\theta\psi+\theta^2F+i\theta\sigma^\mu\bar\theta\,\partial_\mu\phi-\frac{i}{\sqrt2}\theta^2\partial_\mu\psi\sigma^\mu\bar\theta-\frac14\theta^2\bar\theta^2\Box\phi,
\qquad\Box=\eta^{\mu\nu}\partial_\mu\partial_\nu.
$$

The last sign follows from $i^2/2=-1/2$ in the translation expansion. Defining the barred square in the reverse order, $\bar\theta^{\dot\alpha}\bar\theta_{\dot\alpha}$, negates it and writes the same term with a positive quarter coefficient. Spinor contractions and the [Grassmann algebra](linear-algebra.md#grassmann-algebra) convention must therefore accompany the reduced formula.

###### Auxiliary field

↑ **Parent:** [Chiral superfield](#chiral-superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Auxiliary_field)

An auxiliary field has no kinetic term and can be eliminated algebraically. The complex field $F$ in a chiral superfield balances bosonic and fermionic degrees of freedom off shell.

###### Superpotential

↑ **Parent:** [Chiral superfield](#chiral-superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superpotential)

A superpotential is a holomorphic function of chiral superfields integrated over chiral superspace, $\int d^2\theta\,W+\mathrm{h.c.}$

###### Constant superpotential in global supersymmetry

↑ **Parent:** [Superpotential](#superpotential)

Adding a constant to a global [superpotential](#superpotential) does not change the component action because the chiral [superspace](#superspace) integral of that constant vanishes. Neither the [F-term scalar potential](#f-term-scalar-potential) nor the [fermion](quantum-mechanics.md#fermion) mass matrix depends on it. This statement does not extend to [supergravity](#supergravity), where the [superpotential](#superpotential) itself enters the gravitational potential.

###### Superpotential critical-point shift

↑ **Parent:** [Superpotential](#superpotential)

For a canonical [chiral superfield](#chiral-superfield), an affine translation $\Phi=\Psi+s$ preserves the kinetic action up to a vanishing full-superspace term. It removes the linear [superpotential](#superpotential) term exactly when $s$ is a critical point. For $W=\alpha+\kappa\Phi+m\Phi^2/2+g\Phi^3/6$, the shifted quadratic coefficient is $M=m+gs$ with $M^2=m^2-2g\kappa$. A real shift requires a real root; the complex field permits a complex shift as well.

###### Chiral-superfield fermion mass matrix

↑ **Parent:** [Superpotential](#superpotential)

For canonically normalized [chiral superfields](#chiral-superfield), the fermion bilinear is $-\tfrac12W_{ij}\psi_i\psi_j+\mathrm{h.c.}$ at the chosen vacuum. Its matrix is complex symmetric. The nonnegative physical [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) masses are its [singular values](linear-algebra.md#singular-value), and their squared sum is $\operatorname{tr}(m^\dagger m)$. Using signed eigenvalues of a symmetric mass matrix instead can obscure the physical mass count.

###### F-term

↑ **Parent:** [Superpotential](#superpotential)

An F-term is the highest $\theta^2$ component of a chiral superfield, equivalently an integral over chiral half of superspace. Its supersymmetry variation is a spacetime total derivative.

###### F-term scalar potential

↑ **Parent:** [Superpotential](#superpotential)

For canonical global supersymmetry, eliminating the auxiliary fields gives

$$
V_F=\sum_i\left|\frac{\partial W}{\partial\phi_i}\right|^2.
$$

###### Real-slice diagnosis of chiral-scalar vacua

↑ **Parent:** [F-term scalar potential](#f-term-scalar-potential)

A [chiral superfield](#chiral-superfield) has a [complex scalar](scalar-field-theory.md#complex-scalar-field). Minimizing its potential only on the real axis can miss [supersymmetric vacua](#supersymmetric-vacuum). For example $W'(\varphi)=1+\varphi^2$ has positive potential $(1+x^2)^2$ for real $x$, yet its complex vacua $\varphi=\pm i$ have zero energy. [Supersymmetry breaking](#supersymmetry-breaking) must therefore be tested in the full complex field space, not inferred from a positive minimum on an arbitrarily chosen real slice.

###### Tree-level supertrace mass sum rule

↑ **Parent:** [F-term scalar potential](#f-term-scalar-potential)

For canonical positive kinetic terms in global [supersymmetry](supersymmetry.md), $V=\sum_k|W_k|^2$ has mixed [Hessian matrix](calculus.md#hessian-matrix) $V_{i\bar j}=\sum_kW_{ki}\overline{W_{kj}}$ and holomorphic block $V_{ij}=\sum_k\overline{W_k}W_{kij}$. The $2n$ real scalar squared-mass sum is $2\operatorname{tr}(m^\dagger m)$ for the [chiral-superfield fermion mass matrix](#chiral-superfield-fermion-mass-matrix) $m=W_{ij}$. Each [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) contributes two states, giving the same fermion weighted sum. Thus their boson-minus-fermion [supertrace](quantum-mechanics.md#supertrace) vanishes even with [F-term](#f-term) breaking. The holomorphic Hessian splits real scalar masses without changing their sum. Noncanonical [Kähler metrics](complex-geometry.md#kahler-metric), [supergravity](#supergravity), and radiative corrections require different formulas.

###### Gauge contributions to the F-term supertrace

↑ **Parent:** [Tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule)

Canonical gauge interactions preserve the [tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule) at a vacuum with vanishing [D-terms](#d-term). Put $C=\sum_a g_a^2\|T_av\|^2$ for the scalar expectation vector $v$. The extra real-scalar squared-mass trace is $2C$, the extra [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) squared-mass trace from [gaugino](#gaugino) mixing is $4C$, and the [gauge boson](relativistic-quantum-field.md#gauge-boson) squared-mass trace is $2C$. Their spin-weighted [supertrace](quantum-mechanics.md#supertrace) is $2C-2(4C)+3(2C)=0$. The scalar contribution comes from differentiating $\tfrac12\sum_aD_a^2$; the fermionic one counts both blocks of the symmetric mixing matrix with entries $\sqrt2g_aT_av$; the vector one follows from the covariant scalar [kinetic term](quantum-field-theory.md#kinetic-term). Any zero-mass [Goldstone bosons](critical-phenomenon.md#goldstone-boson) in the unreduced scalar Hessian do not change its trace.

###### Non-renormalization theorem

↑ **Parent:** [Superpotential](#superpotential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Non-renormalization_theorem)

The local [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action) [superpotential](#superpotential) receives no perturbative corrections when [supersymmetry](supersymmetry.md) is preserved, an infrared cutoff is retained and the same elementary fields are kept. The [spurion selection rule for perturbative non-renormalization](#spurion-selection-rule-for-perturbative-non-renormalization) gives a holomorphy proof. The [Kähler potential](#kahler-potential) and physical couplings after [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) can change; genuine nonperturbative superpotential terms require a separate analysis.

###### One-loop exactness of the holomorphic gauge kinetic function

↑ **Parent:** [Non-renormalization theorem](#non-renormalization-theorem)

In a supersymmetry-preserving local [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action), the [gauge kinetic function](#gauge-kinetic-function) receives only a one-loop perturbative correction. For one simple gauge factor, $\mu\,df/d\mu=b_0/(8\pi^2)$ with $b_0=3C_2(G)-\sum_iT(R_i)$. A perturbative shift of the topological angle leaves the running coefficient invariant; the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) then make its holomorphic beta function independent of the gauge coupling. Holomorphic regularity and spurionic [R-charges](#r-charge) exclude higher-loop Yukawa combinations, which would require antichiral couplings. The constant is fixed by one-loop matching. This does not assert one-loop exactness of a canonically normalized physical coupling, or forbid nonperturbative terms.

// Target: quantum-field-theory.bigb

###### Holomorphic and canonically normalized superpotential couplings

↑ **Parent:** [Non-renormalization theorem](#non-renormalization-theorem)

Local Wilsonian [superpotential](#superpotential) coefficients can have no perturbative vertex corrections while the [Kähler potential](#kahler-potential) undergoes [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization). Canonical normalization then converts a quadratic coefficient $m$ and cubic coefficient $g$ to the displayed running coefficients. Non-renormalization of a holomorphic F-term is therefore compatible with running physical masses and interactions. The distinction requires keeping a local [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action) separate from infrared-singular one-particle-irreducible effects and from eliminating entire massive fields.

###### Holomorphy argument for superpotential non-renormalization

↑ **Parent:** [Non-renormalization theorem](#non-renormalization-theorem)

A holomorphy argument treats couplings as chiral [spurions](#spurion) and constrains the [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action) [superpotential](#superpotential) to be a [holomorphic function](complex-analysis.md#holomorphic-function) with the required ordinary charges and [R-charges](#r-charge). Perturbative regularity in the couplings can then rule out new terms and loop corrections to the existing [superpotential](#superpotential).

<h6 id="wess-zumino-spurion-charge-assignment">Wess–Zumino spurion charge assignment</h6>

↑ **Parent:** [Holomorphy argument for superpotential non-renormalization](#holomorphy-argument-for-superpotential-non-renormalization)

For quadratic and cubic interactions, assigning the couplings chiral [spurion](#spurion) transformations makes each monomial formally covariant. The ordinary $U(1)$ leaves $\theta$ neutral, while the [R-symmetry](#r-symmetry) gives it charge one and the [superpotential](#superpotential) charge two. The neutral ratio $g\Phi/m$ and the covariant factor $m\Phi^2$ give the symmetry-allowed holomorphic form $m\Phi^2f(g\Phi/m)$. Perturbative regularity and tree matching are additionally needed for [superpotential non-renormalization](#non-renormalization-theorem); symmetry alone leaves an arbitrary function. Fixed numerical couplings need not enjoy these formal symmetries as actual field symmetries.

###### Spurion selection rule for perturbative non-renormalization

↑ **Parent:** [Holomorphy argument for superpotential non-renormalization](#holomorphy-argument-for-superpotential-non-renormalization)

In the local [Wilsonian effective action](perturbative-quantum-field-theory.md#wilsonian-effective-action), retain the elementary [chiral superfields](#chiral-superfield) and a nonzero infrared cutoff. Promote each coefficient in $W=\sum_A\lambda_A\mathcal O_A(\Phi)$ to a chiral [spurion](#spurion). Holomorphy excludes $\bar\lambda_A$. Assigning $R(\Phi_i)=0$ and $R(\lambda_A)=2$ forces a regular perturbative term of [R-charge](#r-charge) two to be linear in these [spurions](#spurion). Ordinary flavor charges constrain its field monomial. The [perturbative gauge-coupling independence of the Wilsonian superpotential](#perturbative-gauge-coupling-independence-of-the-wilsonian-superpotential) removes gauge-dependent coefficients. With the gauge coupling zero, a single holomorphic vertex cannot close a loop through free $\Phi$-$\Phi^\dagger$ propagators; extra vertices would violate the spurion degree or holomorphy. Its coefficient is therefore the tree coefficient. Gauge anomalies of the formal [R-symmetry](#r-symmetry) are tracked by a transforming holomorphic gauge coupling. Keeping the infrared cutoff matters: singular one-particle-irreducible terms and elimination of entire massive fields are different operations.

The background-field holomorphy method is discussed in [Seiberg's non-renormalization paper](https://arxiv.org/abs/hep-ph/9309335).

###### Perturbative gauge-coupling independence of the Wilsonian superpotential

↑ **Parent:** [Spurion selection rule for perturbative non-renormalization](#spurion-selection-rule-for-perturbative-non-renormalization)

The holomorphic coupling is $\tau=\vartheta/(2\pi)+4\pi i/g^2$. Perturbative coefficients are independent of the topological angle $\vartheta$. A [holomorphic function](complex-analysis.md#holomorphic-function) invariant under continuous shifts of $\operatorname{Re}\tau$ is constant by the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations), hence a perturbative local [superpotential](#superpotential) coefficient cannot depend on $\tau$. Terms in $e^{2\pi i\tau}$ can evade this argument nonperturbatively. This does not forbid renormalization of the separate gauge kinetic [F-term](#f-term), or [wave-function renormalization](perturbative-quantum-field-theory.md#wave-function-renormalization) from the [Kähler potential](#kahler-potential).

<h6 id="kahler-potential">Kähler potential</h6>

↑ **Parent:** [Chiral superfield](#chiral-superfield)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kähler_potential)

The Kähler potential is a real function integrated over full superspace. The canonical choice $K=\Phi^\dagger\Phi$ gives canonical kinetic terms.

<h6 id="kahler-transformation">Kähler transformation</h6>

↑ **Parent:** [Kähler potential](#kahler-potential)

Adding a [holomorphic function](complex-analysis.md#holomorphic-function) $f$ and its conjugate does not change the [Kähler metric](complex-geometry.md#kahler-metric). In global [supersymmetry](supersymmetry.md), these terms integrate to zero in the [D-term](#d-term) action. In Planck-unit [supergravity](#supergravity), the simultaneous transformation $W\mapsto e^{-f}W$ leaves the [scalar potential](quantum-field-theory.md#scalar-potential) invariant; shifting $K$ while holding $W$ fixed generally does not.

###### D-term

↑ **Parent:** [Kähler potential](#kahler-potential)

A D-term is a full [superspace integration](#superspace-integration) of a real [superfield](#superfield). In [four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry), a [Kähler potential](#kahler-potential) contributes a D-term containing kinetic terms and quadratic [auxiliary field](#auxiliary-field) terms.

<h3 id="wess-zumino-model">Wess–Zumino model</h3>

↑ **Parent:** [Four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wess–Zumino_model)

The Wess–Zumino model contains chiral superfields with a polynomial superpotential. It is the simplest interacting four-dimensional supersymmetric field theory.

#### Supersymmetric domain wall

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

In a canonical [Wess–Zumino model](#wess-zumino-model), complete the static transverse energy into $|\phi'-e^{i\alpha}\overline{W'}|^2+2\operatorname{Re}(e^{-i\alpha}dW/dz)$. Choosing the phase of $\Delta W$ gives the tension bound. A solution of the displayed first-order equation attains it and preserves two of four real [supercharges](#supersymmetry-generator). For $W=\mu^2\Phi/g-g\Phi^3/3$, $\phi(z)=(\mu/g)\tanh(\mu z)$ interpolates between the two vacua and has tension $8\mu^3/(3g^2)$.

#### Wess-Zumino chiral multiplet coupled to supergravity

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

Localizing the rigid [supersymmetry](supersymmetry.md) of a free [Wess–Zumino model](#wess-zumino-model) produces a derivative of the supersymmetry parameter multiplying the [supercurrent](#supercurrent). The [Noether gauging procedure](quantum-field-theory.md#noether-gauging-procedure) introduces a [gravitino](#gravitino) coupled to this current. Closure also requires a [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime), the [Einstein-Hilbert action](general-relativity.md#einstein-hilbert-action), covariant matter kinetic terms and higher-order interactions. The leading gravitino-matter coupling contains the derivative of the scalar, not its undifferentiated value.

<h4 id="trilinear-scalar-vertices-in-the-wess-zumino-model">Trilinear scalar vertices in the Wess–Zumino model</h4>

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

For canonical [Kähler potential](#kahler-potential) and $W=m\Phi^2/2+g\Phi^3/3$, eliminating the [auxiliary field](#auxiliary-field) gives $V=|m\phi+g\phi^2|^2$. The cubic interaction Lagrangian is $-m^*g\phi^*\phi^2-mg^*\phi(\phi^*)^2$. Differentiating with respect to the three external fields gives the all-incoming [Feynman rules](perturbative-quantum-field-theory.md#feynman-rule) $V_{\phi\phi\phi^*}=-2im^*g$ and $V_{\phi^*\phi^*\phi}=-2img^*$; the factor two counts identical scalar legs. For real $m,g$ and $\phi=(A+iB)/\sqrt2$, the cubic Lagrangian is $-mgA(A^2+B^2)/\sqrt2$, giving $V_{AAA}=-3\sqrt2img$ and $V_{ABB}=-\sqrt2img$.

#### Discriminant mass invariant of a cubic superpotential

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

Under a [superpotential critical-point shift](#superpotential-critical-point-shift), $m\mapsto M=m+gs$ and the linear coefficient vanishes, while $M^2=\Delta$ is unchanged. At either supersymmetric root $v$, the complex [fermion](quantum-mechanics.md#fermion) mass parameter is $W''(v)=\pm\sqrt\Delta$. The physical scalar and [fermion](quantum-mechanics.md#fermion) masses are both $\sqrt{|\Delta|}$, independent of the additive [superpotential](#superpotential) constant. A repeated critical point has a massless multiplet and a quartic leading [scalar potential](quantum-field-theory.md#scalar-potential).

#### Supersymmetric relation between quartic and Yukawa couplings

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

In a canonical [Wess–Zumino model](#wess-zumino-model) with cubic [superpotential](#superpotential) $g\Phi^3/3$, eliminating the [auxiliary field](#auxiliary-field) gives $V\supset|g|^2|\varphi|^4$ and $\mathcal L\supset-g\varphi\psi\psi+\mathrm{h.c.}$. Thus the coefficient of the quartic [scalar field](quantum-field-theory.md#scalar-field) interaction is the squared modulus of this convention for the [Yukawa coupling](standard-model.md#yukawa-interaction).

<h5 id="quartic-complex-scalar-vertex-in-the-wess-zumino-model">Quartic complex-scalar vertex in the Wess–Zumino model</h5>

↑ **Parent:** [Supersymmetric relation between quartic and Yukawa couplings](#supersymmetric-relation-between-quartic-and-yukawa-couplings)

In a canonical [Wess–Zumino model](#wess-zumino-model) with cubic superpotential $g\Phi^3/3$, auxiliary elimination gives a complex-scalar quartic interaction with two legs of each field type. With all momenta incoming and the displayed coefficient, its [Feynman rule](perturbative-quantum-field-theory.md#feynman-rule) is $-i(2!2!)|g|^2$. For $\varphi=(A+iB)/\sqrt2$, the same quartic [scalar potential](quantum-field-theory.md#scalar-potential) is $|g|^2(A^2+B^2)^2/4$, with real-field rules $-6i|g|^2$ for four identical legs and $-2i|g|^2$ for two of each. Factorials depend on how the coefficient is defined, not on a new physical coupling.

#### Supersymmetric cancellation of quadratic divergences

↑ **Parent:** [Wess–Zumino model](#wess-zumino-model)

Supersymmetry fixes scalar and fermion couplings so that bosonic and fermionic loop contributions to scalar masses have equal quadratic ultraviolet parts with opposite signs.

## Supersymmetry breaking

↑ **Parent:** [Supersymmetry](supersymmetry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetry_breaking)

Supersymmetry breaking occurs when the action or vacuum is not invariant under the supercharges. Explicit breaking destroys the exact superalgebra, while spontaneous breaking preserves the action but gives a vacuum not annihilated by every supercharge and produces a Goldstino.

### Dynamical supersymmetry breaking

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)

Dynamical supersymmetry breaking occurs when quantum dynamics produces a vacuum that does not preserve [supersymmetry](supersymmetry.md). An asymptotically free hidden sector can generate the displayed exponentially small scale through [dimensional transmutation](perturbative-quantum-field-theory.md#dimensional-transmutation). This supplies a possible origin of a hierarchy, but strong coupling by itself does not prove breaking: the vacuum equations and dynamics must exclude a [supersymmetric vacuum](#supersymmetric-vacuum).

// Target: supersymmetry.bigb

### Flat F-term breaking with a linear superpotential

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)

With one canonical ungauged [chiral superfield](#chiral-superfield) and $\kappa\ne0$, the auxiliary expectation is nonzero at every scalar value. The potential is flat and positive, so [supersymmetry](supersymmetry.md) is broken without an isolated minimum. The [fermion](quantum-mechanics.md#fermion) is a massless [Goldstino](#goldstino) and the scalar is massless at tree level. Equality of these zero masses does not imply an unbroken [supersymmetric vacuum](#supersymmetric-vacuum).

### Explicit versus spontaneous supersymmetry breaking

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)

Explicit breaking changes the action so that the former [supercharges](#supersymmetry-generator) are not conserved symmetries of the full Hamiltonian. Spontaneous breaking preserves the action and algebra but has a vacuum that some [supercharge](#supersymmetry-generator) does not annihilate. [Energy positivity in global supersymmetry](#energy-positivity-in-global-supersymmetry) then implies positive vacuum energy density, and a [Goldstino](#goldstino) accompanies the broken symmetry. That exact-algebra energy argument does not apply to an arbitrarily explicitly broken Hamiltonian. The physical particle spectrum in a broken vacuum need not assemble into the finite equal-mass [supermultiplets](#supermultiplet) of an invariant vacuum.

### Hidden supersymmetry-breaking sector

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)

A hidden sector contains fields whose [auxiliary fields](#auxiliary-field) acquire expectation values that break [supersymmetry](supersymmetry.md). Loop effects or suppressed interactions communicate the breaking to visible fields as effective [soft supersymmetry breaking](#soft-supersymmetry-breaking). This can avoid the canonical visible-sector [tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule).

### Goldstino

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Goldstino)

A [goldstino](#goldstino) is the massless spin-one-half mode associated with spontaneously broken global [supersymmetry](supersymmetry.md). For [F-term](#f-term) breaking, the [fermion](quantum-mechanics.md#fermion) in a multiplet with nonzero [auxiliary field](#auxiliary-field) transforms by an inhomogeneous term, $\delta G\supset\sqrt2\epsilon F$. In [supergravity](#supergravity), the corresponding mode supplies the longitudinal degrees of freedom of a massive gravitino.

#### Goldstino null vector with F-term and D-term breaking

↑ **Parent:** [Goldstino](#goldstino)

For canonical global [four-dimensional N=1 supersymmetry](#four-dimensional-n-1-supersymmetry), define $F^i=\overline{W_i}$, $H_{ij}=W_{ij}$ and $G_{ia}=g^a\bar\phi_j(T^a)^j{}_i$ at a stationary vacuum. [Gauge invariance](relativistic-quantum-field.md#gauge-invariance) of the [superpotential](#superpotential) gives $G^TF=0$, while stationarity of $V=\sum_i|W_i|^2+\frac12\sum_a(D^a)^2$ gives $HF-GD=0$. Therefore the canonically normalized [fermion mass matrix](standard-model.md#fermion-mass-matrix), after a harmless [gaugino](#gaugino) phase choice, obeys

$$
\begin{pmatrix}H&-\sqrt2G\\-\sqrt2G^T&0\end{pmatrix}\begin{pmatrix}F\\D/\sqrt2\end{pmatrix}=0.
$$

If [supersymmetry](supersymmetry.md) is broken, this vector is nonzero and specifies a massless [Goldstino](#goldstino). The matrix with off-diagonal blocks $-G$ instead acts on $(F,D)$; it is related to the canonical matrix by a change of normalization, not by equality of canonical entries. Additional zero modes can coexist with the [Goldstino](#goldstino).

#### Goldstino zero mode from vacuum stationarity

↑ **Parent:** [Goldstino](#goldstino)

Stationarity of a canonical global [F-term scalar potential](#f-term-scalar-potential) gives $\partial_iV=\sum_jW_{ij}\overline{W_j}=0$. If some $F_j=-\overline{W_j}$ is nonzero, this vector is in the [kernel](linear-algebra.md#kernel-of-a-linear-map) of the [chiral-superfield fermion mass matrix](#chiral-superfield-fermion-mass-matrix). It supplies the massless [goldstino](#goldstino) direction. If every $F_j$ vanishes, this argument gives no broken-symmetry mode.

### Soft supersymmetry breaking

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Soft_supersymmetry_breaking)

Soft supersymmetry breaking adds operators of positive mass dimension that break supersymmetry without reintroducing new ultraviolet quadratic divergences.

#### Soft scalar-mass sensitivity

↑ **Parent:** [Soft supersymmetry breaking](#soft-supersymmetry-breaking)

[Soft supersymmetry breaking](#soft-supersymmetry-breaking) removes quadratic ultraviolet sensitivity but can leave scalar-mass corrections proportional to the soft squared masses and logarithms of scale ratios. The high-momentum difference of a paired scalar and fermion propagator falls as their squared-mass splitting divided by momentum to the fourth power. Heavy soft partners can therefore still create a tuning problem through logarithmic and finite thresholds even though the original quadratic [hierarchy problem](standard-model.md#hierarchy-problem) has been controlled.

#### Sparticle

↑ **Parent:** [Soft supersymmetry breaking](#soft-supersymmetry-breaking)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sparticle)

A sparticle is the supersymmetric partner of a Standard Model particle. It differs in spin by one half and has the opposite R-parity.

##### Neutralino

↑ **Parent:** [Sparticle](#sparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Neutralino)

In the [MSSM](#minimal-supersymmetric-standard-model), [electroweak symmetry breaking](standard-model.md#electroweak-symmetry-breaking) mixes the neutral [bino](#bino), [wino](#wino) and two neutral [higgsinos](#higgsino) into four neutral [Majorana spinor](relativistic-quantum-field.md#majorana-spinor) mass eigenstates, the [neutralinos](#neutralino). A neutralino can be the [lightest supersymmetric particle](#lightest-supersymmetric-particle); with conserved [R-parity](#r-parity) it then provides a stable possible [dark matter](cosmology.md#dark-matter) candidate.

##### Lightest supersymmetric particle

↑ **Parent:** [Sparticle](#sparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lightest_supersymmetric_particle)

The [lightest supersymmetric particle](#lightest-supersymmetric-particle) is the least massive [sparticle](#sparticle) in a given spectrum. Exact [R-parity](#r-parity) makes it stable: a lighter final state cannot contain another odd particle, while a final state of ordinary particles is even. A neutral weakly interacting [lightest supersymmetric particle](#lightest-supersymmetric-particle) is a possible [dark matter](cosmology.md#dark-matter) constituent, but its cosmological abundance must be computed separately.

##### Slepton

↑ **Parent:** [Sparticle](#sparticle)

A [slepton](#slepton) is a scalar [sparticle](#sparticle) partner of a [lepton](standard-model.md#lepton). In the [MSSM](#minimal-supersymmetric-standard-model), the [chiral superfields](#chiral-superfield) $L$ and $E^c$ package the corresponding [Standard Model fermions](standard-model.md#standard-model-fermion) together with their [complex scalar field](scalar-field-theory.md#complex-scalar-field) partners. Their [gauge group representations](relativistic-quantum-field.md#gauge-group-representation) and [hypercharges](standard-model.md#hypercharge) follow those of the left-handed fermion convention, including charge-conjugated singlets.

##### Higgsino

↑ **Parent:** [Sparticle](#sparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Higgsino)

A higgsino is the [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) partner of a Higgs [scalar field](quantum-field-theory.md#scalar-field) in a [chiral superfield](#chiral-superfield). After a [supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism), its combination along a broken gauge direction mixes with the [gaugino](#gaugino) in the resulting [massive N=1 vector multiplet](#massive-n-1-vector-multiplet).

##### Gaugino

↑ **Parent:** [Sparticle](#sparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaugino)

A gaugino is the spin-one-half superpartner of a gauge boson and transforms in the adjoint representation of its gauge group. Gaugino loops modify gauge-coupling beta functions above the supersymmetry-breaking threshold.

###### Bino

↑ **Parent:** [Gaugino](#gaugino)

The [bino](#bino) is the spin-one-half [gaugino](#gaugino) of the [hypercharge](standard-model.md#hypercharge) $U(1)_Y$ [gauge group](relativistic-quantum-field.md#gauge-group). Its adjoint representation is the singlet $(\mathbf1,\mathbf1,0)$, so it has no hypercharge of its own. After [electroweak symmetry breaking](standard-model.md#electroweak-symmetry-breaking), it can mix with the neutral [wino](#wino) and [higgsinos](#higgsino) into [neutralinos](#neutralino).

###### Wino

↑ **Parent:** [Gaugino](#gaugino)

A [wino](#wino) is a spin-one-half [gaugino](#gaugino) of the weak $SU(2)_L$ [gauge group](relativistic-quantum-field.md#gauge-group). Before [electroweak symmetry breaking](standard-model.md#electroweak-symmetry-breaking), its three adjoint components transform as $(\mathbf1,\mathbf3,0)$ and can be described by a triplet of [Majorana spinors](relativistic-quantum-field.md#majorana-spinor). After symmetry breaking, the neutral component can mix with the [bino](#bino) and neutral [higgsinos](#higgsino) into [neutralinos](#neutralino).

###### Gluino

↑ **Parent:** [Gaugino](#gaugino)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gluino)

The [gluino](#gluino) is the spin-one-half [sparticle](#sparticle) paired with a [gluon](standard-model.md#gluon). In the [MSSM](#minimal-supersymmetric-standard-model), the eight adjoint color components form a [Majorana spinor](relativistic-quantum-field.md#majorana-spinor) in $(\mathbf8,\mathbf1,0)$ under $SU(3)_c\times SU(2)_L\times U(1)_Y$. Its gauge representation is real, so the opposite-helicity antiparticle states are already included in the adjoint multiplet.

##### Squark

↑ **Parent:** [Sparticle](#sparticle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squark)

A squark is the spin-zero supersymmetric partner of a quark. It carries the same colour, weak-isospin and hypercharge quantum numbers as the corresponding quark chirality.

###### Top squark

↑ **Parent:** [Squark](#squark)

The top squark, or stop, is the scalar superpartner of the top quark. Its mass controls the leading residual top-sector correction to the Higgs mass after soft supersymmetry breaking.

<h3 id="o-raifeartaigh-model">O'Raifeartaigh model</h3>

↑ **Parent:** [Supersymmetry breaking](#supersymmetry-breaking)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/O'Raifeartaigh_model)

An O'Raifeartaigh model is a theory of chiral superfields whose F-term equations cannot all vanish. Supersymmetry is therefore spontaneously broken, and the classical scalar potential commonly contains a flat pseudomodulus direction.

<h4 id="mass-spectrum-of-the-quadratic-cubic-o-raifeartaigh-model">Mass spectrum of the quadratic-cubic O'Raifeartaigh model</h4>

↑ **Parent:** [O'Raifeartaigh model](#o-raifeartaigh-model)

For positive real $M,\mu,\lambda$ with $M^2>2\lambda^2\mu^2$, minimizing $V=\lambda^2|z^2-\mu^2|^2+M^2|z|^2+|2\lambda xz+My|^2$ gives $z=y=0$ with arbitrary $x$. Around $x=0$, the real scalar squared masses are $0,0,M^2,M^2,M^2-2\lambda^2\mu^2,M^2+2\lambda^2\mu^2$, while the three [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) masses are $0,M,M$. Their weighted [supertrace](quantum-mechanics.md#supertrace) vanishes. The massless $\psi_X$ is the [goldstino](#goldstino); the two real $x$ modes form a tree-level [pseudomodulus](#pseudomodulus). The stability bound follows from $|z^2-\mu^2|^2\ge(|z|^2-\mu^2)^2$, after minimizing the final square over $y$.

#### Pseudomodulus

↑ **Parent:** [O'Raifeartaigh model](#o-raifeartaigh-model)

A pseudomodulus is a classically flat scalar direction in a supersymmetry-breaking vacuum. Quantum corrections usually generate an effective potential along it without restoring simultaneous F-flatness.

## Minimal supersymmetric Standard Model

↑ **Parent:** [Supersymmetry](supersymmetry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimal_supersymmetric_Standard_Model)

The Minimal supersymmetric Standard Model is the supersymmetric extension of the Standard Model with two Higgs doublets and the minimal superpartner field content needed for a renormalizable theory.

### MSSM superpotential

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

With [hypercharge](standard-model.md#hypercharge) normalized by $Q_{\mathrm{em}}=T_3+Y$, the renormalizable [R-parity](#r-parity)-conserving [MSSM](#minimal-supersymmetric-standard-model) [superpotential](#superpotential) is $W=(y_u)_{ij}U_i^c(Q_j\cdot H_u)+(y_d)_{ij}D_i^c(Q_j\cdot H_d)+(y_e)_{ij}E_i^c(L_j\cdot H_d)+\mu H_u\cdot H_d$, with $A\cdot B=\epsilon_{ab}A^aB^b$. Additional renormalizable [R-parity violation](#r-parity-violation) allows $\tfrac12\lambda_{ijk}(L_i\cdot L_j)E_k^c+\lambda'_{ijk}(L_i\cdot Q_j)D_k^c+\tfrac12\lambda''_{ijk}\epsilon_{abc}U_i^{c,a}D_j^{c,b}D_k^{c,c}+\kappa_iL_i\cdot H_u$. The two antisymmetries are $\lambda_{ijk}=-\lambda_{jik}$ and $\lambda''_{ijk}=-\lambda''_{ikj}$. The first, second and fourth additional terms violate [lepton number](standard-model.md#lepton-number); the third violates [baryon number](standard-model.md#baryon-number).

#### Cubic superpotential with right-handed-neutrino superfields

↑ **Parent:** [MSSM superpotential](#mssm-superpotential)

For the [MSSM superfield representations](#mssm-superfield-representations) augmented by singlet [right-handed neutrino](standard-model.md#right-handed-neutrino) [chiral superfields](#chiral-superfield) $N_i$, the homogeneous cubic [gauge-invariant](relativistic-quantum-field.md#gauge-invariance) [superpotential](#superpotential) contains the four Yukawa structures $QH_uU$, $QH_dD$, $LH_dE$, $LH_uN$ and the additional structures $LLE$, $LQD$, $UDD$, $NH_dH_u$, $NNN$. Weak-doublet pairs contract with the antisymmetric two-index tensor; $UDD$ contracts with the color three-index tensor. Consequently the $LLE$ coefficient is antisymmetric in its two $L$ indices, the $UDD$ coefficient in its two $D$ indices, and the $NNN$ coefficient symmetric. With $L(N)=-1$, the last five structures violate [baryon number](standard-model.md#baryon-number) or [lepton number](standard-model.md#lepton-number), whereas the first four conserve both. Singlet fields must not be omitted when classifying a general cubic [superpotential](#superpotential).

#### Supersymmetric mu problem

↑ **Parent:** [MSSM superpotential](#mssm-superpotential)

The [MSSM](#minimal-supersymmetric-standard-model) permits a supersymmetric Higgs mass $\mu$, whose natural size is not fixed by [soft supersymmetry breaking](#soft-supersymmetry-breaking). Weak-scale symmetry breaking requires it to be comparable to the soft scale rather than a much larger fundamental scale. [Superpotential non-renormalization](#non-renormalization-theorem) protects a chosen small value radiatively but does not explain that choice; relating its generation to the breaking mechanism addresses the mu problem.

// Target: supersymmetry.bigb

### Holomorphic need for two Higgs chiral doublets

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

A renormalizable [MSSM](#minimal-supersymmetric-standard-model) [superpotential](#superpotential) is a [holomorphic function](complex-analysis.md#holomorphic-function) of [chiral superfields](#chiral-superfield) and cannot use their conjugates. Gauge-invariant up-type [Yukawa couplings](standard-model.md#yukawa-interaction) require $H_u$ of [hypercharge](standard-model.md#hypercharge) $+1/2$, while down-type and charged-lepton [Yukawa couplings](standard-model.md#yukawa-interaction) require $H_d$ of [hypercharge](standard-model.md#hypercharge) $-1/2$. A single doublet and its conjugate cannot play both roles in the [superpotential](#superpotential). This is distinct from [higgsino anomaly cancellation](#higgsino-anomaly-cancellation).

### Higgsino anomaly cancellation

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

A single weak-doublet [higgsino](#higgsino) of [hypercharge](standard-model.md#hypercharge) $+1/2$ contributes $1/4$ to the cubic [hypercharge](standard-model.md#hypercharge) [gauge anomaly](relativistic-quantum-field.md#gauge-anomaly), $1/4$ to the weak-squared [hypercharge](standard-model.md#hypercharge) coefficient with fundamental index $1/2$, and $1$ to the [mixed gauge-gravitational anomaly](relativistic-quantum-field.md#mixed-gauge-gravitational-anomaly). A second [Higgs chiral doublet](#higgs-chiral-doublet) of opposite [hypercharge](standard-model.md#hypercharge) cancels all three through its [higgsino](#higgsino). The pair also contributes an even number of weak doublets, avoiding a new [Witten SU(2) anomaly](relativistic-quantum-field.md#witten-su-2-anomaly). Higgs [complex scalar fields](scalar-field-theory.md#complex-scalar-field) do not cancel chiral fermion [gauge anomalies](relativistic-quantum-field.md#gauge-anomaly).

### Higgs chiral doublet

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

A [Higgs chiral doublet](#higgs-chiral-doublet) is a weak-doublet [chiral superfield](#chiral-superfield) containing a Higgs [complex scalar field](scalar-field-theory.md#complex-scalar-field), a [higgsino](#higgsino) and an [auxiliary field](#auxiliary-field). In the [MSSM](#minimal-supersymmetric-standard-model), $H_u$ has [hypercharge](standard-model.md#hypercharge) $+1/2$ and $H_d$ has [hypercharge](standard-model.md#hypercharge) $-1/2$. Their paired charges enable [higgsino anomaly cancellation](#higgsino-anomaly-cancellation) and the [holomorphic need for two Higgs chiral doublets](#holomorphic-need-for-two-higgs-chiral-doublets).

### MSSM superfield representations

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

In the [MSSM](#minimal-supersymmetric-standard-model), each [fermion generation](standard-model.md#fermion-generation) has [chiral superfields](#chiral-superfield) $Q:(3,2,1/6)$, $U^c:(\bar3,1,-2/3)$, $D^c:(\bar3,1,1/3)$, $L:(1,2,-1/2)$, and $E^c:(1,1,1)$. This uses [hypercharge](standard-model.md#hypercharge) normalized by $Q_{\rm electric}=T^3+Y$ and only left-handed [Weyl spinors](relativistic-quantum-field.md#weyl-spinor). Two [Higgs chiral doublets](#higgs-chiral-doublet) have charges $\pm1/2$. The three [vector superfields](#vector-superfield) transform as $(8,1,0)$, $(1,3,0)$ and $(1,1,0)$, supplying the [gauge bosons](relativistic-quantum-field.md#gauge-boson) and [gauginos](#gaugino).

### MSSM tree-level sfermion mass constraint

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

With canonical tree-level global [supersymmetry](supersymmetry.md), neutral [F-term](#f-term) breaking and no [D-term](#d-term) mass shifts, the [tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule) applies in conserved electric and color charge blocks. The corresponding scalar squared-mass average equals the fermion squared-mass average, so not every scalar partner can lie above that average. This obstructs making every [squark](#squark) heavy through direct canonical visible-sector breaking while retaining light quarks. Effective [soft supersymmetry breaking](#soft-supersymmetry-breaking), noncanonical interactions, radiative effects or [supergravity](#supergravity) invalidate the assumptions of that argument.

### R-parity

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/R-parity)

R-parity is the multiplicative quantum number $R_p=(-1)^{3(B-L)+2s}$. Standard Model particles are even and their superpartners are odd.

#### Matter parity

↑ **Parent:** [R-parity](#r-parity)

[Matter parity](#matter-parity) assigns odd parity to the quark and lepton [chiral superfields](#chiral-superfield) and even parity to the [Higgs chiral doublets](#higgs-chiral-doublet) and gauge [superfields](#superfield). It is related to component [R-parity](#r-parity) by $R_p=P_M(-1)^{2s}$. The Lorentz-invariant action contains an even number of fermions, so conserved matter parity is equivalent to conserved [R-parity](#r-parity). Products of four matter [superfields](#superfield) can be even while violating [baryon number](standard-model.md#baryon-number); matter parity alone does not exclude higher-dimensional [proton-decay operators](standard-model.md#proton-decay-operator).

##### Matter parity allows Majorana neutrino masses

↑ **Parent:** [Matter parity](#matter-parity)

[Matter parity](#matter-parity) assigns $-1$ to every matter [chiral superfield](#chiral-superfield), including a singlet $N$ describing a conjugate [right-handed neutrino](standard-model.md#right-handed-neutrino), and $+1$ to Higgs [chiral superfields](#chiral-superfield). Thus the quadratic [superpotential](#superpotential) term $\frac12M_{ij}N_iN_j$ is even, although it changes [lepton number](standard-model.md#lepton-number) by two. The higher-degree operators $QQQL$ and $(LH_u)^2$ are also even and violate [baryon number](standard-model.md#baryon-number) or [lepton number](standard-model.md#lepton-number). Exact [R-parity](#r-parity) therefore forbids the renormalizable trilinear violations $LLE$, $LQD$, $UDD$, $NH_dH_u$, $NNN$, but does not imply conservation of these continuous charges in every allowed interaction.

#### R-parity violation

↑ **Parent:** [R-parity](#r-parity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/R-parity_violation)

R-parity violation permits interactions containing an odd number of superpartners. Renormalizable R-parity-violating interactions can violate lepton number or baryon number, and allowing both generically induces rapid proton decay.

##### Squark-mediated proton decay

↑ **Parent:** [R-parity violation](#r-parity-violation)

Simultaneous trilinear [baryon number](standard-model.md#baryon-number) and [lepton number](standard-model.md#lepton-number) violation permits a [squark](#squark) to connect the two interactions and induce a dimension-six [proton-decay operator](standard-model.md#proton-decay-operator). Its coefficient is of order $\lambda'\lambda''/m_{\widetilde q}^2$. A dimensional decay-width estimate then gives $\Gamma_p\sim|\lambda'\lambda''|^2m_p^5/m_{\widetilde q}^4$, up to phase space and hadronic matrix elements. The flavor antisymmetry of $U^cD^cD^c$ matters: the two down-type flavor indices must differ. For example, $\lambda''_{112}$ and $\lambda'_{112}$ allow strange-squark exchange in $p\to e^+\pi^0$.

###### Four-fermion matching for squark-mediated proton decay

↑ **Parent:** [Squark-mediated proton decay](#squark-mediated-proton-decay)

The [R-parity violation](#r-parity-violation) vertices from $LQD$ and $UDD$ can both contain the same down-type [squark](#squark). Write its linear couplings as $-\widetilde d A-\widetilde d^*A^\dagger$ and its mass term as $-M^2|\widetilde d|^2$. Eliminating it gives $A^\dagger A/M^2$. The cross term is $(\lambda'\lambda''^*/M^2)(\nu d_L-eu_L)(u^{c\dagger}d^{c\dagger})+\mathrm{h.c.}$, with the color [Levi-Civita symbol](calculus.md#levi-civita-symbol) contracting the three quarks. It changes [baryon number](standard-model.md#baryon-number) and [lepton number](standard-model.md#lepton-number) together and supplies the dimension-six [proton-decay operator](standard-model.md#proton-decay-operator) for $p\to e^+\pi^0$. The two down-flavor indices in $UDD$ must differ, so strange- or bottom-squark exchange is allowed but identical down flavors vanish.

###### Proton-lifetime bound on a product of R-parity-violating couplings

↑ **Parent:** [Squark-mediated proton decay](#squark-mediated-proton-decay)

Exchanging a down-type [squark](#squark) of mass $M$ between $LQD$ and $UDD$ vertices produces a dimension-six [effective operator](quantum-field-theory.md#effective-operator) with coefficient $C\sim\lambda'\lambda''/M^2$. [Dimensional analysis](physics.md#dimensional-analysis) then gives a [proton decay](standard-model.md#proton-decay) width $\Gamma_p=c_h|\lambda'\lambda''|^2m_p^5/M^4$, with a dimensionless factor $c_h$ containing hadronic matrix elements and phase space. A lifetime bound $\tau_p>\tau_{\min}$ implies $|\lambda'\lambda''|<M^2/\sqrt{c_h\tau_{\min}m_p^5}$. The bound is on the relevant flavour product and depends on the exchanged mass; [dimensional analysis](physics.md#dimensional-analysis) alone does not determine $c_h$.

### Supersymmetric gauge coupling unification

↑ **Parent:** [Minimal supersymmetric Standard Model](#minimal-supersymmetric-standard-model)

In the MSSM, superpartners change the three Standard Model gauge beta functions so that the inverse gauge couplings meet accurately near $2\times10^{16}$ GeV, up to threshold and higher-loop corrections. The corresponding Standard Model one-loop lines miss a common intersection.

## Supersymmetric gauge theory

↑ **Parent:** [Supersymmetry](supersymmetry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetric_gauge_theory)

A supersymmetric gauge theory combines vector superfields with charged matter superfields so that gauge invariance and supersymmetry are both manifest.

### Ten-dimensional super Yang-Mills theory

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

Minimal ten-dimensional [supersymmetric gauge theory](#supersymmetric-gauge-theory) contains a [gauge field](relativistic-quantum-field.md#gauge-field) and an adjoint [Majorana-Weyl spinor](relativistic-quantum-field.md#majorana-weyl-spinor). They have eight propagating [bosonic](quantum-mechanics.md#boson) and eight propagating [fermionic](quantum-mechanics.md#fermion) states per gauge generator and sixteen real [supercharges](#supersymmetry-generator). A toroidal zero-mode [dimensional reduction](physics.md#dimensional-reduction) to four dimensions gives one [gauge field](relativistic-quantum-field.md#gauge-field), six real adjoint [scalar fields](quantum-field-theory.md#scalar-field), and four adjoint [Weyl spinors](relativistic-quantum-field.md#weyl-spinor): a [four-dimensional N=4 super Yang-Mills theory](#four-dimensional-n-4-super-yang-mills-theory). The internal field strength $F_{mn}=-ig[X_m,X_n]$ gives the nonnegative [scalar potential](quantum-field-theory.md#scalar-potential) $V=\frac{g^2}{4}\sum_{m,n}\lVert[X_m,X_n]\rVert^2$, where the norm uses a positive invariant inner product on the [Lie algebra](lie-algebra.md). Its minima are commuting tuples of adjoint [scalar fields](quantum-field-theory.md#scalar-field).

<h3 id="seiberg-witten-theory">Seiberg–Witten theory</h3>

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seiberg–Witten_theory)

In four-dimensional $\mathcal N=2$ [supersymmetric gauge theory](#supersymmetric-gauge-theory), Seiberg–Witten theory determines exact low-energy quantities from the geometry of the vacuum parameter space. For rank one, the [central charge in supersymmetry](#central-charge-in-supersymmetry) is proportional to $n_ea+n_ma_D$, with integral electric and magnetic charges and $a_D$ the dual scalar period. The [BPS bound in supersymmetry](#bps-bound-in-supersymmetry) fixes the mass of a short state by this charge combination. Its vanishing identifies loci where a [magnetic monopole](physics.md#magnetic-monopole) or [dyon](physics.md#dyon) can become massless, even when the original electric description is strongly coupled.

### Supersymmetric Higgs mechanism

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

At a vacuum obeying [F-flatness](#f-flatness) and [D-flatness](#d-flatness), charged [scalar field](quantum-field-theory.md#scalar-field) expectation values can break an internal [gauge symmetry](relativistic-quantum-field.md#gauge-invariance) while preserving [supersymmetry](supersymmetry.md). For each broken generator, a massless [vector multiplet](#supersymmetric-vector-multiplet) combines with a [chiral superfield](#chiral-superfield) into a [massive N=1 vector multiplet](#massive-n-1-vector-multiplet). The vector absorbs one real [Goldstone boson](critical-phenomenon.md#goldstone-boson); a real scalar remains, and the [gaugino](#gaugino) mixes with a [higgsino](#higgsino). All four bosonic and four fermionic on-shell states have a common mass.

<h3 id="four-dimensional-n-4-super-yang-mills-theory">Four-dimensional N=4 super Yang-Mills theory</h3>

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

A four-dimensional $\mathcal N=4$ [supersymmetric gauge theory](#supersymmetric-gauge-theory) has one [supersymmetric vector multiplet](#supersymmetric-vector-multiplet) containing a [gauge boson](relativistic-quantum-field.md#gauge-boson), four [Weyl spinors](relativistic-quantum-field.md#weyl-spinor), and six [real scalar fields](scalar-field-theory.md#real-scalar-field) in the adjoint [group representation](representation-theory.md#group-representation). Its massless [helicity](special-relativity.md#helicity) multiplicities are $1,4,6,4,1$ from [helicity](special-relativity.md#helicity) $1$ to $-1$.

<h4 id="commuting-scalar-vacua-of-four-dimensional-n-4-yang-mills-theory">Commuting-scalar vacua of four-dimensional N=4 Yang-Mills theory</h4>

↑ **Parent:** [Four-dimensional N=4 super Yang-Mills theory](#four-dimensional-n-4-super-yang-mills-theory)

The [scalar potential](quantum-field-theory.md#scalar-potential) is a positive sum of squared commutators of the six adjoint [scalar fields](quantum-field-theory.md#scalar-field). It vanishes precisely when they commute. For a compact gauge group, simultaneous conjugation puts a commuting tuple in a Cartan subalgebra. Its arbitrary $6r$ real coordinates are classical [flat directions of a scalar potential](quantum-field-theory.md#flat-direction-of-a-scalar-potential), with residual identification by the [Weyl group](semisimple-lie-algebra.md#weyl-group). For $SU(N)$ the simultaneous eigenvalue vectors also obey the tracelessness constraint. Generic values break the gauge group to its maximal torus.

### R-symmetry

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/R-symmetry)

An R-symmetry acts nontrivially on the supersymmetry generators. In four-dimensional N=1 supersymmetry, the superspace coordinate $\theta$ has R-charge one, so a superpotential must have R-charge two.

#### R-charge

↑ **Parent:** [R-symmetry](#r-symmetry)

R-charge is the charge under a continuous R-symmetry. In four-dimensional N=1 supersymmetry, the fermion in a chiral multiplet has R-charge one less than its scalar, and every superpotential term has R-charge two.

<h5 id="chiral-primary-operator-in-four-dimensional-n-1-supersymmetry">Chiral primary operator in four-dimensional N=1 supersymmetry</h5>

↑ **Parent:** [R-charge](#r-charge)

A scalar chiral primary operator at a four-dimensional N=1 superconformal fixed point saturates a shortening bound and obeys $\Delta=3R/2$.

#### Vector R-symmetry

↑ **Parent:** [R-symmetry](#r-symmetry)

In two-dimensional N=(2,2) supersymmetry, vector R-symmetry rotates $\theta^+$ and $\theta^-$ with the same phase. A chiral superspace measure has vector R-charge minus two.

#### Axial R-symmetry

↑ **Parent:** [R-symmetry](#r-symmetry)

In two-dimensional N=(2,2) supersymmetry, axial R-symmetry rotates $\theta^+$ and $\theta^-$ with opposite phases. A twisted chiral superspace measure has axial R-charge minus two.

### Supersymmetric vacuum

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

A vacuum of a globally supersymmetric gauge theory preserves supersymmetry exactly when every auxiliary F-field and D-field can vanish simultaneously. Its vacuum energy is then zero because the scalar potential is a sum of nonnegative squares.

#### F-flatness

↑ **Parent:** [Supersymmetric vacuum](#supersymmetric-vacuum)

F-flatness is the system $\partial W/\partial\phi_i=0$ obtained by setting every chiral-multiplet auxiliary field to zero.

#### D-flatness

↑ **Parent:** [Supersymmetric vacuum](#supersymmetric-vacuum)

D-flatness sets every vector-multiplet auxiliary field to zero. Quotienting its solution set by the compact gauge group is equivalent, under standard stability conditions, to quotienting the F-flat variety by the complexified gauge group.

#### Vacuum moduli space of a supersymmetric gauge theory

↑ **Parent:** [Supersymmetric vacuum](#supersymmetric-vacuum)

The vacuum moduli space is the space of simultaneous F-flat and D-flat configurations modulo gauge transformations. Gauge-invariant chiral operators often provide holomorphic coordinates, subject to algebraic constraints.

##### Neutral flat direction with oppositely charged chiral fields

↑ **Parent:** [Vacuum moduli space of a supersymmetric gauge theory](#vacuum-moduli-space-of-a-supersymmetric-gauge-theory)

For canonical [chiral superfields](#chiral-superfield), nonzero $\lambda$, a gauged $U(1)$ with charges $(0,+1,-1)$, and no [Fayet–Iliopoulos term](#fayet-iliopoulos-term), [F-flatness](#f-flatness) requires the charged product to vanish and [D-flatness](#d-flatness) requires equal charged magnitudes. Together they force both charged scalar values to zero, leaving the neutral scalar arbitrary. The [vacuum moduli space of a supersymmetric gauge theory](#vacuum-moduli-space-of-a-supersymmetric-gauge-theory) has zero energy, unbroken gauge symmetry and unbroken [supersymmetry](supersymmetry.md). At $\lambda=0$, equal nonzero charged magnitudes instead permit a gauge-Higgsed supersymmetric branch. A neutral modulus alone does not imply internal gauge breaking.

##### Higgs branch

↑ **Parent:** [Vacuum moduli space of a supersymmetric gauge theory](#vacuum-moduli-space-of-a-supersymmetric-gauge-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Higgs_branch)

A Higgs branch is a component on which charged scalar expectation values break some or all of the gauge group. It is often obtained as a Kähler or hyperkähler quotient.

##### Coulomb branch

↑ **Parent:** [Vacuum moduli space of a supersymmetric gauge theory](#vacuum-moduli-space-of-a-supersymmetric-gauge-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coulomb_branch)

A Coulomb branch is a component on which scalar expectation values in vector or neutral multiplets leave an Abelian gauge sector unbroken. Charged fields can become massless at special points where additional branches meet it.

### Supersymmetric quantum electrodynamics

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

Supersymmetric quantum electrodynamics is an Abelian supersymmetric gauge theory with charged chiral multiplets. Its scalar potential combines F-term constraints with the U(1) D-term and any [Fayet–Iliopoulos term](#fayet-iliopoulos-term).

### Supersymmetric quantum chromodynamics

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supersymmetric_quantum_chromodynamics)

Supersymmetric quantum chromodynamics is an N=1 supersymmetric $SU(N_c)$ gauge theory with $N_f$ fundamental and $N_f$ antifundamental chiral multiplets.

#### Supersymmetric conformal window

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)

The supersymmetric conformal window is the range of flavor numbers for which an asymptotically free supersymmetric gauge theory flows to an interacting infrared fixed point. Its lower edge is often detected when a gauge-invariant chiral operator reaches the scalar unitarity bound.

#### Chiral ring of a supersymmetric gauge theory

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)

The chiral ring is generated by gauge-invariant chiral operators modulo relations that vanish by F-term equations. In SQCD its basic generators are meson and baryon operators.

##### Meson operator in supersymmetric quantum chromodynamics

↑ **Parent:** [Chiral ring of a supersymmetric gauge theory](#chiral-ring-of-a-supersymmetric-gauge-theory)

An SQCD meson is the gauge-invariant chiral bilinear $M^i{}_j=\widetilde Q_jQ^i$. It transforms under both flavor groups and parametrizes mesonic directions of the vacuum moduli space.

##### Baryon operator in supersymmetric quantum chromodynamics

↑ **Parent:** [Chiral ring of a supersymmetric gauge theory](#chiral-ring-of-a-supersymmetric-gauge-theory)

An SQCD baryon contracts $N_c$ fundamental fields with the gauge epsilon tensor; an antibaryon similarly contracts antifundamentals. Such operators exist when enough flavors are available and obey relations with the mesons.

#### Holomorphic strong-coupling scale

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)

The holomorphic strong-coupling scale packages the gauge coupling and theta angle into $\Lambda^{b_0}$. Treating it as a spurion under anomalous chiral symmetries strongly constrains nonperturbative superpotentials and moduli-space deformations.

<h5 id="affleck-dine-seiberg-superpotential">Affleck–Dine–Seiberg superpotential</h5>

↑ **Parent:** [Holomorphic strong-coupling scale](#holomorphic-strong-coupling-scale)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Affleck–Dine–Seiberg_superpotential)

For SQCD with $N_f<N_c$, strong dynamics generates the Affleck–Dine–Seiberg superpotential. For $SU(2)$ with one flavor it is proportional to $\Lambda^5/M$ and produces a runaway to infinite meson expectation value.

#### Quantum-deformed moduli space

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)

When $N_f=N_c$, SQCD has no generated superpotential but its classical constraint is shifted by the strong-coupling scale. For $SU(2)$ with two flavors, one convention gives $\det M-B\widetilde B=\Lambda^4$.

#### s-confinement

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)

A theory s-confines when its infrared physics is described smoothly everywhere on moduli space by gauge-invariant composites with a local superpotential and no remaining gauge group. SQCD with $N_f=N_c+1$ is the standard example.

#### Seiberg duality

↑ **Parent:** [Supersymmetric quantum chromodynamics](#supersymmetric-quantum-chromodynamics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seiberg_duality)

Seiberg duality states that two different N=1 supersymmetric gauge theories flow to the same infrared quantum field theory. Gauge-invariant operators, global symmetries, 't Hooft anomalies and deformations match even though the ultraviolet gauge groups and elementary fields differ.

### One-loop beta function of a supersymmetric gauge theory

↑ **Parent:** [Supersymmetric gauge theory](#supersymmetric-gauge-theory)

With the index convention $I(\mathbf N)=1$ for an $SU(N)$ fundamental, an N=1 supersymmetric gauge theory has $b_0=\tfrac32I(\mathrm{adj})-\tfrac12\sum_i I(R_i)$. Positive $b_0$ gives asymptotic freedom, while negative $b_0$ makes the gauge interaction infrared free near the Gaussian fixed point.

## Supergravity

↑ **Parent:** [Supersymmetry](supersymmetry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supergravity)

Supergravity is a theory with local supersymmetry and necessarily contains gravity.

<h3 id="composite-kahler-connection">Composite Kähler connection</h3>

↑ **Parent:** [Supergravity](#supergravity)

The scalar fields of chiral matter induce a composite phase connection proportional to $i(K_i\partial_\mu z^i-K_{\bar i}\partial_\mu\bar z^{\bar i})$. For canonical [Kähler potential](#kahler-potential) it is proportional to the scalar phase current. The chiral matter fermions and [gravitino](#gravitino) have appropriate Kähler weights; expanding their connection terms produces scalar-current–fermion-bilinear couplings. Overall signs and coefficients depend on spinor and Planck-scale conventions.

### Eleven-dimensional supergravity

↑ **Parent:** [Supergravity](#supergravity)

Eleven-dimensional supergravity contains a metric, a three-form potential and a gravitino. Its bosonic on-shell counts are $11(11-3)/2=44$ for the metric and $\binom93=84$ for the three-form, totaling $128$. Flat toroidal zero-mode reduction gives [type IIA supergravity](#type-iia-supergravity) in ten dimensions and [four-dimensional N=8 supergravity](#four-dimensional-n-8-supergravity) in four dimensions without losing these bosonic polarizations.

// Target: supersymmetry.bigb

#### Freund-Rubin compactification

↑ **Parent:** [Eleven-dimensional supergravity](#eleven-dimensional-supergravity)

A product compactification supported by a four-form proportional to one factor's volume form. For the maximally supersymmetric membrane throat, the other factor is a round $S^7$ and the radii obey $R_{S^7}=2R_{\rm AdS}$. The flux links the curvature scales through the supergravity field equations.

##### Maximal supersymmetry of AdS4 times S7

↑ **Parent:** [Freund-Rubin compactification](#freund-rubin-compactification)

With the membrane [Freund-Rubin compactification](#freund-rubin-compactification) flux and the required radius ratio, the [Killing spinor](#killing-spinor) equation separates into AdS4 and sphere equations with correlated signs. The respective real solution dimensions are four and eight, giving thirty-two. The associated Killing-spinor connections have vanishing curvature for these choices, so arbitrary initial spinor data generate solutions locally; standard global spin structures give the usual maximally supersymmetric background.

// Target: geometry-and-topology.bigb

#### Toroidal reduction of eleven-dimensional supergravity

↑ **Parent:** [Eleven-dimensional supergravity](#eleven-dimensional-supergravity)

Circle reduction splits the metric into a ten-dimensional graviton, one vector and one scalar, and the three-form into a three-form and two-form. Seven-torus reduction gives a four-dimensional graviton, $7+21=28$ vectors, $28+35$ direct scalars and seven two-forms. The [two-form scalar duality](relativistic-quantum-field.md#two-form-scalar-duality) turns the latter into seven more scalars, giving $70$ in all. A remaining four-dimensional three-form has no local polarization. These are zero-mode counts without fluxes, orbifold projections or moduli freezing.

##### Circle reduction of eleven-dimensional supergravity

↑ **Parent:** [Toroidal reduction of eleven-dimensional supergravity](#toroidal-reduction-of-eleven-dimensional-supergravity)

For circle-independent fields, the metric gives the type-IIA string-frame metric, [dilaton](string-theory.md#dilaton) and RR one-form. Decomposing $A_3=C_3+B_2\wedge dy$ gives the RR three-form and [Kalb–Ramond field](string-theory.md#kalb-ramond-field). With $H_3=dB_2$, $F_2=dC_1$, the horizontal four-form is $\widetilde F_4=dC_3-C_1\wedge H_3$. The Einstein term reduces, modulo a total derivative, to $\sqrt{-g}[e^{-2\Phi}(R+4(\nabla\Phi)^2)-\tfrac14F_{2,\mu\nu}F_2^{\mu\nu}]$. The eleven-dimensional form norm gives $\sqrt{-g}[e^{-2\Phi}|H_3|^2+|\widetilde F_4|^2]$, where $|F_k|^2=F^2/k!$. Ordinary reduction generates massless [type IIA supergravity](#type-iia-supergravity), not [Romans mass](#romans-mass).

###### Reduction of the eleven-dimensional Chern-Simons term

↑ **Parent:** [Circle reduction of eleven-dimensional supergravity](#circle-reduction-of-eleven-dimensional-supergravity)

Put $A_3=C_3+B_2\wedge dy$ and $F_4=G_4+H_3\wedge dy$, where $G_4=dC_3$. The circle component of $A_3\wedge F_4\wedge F_4$ is $[B_2\wedge G_4\wedge G_4+2C_3\wedge G_4\wedge H_3]\wedge dy$. Since $d(C_3\wedge B_2\wedge G_4)=B_2\wedge G_4\wedge G_4-C_3\wedge H_3\wedge G_4$, its integral equals three copies of $B_2\wedge G_4\wedge G_4$ up to a boundary term. The coefficient therefore becomes $-1/2$ after circle integration. Boundary terms and global potential patching must be retained when the spacetime has boundary or nontrivial flux topology.

### Killing spinor

↑ **Parent:** [Supergravity](#supergravity)

A [Killing spinor](#killing-spinor) is a nonzero [supersymmetry](supersymmetry.md) parameter that makes the fermionic transformations vanish on a bosonic background. In undeformed [minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity) it is parallel, $\nabla_\mu\epsilon=0$; in its cosmological deformation the equation uses $\mathcal D_\mu=\nabla_\mu+(m/2)\gamma_\mu$. Its commuting [Dirac current](quantum-field-theory.md#dirac-current) is a [Killing vector](general-relativity.md#killing-vector-field), since the spinor equation makes the symmetric [covariant derivative](general-relativity.md#covariant-derivative) of the current vanish. General [supergravity](#supergravity) theories also impose the vanishing of matter-fermion transformations.

#### Anti-de Sitter Killing-spinor connection

↑ **Parent:** [Killing spinor](#killing-spinor)

For constant sectional curvature $-1/a^2$, spin curvature is $[\nabla_\mu,\nabla_\nu]=-\gamma_{\mu\nu}/(2a^2)$. The added Clifford term in $\mathcal D$ has the opposite commutator, making $\mathcal D$ flat. On a simply connected region, parallel transport of any initial spinor is path independent and constructs solutions of $\mathcal D\epsilon=0$. Thus [Anti-de Sitter spacetime](general-relativity.md#anti-de-sitter-spacetime) and its universal cover admit the associated [Killing spinors](#killing-spinor) locally and, with appropriate global spin data, globally.

#### Parallel-spinor classification of vacuum four-geometries

↑ **Parent:** [Killing spinor](#killing-spinor)

A parallel commuting [Dirac current](quantum-field-theory.md#dirac-current) is causal. If timelike, the geometry locally splits as a time line times a three-dimensional Ricci-flat metric; three-dimensional Ricci flatness implies flatness. If null, the stabilizer of a parallel spinor in $\operatorname{Spin}(1,3)$ contains only null rotations, and the local vacuum metric is $ds^2=-2du\,dv+dx^2+dy^2+H(u,x,y)du^2$ with $H_{xx}+H_{yy}=0$. Constant spinors obeying $\gamma^+\epsilon=0$ are parallel. These are local statements; global quotients must preserve a compatible [spin structure](riemannian-geometry.md#spin-structure).

### Minimal four-dimensional supergravity

↑ **Parent:** [Supergravity](#supergravity)

Minimal four-dimensional [supergravity](#supergravity) couples a graviton to one Majorana [gravitino](#gravitino). In the normalization $\delta e_\mu{}^a=2\kappa\bar\epsilon\gamma^a\psi_\mu$, $\delta\psi_\mu=\nabla_\mu\epsilon/\kappa$, its [action](classical-mechanics.md#action) through quadratic [fermion](quantum-mechanics.md#fermion) order is $\int e[R/(2\kappa^2)-2\bar\psi_\mu\gamma^{\mu\nu\rho}\nabla_\nu\psi_\rho]$. Rescaling the [gravitino](#gravitino) and parameter by two gives the usual canonical kinetic coefficient $-1/2$. The [curvature](differential-geometry.md#curvature) identity $\gamma^{\mu\nu\rho}\nabla_\nu\nabla_\rho\epsilon=G^{\mu\nu}\gamma_\nu\epsilon/2$ cancels the Einstein-Hilbert variation against the Rarita-Schwinger variation. The omitted cubic-fermion variations require the quartic-fermion completion.

#### Old-minimal supergravity

↑ **Parent:** [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)

Old-minimal four-dimensional [supergravity](#supergravity) adds a complex scalar $M$ and a real vector $b_\mu$ to the [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime) and [gravitino](#gravitino). These six real bosonic [auxiliary field](#auxiliary-field) components have no propagating kinetic terms. They balance the [off-shell component count of minimal supergravity](#off-shell-component-count-of-minimal-supergravity) and permit the local [supersymmetry](supersymmetry.md) algebra to close without imposing the propagating [Euler-Lagrange field equations](quantum-field-theory.md#euler-lagrange-field-equation).

#### Off-shell component count of minimal supergravity

↑ **Parent:** [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)

A four-dimensional [Majorana spinor](relativistic-quantum-field.md#majorana-spinor) [gravitino](#gravitino) has $4\times4=16$ real components, minus four local [supersymmetry](supersymmetry.md) gauge functions, leaving twelve before using any [Euler-Lagrange field equation](quantum-field-theory.md#euler-lagrange-field-equation). A [vierbein](general-relativity.md#orthonormal-coframe-in-spacetime) has sixteen real components, minus six local [Lorentz transformation](special-relativity.md#lorentz-transformation) and four [diffeomorphism](geometry-and-topology.md#diffeomorphism) gauge functions, leaving six. Equivalently, a symmetric [metric tensor](general-relativity.md#metric-tensor) has $10-4=6$. The propagating [graviton](quantum-theory.md#graviton) and massless [gravitino](#gravitino) each have two states [on shell](quantum-field-theory.md#on-shell). Six bosonic [auxiliary field](#auxiliary-field) components complete an off-shell [supergravity multiplet](#supergravity-multiplet).

#### Gravitino-induced torsion

↑ **Parent:** [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)

With canonical [Rarita-Schwinger field](relativistic-quantum-field.md#rarita-schwinger-field) normalization, one convention gives the displayed [torsion tensor](fiber-bundle.md#torsion-tensor). Its [contorsion tensor](fiber-bundle.md#contorsion-tensor) is $K_{\mu ab}=\kappa^2(\bar\psi_\mu\gamma_a\psi_b-\bar\psi_\mu\gamma_b\psi_a+\bar\psi_a\gamma_\mu\psi_b)/4$. The algebraic [spin connection](connection-1-form.md#spin-connection) equation determines $\widetilde\omega=\omega(e)+K$; substituting it in the [action](classical-mechanics.md#action) produces four-[fermion](quantum-mechanics.md#fermion) terms. This is an instance of [Einstein-Cartan theory](general-relativity.md#einstein-cartan-theory) and is efficiently varied using the [1.5-order formalism](general-relativity.md#1-5-order-formalism). A rescaled [gravitino](#gravitino) changes the displayed coefficient.

#### Supergravity coupling of an Abelian vector multiplet

↑ **Parent:** [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)

An Abelian [vector multiplet](#supersymmetric-vector-multiplet) contains a [Maxwell field](electromagnetism.md#electromagnetic-field) and a Majorana [gaugino](#gaugino). With the doubled [gravitino](#gravitino) normalization, add $e[-F^2/4-\bar\lambda\not\nabla\lambda/2-(\kappa/2)\bar\psi_\mu F_{ab}\gamma^{ab}\gamma^\mu\lambda]$. The leading transformations are $\delta A_\mu=\bar\epsilon\gamma_\mu\lambda$ and $\delta\lambda=-F_{ab}\gamma^{ab}\epsilon/2$. Promoting the rigid parameter to a function produces the current $(F_{ab}/2)\gamma^{ab}\gamma^\mu\lambda$ multiplying $\nabla_\mu\bar\epsilon$; the gravitino-current term cancels it. The Clifford identity $(F_{ab}\gamma^{ab})\gamma^\mu(F_{cd}\gamma^{cd})=8T_{\rm EM}^{\mu\nu}\gamma_\nu$ cancels the Maxwell stress variation. Supercovariant field strengths and quartic [fermions](quantum-mechanics.md#fermion) complete the transformations beyond this order.

#### Anti-de Sitter deformation of minimal supergravity

↑ **Parent:** [Minimal four-dimensional supergravity](#minimal-four-dimensional-supergravity)

A real cosmological deformation adds $3m^2e/\kappa^2+2me\bar\psi_\mu\gamma^{\mu\nu}\psi_\nu$ and changes the [gravitino](#gravitino) variation to $\mathcal D_\mu\epsilon/\kappa$. The modified [commutator](lie-algebra.md#commutator) identity is $\gamma^{\mu\nu\rho}\mathcal D_\nu\mathcal D_\rho\epsilon=(G^{\mu\nu}+\Lambda g^{\mu\nu})\gamma_\nu\epsilon/2$. It fixes the negative [cosmological constant](cosmology.md#cosmological-constant) in terms of the [gravitino](#gravitino) [mass](classical-mechanics.md#mass) parameter. A positive [cosmological constant](cosmology.md#cosmological-constant) is not obtained by this real unbroken minimal deformation.

### Maximal nine-dimensional supergravity

↑ **Parent:** [Supergravity](#supergravity)

The ungauged maximal nine-dimensional [supergravity](#supergravity) zero-mode multiplet has one metric, three vectors, two two-forms, one three-form and three scalars, giving $128$ bosonic states. Two Majorana [gravitini](#gravitino) and four Majorana spin-one-half fields give $128$ fermionic states. Flat-circle reductions of massless type IIA and type IIB theories, and a flat-two-torus reduction of eleven-dimensional [supergravity](#supergravity), give this same nonchiral spectrum.

### Type IIB supergravity

↑ **Parent:** [Supergravity](#supergravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_IIB_supergravity)

Type IIB supergravity is the chiral ten-dimensional maximal [supergravity](#supergravity) with metric, [Kalb–Ramond field](string-theory.md#kalb-ramond-field), [dilaton](string-theory.md#dilaton), Ramond-Ramond zero-form, two-form and four-form potentials, and a self-dual five-form field strength. Two same-chirality Majorana-Weyl [gravitini](#gravitino) and two opposite-to-gravitino-chirality Majorana-Weyl [dilatini](#dilatino) complete its $128+128$ massless spectrum.

### Type IIA supergravity

↑ **Parent:** [Supergravity](#supergravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_IIA_supergravity)

Massless type IIA supergravity is the nonchiral ten-dimensional maximal [supergravity](#supergravity) with metric, [Kalb–Ramond field](string-theory.md#kalb-ramond-field), [dilaton](string-theory.md#dilaton), Ramond-Ramond one-form and three-form potentials, two opposite-chirality Majorana-Weyl [gravitini](#gravitino), and two opposite-chirality Majorana-Weyl [dilatini](#dilatino). Its massless spectrum has $128$ bosonic and $128$ fermionic polarizations. The two [supercharges](#supersymmetry-generator) have opposite ten-dimensional [chirality](relativistic-quantum-field.md#chirality-physics).

#### Massive type IIA supergravity

↑ **Parent:** [Type IIA supergravity](#type-iia-supergravity)

##### Romans mass

↑ **Parent:** [Massive type IIA supergravity](#massive-type-iia-supergravity)

The zero-form field strength deforms massless [type IIA supergravity](#type-iia-supergravity). A [D8-brane](string-theory.md#d8-brane) changes this flux across its worldvolume; it is therefore outside the elementary massless [M-theory circle duality](string-theory.md#m-theory-circle-duality) dictionary.

// Target: physics.bigb

### Dilatino

↑ **Parent:** [Supergravity](#supergravity)

A dilatino is a spin-one-half fermionic partner in a [supergravity](#supergravity) theory containing a [dilaton](string-theory.md#dilaton). Type IIA and type IIB theories each contain two Majorana-Weyl dilatini with eight physical polarizations apiece. Their chirality assignments differ between the two theories.

### Super-Higgs mechanism

↑ **Parent:** [Supergravity](#supergravity)

When local [supersymmetry](supersymmetry.md) is spontaneously broken, the [gravitino](#gravitino) absorbs the [goldstino](#goldstino) and becomes massive. The two [goldstino](#goldstino) states provide its longitudinal spin-$1/2$ polarizations. With only global [supersymmetry breaking](#supersymmetry-breaking), the [goldstino](#goldstino) remains a physical massless particle. An ordinary [supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism) instead makes an internal spin-one [gauge boson](relativistic-quantum-field.md#gauge-boson) massive and can leave [supersymmetry](supersymmetry.md) unbroken.

### Gravitino

↑ **Parent:** [Supergravity](#supergravity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gravitino)

The gravitino is the spin-$3/2$ gauge field of local [supersymmetry](supersymmetry.md) and the partner of the [graviton](quantum-theory.md#graviton). A massless four-dimensional gravitino has two physical [helicities](special-relativity.md#helicity), $\pm3/2$; a massive one has four, adding $\pm1/2$. The [super-Higgs mechanism](#super-higgs-mechanism) supplies these extra states from the [goldstino](#goldstino).

### No-scale supergravity

↑ **Parent:** [Supergravity](#supergravity)

In a no-scale sector, the [Kähler metric](complex-geometry.md#kahler-metric) satisfies $K_iK^{i\bar j}K_{\bar j}=3$. If the [superpotential](#superpotential) is independent of that sector, its covariant derivatives contribute $3e^K|W|^2$, cancelling the universal $-3e^K|W|^2$ in the [supergravity F-term potential](#supergravity-f-term-potential). Spectator sectors can still contribute to the potential. This cancellation permits zero-energy minima with broken [supersymmetry](supersymmetry.md) and exact flat scalar directions.

#### Matter-logarithm no-scale potential

↑ **Parent:** [No-scale supergravity](#no-scale-supergravity)

For $s=S+\bar S>0$, $t=T+\bar T-|C|^2>0$, $K=-\log s-3\log t$ and a holomorphic [superpotential](#superpotential) independent of $T$, the exact [F-term](#f-term) potential is $V=e^K[s^2|D_SW|^2+(t/3)|W_C|^2]$. Inverting the mixed $T,C$ metric gives $K^{T\bar T}=t(t+|C|^2)/3$, $K^{T\bar C}=t\bar C/3$, $K^{C\bar T}=tC/3$, and $K^{C\bar C}=t/3$. Substitution of $D_TW=-3W/t$ and $D_CW=W_C+3\bar CW/t$ cancels all mixed terms, leaving $3|W|^2+(t/3)|W_C|^2$; the first term cancels the [supergravity](#supergravity) negative term.

##### No-scale volume runaway criterion

↑ **Parent:** [Matter-logarithm no-scale potential](#matter-logarithm-no-scale-potential)

If a [no-scale supergravity](#no-scale-supergravity) [scalar potential](quantum-field-theory.md#scalar-potential) has the displayed form with $y>0$ and nonnegative $A,B$ independent of the volume coordinate $y$, every point with $A+B>0$ has a direction of strictly decreasing potential. Thus a finite stationary vacuum requires $A=B=0$. If that common zero set is empty, the potential has infimum zero along $y\to\infty$ but no finite minimum. If the common zero set is nonempty, varying $y$ on it is a [flat direction of a scalar potential](quantum-field-theory.md#flat-direction-of-a-scalar-potential). This distinguishes an attained zero-energy vacuum from a decompactification runaway.

##### Cubic-matter no-scale vacuum with an exponential dilaton

↑ **Parent:** [Matter-logarithm no-scale potential](#matter-logarithm-no-scale-potential)

For $W=C^3+A+b$, $A=ae^{-\alpha S}$, the potential is $V=|C^3+b+(1+\alpha s)A|^2/(st^3)+3|C|^4/(st^2)$. A finite zero-energy vacuum requires $C=0$ and $b+(1+\alpha s)A=0$. With $a,b\ne0$, such a solution exists exactly when $0<|b/a|\le2e^{-1/2}$: the magnitude equation is $|b/a|=(1+x)e^{-x/2}$, $x=\alpha s>0$, whose maximum occurs at $x=1$. At that vacuum $F^S=F^C=0$ but $F^T=e^{K/2}t\bar W\ne0$. Both components of $T$ are flat, while $C$ is quartically lifted. If no root exists, the positive potential falls toward zero as $t\to\infty$ and has no finite minimum. If $a=b=0$, the $C=0$ family is supersymmetric instead.

###### Quartic stabilization at a double no-scale root

↑ **Parent:** [Cubic-matter no-scale vacuum with an exponential dilaton](#cubic-matter-no-scale-vacuum-with-an-exponential-dilaton)

For the [cubic-matter no-scale vacuum with an exponential dilaton](#cubic-matter-no-scale-vacuum-with-an-exponential-dilaton), put $x=S+\bar S$ and $A=ae^{-\alpha S}$. At $C=0$, zero energy requires $G(S)=b+(1+\alpha x)A=0$. On a fixed-imaginary-part slice, $s=\operatorname{Re}S$ gives $dG/ds=\alpha(1-2\alpha s)A$. At the double root $s_0=1/(2\alpha)$, the first derivative vanishes but the second is $-2\alpha^2A$, so $G=-\alpha^2A(s-s_0)^2+O((s-s_0)^3)$. Therefore $V=|G|^2/(xy^3)$ begins at fourth order. This real scalar has zero quadratic mass but is not an exact [flat direction of a scalar potential](quantum-field-theory.md#flat-direction-of-a-scalar-potential). The imaginary part of $S$ is still lifted quadratically, and the matter field $C$ also has a quartic leading potential. Exact flat directions instead come from the complex volume modulus $T$ along the zero-energy locus.

#### No-scale vacuum with a cubic matter superpotential

↑ **Parent:** [No-scale supergravity](#no-scale-supergravity)

The [no-scale supergravity](#no-scale-supergravity) identity cancels the negative gravitino contribution, leaving $V=e^{|C|^2}|3C^2+\bar C(C^3+B)|^2/(T+\bar T)^3$. Zero-energy minima occur at $C=0$ and, for $B\ne0$, three phase-related nonzero solutions with $|B|=|C|(3+|C|^2)$. Their $T$ [supergravity auxiliary field](#supergravity-auxiliary-field) is nonzero if $B\ne0$, while both real components of $T$ are flat on each vacuum branch. For $B=0$, the $C=0$ branch is instead supersymmetric and has zero [gravitino mass from a superpotential](#gravitino-mass-from-a-superpotential).

#### Finite zero-energy vacuum for a single exponential superpotential

↑ **Parent:** [No-scale supergravity](#no-scale-supergravity)

For $K=-\log(S+\bar S)-3\log(T+\bar T)$ and $W=ae^{-\alpha S}+b$ with $\alpha>0$, the potential is $|b+[1+\alpha(S+\bar S)]ae^{-\alpha S}|^2/[(S+\bar S)(T+\bar T)^3]$. With nonzero $a,b$, a finite zero-energy vacuum exists exactly when $0<|b/a|\le2e^{-1/2}$. To prove this, set $x=\alpha\operatorname{Re}S>0$; the magnitude equation is $|b/a|=(1+2x)e^{-x}$, whose derivative changes sign at $x=1/2$ and whose maximum is $2e^{-1/2}$. The phase fixes the imaginary part of $S$. At a zero-energy solution the $T$ [auxiliary field](#auxiliary-field) remains nonzero, so [supersymmetry](supersymmetry.md) is broken and both real components of $T$ are flat. If $a=b=0$, the family is instead supersymmetric.

#### No-scale identity from degree-one homogeneity

↑ **Parent:** [No-scale supergravity](#no-scale-supergravity)

Let $K=-3\log\Gamma$ where $\Gamma>0$ is twice differentiable and homogeneous of degree one. If the Kähler Hessian is invertible, the [Euler theorem for homogeneous functions](real-analysis.md#euler-theorem-for-homogeneous-functions) identities give $\tau_iK_{ij}=3\Gamma_j/\Gamma$, then $K^{-1}_{ij}\Gamma_j/\Gamma=\tau_i/3$ and $\Gamma_iK^{-1}_{ij}\Gamma_j/\Gamma^2=1/3$. Multiplication by nine gives the no-scale identity. A positive degree-one $\Gamma$ need not induce an invertible or positive [Kähler metric](complex-geometry.md#kahler-metric): $\Gamma=\tau_1+\tau_2$ gives a rank-one metric for $K$. The [Hessian matrix](calculus.md#hessian-matrix) $(\Gamma_{ij})$ itself always has the radial null vector $\tau$, whereas the [Hessian matrix](calculus.md#hessian-matrix) of $K$ can be invertible. In a larger theory the relevant full inverse metric, or a decoupled block, must obey the identity.

### Supergravity auxiliary field

↑ **Parent:** [Supergravity](#supergravity)

After eliminating the chiral [auxiliary fields](#auxiliary-field) in Planck-unit [supergravity](#supergravity), one convention gives $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$. The upper-index inverse satisfies $K_{i\bar j}K^{k\bar j}=\delta_i^k$. Nonzero auxiliary expectation values diagnose [supersymmetry breaking](#supersymmetry-breaking); their common phase convention does not affect the vanishing condition.

<h3 id="four-dimensional-n-8-supergravity">Four-dimensional N=8 supergravity</h3>

↑ **Parent:** [Supergravity](#supergravity)

Four-dimensional $\mathcal N=8$ [supergravity](#supergravity) has eight independent [Weyl spinor](relativistic-quantum-field.md#weyl-spinor) [supercharges](#supersymmetry-generator). Its [supergravity multiplet](#supergravity-multiplet) has [helicities](special-relativity.md#helicity) from $2$ to $-2$, with multiplicities $1,8,28,56,70,56,28,8,1$.

### Supergravity multiplet

↑ **Parent:** [Supergravity](#supergravity)

A supergravity multiplet is a [supermultiplet](#supermultiplet) containing a [graviton](quantum-theory.md#graviton) and its supersymmetric partners. In [four-dimensional N=8 supergravity](#four-dimensional-n-8-supergravity), the irreducible [massless supermultiplet](#massless-supermultiplet) contains $128$ [boson](quantum-mechanics.md#boson) and $128$ [fermion](quantum-mechanics.md#fermion) states.

### Supergravity F-term potential

↑ **Parent:** [Supergravity](#supergravity)

In Planck units, chiral multiplets in four-dimensional $\mathcal N=1$ supergravity have

$$
V_F=e^K\left(K^{i\bar j}D_iW\,D_{\bar j}\overline W-3|W|^2\right),
\qquad
D_iW=\partial_iW+(\partial_iK)W.
$$

#### Supergravity moment-map constraint on D-term breaking

↑ **Parent:** [Supergravity F-term potential](#supergravity-f-term-potential)

Let $k^i$ generate a holomorphic [gauge transformation](electromagnetism.md#gauge-transformation), with $k^i\partial_iW=-\kappa^2rW$ and [moment map](symplectic-geometry.md#moment-map) $\mathcal P=i(k^iK_i-r)$. Substitution of the [Kähler covariant derivative of a superpotential](#kahler-covariant-derivative-of-a-superpotential) gives the displayed identity. Consequently, a finite point with $W\ne0$ and all $D_iW=0$ also has $\mathcal P=0$. Pure [D-term](#d-term) breaking with vanishing chiral [auxiliary fields](#auxiliary-field) can therefore evade this argument only where $W=0$ or outside its hypotheses. In conventional two-derivative matter-coupled [supergravity](#supergravity), a constant [Fayet–Iliopoulos term](#fayet-iliopoulos-term) gauges an [R-symmetry](#r-symmetry) and constrains the transformation of $W$; a neutral [superpotential](#superpotential) and an independently assigned nonzero constant shift are not generally consistent. The gauge-covariance restriction is derived in [Van Proeyen's discussion of Fayet–Iliopoulos terms and R-symmetry](https://arxiv.org/abs/hep-th/0410053).

#### Gravitino mass from a superpotential

↑ **Parent:** [Supergravity F-term potential](#supergravity-f-term-potential)

The [gravitino](#gravitino) mass parameter in four-dimensional [supergravity](#supergravity) is the displayed expression. In a zero-energy [supersymmetry breaking](#supersymmetry-breaking) vacuum with only [F-term](#f-term) breaking, $K_{i\bar j}F^i\overline{F^j}=3m_{3/2}^2/\kappa^2$. Writing this norm as $\Lambda_{\mathrm{SUSY}}^4$ gives $m_{3/2}=\Lambda_{\mathrm{SUSY}}^2/(\sqrt3m_p)$. It is small relative to $\Lambda_{\mathrm{SUSY}}$ when the breaking scale is below the [Planck mass](physics.md#planck-mass). The [super-Higgs mechanism](#super-higgs-mechanism) supplies the longitudinal [gravitino](#gravitino) states.

<h4 id="kahler-covariant-derivative-of-a-superpotential">Kähler covariant derivative of a superpotential</h4>

↑ **Parent:** [Supergravity F-term potential](#supergravity-f-term-potential)

The Kähler covariant derivative of a [superpotential](#superpotential) transforms by the same holomorphic factor as the [superpotential](#superpotential) under a [Kähler transformation](#kahler-transformation). This follows by differentiating $e^{-f}W$ and cancelling the extra derivative of $f$ against the shift of $K_i$.

#### Polonyi model

↑ **Parent:** [Supergravity F-term potential](#supergravity-f-term-potential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polonyi_model)

The Polonyi model uses a canonical Kähler potential and a superpotential linear in one chiral superfield to obtain spontaneous supersymmetry breaking.

##### Stable zero-energy Polonyi vacuum

↑ **Parent:** [Polonyi model](#polonyi-model)

For $m\ne0$ and positive $\beta$, the [Polonyi model](#polonyi-model) has a unique zero-energy [global minimum](analysis.md#global-minimum) at $\beta=2-\sqrt3$, $\langle z\rangle=\sqrt3-1$. Writing $u=\operatorname{Re}z-(\sqrt3-1)$ and $y=\operatorname{Im}z$, its potential bracket is $(u^2+y^2+\sqrt3u)^2+(2\sqrt3-3)u^2+(4-2\sqrt3)y^2$, a sum of nonnegative terms. The real and imaginary curvatures are $4\sqrt3$ and $8-4\sqrt3$. The other zero-energy [stationary point](calculus-of-variations.md#stationary-point) with $\beta=2+\sqrt3$ and $z=-\sqrt3-1$ is a [saddle point](analysis.md#saddle-point). The stable vacuum has nonzero [supergravity auxiliary field](#supergravity-auxiliary-field), so it has [supersymmetry breaking](#supersymmetry-breaking) even with zero [cosmological constant](cosmology.md#cosmological-constant). The $m=0$ branch does not fix these values.

##### Polonyi supersymmetry branches

↑ **Parent:** [Polonyi model](#polonyi-model)

For the [Polonyi model](#polonyi-model) with canonical [Kähler potential](#kahler-potential) and $W=m^2(z+\beta)$, $\beta>0$, a constant [supersymmetric vacuum](#supersymmetric-vacuum) with $m\ne0$ requires real $z=(-\beta\pm\sqrt{\beta^2-4})/2$ and exists exactly for $\beta\geq2$. Its [supergravity F-term potential](#supergravity-f-term-potential) is negative because $W\ne0$. For $0<\beta<2$, the [supergravity auxiliary field](#supergravity-auxiliary-field) cannot vanish. If $m=0$, the model is flat with unbroken [supersymmetry](supersymmetry.md). This parameter-dependent statement is sharper than asserting that every linear [superpotential](#superpotential) breaks [supersymmetry](supersymmetry.md) in [supergravity](#supergravity).

## Spurion

↑ **Parent:** [Supersymmetry](supersymmetry.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spurion)

A spurion is a nondynamical background field assigned transformation properties so that couplings or symmetry-breaking parameters can be treated as if they arose from symmetry-covariant fields.

## ↑ Ancestors (3)

1. [Branches of physics](physics.md#branches-of-physics)
2. [Physics](physics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (129)

- [1.5-order formalism](general-relativity.md#1-5-order-formalism)
- [BPS state](#bps-state)
- [Chiral multiplet](#chiral-multiplet)
- [Chiral projection by squared supercovariant derivatives](#chiral-projection-by-squared-supercovariant-derivatives)
- [Chiral protection of a fermion mass](standard-model.md#chiral-protection-of-a-fermion-mass)
- [Chirality constraint on extended supersymmetry](#chirality-constraint-on-extended-supersymmetry)
- [Cosmological constant problem](cosmology.md#cosmological-constant-problem)
- [Dynamical supersymmetry breaking](#dynamical-supersymmetry-breaking)
- [Energy positivity in global supersymmetry](#energy-positivity-in-global-supersymmetry)
- [Extended supersymmetry](#extended-supersymmetry)
- [F-term hybrid inflation](cosmic-inflation.md#f-term-hybrid-inflation)
- [Finite zero-energy vacuum for a single exponential superpotential](#finite-zero-energy-vacuum-for-a-single-exponential-superpotential)
- [First massive level of a chiral RNS sector](string-theory.md#first-massive-level-of-a-chiral-rns-sector)
- [Flat F-term breaking with a linear superpotential](#flat-f-term-breaking-with-a-linear-superpotential)
- [Flux compactification](string-theory.md#flux-compactification)
- [Goldstino](#goldstino)
- [Goldstino null vector with F-term and D-term breaking](#goldstino-null-vector-with-f-term-and-d-term-breaking)
- [Gravitino](#gravitino)
- [Heterotic Calabi-Yau compactification](string-theory.md#heterotic-calabi-yau-compactification)
- [Heterotic string](string-theory.md#heterotic-string)
- [Hidden supersymmetry-breaking sector](#hidden-supersymmetry-breaking-sector)
- [Kähler transformation](#kahler-transformation)
- [Killing spinor](#killing-spinor)
- [Mass spectrum of single charged-field D-term breaking](#mass-spectrum-of-single-charged-field-d-term-breaking)
- [Massive chiral superstring supersymmetry multiplet](string-theory.md#massive-chiral-superstring-supersymmetry-multiplet)
- [Massive supermultiplet](#massive-supermultiplet)
- [Moduli stabilization](string-theory.md#moduli-stabilization)
- [MSSM tree-level sfermion mass constraint](#mssm-tree-level-sfermion-mass-constraint)
- [Neutral flat direction with oppositely charged chiral fields](#neutral-flat-direction-with-oppositely-charged-chiral-fields)
- [Nilpotent chiral superfield](#nilpotent-chiral-superfield)
- [No-scale supergravity](#no-scale-supergravity)
- [Noether gauging procedure](quantum-field-theory.md#noether-gauging-procedure)
- [Non-renormalization theorem](#non-renormalization-theorem)
- [Off-shell component count of minimal supergravity](#off-shell-component-count-of-minimal-supergravity)
- [Old-minimal supergravity](#old-minimal-supergravity)
- [Orientifold](string-theory.md#orientifold)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-65.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-67.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-68.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-50.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#10/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#8/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-53.md#9/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-50.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-54.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-55.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-55.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-54.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-54.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-54.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-54.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-55.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-55.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-57.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-57.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-57.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-52.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-53.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-42.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-42.md#4/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-60.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-60.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-56.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-56.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-56.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-45.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-45.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-45.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-45.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-45.md#2/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-43.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-43.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-43.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-43.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-48.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-307.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-307.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-307.md#1/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-307.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-307.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-307.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-307.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-307.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-307.md#3/solution)
- [Polonyi supersymmetry branches](#polonyi-supersymmetry-branches)
- [Pure-scalar truncation of a superfield](#pure-scalar-truncation-of-a-superfield)
- [Single charged-field D-term breaking](#single-charged-field-d-term-breaking)
- [Spacetime supercharge from an RNS spin field](string-theory.md#spacetime-supercharge-from-an-rns-spin-field)
- [Spin bound for massless supermultiplets](#spin-bound-for-massless-supermultiplets)
- [Super-Higgs mechanism](#super-higgs-mechanism)
- [Superconformal gauge](string-theory.md#superconformal-gauge)
- [Supercurrent](#supercurrent)
- [Supermembrane closed four-form](string-theory.md#supermembrane-closed-four-form)
- [Superstring theory](string-theory.md#superstring-theory)
- [Supersymmetric action](#supersymmetric-action)
- [Supersymmetric factorization and zero-mode normalizability](quantum-mechanics.md#supersymmetric-factorization-and-zero-mode-normalizability)
- [Supersymmetric Higgs mechanism](#supersymmetric-higgs-mechanism)
- [Supersymmetry transformation](#supersymmetry-transformation)
- [Symmetry protection of a small mass](standard-model.md#symmetry-protection-of-a-small-mass)
- [Tree-level supertrace mass sum rule](#tree-level-supertrace-mass-sum-rule)
- [Two-dimensional N=(1,1) superspace](#two-dimensional-n-1-1-superspace)
- [Wess-Zumino chiral multiplet coupled to supergravity](#wess-zumino-chiral-multiplet-coupled-to-supergravity)
- [Worldsheet supersymmetry](string-theory.md#worldsheet-supersymmetry)
