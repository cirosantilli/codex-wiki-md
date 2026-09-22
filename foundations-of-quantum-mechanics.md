# Foundations of quantum mechanics

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Foundations_of_quantum_mechanics)

The foundations of quantum mechanics study the physical and conceptual status of quantum states, measurement, nonlocal correlations, and possible extensions of quantum theory.

**Table of contents**

- [Complementarity (physics)](#complementarity-physics)
- [Many-worlds interpretation](#many-worlds-interpretation)
- [Consistent histories](#consistent-histories)
  - [Decoherence functional](#decoherence-functional)
- [Einstein–Podolsky–Rosen paradox](#einstein-podolsky-rosen-paradox)
  - [Quantum steering](#quantum-steering)
  - [Einstein–Podolsky–Rosen criterion of reality](#einstein-podolsky-rosen-criterion-of-reality)
- [Superselection rule](#superselection-rule)
- [EPR criterion of reality](#epr-criterion-of-reality)
- [de Broglie-Bohm theory](#de-broglie-bohm-theory)
  - [Bohmian circulation of an angular-momentum eigenstate](#bohmian-circulation-of-an-angular-momentum-eigenstate)
  - [Quantum potential](#quantum-potential)
  - [Guidance equation](#guidance-equation)
    - [Quantum equilibrium equivariance](#quantum-equilibrium-equivariance)
- [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)
  - [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)
    - [Tensor-power reduction of PBR overlap](#tensor-power-reduction-of-pbr-overlap)
    - [PBR exclusion measurement for zero and plus](#pbr-exclusion-measurement-for-zero-and-plus)
  - [Preparation independence](#preparation-independence)
  - [Psi-epistemic model](#psi-epistemic-model)
  - [Psi-ontic model](#psi-ontic-model)
- [Bell theorem](#bell-theorem)
  - [Quantum nonlocality](#quantum-nonlocality)
  - [Hardy's paradox](#hardy-s-paradox)
  - [Bell test](#bell-test)
    - [Delft electron-spin Bell test](#delft-electron-spin-bell-test)
    - [Freedman-Clauser experiment](#freedman-clauser-experiment)
    - [Aspect switching experiment](#aspect-switching-experiment)
    - [Photonic entanglement-swapping experiment](#photonic-entanglement-swapping-experiment)
    - [Photonic Bell test with efficient detection and random settings](#photonic-bell-test-with-efficient-detection-and-random-settings)
    - [Detection loophole](#detection-loophole)
      - [Fair sampling](#fair-sampling)
    - [Locality loophole](#locality-loophole)
  - [Bell inequality](#bell-inequality)
    - [Tsirelson's bound](#tsirelson-s-bound)
      - [CHSH Tsirelson bound](#chsh-tsirelson-bound)
  - [Chained modular Bell inequality](#chained-modular-bell-inequality)
    - [Coplanar qubit realization of the chained Bell inequality](#coplanar-qubit-realization-of-the-chained-bell-inequality)
  - [Local hidden-variable theory](#local-hidden-variable-theory)
    - [Setting-independent heralding preserves Bell locality](#setting-independent-heralding-preserves-bell-locality)
    - [Outcome independence](#outcome-independence)
    - [Bell local causality](#bell-local-causality)
    - [Deterministic local hidden-variable model](#deterministic-local-hidden-variable-model)
    - [Outcome determinism](#outcome-determinism)
    - [Parameter independence](#parameter-independence)
    - [Measurement independence](#measurement-independence)
  - [CHSH inequality](#chsh-inequality)
    - [Polarization CHSH count model](#polarization-chsh-count-model)
    - [CHSH optimum from the correlation tensor](#chsh-optimum-from-the-correlation-tensor)
    - [Gisin's theorem](#gisin-s-theorem)
      - [CHSH axes for an entangled pure two-qubit state](#chsh-axes-for-an-entangled-pure-two-qubit-state)
    - [No-signalling box](#no-signalling-box)
      - [Popescu–Rohrlich box](#popescu-rohrlich-box)
        - [One-bit computation using Popescu–Rohrlich boxes](#one-bit-computation-using-popescu-rohrlich-boxes)
- [Objective-collapse theory](#objective-collapse-theory)
  - [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)
    - [GRW localization operator](#grw-localization-operator)
      - [GRW collapse-centre event probabilities](#grw-collapse-centre-event-probabilities)
    - [GRW amplification mechanism](#grw-amplification-mechanism)
      - [GRW branch persistence versus geometric containment](#grw-branch-persistence-versus-geometric-containment)
    - [GRW spontaneous heating](#grw-spontaneous-heating)
  - [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)
    - [Quantum state readout device](#quantum-state-readout-device)
    - [Proper mixed state](#proper-mixed-state)
    - [Improper mixed state](#improper-mixed-state)

## Complementarity (physics)

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complementarity_(physics))

The need for mutually exclusive experimental arrangements or incompatible observables to exhibit different aspects of a quantum system. For example, path discrimination and interference contrast obey a tradeoff, while sharp [Pauli operator](quantum-circuit.md#pauli-operator) $X$ and $Z$ measurements have incompatible eigenbases. [Which-path information](physical-optics.md#which-path-information) is an operational record, rather than a requirement that a conscious observer reads it.

## Many-worlds interpretation

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Many-worlds_interpretation)

An interpretation retaining universal unitary evolution of the [quantum state](quantum-system.md#quantum-state), with definite measurement records described relative to outcome branches. [Quantum decoherence](quantum-theory.md#quantum-decoherence) explains the practical isolation and stable record basis of emergent branches. It does not insert a physical collapse selecting just one component. The emergence of branch structure and justification of [Born rule](wave-function.md#born-rule) weights involve additional interpretive arguments beyond writing the [Schrödinger equation](mathematical-physics.md#schrodinger-equation).

## Consistent histories

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Consistent_histories)

An approach assigning probabilities to compatible families of time-ordered quantum alternatives. A [decoherence functional](#decoherence-functional) measures [interference](physical-optics.md#interference-wave-propagation) between histories; when its relevant cross-terms vanish, coarse-grained probabilities add as in [probability theory](probability-theory.md). Different incompatible families must not be combined as if they were one classical history space. The formalism does not require a fundamental external measurement apparatus.

### Decoherence functional

↑ **Parent:** [Consistent histories](#consistent-histories)

For alternatives represented by [projection operators](vector-space.md#projection-linear-algebra) at successive times, set $C_\alpha=P_{\alpha_n}(t_n)\cdots P_{\alpha_1}(t_1)$ in the [Heisenberg picture](quantum-system.md#heisenberg-picture). The displayed functional uses the initial [density operator](density-matrix.md) $\rho$. Combining two histories gives $D(\alpha+\beta,\alpha+\beta)=D(\alpha,\alpha)+D(\beta,\beta)+2\operatorname{Re}D(\alpha,\beta)$. Thus vanishing real cross-terms gives the [probability](probability-theory.md#probability) sum rule; the stronger commonly used condition $D(\alpha,\beta)=0$ for distinct histories is sufficient as well. Its diagonal is nonnegative because each $C_\alpha\rho C_\alpha^\dagger$ is positive.

<h2 id="einstein-podolsky-rosen-paradox">Einstein–Podolsky–Rosen paradox</h2>

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Einstein–Podolsky–Rosen_paradox)

The EPR argument uses correlations of an entangled state and a locality assumption to challenge the completeness of the quantum description. Its [Einstein–Podolsky–Rosen criterion of reality](#einstein-podolsky-rosen-criterion-of-reality) identifies quantities predictable with certainty without disturbing a distant system as elements of physical reality.

### Quantum steering

↑ **Parent:** [Einstein–Podolsky–Rosen paradox](#einstein-podolsky-rosen-paradox)

For a shared [quantum entanglement](bell-state.md#entangled-state) resource, one party's choice of measurement can prepare different conditional ensembles for the distant party. Discarding the outcome leaves the same distant [reduced density matrix](bell-state.md#reduced-density-matrix), so steering does not itself permit signalling. Demonstrating steering against a local hidden-state model is stronger than merely observing a change in a postselected description.

<h3 id="einstein-podolsky-rosen-criterion-of-reality">Einstein–Podolsky–Rosen criterion of reality</h3>

↑ **Parent:** [Einstein–Podolsky–Rosen paradox](#einstein-podolsky-rosen-paradox)

The Einstein–Podolsky–Rosen criterion says that if one can predict a physical quantity with certainty without disturbing the system, then there is an element of physical reality corresponding to that quantity.

## Superselection rule

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)

A [superselection rule](#superselection-rule) partitions a representation into sectors between which the specified observable algebra has no matrix elements. Relative phases between vectors in different sectors cannot be detected by those observables, so a coherent vector spanning sectors and its sector-diagonal mixture define the same observable state. The restriction is relative to the observable algebra; it is not by itself a physical wave-function collapse. Infinite-system phases can yield disjoint representations and emergent superselection sectors even though each finite system permits global connecting operators.

## EPR criterion of reality

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)

The certainty of a prediction made without disturbing the system is proposed as sufficient evidence that the predicted quantity corresponds to an element of physical reality. It motivates the discussion of completeness and locality in [foundations of quantum mechanics](foundations-of-quantum-mechanics.md), but is distinct from the conditional factorization assumed by [local hidden-variable theory](#local-hidden-variable-theory).

## de Broglie-Bohm theory

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Broglie–Bohm_theory)

A deterministic interpretation with a definite particle configuration guided by the [wavefunction](wave-function.md). The latter obeys the [Time-dependent Schrödinger equation](mathematical-physics.md#time-dependent-schrodinger-equation), while the particle follows the [guidance equation](#guidance-equation). A [Born rule](wave-function.md#born-rule) distribution of initial positions is preserved by [quantum equilibrium equivariance](#quantum-equilibrium-equivariance). The guidance law restricts admissible initial velocities, even when trajectories are rewritten as a second-order force equation.

### Bohmian circulation of an angular-momentum eigenstate

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)

For the [separation of a two-dimensional central-potential eigenstate](quantum-mechanics.md#separation-of-a-two-dimensional-central-potential-eigenstate), the [guidance equation](#guidance-equation) gives zero radial velocity and constant-radius circular motion, with circulation $2\pi\hbar k/m$. A real superposition of the degenerate $k$ and $-k$ [eigenstates](energy-eigenvalue.md#eigenstate) has zero current away from nodes instead. The speed depends on the actual [wavefunction](wave-function.md), not just its energy.

### Quantum potential

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_potential)

The amplitude-dependent extra potential in the [Madelung equations](mathematical-physics.md#madelung-equations). Taking the [gradient](multivariable-calculus.md#gradient) of their phase equation and using the [guidance equation](#guidance-equation) yields $mD\mathbf v/Dt=-\nabla(V+Q)$, where $D/Dt$ is the [material derivative](continuum-mechanics.md#material-derivative). At [wavefunction](wave-function.md) nodes this local expression may be singular.

### Guidance equation

↑ **Parent:** [de Broglie-Bohm theory](#de-broglie-bohm-theory)

For a spinless particle without a magnetic vector potential, [Bohmian mechanics](#de-broglie-bohm-theory) sets $\dot{\mathbf X}=\hbar\nabla S/m$, where $S$ is the dimensionless [quantum phase](quantum-system.md#quantum-phase). Equivalently the velocity is the [probability current](wave-function.md#probability-current) divided by the [probability density](wave-function.md#probability-density). This formula is local to nonzero [wavefunction](wave-function.md) regions.

#### Quantum equilibrium equivariance

↑ **Parent:** [Guidance equation](#guidance-equation)

Both the ensemble position density transported by the [guidance equation](#guidance-equation) and the squared wave amplitude satisfy the same [probability continuity equation](wave-function.md#probability-continuity-equation). Subject to existence and uniqueness of that transport, an initial [Born rule](wave-function.md#born-rule) distribution stays a [Born rule](wave-function.md#born-rule) distribution. This is a preservation statement, not a derivation that every initial ensemble is already in equilibrium.

## Ontological model of a quantum system

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)

An ontological model associates each [quantum state preparation](quantum-circuit.md#quantum-state-preparation) with a [probability distribution](probability-distribution.md) over underlying physical states $\lambda$. A [measurement in quantum mechanics](quantum-measurement.md)'s response probabilities depend on its specification and $\lambda$, sum to one, and reproduce the [Born rule](wave-function.md#born-rule) when averaged over the preparation distribution. The model need not assign deterministic outcomes. Overlap or disjointness of preparation measures defines the [psi-epistemic model](#psi-epistemic-model) versus [psi-ontic model](#psi-ontic-model) distinction.

### Pusey-Barrett-Rudolph theorem

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

Under [preparation independence](#preparation-independence), an [ontological model of a quantum system](#ontological-model-of-a-quantum-system) reproducing exact quantum [measurement in quantum mechanics](quantum-measurement.md) probabilities cannot assign overlapping preparation measures to distinct [pure states](quantum-theory.md#pure-state). An exclusion [measurement in quantum mechanics](quantum-measurement.md) on independent copies makes every outcome impossible for one possible preparation; a common ontic region would require every response to vanish there. Thus the conclusion is a [psi-ontic model](#psi-ontic-model), not a blanket exclusion of hidden variables or all informational interpretations.

#### Tensor-power reduction of PBR overlap

↑ **Parent:** [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)

If two pure [quantum states](quantum-system.md#quantum-state) overlap by $(1/\sqrt2)^{1/n}$, their $n$-copy states have overlap $1/\sqrt2$. Each block spans an effective [qubit](quantum-system.md#qubit), with [orthonormal basis](inner-product.md#orthonormal-basis) $e_0=\Psi_1$ and $e_1=\sqrt2\Psi_2-\Psi_1$. Applying the two-block [PBR exclusion measurement for zero and plus](#pbr-exclusion-measurement-for-zero-and-plus) uses $2n$ independently prepared copies. A common single-copy ontic overlap of positive mass remains positive under this finite tensor power.

#### PBR exclusion measurement for zero and plus

↑ **Parent:** [Pusey-Barrett-Rudolph theorem](#pusey-barrett-rudolph-theorem)

The product preparations $00,0+,+0,++$ are excluded respectively by the orthonormal vectors $(01+10)/\sqrt2$, $(00-01+10+11)/2$, $(00+01-10+11)/2$ and $(00-11)/\sqrt2$, written in the computational basis. Each vector has zero inner product with its labelled preparation. This [projective measurement](quantum-measurement.md#projective-measurement) gives [antidistinguishable quantum states](quantum-measurement.md#antidistinguishable-quantum-states) and drives the two-copy [PBR theorem](#pusey-barrett-rudolph-theorem) contradiction.

### Preparation independence

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

Independently operated [quantum state preparations](quantum-circuit.md#quantum-state-preparation) are assumed to produce independent underlying physical states. Their joint preparation measure factors into the single-system measures. This ontic factorization is an additional assumption, not a consequence of operational independence alone. It turns a common single-system overlap of mass $\varepsilon$ into a common $n$-system overlap of mass $\varepsilon^n$ in the [PBR theorem](#pusey-barrett-rudolph-theorem).

### Psi-epistemic model

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

An [ontological model of a quantum system](#ontological-model-of-a-quantum-system) is psi-epistemic if some pair of distinct [pure states](quantum-theory.md#pure-state) has preparation measures with nonzero overlap. The same physical state can then be compatible with either preparation. This precise measure-overlap definition is stronger than merely interpreting a [wave function](wave-function.md) as information or a computational tool.

### Psi-ontic model

↑ **Parent:** [Ontological model of a quantum system](#ontological-model-of-a-quantum-system)

An [ontological model of a quantum system](#ontological-model-of-a-quantum-system) is psi-ontic if distinct [pure states](quantum-theory.md#pure-state) have mutually singular preparation distributions. The physical state then determines which pure [quantum state](quantum-system.md#quantum-state) was prepared, almost surely in the pairwise sense. Extra underlying variables may still exist. The [PBR theorem](#pusey-barrett-rudolph-theorem) establishes this conclusion under [preparation independence](#preparation-independence) and exact quantum predictions.

## Bell theorem

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_theorem)

Bell's theorem shows that no theory assigning outcomes through local hidden variables can reproduce every quantum correlation.

The force of the [Bell theorem](#bell-theorem) is that a disagreement about a [local hidden-variable theory](#local-hidden-variable-theory) becomes a constraint on frequencies in a [Bell test](#bell-test). [Quantum entanglement](bell-state.md#entangled-state) alone does not guarantee a violation for every [measurement in quantum mechanics](quantum-measurement.md): the [quantum state](quantum-system.md#quantum-state), analyzer settings and treatment of missed events all matter. A violation of the [CHSH inequality](#chsh-inequality) tests the conjunction of [Bell local causality](#bell-local-causality), [measurement independence](#measurement-independence) and the stated outcome and sampling assumptions; it remains compatible with [quantum no-signalling](quantum-theory.md#quantum-no-signalling).

### Quantum nonlocality

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_nonlocality)

Quantum correlations incompatible with [Bell local causality](#bell-local-causality) under additional assumptions including [measurement independence](#measurement-independence). This is an operational statement about joint probabilities, not controllable faster-than-light signaling: quantum predictions also obey [quantum no-signalling](quantum-theory.md#quantum-no-signalling). Entanglement alone does not guarantee violation of a specified Bell inequality in a given measurement arrangement.

<h3 id="hardy-s-paradox">Hardy's paradox</h3>

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hardy's_paradox)

A two-setting nonlocality argument in which several zero-probability events forbid a further coincidence in any [deterministic local hidden-variable model](#deterministic-local-hidden-variable-model), but quantum theory assigns that coincidence positive [probability](probability-theory.md#probability). For binary indicators, suppose $C_+^RC_-^R=0$, $D_+^I=1\Rightarrow C_-^R=1$ and $D_-^I=1\Rightarrow C_+^R=1$. Any assignment with $D_+^ID_-^I=1$ would violate the first relation. A quantum implementation can nevertheless give such a coincidence. Real imperfect experiments require an inequality that accounts for their nonzero error probabilities. [Lucien Hardy](physicist.md#lucien-hardy) gave a two-particle inequality-free argument in 1992.[1992 abstract](physics-bibliography.md#quantum-mechanics-local-realistic-theories-and-lorentz-invariant-realistic-theories-by-lucien-hardy)

### Bell test

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_test)

A [Bell test](#bell-test) compares experimental [probabilities](probability-theory.md#probability) or [expectation values](quantum-system.md#expectation-value) with a [Bell inequality](#bell-inequality). In a two-setting [photon polarization](quantum-mechanics.md#photon-polarization) test, each station chooses a [polarizer](electromagnetic-wave.md#polarizer) orientation and records an outcome. A [coincidence circuit](particle-detection.md#coincidence-circuit) identifies candidate pairs using an agreed timing rule. The choice of which trials enter the statistic is part of the experiment: correlations calculated only from detected pairs can differ from correlations of all emitted pairs. The [Polarization CHSH count model](#polarization-chsh-count-model) separates ideal [expectation values](quantum-system.md#expectation-value) from this experimental selection problem.

<a id="image-two-setting-polarization-measurements-and-coincidence-readout"></a>
![](bell-test-analyzers-and-settings.png)

**[Figure 1](#image-two-setting-polarization-measurements-and-coincidence-readout). Two-setting polarization measurements and coincidence readout**. Conceptual apparatus for the ideal two-output model. The displayed angles belong to the worked CHSH example; they are not a reconstruction of a historical apparatus. Each station chooses one basis, then records either output. The coincidence record also needs a rule for missed detections.

#### Delft electron-spin Bell test

↑ **Parent:** [Bell test](#bell-test)

The [Bell test](#bell-test) reported by [Bas Hensen](physicist.md#bas-hensen) and collaborators used electron spins separated by $1.3\,\mathrm{km}$, efficient spin readout and rapid random measurement settings. Those features addressed detection and locality loopholes together. Its result tests [Bell local causality](#bell-local-causality) with the stated experimental assumptions, rather than ruling out every possible hidden-variable theory.[2015 abstract: spin separation, efficient readout and basis-choice timing](physics-bibliography.md#experimental-loophole-free-violation-of-a-bell-inequality-by-bas-hensen-and-others)

#### Freedman-Clauser experiment

↑ **Parent:** [Bell test](#bell-test)

In 1972, [Stuart J. Freedman](physicist.md#stuart-jay-freedman) and [John F. Clauser](physicist.md#john-francis-clauser) excited a [calcium](chemical-substance.md#calcium) beam from an oven with a filtered [deuterium](chemical-substance.md#deuterium) arc lamp. A [calcium](chemical-substance.md#calcium) emission cascade supplied paired [photons](quantum-mechanics.md#photon); an [optical lens](geometrical-optics.md#lens-optics) system, [optical filters](optical-instrument.md#optical-filter), removable glass-plate [polarizers](electromagnetic-wave.md#polarizer) and cooled [photomultipliers](particle-detection.md#photomultiplier) selected their [linear polarizations](electromagnetic-wave.md#linear-polarization). They compared [coincidence circuit](particle-detection.md#coincidence-circuit) rates at relative angles $22.5^\circ$ and $67.5^\circ$, normalized with [polarizers](electromagnetic-wave.md#polarizer) removed. Alternating configurations controlled drift; delayed counts estimated [accidental coincidences](particle-detection.md#accidental-coincidence). The violation agreed with [quantum mechanics](quantum-mechanics.md), conditional on their explicit assumption that passage through a [polarizer](electromagnetic-wave.md#polarizer) did not change a photon's detection [probability](probability-theory.md#probability). This was a static-analyzer test with a [detection loophole](#detection-loophole), rather than the ideal four-output [CHSH inequality](#chsh-inequality) statistic.[Printed pp. 2-7, assumption (3), Eq. (3), Figs. 1-3](physics-bibliography.md#experimental-test-of-local-hidden-variable-theories-by-stuart-jay-freedman-and-john-francis-clauser)

#### Aspect switching experiment

↑ **Parent:** [Bell test](#bell-test)

In 1982, [Alain Aspect](physicist.md#alain-aspect), [Jean Dalibard](physicist.md#jean-dalibard) and [Gérard Roger](engineering.md#gerard-roger) used a [calcium](chemical-substance.md#calcium) cascade and an acoustic [standing wave](mathematical-physics.md#standing-wave) in [water](chemical-substance.md#water) to route each [photon](quantum-mechanics.md#photon) toward one of two fixed [polarizers](electromagnetic-wave.md#polarizer). Switching took about $10\,\mathrm{ns}$, against $40\,\mathrm{ns}$ for light to cross between stations. [Photomultiplier](particle-detection.md#photomultiplier) [coincidence circuit](particle-detection.md#coincidence-circuit) rates, with delayed-background subtraction and [polarizer](electromagnetic-wave.md#polarizer)-removal normalization, violated their [Bell inequality](#bell-inequality). Supplementary [polarizers](electromagnetic-wave.md#polarizer) checked each channel against [Malus's law](wave.md#malus-s-law). The timing attacked the [locality loophole](#locality-loophole), but the authors emphasized that switching was quasiperiodic, not random; incomplete switching and inefficient collection also limited the test. Its normalized statistic differs from the [CHSH inequality](#chsh-inequality) convention used below.[pp. 1805-1807, Figs. 2-4; final discussion](physics-bibliography.md#experimental-test-of-bell-s-inequalities-using-time-varying-analyzers-by-alain-aspect-and-others)

#### Photonic entanglement-swapping experiment

↑ **Parent:** [Bell test](#bell-test)

In 1998, [Jian-Wei Pan](physicist.md#jian-wei-pan), [Dik Bouwmeester](physicist.md#dirk-bouwmeester), [Harald Weinfurter](physicist.md#harald-weinfurter) and [Anton Zeilinger](physicist.md#anton-zeilinger) created two [photon](quantum-mechanics.md#photon) pairs by two passages of a pulsed pump through a [crystal](thermodynamics.md#crystal) using [spontaneous parametric down-conversion](optics.md#spontaneous-parametric-down-conversion). Interfering the inner [photons](quantum-mechanics.md#photon) at a [nonpolarizing beam splitter](optical-instrument.md#nonpolarizing-beam-splitter) implemented a partial [Bell-basis measurement](bell-state.md#bell-basis-measurement). Narrow [optical filters](optical-instrument.md#optical-filter) and spatial filtering removed distinguishing information; changing the outer [polarizer](electromagnetic-wave.md#polarizer) bases checked the conditional correlations. Fourfold detections selected the [entanglement swapping](bell-state.md#entanglement-swapping) events. The reported interference supported conditional [quantum entanglement](bell-state.md#entangled-state), but the paper reserved a statistically significant [Bell inequality](#bell-inequality) violation for improved visibility; it was not a demonstration closing the [detection loophole](#detection-loophole).[pp. 3892-3894, Eq. (3), Figs. 2-3; visibility discussion](physics-bibliography.md#experimental-entanglement-swapping-entangling-photons-that-never-interacted-by-jian-wei-pan-and-others)

The ideal calculation makes the distinction between conditional and unconditional [quantum states](quantum-system.md#quantum-state) explicit. Start with [spin singlet states](bell-state.md#spin-singlet-state) $|\psi^-\rangle_{12}|\psi^-\rangle_{34}$, where $|\psi^-\rangle=(|HV\rangle-|VH\rangle)/\sqrt2$ and $H,V$ denote orthogonal [photon polarizations](quantum-mechanics.md#photon-polarization). Taking the [inner product](inner-product.md) with $\langle\psi^-|_{23}$ gives $-|\psi^-\rangle_{14}/2$: expanding the four terms leaves precisely the two antisymmetric outer terms. That [Bell-basis measurement](bell-state.md#bell-basis-measurement) outcome has [probability](probability-theory.md#probability) $1/4$ and leaves the outer pair in a [spin singlet state](bell-state.md#spin-singlet-state). Ignoring the inner outcome instead leaves the outer [density matrix](density-matrix.md) $I_4/4$, a [maximally mixed state](density-matrix.md#maximally-mixed-state). A conditional preparation flag is useful for later [Bell tests](#bell-test) only with the timing and setting conditions in [setting-independent heralding preserves Bell locality](#setting-independent-heralding-preserves-bell-locality).

#### Photonic Bell test with efficient detection and random settings

↑ **Parent:** [Bell test](#bell-test)

In 2015, [Marissa Giustina](electrical-engineering.md#marissa-giustina), [Anton Zeilinger](physicist.md#anton-zeilinger) and collaborators combined [spontaneous parametric down-conversion](optics.md#spontaneous-parametric-down-conversion) with rapid random analyzer choices and efficient [transition-edge sensors](particle-detection.md#transition-edge-sensor). Local records included settings and detector signals; their [Bell inequality](#bell-inequality) used detected and undetected trials, avoiding [fair sampling](#fair-sampling). Locally fixed time slots prevented coincidence-based trial selection. Calibrated optical and electrical delays checked [spacelike separation](special-relativity.md#spacelike-separation) of each choice from the remote readout. The violation addressed detection and locality together. [Measurement independence](#measurement-independence) still requires assumptions about the hidden state's origin; the experiment cannot exclude every possible common cause of source and settings.[Version 2, pp. 1-4, Figs. 1-2 and Eq. (1)](physics-bibliography.md#significant-loophole-free-test-of-bell-s-theorem-with-entangled-photons-by-marissa-giustina-and-others)

#### Detection loophole

↑ **Parent:** [Bell test](#bell-test)

The [detection loophole](#detection-loophole) arises when missed events allow the retained sample to depend on settings and hidden variables. For example, a [local hidden-variable theory](#local-hidden-variable-theory) may retain different underlying pairs at different [polarizer](electromagnetic-wave.md#polarizer) angles. Applying the [CHSH inequality](#chsh-inequality) to that selected sample does not test the original setting-independent ensemble. A valid protocol specifies outcomes and trials, including failures, or justifies an appropriate [fair sampling](#fair-sampling) assumption. Subtracting [accidental coincidences](particle-detection.md#accidental-coincidence) addresses background contamination; it does not by itself repair this selection problem.

##### Fair sampling

↑ **Parent:** [Detection loophole](#detection-loophole)

For a specified [Bell test](#bell-test) statistic, [fair sampling](#fair-sampling) assumes that conditioning on successful detections preserves the correlations needed to represent the intended ensemble. Constant detector efficiency in an independently specified loss model can ensure this; constant observed count rates alone do not establish independence from the hidden state. The [Polarization CHSH count model](#polarization-chsh-count-model) explicitly assumes independent losses.

#### Locality loophole

↑ **Parent:** [Bell test](#bell-test)

The [locality loophole](#locality-loophole) permits a station's outcome to be influenced by the distant setting through an ordinary signal arriving before readout. [Spacelike separation](special-relativity.md#spacelike-separation) excludes such communication at or below the [speed of light](special-relativity.md#speed-of-light). Fast changes only help if the relevant choice and detection events have the required timing. Predictable switching also leaves open correlations with earlier settings; closing a communication channel does not prove [measurement independence](#measurement-independence).

### Bell inequality

↑ **Parent:** [Bell theorem](#bell-theorem)

A [Bell inequality](#bell-inequality) is a constraint on observable correlations satisfied by the specified class of local hidden-variable models. In finite-setting scenarios such constraints bound linear combinations of probabilities or expectation values. The [CHSH inequality](#chsh-inequality) is one example, following from Bell factorization, measurement independence and bounded outcomes. A violation rules out the conjunction of the assumptions defining that model class; it does not alone identify a unique false premise.

<h4 id="tsirelson-s-bound">Tsirelson's bound</h4>

↑ **Parent:** [Bell inequality](#bell-inequality)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tsirelson's_bound)

A bound on the correlations attainable by [measurement in quantum measurements](quantum-measurement.md) for a specified Bell expression. The [CHSH Tsirelson bound](#chsh-tsirelson-bound) is $2\sqrt2$; the number depends on which Bell expression is being optimized.

##### CHSH Tsirelson bound

↑ **Parent:** [Tsirelson's bound](#tsirelson-s-bound)

For dichotomic [observables](quantum-system.md#observable) with $A_i^2=B_j^2=I$, let $\mathcal B=A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)$. Expanding gives $\mathcal B^2=4I-[A_0,A_1]\otimes[B_0,B_1]$. Each commutator has [operator norm](continuous-dual-space.md#operator-norm) at most two, so $\|\mathcal B\|^2\le8$ and $|\langle\mathcal B\rangle|\le2\sqrt2$. Appropriate spin measurements of a [Bell state](bell-state.md) attain equality. The local hidden-variable bound of the corresponding [CHSH inequality](#chsh-inequality) is two.

### Chained modular Bell inequality

↑ **Parent:** [Bell theorem](#bell-theorem)

For outcomes in $\{0,\ldots,d-1\}$, let $[x]_d$ be their nonnegative modular representative. A [deterministic local hidden-variable model](#deterministic-local-hidden-variable-model) satisfies

$$
I_{N,d}=\sum_{j=1}^N\mathbb E\big([A_j-B_j]_d\big)+\sum_{j=1}^{N-1}\mathbb E\big([B_j-A_{j+1}]_d\big)+\mathbb E\big([B_N-A_1-1]_d\big)\geq d-1.
$$

The unreduced chain telescopes to $-1$, so its reduced nonnegative sum is at least $d-1$ for each assignment. For binary outcomes and two settings, it is a form of the [CHSH inequality](#chsh-inequality): $I_{2,2}=2-(E_{11}+E_{21}+E_{22}-E_{12})/2$.

#### Coplanar qubit realization of the chained Bell inequality

↑ **Parent:** [Chained modular Bell inequality](#chained-modular-bell-inequality)

On $|\Phi^+\rangle$, measure $\sigma_z\cos\theta+\sigma_x\sin\theta$, assigning [bit](information-theory.md#bit) $a$ to eigenvalue $(-1)^a$. Choose Alice's angles $2(i-1)\delta$ and Bob's angles $(2i-1)\delta$, with $\delta=\pi/(2N)$. The [Bell state](bell-state.md) correlation is $\cos(\theta-\phi)$. Each adjacent disagreement term and the last agreement term therefore has [probability](probability-theory.md#probability) $\sin^2(\pi/(4N))$. For $N\geq2$, their total violates the [chained modular Bell inequality](#chained-modular-bell-inequality) bound one, and it tends to zero as $N\to\infty$. At $N=1$ the value is exactly one.

// Target: probability-and-statistics.bigb

### Local hidden-variable theory

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_hidden-variable_theory)

A local hidden-variable theory assigns each party's outcome from a shared hidden state and that party's own setting, independently of the spacelike-separated setting chosen by the other party.

#### Setting-independent heralding preserves Bell locality

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

If a successful preparation flag is fixed before freely selected [Bell inequality](#bell-inequality) settings, conditioning a [local hidden-variable theory](#local-hidden-variable-theory) on that flag only replaces its hidden-variable distribution by the conditional distribution. The later response functions remain local and the distribution is independent of the later settings, so the [CHSH inequality](#chsh-inequality) still holds. Setting-dependent rejection during the Bell measurements does not satisfy this argument.

#### Outcome independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

[Outcome independence](#outcome-independence) requires $P(A,B\mid a,b,\lambda)=P(A\mid a,b,\lambda)P(B\mid a,b,\lambda)$. It says that, once settings and the proposed complete state are fixed, learning the distant outcome does not change the local outcome probability. Combining it with [parameter independence](#parameter-independence) gives Bell factorization. Entangled quantum states generally fail outcome independence even though their observable marginal distributions obey [quantum no-signalling](quantum-theory.md#quantum-no-signalling).

#### Bell local causality

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

For spacelike-separated measurement regions, a sufficient specification $\lambda$ of their relevant past should screen each outcome from additional information in the other wing. In a two-setting experiment a Bell-local model has $P(A,B\mid a,b,\lambda)=P(A\mid a,\lambda)P(B\mid b,\lambda)$. Together with [measurement independence](#measurement-independence) and bounded outcomes, this implies the [CHSH inequality](#chsh-inequality). [Bell local causality](#bell-local-causality) is stronger than [quantum no-signalling](quantum-theory.md#quantum-no-signalling) and is not an assumption that every outcome was predetermined.

#### Deterministic local hidden-variable model

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

A setting-independent hidden variable fixes responses for every measurement choice, and each response depends only on the local setting. Stochastic [local hidden-variable theories](#local-hidden-variable-theory) can be represented as mixtures of these assignments by including local random seeds in the hidden variable. Deterministic counterfactual assignments are the starting point of the [chained modular Bell inequality](#chained-modular-bell-inequality).

#### Outcome determinism

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

Outcome determinism says that a complete hidden state and the measurement settings fix each measurement outcome with probability one.

#### Parameter independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)

Parameter independence says that, conditional on the complete hidden state, the probability distribution of one party's outcome is independent of the other party's measurement setting.

#### Measurement independence

↑ **Parent:** [Local hidden-variable theory](#local-hidden-variable-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurement_independence)

Measurement independence says that the distribution of the hidden state is independent of the measurement settings: $\rho(\lambda|a,b)=\rho(\lambda)$. Its failure is the measurement-dependence loophole in a [Bell test](#bell-theorem).

### CHSH inequality

↑ **Parent:** [Bell theorem](#bell-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CHSH_inequality)

For local outcomes $A_0,A_1,B_0,B_1\in\{-1,1\}$, the Clauser–Horne–Shimony–Holt inequality is

$$
|E(A_0B_0)+E(A_0B_1)+E(A_1B_0)-E(A_1B_1)|\leq2.
$$

An arbitrary no-signalling correlation can reach the algebraic maximum $4$, while quantum correlations are bounded by $2\sqrt2$.

For a short proof of the local bound, fix a [deterministic local hidden-variable model](#deterministic-local-hidden-variable-model) assignment. The combination is $A_0(B_0+B_1)+A_1(B_0-B_1)$. Exactly one bracket vanishes and the other is $\pm2$, so every assignment contributes $\pm2$. Averaging with a single setting-independent [probability distribution](probability-distribution.md) preserves the interval $[-2,2]$. Mixtures also cover stochastic [local hidden-variable theories](#local-hidden-variable-theory). Rejecting a different sample at each setting would invalidate precisely that common-average step.

The quantum bound follows just as economically. For [Hermitian operators](hilbert-space.md#hermitian-operator) with $A_i^2=B_j^2=I$, the [CHSH inequality](#chsh-inequality) operator $C=A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)$ obeys $C^2=4I-[A_0,A_1]\otimes[B_0,B_1]$. Each [commutator](lie-algebra.md#commutator) has [operator norm](continuous-dual-space.md#operator-norm) at most two, giving $\|C\|\leq2\sqrt2$. The [Polarization CHSH count model](#polarization-chsh-count-model) attains this bound without allowing either station to control the distant marginal [probability distribution](probability-distribution.md).

#### Polarization CHSH count model

↑ **Parent:** [CHSH inequality](#chsh-inequality)

Let $H,V$ be orthogonal [linear polarizations](electromagnetic-wave.md#linear-polarization), and prepare the [Bell state](bell-state.md) $|\Phi^+\rangle=(|HH\rangle+|VV\rangle)/\sqrt2$. The $+1$ analyzer vector is $|a\rangle=\cos a|H\rangle+\sin a|V\rangle$; its orthogonal companion has outcome $-1$. Direct [inner products](inner-product.md) with the [Bell state](bell-state.md) give $P_{++}=P_{--}=\cos^2(a-b)/2$ and $P_{+-}=P_{-+}=\sin^2(a-b)/2$. Thus the [expectation value](quantum-system.md#expectation-value) of the outcome product is $E(a,b)=\cos2(a-b)$. These are physical [polarizer](electromagnetic-wave.md#polarizer) angles; their corresponding [Bloch sphere](density-matrix.md#bloch-sphere) angles are doubled.

For a stipulated isotropic admixture, use the [density matrix](density-matrix.md)

$$
\rho_v=v|\Phi^+\rangle\langle\Phi^+|+(1-v)I_4/4,\qquad 0\leq v\leq1.
$$

The [maximally mixed state](density-matrix.md#maximally-mixed-state) contributes zero correlation, so $P_{st}(a,b)=[1+st\,v\cos2(a-b)]/4$ for $s,t\in\{-1,1\}$. Each local marginal is $1/2$, independently of the other setting, illustrating [quantum no-signalling](quantum-theory.md#quantum-no-signalling). In this model $v$ is the [interferometric visibility](physical-optics.md#interferometric-visibility) of the coincidence fringe; other noise models need not have one common visibility for every basis.

Choose $a_0=0^\circ$, $a_1=45^\circ$, $b_0=22.5^\circ$ and $b_1=-22.5^\circ$. The four correlations in the displayed [CHSH inequality](#chsh-inequality) are $v/\sqrt2,v/\sqrt2,v/\sqrt2,-v/\sqrt2$. Consequently $S=2\sqrt2v$, exceeding the local bound exactly when $v>1/\sqrt2$. Perfect correlation at a single common setting would not yield this comparison between incompatible [measurement in quantum measurements](quantum-measurement.md).

To connect [probabilities](probability-theory.md#probability) with expected counts, stipulate $M$ emitted pairs per setting pair and independent detection efficiencies $\eta_A,\eta_B$, independent also of settings, outcomes and hidden variables. The expected joint counts are $n_{st}=M\eta_A\eta_BP_{st}$. Their normalized correlation is

$$
E_{\rm det}=\frac{n_{++}+n_{--}-n_{+-}-n_{-+}}{n_{++}+n_{--}+n_{+-}+n_{-+}}=v\cos2(a-b).
$$

For original teaching inputs $M=1000$, $\eta_A=0.8$, $\eta_B=0.75$ and $v=0.8$, the $(a_0,b_0)$ expected counts are $n_{++}=n_{--}\simeq234.85$ and $n_{+-}=n_{-+}\simeq65.15$. They total $600$ and give $E_{\rm det}\simeq0.56569$, hence $S\simeq2.26274$. Fractional expected counts are not measured data. Efficiency cancels here because the loss model was specified to be independent; this algebra supplies no justification for discarding failures in an arbitrary [Bell test](#bell-test) with a [detection loophole](#detection-loophole).

<a id="image-ideal-chsh-visibility-threshold-and-expected-detection-counts"></a>
![](polarization-chsh-visibility-counts.png)

**[Figure 2](#image-ideal-chsh-visibility-threshold-and-expected-detection-counts). Ideal CHSH visibility threshold and expected detection counts**. Original model predictions, not experimental data. The first panel shows the visibility needed to exceed the local bound. The second uses 1000 emitted pairs, efficiencies 0.8 and 0.75, and visibility 0.8; each bar is an expected joint count.

#### CHSH optimum from the correlation tensor

↑ **Parent:** [CHSH inequality](#chsh-inequality)

For spin-projective measurements on a two-qubit state, let $\lambda_1\geq\lambda_2\geq\lambda_3$ be the [eigenvalues](linear-operator-theory.md#eigenvalue) of $T^TT$, where $T$ is its [Pauli correlation tensor](density-matrix.md#pauli-correlation-tensor). Bob's sum and difference of unit axes are orthogonal and have lengths $2\cos\phi$ and $2\sin\phi$. Maximizing Alice's two axes aligns them with the corresponding images under $T$. Maximizing $\phi$ then gives $2\sqrt{\|T\mathbf u\|^2+\|T\mathbf v\|^2}$ for orthonormal $\mathbf u,\mathbf v$. The maximum of this quadratic-form sum is $\lambda_1+\lambda_2$, by diagonalizing $T^TT$ and selecting its top two [eigenvectors](linear-operator-theory.md#eigenvector). Thus the displayed expression is both an upper bound and attainable. The same maximum applies to the form with the sum of two absolute values, since local outcome signs can select their positive branches.

<h4 id="gisin-s-theorem">Gisin's theorem</h4>

↑ **Parent:** [CHSH inequality](#chsh-inequality)

Every entangled pure state of two qubits violates a [CHSH inequality](#chsh-inequality) for a suitable choice of local measurement axes. If its two [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are $c_0,c_1>0$, the optimal construction already gives a value $2\sqrt{1+(2c_0c_1)^2}>2$.

##### CHSH axes for an entangled pure two-qubit state

↑ **Parent:** [Gisin's theorem](#gisin-s-theorem)

For the [Schmidt-basis Pauli correlation tensor](von-neumann-entropy.md#schmidt-basis-pauli-correlation-tensor), choose Alice's axes $\mathbf e_z,\mathbf e_x$ and Bob's $(\mathbf e_z\pm s\mathbf e_x)/\sqrt{1+s^2}$. The [CHSH inequality](#chsh-inequality) expression is $2\sqrt{1+s^2}$. It exceeds two exactly when both [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are nonzero, reaching $2\sqrt2$ for maximal [quantum entanglement](bell-state.md#entangled-state). A [product state](bell-state.md#product-state) gives $s=0$ and saturates rather than violates the inequality.

#### No-signalling box

↑ **Parent:** [CHSH inequality](#chsh-inequality)

A no-signalling box is a conditional probability distribution $P(x,y|a,b)$ whose marginal distribution for either party is independent of the other party's input. It can therefore exhibit correlations stronger than quantum correlations without transmitting information superluminally.

<h5 id="popescu-rohrlich-box">Popescu–Rohrlich box</h5>

↑ **Parent:** [No-signalling box](#no-signalling-box)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Popescu–Rohrlich_box)

A Popescu–Rohrlich box is a bipartite no-signalling box attaining the algebraic maximum of the [CHSH inequality](#chsh-inequality).

<h6 id="one-bit-computation-using-popescu-rohrlich-boxes">One-bit computation using Popescu–Rohrlich boxes</h6>

↑ **Parent:** [Popescu–Rohrlich box](#popescu-rohrlich-box)

Take a [separated Boolean decomposition](analysis-of-boolean-functions.md#separated-boolean-decomposition) $f(x,y)=\bigoplus_{\ell}u_\ell(x)v_\ell(y)$. Feed $(u_\ell,v_\ell)$ to one independent [PR box](#popescu-rohrlich-box), obtaining outputs with $a_\ell\oplus b_\ell=u_\ell v_\ell$. Alice forms $A=\bigoplus_\ell a_\ell$, Bob forms $B=\bigoplus_\ell b_\ell$, and their parities satisfy $A\oplus B=f$. Sending the single bit $A$ lets Bob compute the answer with certainty. The truth-table decomposition needs at most $2^{\min(m,n)}$ boxes for input lengths $m,n$. Each box's local output is uniform, so Bob's uncommunicated output string carries no information about Alice's input; the final parity bit is essential for a general function depending on that input.

## Objective-collapse theory

↑ **Parent:** [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Objective-collapse_theory)

An objective-collapse theory treats wave-function collapse as a physical process localized in spacetime, rather than only as an observer's update of information.

### Ghirardi-Rimini-Weber theory

↑ **Parent:** [Objective-collapse theory](#objective-collapse-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ghirardi–Rimini–Weber_theory)

The Ghirardi--Rimini--Weber theory modifies [unitary time evolution](quantum-system.md#unitary-time-evolution) by random Gaussian position localizations. Each constituent collapses at a small fixed rate, while the rate for an entangled macroscopic body grows with its number of constituents.

#### GRW localization operator

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

For localization length $r_C$, the GRW localization operator acting on particle $i$ is

$$
L_i(\mathbf X)=(\pi r_C^2)^{-3/4}
\exp\left[-\frac{(\mathbf q_i-\mathbf X)^2}{2r_C^2}\right].
$$

A collapse centred at $\mathbf X$ sends $|\psi\rangle$ to the normalized state $L_i(\mathbf X)|\psi\rangle$ with probability density $\|L_i(\mathbf X)|\psi\rangle\|^2$.

##### GRW collapse-centre event probabilities

↑ **Parent:** [GRW localization operator](#grw-localization-operator)

For equal particle rates in the [GRW model](#ghirardi-rimini-weber-theory), the next centre falls in $B$ with probability $N^{-1}\sum_i\int_B\|L_i(c)\Psi\|^2dc$. With zero [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics), two successive centres in $B$ have joint probability $N^{-2}\sum_{ij}\int_Bdc\int_Bdd\|L_j(d)L_i(c)\Psi\|^2$. Dividing by the first-event probability gives the conditional second event, including repeated particle labels. Spatial probabilities depend on actual packet mass, not solely the nominal packet centres.

#### GRW amplification mechanism

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

For $N$ entangled constituents, independent localization rates add to approximately $N\lambda$. One constituent's collapse localizes the correlated macroscopic configuration, rapidly suppressing macroscopically separated branches.

##### GRW branch persistence versus geometric containment

↑ **Parent:** [GRW amplification mechanism](#grw-amplification-mechanism)

A first localization near one macroscopically separated branch suppresses the other branch through the Gaussian [GRW localization operator](#grw-localization-operator). This selects a correlated pointer alternative. However, if a region contains only packet centres and excludes substantial packet mass, the next centre need not lie in that region's small enlargement. Probabilities $|\alpha|^2$ for the first event and approximately one for the next require regions containing essentially all corresponding branch mass. The general [GRW collapse-centre event probabilities](#grw-collapse-centre-event-probabilities) retain the geometry exactly.

#### GRW spontaneous heating

↑ **Parent:** [Ghirardi-Rimini-Weber theory](#ghirardi-rimini-weber-theory)

GRW position localization increases the ensemble mean momentum variance. In three dimensions one collapse adds $3\hbar^2/(2r_C^2)$ to $\langle\mathbf p^2\rangle$, producing mean kinetic-energy increase $3\hbar^2/(4mr_C^2)$.

### Local quantum state under objective collapse

↑ **Parent:** [Objective-collapse theory](#objective-collapse-theory)

At a spacetime point $x$, the local quantum state is the reduced density operator obtained on spacelike hypersurfaces approaching the past light cone of $x$. It includes the effects of objective collapses in that past light cone and excludes spacelike-separated collapses.

#### Quantum state readout device

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

A quantum state readout device at $x$ hypothetically outputs a classical description of the [local quantum state under objective collapse](#local-quantum-state-under-objective-collapse) without changing that state. Its output can respond to a remote collapse only after the collapse enters the past light cone of $x$, so the device preserves [relativistic causality](special-relativity.md#relativistic-causality).

#### Proper mixed state

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

A proper mixed state represents classical uncertainty over states selected by an actual preparation or collapse. Once that selecting event lies in the readout point's past light cone, a [quantum state readout device](#quantum-state-readout-device) returns the selected component rather than merely the ensemble average.

#### Improper mixed state

↑ **Parent:** [Local quantum state under objective collapse](#local-quantum-state-under-objective-collapse)

An improper mixed state is the [reduced density matrix](bell-state.md#reduced-density-matrix) of a subsystem entangled with unobserved degrees of freedom. A [quantum state readout device](#quantum-state-readout-device) returns that reduced state until a relevant collapse lies in its past light cone.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [EPR criterion of reality](#epr-criterion-of-reality)
