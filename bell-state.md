# Bell state

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bell_state)

The four Bell states form an orthonormal maximally entangled basis for two qubits.

**Table of contents**

- [Polarization correlations of the Psi-plus Bell state](#polarization-correlations-of-the-psi-plus-bell-state)
- [Phase averaging of a polarization Bell state](#phase-averaging-of-a-polarization-bell-state)
- [Magic basis](#magic-basis)
  - [Real local-unitary representation in the magic basis](#real-local-unitary-representation-in-the-magic-basis)
- [Local flag correction of a Bell-state phase mixture](#local-flag-correction-of-a-bell-state-phase-mixture)
- [Bell pair](#bell-pair)
- [Dephased Bell-state mixture](#dephased-bell-state-mixture)
- [Bell-basis measurement](#bell-basis-measurement)
  - [Bell state analyzer](#bell-state-analyzer)
  - [Bell-state nondemolition measurement](#bell-state-nondemolition-measurement)
- [Superdense coding](#superdense-coding)
  - [Two-component Bell resource in dense coding](#two-component-bell-resource-in-dense-coding)
    - [Bell-label Hamming distance and bit errors](#bell-label-hamming-distance-and-bit-errors)
  - [Single-local-gate Bell readout information](#single-local-gate-bell-readout-information)
- [Spin singlet state](#spin-singlet-state)
  - [Collective-unitary covariance of the two-qubit singlet](#collective-unitary-covariance-of-the-two-qubit-singlet)
- [Reduced density matrix](#reduced-density-matrix)
  - [Equal reduced states give identical local statistics](#equal-reduced-states-give-identical-local-statistics)
  - [No-communication theorem](#no-communication-theorem)
    - [Remote state invariance under a local trace-preserving operation](#remote-state-invariance-under-a-local-trace-preserving-operation)
  - [Product state](#product-state)
    - [Conditional-vector product-state criterion](#conditional-vector-product-state-criterion)
    - [Two-qubit product-state determinant criterion](#two-qubit-product-state-determinant-criterion)
  - [Entangled state](#entangled-state)
    - [Impossibility of universal identical-basis perfect correlations](#impossibility-of-universal-identical-basis-perfect-correlations)
    - [Polarization entanglement](#polarization-entanglement)
      - [Polarization-entangled photon pair](#polarization-entangled-photon-pair)
    - [Entanglement distillation](#entanglement-distillation)
    - [Entanglement dilution](#entanglement-dilution)
      - [Exact dilution obstruction from Schmidt rank](#exact-dilution-obstruction-from-schmidt-rank)
      - [Deterministic two-qubit entanglement dilution](#deterministic-two-qubit-entanglement-dilution)
    - [Entanglement monotone](#entanglement-monotone)
      - [Relative entropy of entanglement](#relative-entropy-of-entanglement)
      - [Schmidt-tail entanglement monotone](#schmidt-tail-entanglement-monotone)
    - [Concurrence](#concurrence)
      - [Concurrence in the magic basis](#concurrence-in-the-magic-basis)
      - [Mixed-state concurrence of two qubits](#mixed-state-concurrence-of-two-qubits)
        - [Concurrence scaling under invertible local filters](#concurrence-scaling-under-invertible-local-filters)
    - [Entanglement criterion for a two-term correlated state](#entanglement-criterion-for-a-two-term-correlated-state)
    - [Entanglement concentration](#entanglement-concentration)
      - [Single-copy entanglement concentration](#single-copy-entanglement-concentration)
      - [Binary Schmidt filter](#binary-schmidt-filter)
      - [Schmidt projection entanglement concentration](#schmidt-projection-entanglement-concentration)
        - [Tripartite Schmidt projection entanglement concentration](#tripartite-schmidt-projection-entanglement-concentration)
  - [Local indistinguishability of Bell-state phase](#local-indistinguishability-of-bell-state-phase)
- [Local operations and classical communication](#local-operations-and-classical-communication)
  - [Entanglement catalysis](#entanglement-catalysis)
  - [Two-outcome LOCC dilution of a Bell pair](#two-outcome-locc-dilution-of-a-bell-pair)
  - [Deterministic reduction of maximally entangled Schmidt rank](#deterministic-reduction-of-maximally-entangled-schmidt-rank)
  - [Asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate)
    - [Collective advantage over independent two-qubit filtering](#collective-advantage-over-independent-two-qubit-filtering)
  - [Optimal stochastic conversion of a two-qubit pure state](#optimal-stochastic-conversion-of-a-two-qubit-pure-state)
  - [Local unitary operation](#local-unitary-operation)
    - [Local-unitary equivalence](#local-unitary-equivalence)
    - [Local-unitary invariance of entanglement entropy](#local-unitary-invariance-of-entanglement-entropy)
    - [Local-unitary invariance of reduced-state spectra](#local-unitary-invariance-of-reduced-state-spectra)
  - [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem)
  - [LOCC discrimination of two Bell states](#locc-discrimination-of-two-bell-states)
  - [Quantum teleportation](#quantum-teleportation)
    - [Controlled quantum teleportation](#controlled-quantum-teleportation)
      - [GHZ-assisted quantum teleportation](#ghz-assisted-quantum-teleportation)
    - [Classical communication lower bound for exact qubit teleportation](#classical-communication-lower-bound-for-exact-qubit-teleportation)
    - [Teleportation with an ambiguous Bell-state phase label](#teleportation-with-an-ambiguous-bell-state-phase-label)
    - [Bit-flipped Bell resource teleportation](#bit-flipped-bell-resource-teleportation)
    - [Bouwmeester quantum teleportation experiment](#bouwmeester-quantum-teleportation-experiment)
    - [Teleportation fidelity](#teleportation-fidelity)
    - [Dicke-resource telecloning](#dicke-resource-telecloning)
    - [Exact teleportation resource criterion](#exact-teleportation-resource-criterion)
    - [Entanglement swapping](#entanglement-swapping)
      - [Identical-resource entanglement swapping](#identical-resource-entanglement-swapping)
      - [Heralded Bell-pair projection with two polarization parity filters](#heralded-bell-pair-projection-with-two-polarization-parity-filters)
      - [Bell swapping visibility under random labels](#bell-swapping-visibility-under-random-labels)
    - [Qudit teleportation](#qudit-teleportation)
    - [Teleportation as an identity channel on a reference](#teleportation-as-an-identity-channel-on-a-reference)
    - [One-bit teleportation](#one-bit-teleportation)
      - [Pauli-frame propagation along a measurement wire](#pauli-frame-propagation-along-a-measurement-wire)
      - [Graph-state preparation of a computational-basis input](#graph-state-preparation-of-a-computational-basis-input)
      - [Heralded Pauli X correction using controlled-Z and measurements](#heralded-pauli-x-correction-using-controlled-z-and-measurements)
      - [J gate in measurement-based quantum computation](#j-gate-in-measurement-based-quantum-computation)
        - [J-gate phase-error operator norm](#j-gate-phase-error-operator-norm)
    - [Bell-basis teleportation identity](#bell-basis-teleportation-identity)
    - [No-programming theorem](#no-programming-theorem)
    - [Teleportation with the psi-plus Bell state](#teleportation-with-the-psi-plus-bell-state)

## Polarization correlations of the Psi-plus Bell state

↑ **Parent:** [Bell state](bell-state.md)

For $|\Psi^+\rangle=(|01\rangle+|10\rangle)/\sqrt2$, the [Pauli operator](quantum-circuit.md#pauli-operator) correlations are $\langle XX\rangle=1$, $\langle ZZ\rangle=-1$, and $\langle XZ\rangle=\langle ZX\rangle=0$. Substituting the [measurement of linear photon polarization](quantum-measurement.md#measurement-of-linear-photon-polarization) into $\langle M(\alpha)\otimes M(\beta)\rangle$ gives $\sin2\alpha\sin2\beta-\cos2\alpha\cos2\beta=-\cos2(\alpha+\beta)$. In particular, opposite physical angles give perfect anticorrelation. The sum of angles here depends on this choice of [Bell state](bell-state.md) and basis conventions.

## Phase averaging of a polarization Bell state

↑ **Parent:** [Bell state](bell-state.md)

Uniformly averaging $(|01\rangle+e^{i\varphi}|10\rangle)/\sqrt2$ over $|\varphi|\leq\varphi_0$ leaves the two populations unchanged and multiplies the off-diagonal coherences by $\operatorname{sinc}\varphi_0=\sin\varphi_0/\varphi_0$. For real-plane analyser settings giving the pure-state Bell signal $\sqrt2(1+\cos\varphi)$, linearity of expectation gives the displayed mixed-state signal. Its local-bound violation requires $\operatorname{sinc}\varphi_0>\sqrt2-1$, or $0\leq\varphi_0<2.092751\ldots$ radians. This threshold concerns fixed measurement settings rather than all possible tests of entanglement.

## Magic basis

↑ **Parent:** [Bell state](bell-state.md)

A [Bell basis](quantum-theory.md#bell-basis) with [phases](wave.md#phase-waves) chosen so that local special-unitary transformations of the two [qubits](quantum-system.md#qubit) are represented by real four-dimensional rotations. For one standard ordering it is $\Phi_+,i\Phi_-,i\Psi_+,\Psi_-$. Permuting these vectors changes generator conventions but preserves the invariant [concurrence](#concurrence) $|\sum_jb_j^2|$.[Eqs.(3)–(6), phased Bell basis and concurrence](physics-bibliography.md#entanglement-of-a-pair-of-quantum-bits-by-scott-hill-and-william-k-wootters)

### Real local-unitary representation in the magic basis

↑ **Parent:** [Magic basis](#magic-basis)

The [anti-Hermitian](linear-operator-theory.md#skew-hermitian-matrix) generators of local [qubit](quantum-system.md#qubit) rotations become real [antisymmetric matrices](linear-algebra.md#skew-symmetric-matrix) in the [magic basis](#magic-basis). Their exponentials preserve $b^{\mathsf T}b$, and hence its modulus and pure-state [concurrence](#concurrence). A common [phase](wave.md#phase-waves) changes that bilinear quantity by a [phase](wave.md#phase-waves) but not its modulus.

## Local flag correction of a Bell-state phase mixture

↑ **Parent:** [Bell state](bell-state.md)

Suppose Alice holds a classical orthogonal flag $F$ for the phase of a [Bell state](bell-state.md):

$$
\rho_{ABF}=p|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes|0\rangle\langle0|_F+(1-p)|\Phi^-\rangle\langle\Phi^-|_{AB}\otimes|1\rangle\langle1|_F.
$$

Her local controlled phase correction $U=I_{AB}\otimes|0\rangle\langle0|_F+(Z_A\otimes I_B)\otimes|1\rangle\langle1|_F$ maps this to $|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes[p|0\rangle\langle0|+(1-p)|1\rangle\langle1|]_F$. Thus Alice and Bob recover an exact [Bell pair](#bell-pair) without revealing its bit value. Even if Eve knows the flag, [purity decouples a subsystem from its purification](density-matrix.md#purity-decouples-a-subsystem-from-its-purification), so the corrected pair can supply a private bit. Discarding the flag first can instead yield a [separable quantum state](quantum-information-theory.md#separable-quantum-state), as happens at $p=1/2$.

## Bell pair

↑ **Parent:** [Bell state](bell-state.md)

A Bell pair consists of two [qubits](quantum-system.md#qubit) prepared jointly in a [Bell state](bell-state.md). It is a maximally entangled two-qubit resource with [Schmidt rank](von-neumann-entropy.md#schmidt-rank) two. Two independent [Bell pairs](#bell-pair) have resource [Schmidt rank](von-neumann-entropy.md#schmidt-rank) four across the same party partition.

## Dephased Bell-state mixture

↑ **Parent:** [Bell state](bell-state.md)

For real $-1\leq\alpha\leq1$, this two-[qubit](quantum-system.md#qubit) [density operator](density-matrix.md) has equal $00$ and $11$ populations and off-diagonal coherences $\alpha/2$. It is a [pure state](quantum-theory.md#pure-state) exactly when $\alpha=\pm1$, and a [separable quantum state](quantum-information-theory.md#separable-quantum-state) exactly when $\alpha=0$. Its [partial transpose](quantum-information-theory.md#partial-transpose) has [eigenvalues](linear-operator-theory.md#eigenvalue) $1/2,1/2,\alpha/2,-\alpha/2$, directly witnessing entanglement for every nonzero admissible coherence.

## Bell-basis measurement

↑ **Parent:** [Bell state](bell-state.md)

A Bell-basis measurement is the four-outcome projective measurement whose projectors are onto the four [Bell states](bell-state.md). It jointly measures two qubits and is the sender's measurement in [quantum teleportation](#quantum-teleportation).

### Bell state analyzer

↑ **Parent:** [Bell-basis measurement](#bell-basis-measurement)

A device implementing a [Bell-basis measurement](#bell-basis-measurement) on two [qubits](quantum-system.md#qubit). A complete analyzer distinguishes all four [Bell states](bell-state.md). A basic passive [linear optics](optics.md#linear-optics) analyzer for two polarization [qubits](quantum-system.md#qubit) uses a [balanced beam splitter](optical-instrument.md#balanced-beam-splitter), [polarizing beam splitters](optical-instrument.md#polarizing-beam-splitter) and [single-photon detectors](optical-instrument.md#single-photon-detector). Its ideal unambiguous success probability is $1/2$: the two opposite-polarization [Bell states](bell-state.md) have distinct click patterns, while the two same-polarization [Bell states](bell-state.md) remain mutually ambiguous. Additional physical resources can change this restriction. A destructive analyzer absorbs the measured [photons](quantum-mechanics.md#photon); it need not preserve the detected [Bell state](bell-state.md).

### Bell-state nondemolition measurement

↑ **Parent:** [Bell-basis measurement](#bell-basis-measurement)

The [Bell states](bell-state.md) are joint [eigenstates](energy-eigenvalue.md#eigenstate) of commuting $Z_AZ_B$ and $X_AX_B$. Two shared [Bell state](bell-state.md) meter pairs realize their two [entanglement-assisted nondemolition parity measurements](quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement) using spacelike local circuits. Their projector products give the four rank-one [Bell state](bell-state.md) outcomes and preserve each input [Bell state](bell-state.md). The globally identified outcome requires later [local operations and classical communication](#local-operations-and-classical-communication).

## Superdense coding

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Superdense_coding)

[Superdense coding](#superdense-coding) uses a shared [Bell state](bell-state.md) to communicate two classical [bits](information-theory.md#bit) by transmitting one [qubit](quantum-system.md#qubit). The sender selects one of four orthogonal [Bell states](bell-state.md) with a local [Pauli operator](quantum-circuit.md#pauli-operator), and the receiver performs a [Bell-basis measurement](#bell-basis-measurement). For an ideal shared [Bell pair](#bell-pair), the transmitted [qubit](quantum-system.md#qubit) alone has a [maximally mixed state](density-matrix.md#maximally-mixed-state) for every message and reveals no information about the chosen encoding.

### Two-component Bell resource in dense coding

↑ **Parent:** [Superdense coding](#superdense-coding)

With phase/parity labels $(u,v)$ encoded by $X^vZ^u$, a resource $a|\Phi^+\rangle+b|\Phi^-\rangle$ gives intended-label probability $|a|^2$ and phase-label-flip probability $|b|^2$ under a [Bell-basis measurement](#bell-basis-measurement). This follows because the local [Pauli operator](quantum-circuit.md#pauli-operator) maps the two orthogonal components into the two Bell states whose phase label differs. The resource is a coherent [pure state](quantum-theory.md#pure-state), even though its measured label statistics form a classical noisy channel.

#### Bell-label Hamming distance and bit errors

↑ **Parent:** [Two-component Bell resource in dense coding](#two-component-bell-resource-in-dense-coding)

If a wrong Bell-label partner occurs with probability $\epsilon$ and differs from the intended two-bit label in $w$ positions, its contribution to the error probability of a uniformly selected bit is $\epsilon w/2$. Relabeling the [Bell states](bell-state.md) can change $w$ while preserving the physical wrong-state probability. Thus symbol error probability and bit error probability are different quantities.

### Single-local-gate Bell readout information

↑ **Parent:** [Superdense coding](#superdense-coding)

For four uniformly distributed [Bell states](bell-state.md), measure one [qubit](quantum-system.md#qubit) along [Bloch vector](density-matrix.md#bloch-vector) $\boldsymbol n$ and the other along $z$. The sign within each $\Phi^\pm$ or $\Psi^\pm$ pair is invisible and the displayed [mutual information](information-theory.md#mutual-information) is at most one bit. A local [Hadamard gate](quantum-theory.md#hadamard-gate) before a computational detector changes $n_z$ from one to zero and destroys the remaining information. An entangling Bell decoder falls outside this product-measurement restriction and recovers two bits.

## Spin singlet state

↑ **Parent:** [Bell state](bell-state.md)

The two-spin singlet is

$$
|\Psi^-\rangle=\frac{|01\rangle-|10\rangle}{\sqrt2}.
$$

Spin measurements along axes $\mathbf a$ and $\mathbf b$ have correlation $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$, and equal axes give perfect anticorrelation.

This is the [spin-one-half singlet state](angular-momentum-operator.md#spin-one-half-singlet-state), an example of an [angular momentum singlet state](angular-momentum-operator.md#singlet-state). The general singlet condition is zero total angular momentum, not the choice of a particular two-qubit Bell basis.

### Collective-unitary covariance of the two-qubit singlet

↑ **Parent:** [Spin singlet state](#spin-singlet-state)

For $|s\rangle=(|01\rangle-|10\rangle)/\sqrt2$ and any two-by-two [unitary matrix](linear-operator-theory.md#unitary-matrix), expand the two columns of $U$. The equal-index coefficients cancel, and the coefficient of $|01\rangle-|10\rangle$ is the determinant. Its modulus is one, so a common change of qubit basis preserves the [spin singlet state](#spin-singlet-state) up to a [global phase](quantum-system.md#global-phase). The density projector is exactly invariant.

## Reduced density matrix

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_density_matrix)

For a bipartite density operator $\rho_{AB}$, the reduced state of subsystem $A$ is the partial trace $\rho_A=\operatorname{Tr}_B\rho_{AB}$. Every measurement performed only on $A$ has outcome probabilities determined entirely by $\rho_A$.

### Equal reduced states give identical local statistics

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)

Suppose two [density operators](density-matrix.md) on $R\otimes E$ have the same [reduced density matrix](#reduced-density-matrix) $\sigma_R$. Every measurement confined to $R$ then has the same outcome [probabilities](probability-theory.md#probability) for the two preparations: a [POVM](quantum-measurement.md#positive-operator-valued-measure) effect $F_R$ has [probability](probability-theory.md#probability) $\operatorname{Tr}(F_R\sigma_R)$ in either case. This remains true when $R$ contains several laboratories brought together for a joint measurement.

For independent copies, the accessible states are both $\sigma_R^{\otimes n}$. No collective measurement on those copies can distinguish the original preparations. Adaptive local processing also cannot help, since applying the same quantum operation to equal inputs gives equal outputs. Access to an additional environment measurement record is a change of resources, and can reveal differences hidden by the [partial trace](quantum-theory.md#partial-trace).

### No-communication theorem

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/No-communication_theorem)

A trace-preserving operation on subsystem $B$ cannot change the [reduced density matrix](#reduced-density-matrix) of a disjoint subsystem $A$ when its unobserved outcomes are averaged. Local measurements on $A$ therefore cannot reveal which operation was chosen on $B$.

#### Remote state invariance under a local trace-preserving operation

↑ **Parent:** [No-communication theorem](#no-communication-theorem)

For local [Kraus operators](quantum-information-theory.md#kraus-operator) $A_i$ with $\sum_iA_i^\dagger A_i=I$, let $\rho'_{AB}=\sum_i(A_i\otimes I)\rho_{AB}(A_i^\dagger\otimes I)$. For every remote operator $B$, cyclicity of the [trace](linear-algebra.md#matrix-trace) gives $\operatorname{Tr}[(I\otimes B)\rho'_{AB}]=\sum_i\operatorname{Tr}[(A_i^\dagger A_i\otimes B)\rho_{AB}]=\operatorname{Tr}[(I\otimes B)\rho_{AB}]$. Hence the remote [reduced density matrix](#reduced-density-matrix) is unchanged. In particular every remote [POVM](quantum-measurement.md#positive-operator-valued-measure) has the same outcome probabilities, proving the [no-communication theorem](#no-communication-theorem) from the measurement rule rather than assuming it as a physical postulate.

### Product state

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Product_state)

A bipartite [density operator](density-matrix.md) is a product state when it factors as $\rho_A\otimes\rho_B$. A pure product state factors as $|\psi_A\rangle\otimes|\psi_B\rangle$; its [reduced density matrices](#reduced-density-matrix) have rank one and zero [entanglement entropy](von-neumann-entropy.md#entanglement-entropy). Mixed product states can have nonzero marginal [Von Neumann entropy](von-neumann-entropy.md).

#### Conditional-vector product-state criterion

↑ **Parent:** [Product state](#product-state)

A nonzero bipartite [pure state](quantum-theory.md#pure-state) is a [product state](#product-state) if and only if all its [partial inner products](multilinear-algebra.md#partial-inner-product) on the first subsystem lie in a common one-dimensional [vector subspace](vector-space.md#vector-subspace) of the second. For a product $|a\rangle\otimes|b\rangle$, every contraction equals $\langle u|a\rangle|b\rangle$. Conversely, contract against each [vector](vector-space.md#vector) of an [orthonormal basis](inner-product.md#orthonormal-basis) to write $|\Psi\rangle=\sum_i|i\rangle\otimes|\chi_i\rangle$. If $|\chi_i\rangle=c_i|b\rangle$ for a common nonzero $|b\rangle$, then $|\Psi\rangle=(\sum_ic_i|i\rangle)\otimes|b\rangle$. Zero conditional [vectors](vector-space.md#vector) are allowed. A nontrivial [linear dependence](vector-space.md#linear-dependence) relation requires multipliers not both zero; allowing both multipliers to vanish would give no test at all.

#### Two-qubit product-state determinant criterion

↑ **Parent:** [Product state](#product-state)

Write a two-qubit pure state as $\sum_{i,j=0}^1c_{ij}|ij\rangle$ and form its coefficient matrix $C=(c_{ij})$. The state is a [product state](#product-state) exactly when $C$ has rank one, equivalently when

$$
c_{00}c_{11}=c_{01}c_{10}.
$$

### Entangled state

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)

A bipartite [density operator](density-matrix.md) is entangled when it is not a [separable quantum state](quantum-information-theory.md#separable-quantum-state). For a pure state, this is equivalent to not being a [product state](#product-state), or to either [reduced density matrix](#reduced-density-matrix) having rank greater than one.

#### Impossibility of universal identical-basis perfect correlations

↑ **Parent:** [Entangled state](#entangled-state)

For two systems of equal dimension $d\ge2$, no joint [pure state](quantum-theory.md#pure-state) guarantees equal outcome labels whenever both systems undergo the same arbitrary [basic measurement](quantum-measurement.md#basic-measurement). Equal outcomes in the [computational basis](quantum-theory.md#computational-basis) would force $|\Psi\rangle=\sum_jc_j|jj\rangle$. On any two coordinates j,k, changing both bases to the real sum/difference pair makes the different-outcome amplitude $(c_j-c_k)/2$, so all coefficients must agree. Changing both to the imaginary-phase pair makes a different-outcome amplitude $(c_j+c_k)/2$, so those coefficients must also be negatives. They must all vanish, contradicting [normalization](mathematics.md#normalization). The one-dimensional case is an exception.

The requirement of all _complex_ bases matters. A maximally entangled [vector](vector-space.md#vector) $d^{-1/2}\sum_j|jj\rangle$ does produce matching labels if one party uses a basis and the other its coordinatewise [complex conjugate](complex-analysis.md#complex-conjugate) basis. [Conjugate-state steering from a maximally entangled pair](quantum-theory.md#conjugate-state-steering-from-a-maximally-entangled-pair) gives this conjugation explicitly. Identical real bases are a special case, not evidence for identical arbitrary complex bases.

#### Polarization entanglement

↑ **Parent:** [Entangled state](#entangled-state)

[Quantum entanglement](#entangled-state) between [electromagnetic polarization](electromagnetic-wave.md#polarization-of-an-electromagnetic-wave) degrees of freedom. For example, $(|HV\rangle+|VH\rangle)/\sqrt2$ is a [Bell state](bell-state.md) of two [photons](quantum-mechanics.md#photon); neither photon separately has a definite [horizontal polarization](electromagnetic-wave.md#horizontal-polarization) or [vertical polarization](electromagnetic-wave.md#vertical-polarization) in this description.

##### Polarization-entangled photon pair

↑ **Parent:** [Polarization entanglement](#polarization-entanglement)

A pair of [photons](quantum-mechanics.md#photon) whose joint [electromagnetic polarization](electromagnetic-wave.md#polarization-of-an-electromagnetic-wave) has [polarization entanglement](#polarization-entanglement).

#### Entanglement distillation

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_distillation)

Entanglement distillation uses [local operations and classical communication](#local-operations-and-classical-communication) on many noisy [entangled states](#entangled-state) to produce fewer high-fidelity [Bell pairs](#bell-pair). It is also called entanglement purification. The protocol may fail or abort; naming a purification step does not guarantee successful output for arbitrary inputs. If the output is an exact [pure state](quantum-theory.md#pure-state) of [Bell pairs](#bell-pair), every [purification of a density operator](density-matrix.md#purification-of-a-density-operator) factors between those pairs and the environment, so measuring each pair in the [computational basis](quantum-theory.md#computational-basis) gives a shared uniform bit independent of an eavesdropper. Approximate privacy follows when the entire retained output is sufficiently close to that pure target. A [separable quantum state](quantum-information-theory.md#separable-quantum-state) cannot be distilled into a [Bell pair](#bell-pair) by [LOCC](#local-operations-and-classical-communication), because each local branch preserves separability.

#### Entanglement dilution

↑ **Parent:** [Entangled state](#entangled-state)

Entanglement dilution uses [local operations and classical communication](#local-operations-and-classical-communication) to prepare partially entangled states from [maximally entangled states](quantum-theory.md#maximally-entangled-state), such as [Bell pairs](#bell-pair). For many identical bipartite pure targets, the asymptotic cost in Bell pairs per target, allowing a vanishing approximation error, is their [entanglement entropy](von-neumann-entropy.md#entanglement-entropy) in bits. The [quantum typical subspace](quantum-information-theory.md#quantum-typical-subspace) of the target's [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) has almost all its weight and dimension at most $2^{m(S+\delta)}$. A maximally entangled state of this dimension can be converted to the normalized truncated target by [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem). The resulting state approaches the full target as the retained weight tends to one. [Average monotonicity of pure-state entanglement entropy](von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy) and entropy continuity give the converse lower bound. This is the reverse asymptotic task to [entanglement concentration](#entanglement-concentration).

##### Exact dilution obstruction from Schmidt rank

↑ **Parent:** [Entanglement dilution](#entanglement-dilution)

For $0<p<1$, every bipartition of $\Psi_p^{\otimes n}$ has [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $2^n$, while $m$ copies of a [GHZ state](quantum-theory.md#greenberger-horne-zeilinger-state) have [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $2^m$. [Schmidt-rank contraction under product operators](von-neumann-entropy.md#schmidt-rank-contraction-under-product-operators) therefore forbids any exact successful [LOCC](#local-operations-and-classical-communication) branch when $m<n$. Approximate [entanglement dilution](#entanglement-dilution) avoids this obstruction by retaining only a high-weight [quantum typical subspace](quantum-information-theory.md#quantum-typical-subspace), whose dimension has logarithm $nh_2(p)+o(n)$. Exact finite-block conversion and asymptotically faithful conversion are different tasks.

##### Deterministic two-qubit entanglement dilution

↑ **Parent:** [Entanglement dilution](#entanglement-dilution)

For nonnegative $u,v$ with $u^2+v^2=1$, Alice applies [Kraus operators](quantum-information-theory.md#kraus-operator) $M_0=\operatorname{diag}(u,v)$ and $M_1=\operatorname{diag}(v,u)$ to one half of a [Bell state](bell-state.md). Their squared effects sum to the identity, and both outcomes have probability one half. The first branch is the target; the second becomes the target after both parties apply [Pauli X gates](quantum-theory.md#pauli-x-gate). Sending the outcome by [classical communication](quantum-information-theory.md#classical-communication) makes this exact deterministic [entanglement dilution](#entanglement-dilution), rather than a postselected conversion.

#### Entanglement monotone

↑ **Parent:** [Entangled state](#entangled-state)

An entanglement monotone quantifies [entanglement](#entangled-state) without increasing on average under [local operations and classical communication](#local-operations-and-classical-communication). The average is over recorded [quantum measurement](quantum-measurement.md) outcomes: individual successful branches can have more entanglement, provided their probabilities compensate for that increase. This distinction makes an entanglement monotone useful for bounding probabilistic state conversion. A pure-state entanglement monotone need only satisfy this inequality on pure input states and pure conditional branches, with local measurement outcomes refined to individual [Kraus operators](quantum-information-theory.md#kraus-operator).

##### Relative entropy of entanglement

↑ **Parent:** [Entanglement monotone](#entanglement-monotone)

The relative entropy of entanglement is the smallest [quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy) from a [density operator](density-matrix.md) to a [separable quantum state](quantum-information-theory.md#separable-quantum-state), with the separable set specified for the relevant division into parties. [Nonnegativity of quantum relative entropy](von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) implies $E_R\geq0$. For a [separable quantum state](quantum-information-theory.md#separable-quantum-state), choosing $\sigma=\rho$ gives $E_R=0$. For finite-dimensional bipartite states, compactness of the separable set and lower semicontinuity of the relative entropy give the converse. The support convention is $D(\rho\|\sigma)=+\infty$ unless $\operatorname{supp}\rho\subseteq\operatorname{supp}\sigma$.

##### Schmidt-tail entanglement monotone

↑ **Parent:** [Entanglement monotone](#entanglement-monotone)

For a bipartite [pure state](quantum-theory.md#pure-state), the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) are the nonzero [eigenvalues](linear-operator-theory.md#eigenvalue) of either [reduced density matrix](#reduced-density-matrix). Their sum except the largest defines $E_2=1-\lambda_{\max}(\rho_A)$. The largest eigenvalue is a convex function, since $\lambda_{\max}(\rho)=\max_{\|v\|=1}\langle v|\rho|v\rangle$; consequently $E_2$ is concave. If Alice measures locally and records outcome $r$, Bob's conditional reductions satisfy $\sum_r p_r\rho_{B,r}=\rho_B$. Concavity gives $\sum_r p_rE_2(\chi_r)\leq E_2(\chi)$. For Bob's measurements use Alice's unchanged average reduction instead. Iteration proves average monotonicity under [LOCC](#local-operations-and-classical-communication). For [Schmidt rank](von-neumann-entropy.md#schmidt-rank) at most two, $E_2$ is the smaller squared Schmidt coefficient. A conversion succeeding with probability $p$ therefore obeys $pE_2(\phi)\leq E_2(\psi)$, since failure branches contribute nonnegative amounts.

#### Concurrence

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Concurrence)

For a normalized pure state of two qubits with coefficient matrix $C$, the concurrence is $2|\det C|$. It ranges from zero for a [product state](#product-state) to one for a [maximally entangled state](quantum-theory.md#maximally-entangled-state).

##### Concurrence in the magic basis

↑ **Parent:** [Concurrence](#concurrence)

For a normalized pure two-qubit state written in a [magic basis](#magic-basis), [concurrence](#concurrence) is $\mathcal C=|\sum_jb_j^2|$, while $\det\rho_A=\mathcal C^2/4$. This bilinear sum uses no [complex conjugation](complex-analysis.md#complex-conjugation) inside its square; replacing it by $\sum_j|b_j|^2$ would incorrectly give maximal [concurrence](#concurrence) for every state.

##### Mixed-state concurrence of two qubits

↑ **Parent:** [Concurrence](#concurrence)

For a normalized two-[qubit](quantum-system.md#qubit) [pure state](quantum-theory.md#pure-state) with coefficient matrix $M$, [concurrence](#concurrence) is $2|\det M|$. The displayed [convex roof extension](density-matrix.md#convex-roof-extension) defines its mixed-state version. Combining decompositions proves convexity: $C(\sum_jr_j\rho_j)\leq\sum_jr_jC(\rho_j)$. Every [separable quantum state](quantum-information-theory.md#separable-quantum-state) has a decomposition into product vectors, each with zero determinant, so its concurrence is zero.

###### Concurrence scaling under invertible local filters

↑ **Parent:** [Mixed-state concurrence of two qubits](#mixed-state-concurrence-of-two-qubits)

For $\rho'=(A\otimes B)\rho(A^\dagger\otimes B^\dagger)/p$, with invertible $A,B$, a pure coefficient matrix transforms as $M\mapsto AMB^{\mathsf T}$. Its unnormalized determinant is multiplied by $\det A\det B$. The invertible filter bijects pure decompositions before and after conditioning, with branch weights rescaled by their success probabilities. Taking both infima in the [convex roof extension](density-matrix.md#convex-roof-extension) gives the displayed exact scaling. If either filter has rank one, the retained state is separable across that party.

#### Entanglement criterion for a two-term correlated state

↑ **Parent:** [Entangled state](#entangled-state)

The state $a|00\rangle+b|11\rangle$ is entangled exactly when $ab\ne0$. Its reduced density matrix has nonzero eigenvalues $|a|^2$ and $|b|^2$.

#### Entanglement concentration

↑ **Parent:** [Entangled state](#entangled-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_concentration)

Entanglement concentration probabilistically converts partially entangled pure states into fewer maximally entangled states by local operations and classical communication.

##### Single-copy entanglement concentration

↑ **Parent:** [Entanglement concentration](#entanglement-concentration)

For one pure rank-two entangled state with descending squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) $(\lambda_0,\lambda_1)$, the success operator $F=\operatorname{diag}(\sqrt{\lambda_1/\lambda_0},1)$ gives a [Bell pair](#bell-pair) with probability $2\lambda_1$. The complementary operator $\sqrt{I-F^\dagger F}$ makes a valid [quantum instrument](quantum-measurement.md#quantum-instrument). Optimality follows from the [Schmidt-tail entanglement monotone](#schmidt-tail-entanglement-monotone): a successful Bell branch has smallest weight $1/2$, so its probability cannot exceed $2\lambda_1$. Failure branches have nonnegative monotone and cannot loosen this bound.

##### Binary Schmidt filter

↑ **Parent:** [Entanglement concentration](#entanglement-concentration)

For a pure state with two descending squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) $\lambda_0\ge\lambda_1$, this [quantum instrument](quantum-measurement.md#quantum-instrument) acts in one party's [Schmidt basis](von-neumann-entropy.md#schmidt-basis). The first outcome balances the two Schmidt amplitudes when $\tan\theta=\sqrt{\lambda_1/\lambda_0}$, with probability $2\lambda_0\lambda_1$. This is not the optimal unrestricted success probability $2\lambda_1$ in [single-copy entanglement concentration](#single-copy-entanglement-concentration). An embedding in a larger subsystem requires a [POVM on the occupied support](quantum-measurement.md#povm-on-the-occupied-support) or a full-space completion.

##### Schmidt projection entanglement concentration

↑ **Parent:** [Entanglement concentration](#entanglement-concentration)

For $n$ copies of a normalized [pure state](quantum-theory.md#pure-state) $\alpha|00\rangle+\beta|11\rangle$, regroup Alice's and Bob's tensor factors. Alice performs a [projective measurement](quantum-measurement.md#projective-measurement) of the total number $k$ of zeroes, preserving all coherence among strings with that count. The outcome has [binomial distribution](discrete-probability-distribution.md#binomial-distribution)

$$
p_k=\binom nk|\alpha|^{2k}|\beta|^{2(n-k)}.
$$

Each retained string has the same complex amplitude $\alpha^k\beta^{n-k}$, so, up to a common phase, the conditional [quantum state](quantum-system.md#quantum-state) is

$$
|T_k\rangle=\binom nk^{-1/2}\sum_{z(x)=k}|x\rangle_A|x\rangle_B.
$$

Its equal [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) make it a [maximally entangled state](quantum-theory.md#maximally-entangled-state) of [Schmidt rank](von-neumann-entropy.md#schmidt-rank) $\binom nk$. Alice sends the count to Bob. They can relabel the corresponding local [computational basis](quantum-theory.md#computational-basis) strings with local unitary operations, and convert the resulting resource to [Bell pairs](#bell-pair). Measuring the individual bits instead would reveal the entire string and leave a [product state](#product-state).

###### Tripartite Schmidt projection entanglement concentration

↑ **Parent:** [Schmidt projection entanglement concentration](#schmidt-projection-entanglement-concentration)

For $\sqrt p\,|000\rangle+\sqrt{1-p}\,|111\rangle$, a [projective measurement](quantum-measurement.md#projective-measurement) of the number of ones in one party's $n$ local [qubits](quantum-system.md#qubit) gives a common type class of size $d_k=\binom nk$. The conditional [pure state](quantum-theory.md#pure-state) is $d_k^{-1/2}\sum_{|x|=k}|x,x,x\rangle$. It can be converted exactly and deterministically to a uniform common-label state of any dimension $m\leq d_k$: one party measures an $m$-element subset $S$ with [Kraus operator](quantum-information-theory.md#kraus-operator) $\Pi_S/\sqrt{\binom{d_k-1}{m-1}}$, and all parties relabel their common retained labels after receiving $S$. Choosing $m=2^f$ gives $f$ independent [GHZ states](quantum-theory.md#greenberger-horne-zeilinger-state). [Stirling's formula](real-analysis.md#stirling-formula) and the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) give $f/n\to h_2(p)$ in probability. Measuring every local bit separately would instead destroy the coherence and leave a [product state](#product-state).

### Local indistinguishability of Bell-state phase

↑ **Parent:** [Reduced density matrix](#reduced-density-matrix)

The Bell states $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$ and $|\Phi^-\rangle=(|00\rangle-|11\rangle)/\sqrt2$ both have reduced state $I/2$ on either qubit. No measurement on one qubit alone can distinguish their relative sign.

## Local operations and classical communication

↑ **Parent:** [Bell state](bell-state.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_operations_and_classical_communication)

Local operations and classical communication allow separated parties to measure or transform their own subsystems and exchange ordinary classical messages.

### Entanglement catalysis

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

An auxiliary entangled [pure state](quantum-theory.md#pure-state) can enable an otherwise forbidden deterministic bipartite [LOCC](#local-operations-and-classical-communication) transformation while being returned exactly and uncorrelated with the output. [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem) reduces this to the displayed [majorization](vector-space.md#majorization) condition on sorted squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient). It does not follow from a scalar comparison of [entanglement entropies](von-neumann-entropy.md#entanglement-entropy): tensoring changes which products occupy the largest cumulative-weight sums. An exact returned catalyst can be reused; merely restoring its marginal while allowing correlations is a different resource task.[Introduction and explicit two-qubit catalyst example](physics-bibliography.md#entanglement-assisted-local-manipulation-of-pure-quantum-states-by-daniel-jonathan-and-martin-b-plenio)

### Two-outcome LOCC dilution of a Bell pair

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Let $c,s\geq0$ and $c^2+s^2=1$. Starting from the [Bell state](bell-state.md) $(|00\rangle+|11\rangle)/\sqrt2$, Alice applies the [quantum measurement](quantum-measurement.md) with [Kraus operators](quantum-information-theory.md#kraus-operator) $M_0,M_1$ displayed above. Completeness follows from $M_0^\dagger M_0+M_1^\dagger M_1=I$. Each outcome has [probability](probability-theory.md#probability) $1/2$. The normalized outputs are $c|00\rangle+s|11\rangle$ and $s|00\rangle+c|11\rangle$. Communicating the outcome allows both parties to apply a [Pauli X gate](quantum-theory.md#pauli-x-gate) in the second branch, making both outputs equal to the first. Thus this [LOCC](#local-operations-and-classical-communication) protocol deterministically converts one [Bell pair](#bell-pair) into any two-[qubit](quantum-system.md#qubit) [pure state](quantum-theory.md#pure-state) with these [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient), after appropriate [local unitary operations](#local-unitary-operation). It includes the [product state](#product-state) endpoint without [postselection](quantum-measurement.md#postselection).

### Deterministic reduction of maximally entangled Schmidt rank

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Let $|\Phi_d\rangle=d^{-1/2}\sum_{j=0}^{d-1}|j,j\rangle$ and $1\leq m\leq d$. It can be converted deterministically by [LOCC](#local-operations-and-classical-communication) to $|\Phi_m\rangle$. For each $m$-element subset $S$ of the local basis labels, let $\Pi_S$ be its projector and let Alice's [Kraus operator](quantum-information-theory.md#kraus-operator) be $K_S=\Pi_S/\sqrt{\binom{d-1}{m-1}}$. Every label occurs in $\binom{d-1}{m-1}$ subsets, so $\sum_SK_S^\dagger K_S=I$. Each outcome has [probability](probability-theory.md#probability) $m/[d\binom{d-1}{m-1}]=1/\binom dm$ and leaves the [maximally entangled state](quantum-theory.md#maximally-entangled-state) $m^{-1/2}\sum_{j\in S}|j,j\rangle$. Alice reports $S$, and both parties relabel these $m$ basis states to $0,\ldots,m-1$ by [local unitary operations](#local-unitary-operation).

For $d=6$, $m=4$, only three outcomes are needed: partition the six labels into disjoint pairs $T_0,T_1,T_2$ and use $K_r=(I-\Pi_{T_r})/\sqrt2$. Each label is retained twice, proving completeness, and each outcome has [probability](probability-theory.md#probability) $1/3$. Every branch leaves four equal [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient), hence two independent [Bell pairs](#bell-pair) after binary relabelling.

### Asymptotic pure-state entanglement conversion rate

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

For bipartite pure source and target states with positive target [entanglement entropy](von-neumann-entropy.md#entanglement-entropy), the optimal rate of [LOCC](#local-operations-and-classical-communication) conversion with vanishing output error is the ratio of their entanglement entropies. Here vanishing error means that the [trace distance](density-matrix.md#trace-distance) between the output and $|\phi\rangle\langle\phi|^{\otimes m}$ tends to zero; a recorded failure probability must also tend to zero. [Entanglement concentration](#entanglement-concentration) first provides $nS(\rho_A^\psi)-o(n)$ [Bell pairs](#bell-pair), and [entanglement dilution](#entanglement-dilution) needs $mS(\rho_A^\phi)+o(m)$ such pairs. This achieves the ratio. Conversely, refine the output into pure branches. [Average monotonicity of pure-state entanglement entropy](von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy) bounds their average entropy by the input entropy; [continuity bound for quantum conditional entropy](von-neumann-entropy.md#continuity-bound-for-quantum-conditional-entropy), with trivial conditioning, makes the output entropy loss per target tend to zero. This forbids a larger rate. The convention permits approximations for finite blocks: exact deterministic conversion of every finite block can obey stricter [majorization](vector-space.md#majorization) constraints. The reversible concentration construction is given in the [original concentration paper](https://arxiv.org/abs/quant-ph/9511030).

#### Collective advantage over independent two-qubit filtering

↑ **Parent:** [Asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate)

For two-qubit pure states with smaller squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) $s<t$, [optimal stochastic conversion of a two-qubit pure state](#optimal-stochastic-conversion-of-a-two-qubit-pure-state) succeeds independently with probability $s/t$. The [asymptotic pure-state entanglement conversion rate](#asymptotic-pure-state-entanglement-conversion-rate) of collective [LOCC](#local-operations-and-classical-communication) is instead $h_2(s)/h_2(t)$, where $h_2$ is [binary entropy](information-entropy.md#binary-entropy). The difference is strict: differentiating gives $\frac{d}{dx}[h_2(x)/x]=\log_2(1-x)/x^2<0$. Hence $h_2(s)/s>h_2(t)/t$. Independent filtering loses entanglement in its product-state failure branches, whereas collective concentration and dilution preserve entanglement asymptotically.

### Optimal stochastic conversion of a two-qubit pure state

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Write a source and target in [Schmidt decomposition](von-neumann-entropy.md#schmidt-decomposition) with squared coefficients $(1-s,s)$ and $(1-t,t)$, where $0<s,t\leq1/2$. If $s\geq t$, [Nielsen's pure-state conversion theorem](#nielsen-s-pure-state-conversion-theorem) allows deterministic conversion. If $s<t$, the [Schmidt-tail entanglement monotone](#schmidt-tail-entanglement-monotone) gives $p\leq s/t$. Alice attains this bound with a local two-outcome [quantum measurement](quantum-measurement.md) whose success [Kraus operator](quantum-information-theory.md#kraus-operator) is $K_s=\operatorname{diag}(\sqrt{s(1-t)/(t(1-s))},1)$ and whose failure operator is $K_f=\operatorname{diag}(\sqrt{1-s(1-t)/(t(1-s))},0)$. They obey $K_s^\dagger K_s+K_f^\dagger K_f=I$. The successful unnormalized state is $\sqrt{s/t}$ times the target, and failure leaves a [product state](#product-state). A classical message tells Bob which branch occurred. Known local changes of Schmidt bases allow the same protocol for arbitrary two-qubit pure states with these coefficients.

### Local unitary operation

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

An operation that applies a [unitary operator](vector-space.md#unitary-operator) to one party's subsystem and the identity to the other is a local unitary operation. Several separated parties may each apply a known unitary, resulting in a product of their local unitaries. Such operations preserve the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) across the relevant bipartition.

#### Local-unitary equivalence

↑ **Parent:** [Local unitary operation](#local-unitary-operation)

Two bipartite [pure states](quantum-theory.md#pure-state) on fixed subsystem spaces are [local-unitary equivalent](#local-unitary-equivalence) when related by the displayed product of [unitary operators](vector-space.md#unitary-operator). [Identity operators](vector-space.md#identity-operator) give [reflexivity](set-theory.md#reflexive-relation), inverse operators give symmetry, and products of local operators give [transitivity](set-theory.md#transitive-relation). Thus this is an [equivalence relation](set-theory.md#equivalence-relation), whose classes are the orbits under local unitaries.

Every pair of normalized [product states](#product-state) is [local-unitary equivalent](#local-unitary-equivalence): extend each factor to an [orthonormal basis](inner-product.md#orthonormal-basis) and use a [unitary operator](vector-space.md#unitary-operator) carrying one [basis](vector-space.md#basis) to the other. Local operators preserve a product factorization, and their inverses do too, so [quantum entanglement](#entangled-state) cannot be created or removed this way. More generally, the [tensor-product coefficient matrix](multilinear-algebra.md#tensor-product-coefficient-matrix) changes as $C\mapsto UCV^T$, which preserves its [singular values](linear-algebra.md#singular-value) and therefore its [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient). The transpose on the second factor is ordinary, not a [conjugate transpose](linear-operator-theory.md#conjugate-transpose), because coefficients of a [tensor product](multilinear-algebra.md#tensor-product) depend bilinearly on the two input [vectors](vector-space.md#vector).

#### Local-unitary invariance of entanglement entropy

↑ **Parent:** [Local unitary operation](#local-unitary-operation)

A local unitary sends a [reduced density matrix](#reduced-density-matrix) to a unitary conjugate on the acted-on subsystem and leaves the other subsystem unchanged. Its [eigenvalues](linear-operator-theory.md#eigenvalue) and von Neumann entropy therefore do not change. This distinguishes a deterministic change of local basis from a selective measurement or nonunitary local filter.

#### Local-unitary invariance of reduced-state spectra

↑ **Parent:** [Local unitary operation](#local-unitary-operation)

Under a product [unitary operator](vector-space.md#unitary-operator) $U_A\otimes U_B$, the [reduced density matrix](#reduced-density-matrix) of $A$ becomes $U_A\rho_AU_A^\dagger$. The unitary on $B$ cancels under the [partial trace](quantum-theory.md#partial-trace). Unitary conjugation preserves [eigenvalues](linear-operator-theory.md#eigenvalue), so the squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) of a bipartite [pure state](quantum-theory.md#pure-state) are unchanged. Conversely, two normalized bipartite pure states with the same squared Schmidt coefficients, including multiplicities and zero padding, have [Schmidt decompositions](von-neumann-entropy.md#schmidt-decomposition) carried into each other by local unitaries mapping their Schmidt bases. Thus reduced-state spectra completely classify bipartite pure states up to local unitary operations.

<h3 id="nielsen-s-pure-state-conversion-theorem">Nielsen's pure-state conversion theorem</h3>

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

An exact deterministic [LOCC](#local-operations-and-classical-communication) conversion of a bipartite pure state to another is possible exactly when the input vector of squared [Schmidt coefficients](von-neumann-entropy.md#schmidt-coefficient) is majorized by the output vector. Sort the two probability vectors decreasingly and pad with zeros to a common length before applying [majorization](vector-space.md#majorization). A maximally entangled state may therefore be converted to a product state, while the reverse conversion is forbidden. The criterion does not assert conversion by postselection or with a catalyst.

### LOCC discrimination of two Bell states

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)

Two parties can distinguish $|\Phi^+\rangle$ from $|\Phi^-\rangle$ by both measuring in the Hadamard basis and comparing outcomes: equal outcomes identify $|\Phi^+\rangle$, while unequal outcomes identify $|\Phi^-\rangle$.

### Quantum teleportation

↑ **Parent:** [Local operations and classical communication](#local-operations-and-classical-communication)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_teleportation)

Quantum teleportation transfers an unknown qubit using one shared Bell pair, a Bell-basis measurement by the sender, two classical bits, and a Pauli correction by the receiver.

#### Controlled quantum teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A [quantum teleportation](#quantum-teleportation) protocol in which a further participant supplies a resource or classical measurement record needed for exact reconstruction of an arbitrary unknown input at the receiver. Without that cooperation, some classical information about the input may remain accessible; control need not mean complete information-theoretic concealment.

##### GHZ-assisted quantum teleportation

↑ **Parent:** [Controlled quantum teleportation](#controlled-quantum-teleportation)

Share a [GHZ state](quantum-theory.md#greenberger-horne-zeilinger-state) on $A,B,C$ and let the unknown input $Q$ be $|\chi\rangle$. Alice applies CNOT from $Q$ to $A$, then a [Hadamard gate](quantum-theory.md#hadamard-gate) to $Q$, and measures $Q,A$ computationally, giving $s,t$. Charlie measures $C$ in the [Hadamard basis](quantum-theory.md#hadamard-basis), giving $c$. Bob's conditional state is

$$
X^tZ^{s\oplus c}|\chi\rangle,
$$

up to a [global phase](quantum-system.md#global-phase). Alice's two [bits](information-theory.md#bit) and Charlie's one [bit](information-theory.md#bit) therefore specify Bob's inverse correction $Z^{s\oplus c}X^t$.

To prove the phase rule, write $|\chi\rangle=\alpha|0\rangle+\beta|1\rangle$. After Alice's result, $BC$ is $\alpha|tt\rangle+(-1)^s\beta|(1\oplus t)(1\oplus t)\rangle$. Taking Charlie's [Hadamard basis](quantum-theory.md#hadamard-basis) partial [inner product](inner-product.md) multiplies its second term relative to its first by $(-1)^c$. The remaining common phase is $(-1)^{ct}$, which is physically irrelevant. All eight result triples have [probability](probability-theory.md#probability) $1/8$. Charlie's record localizes a known-phase [Bell pair](#bell-pair), allowing the standard [Bell-basis teleportation identity](#bell-basis-teleportation-identity) to complete the transfer.

#### Classical communication lower bound for exact qubit teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Exact [quantum teleportation](#quantum-teleportation) that preserves an arbitrary reference requires at least two classical [bits](information-theory.md#bit) from sender to receiver, even with preshared [quantum entanglement](#entangled-state). For the essential reduction, encode two classical [bits](information-theory.md#bit) in the four [Bell states](bell-state.md) by [Pauli gates](quantum-circuit.md#pauli-gate) on the sender's half of a [Bell pair](#bell-pair). [Teleportation as an identity channel on a reference](#teleportation-as-an-identity-channel-on-a-reference) transfers this half while preserving the encoding. The receiver then has both halves and recovers both [bits](information-theory.md#bit) by a [Bell-basis measurement](#bell-basis-measurement), as in [superdense coding](#superdense-coding).

The classical [bit](information-theory.md#bit) bound itself has a short [no-communication theorem](#no-communication-theorem) proof. For $N$ possible messages and $K$ possible classical transmissions, let $\sigma_{m,c}$ be the receiver's subnormalized conditional [density matrix](density-matrix.md) before decoding. The [no-communication theorem](#no-communication-theorem) gives $\sum_c\sigma_{m,c}=\tau$, independent of $m$, so $0\leq\sigma_{m,c}\leq\tau$. For each transmission $c$, let $\{E_{m|c}\}_m$ be the decoding [POVM](quantum-measurement.md#positive-operator-valued-measure). Averaging over equiprobable messages,

$$
p_{\mathrm{success}}=\frac1N\sum_{m,c}\operatorname{Tr}(E_{m|c}\sigma_{m,c})
\leq\frac1N\sum_c\operatorname{Tr}\left(\sum_m E_{m|c}\tau\right)=\frac KN.
$$

Perfect decoding of four messages requires $K\geq4$, hence at least two classical [bits](information-theory.md#bit). This applies to the preshared resources of the proposed [quantum teleportation](#quantum-teleportation) protocol as well as the [Bell pair](#bell-pair) used for the encoding.

#### Teleportation with an ambiguous Bell-state phase label

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Suppose a perfect $|\phi^+\rangle$ [Bell pair](#bell-pair) is used for [quantum teleportation](#quantum-teleportation), but the sender cannot distinguish the $\phi^+$ and $\phi^-$ [Bell-basis measurement](#bell-basis-measurement) outcomes and guesses their labels uniformly. Each of the four actual outcomes has [probability](probability-theory.md#probability) $1/4$. Either ambiguous outcome gives an incorrect [Pauli Z gate](quantum-theory.md#pauli-z-gate) correction with conditional [probability](probability-theory.md#probability) $1/2$, so the total phase-flip [probability](probability-theory.md#probability) is $1/4$. The unconditional output is therefore the displayed [phase-flip channel](quantum-information-theory.md#phase-flip-channel). For $|\psi\rangle=\alpha|0\rangle+\beta|1\rangle$, its [teleportation fidelity](#teleportation-fidelity) is $\langle\psi|\mathcal E(|\psi\rangle\langle\psi|)|\psi\rangle=1-|\alpha|^2|\beta|^2$. It ranges from $3/4$ on the [Bloch sphere](density-matrix.md#bloch-sphere) equator to $1$ at its poles. This averages the output [density operators](density-matrix.md), including the ambiguous rounds.

#### Bit-flipped Bell resource teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Distributing one half of $|\Phi^+\rangle$ through a [quantum bit-flip channel](quantum-information-theory.md#quantum-bit-flip-channel) produces $p\Pi_{\Phi^+}+(1-p)\Pi_{\Psi^+}$. Ideal [quantum teleportation](#quantum-teleportation) with error-free classical correction bits induces the same bit-flip map on the input: conjugating the resource error by any [Pauli gate](quantum-circuit.md#pauli-gate) correction changes at most its sign. For a pure target the squared [quantum fidelity](quantum-information-theory.md#fidelity-of-quantum-states) is $p+(1-p)|\langle X\rangle|^2$. This describes noise in resource distribution, not a perfect resource supplied by an independent channel.

#### Bouwmeester quantum teleportation experiment

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

[Dik Bouwmeester](quantum-mechanics-physicist.md#dirk-bouwmeester) and colleagues demonstrated selected-outcome photon-polarization [quantum teleportation](#quantum-teleportation). An ultraviolet pump traversed a nonlinear crystal twice: one passage supplied an entangled pair, the other the input [photon](quantum-mechanics.md#photon) and its trigger partner. The input and one resource [photon](quantum-mechanics.md#photon) interfered at a beam splitter; output-detector coincidences selected their antisymmetric [Bell state](bell-state.md). Narrow filters made their coherence time exceed the pump duration, preserving temporal indistinguishability.

The reported pump pulses were $200\,\mathrm{fs}$ long at $76\,\mathrm{MHz}$; $788\,\mathrm{nm}$ [photons](quantum-mechanics.md#photon) filtered to $4\,\mathrm{nm}$ bandwidth had a quoted $520\,\mathrm{fs}$ coherence time. A [polarization](wave.md#polarization-waves) analyzer measured the remote output. Trigger-conditioned fourfold coincidences excluded a double-pair background without subtraction. The selected Bell result had ideal [probability](probability-theory.md#probability) $1/4$; this demonstration did not distinguish and actively correct all four outcomes.[pp. 576–578, Figures 1, 4 and 5: source, filters, Bell analyzer and background control](physics-bibliography.md#experimental-quantum-teleportation-by-dik-bouwmeester-and-others)

#### Teleportation fidelity

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

For a pure input target $|\psi\rangle$ and normalized output [density operator](density-matrix.md) $\rho_{\rm out}$, the displayed squared [quantum fidelity](quantum-information-theory.md#fidelity-of-quantum-states) measures how well a teleportation channel reproduces that target. A mean value additionally specifies the input ensemble and whether it is conditioned on success. Detection efficiency, conditional fidelity, heralding and overall success [probability](probability-theory.md#probability) are distinct experimental quantities.

#### Dicke-resource telecloning

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

For odd $n=2k+1$, a symmetric [quantum teleportation](#quantum-teleportation) resource can encode an unknown [qubit](quantum-system.md#qubit) into $E(\alpha|0\rangle+\beta|1\rangle)=\alpha|D_k^n\rangle+\beta|D_{k+1}^n\rangle$. Begin with $|D_{k+1}^{n+1}\rangle$, apply a [controlled-NOT gate](quantum-theory.md#controlled-not-gate) from the input to the sender's resource qubit, apply a [Pauli X gate](quantum-theory.md#pauli-x-gate) to that resource qubit and a [Hadamard gate](quantum-theory.md#hadamard-gate) to the input, and measure those two qubits. The four unnormalized remaining vectors are $E|\psi\rangle/2$, $EX|\psi\rangle/2$, $EZ|\psi\rangle/2$ and $EXZ|\psi\rangle/2$. Each outcome has probability $1/4$. Since $X^{\otimes n}$ interchanges $|D_k^n\rangle$ and $|D_{k+1}^n\rangle$, and $Z^{\otimes n}$ acts as logical $Z$ up to the common phase $(-1)^k$, local Pauli corrections make the output independent of the result. The [one-qubit reduction of Dicke-state superpositions](quantum-system.md#one-qubit-reduction-of-dicke-state-superpositions) gives

$$
\rho=\frac1n\begin{pmatrix}k+|\alpha|^2&(k+1)\alpha\beta^*\\(k+1)\alpha^*\beta&k+|\beta|^2\end{pmatrix},\qquad \langle\psi|\rho|\psi\rangle=\frac{k+1+2k|\alpha|^2|\beta|^2}{n}.
$$

For $n>1$ this distributes imperfect copies, as required by the [no-cloning theorem](quantum-theory.md#no-cloning-theorem). For $n=1$ it reduces to exact [quantum teleportation](#quantum-teleportation).

#### Exact teleportation resource criterion

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A shared resource enables deterministic exact transmission of an arbitrary unknown [qubit](quantum-system.md#qubit) using only [local operations and classical communication](#local-operations-and-classical-communication) if and only if it can produce a shared [Bell pair](#bell-pair) deterministically by such operations. Sufficiency follows from [quantum teleportation](#quantum-teleportation). For necessity, prepare a Bell pair locally at the sender and apply the purported transmission protocol to one half: exact identity-channel action leaves a shared Bell pair between the retained reference and the receiver. A separable shared resource cannot satisfy this condition because local operations and classical communication preserve separability.

#### Entanglement swapping

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_swapping)

Two initial maximally entangled pairs $AB_1$ and $B_2C$ can be turned into an entangled pair $AC$ by a [generalized Bell basis](quantum-theory.md#generalized-bell-basis) measurement on $B_1B_2$, followed by a local correction at an endpoint using its classical label. This is [qudit teleportation](#qudit-teleportation) of $B_1$, including its correlations with $A$, to $C$. The initial two pairs are consumed. Without the classical label, averaging the conditional endpoint states need not leave entanglement.

##### Identical-resource entanglement swapping

↑ **Parent:** [Entanglement swapping](#entanglement-swapping)

Take two identical normalized entangled qubit pairs $\sum_{r=0}^1b_r|\xi_r\eta_r\rangle$. Project their two $\eta$ systems onto $|\Phi\rangle=2^{-1/2}\sum_k|\eta_k\eta_k\rangle$. The overlap with $|\eta_r\eta_s\rangle$ is $\delta_{rs}/\sqrt2$, so the unnormalized remote state is $\sum_rb_r^2|\xi_r\xi_r\rangle/\sqrt2$. Its squared norm gives success probability $\tfrac12\sum_r|b_r|^4$, and its normalized Schmidt coefficients are $b_r^2/(\sum_s|b_s|^4)^{1/2}$. At least two survive whenever the original pair was entangled. This is a conditional [entanglement swapping](#entanglement-swapping) result; disregarding the local measurement outcome leaves the remote reduced state unchanged. The coefficients are squared amplitudes, not their absolute squares, because the two input kets multiply before the Bell-state contraction.

##### Heralded Bell-pair projection with two polarization parity filters

↑ **Parent:** [Entanglement swapping](#entanglement-swapping)

Start from three normalized [Bell states](bell-state.md) $\Phi^+_{12}\Phi^+_{34}\Phi^+_{56}$. A [polarizing beam splitter](optical-instrument.md#polarizing-beam-splitter) parity filter $\Pi_Z^{25}$ followed by $X$-basis outcome $++$, and a second filter $\Pi_X^{46}$ followed by $Z$-basis outcome $00$, have effective bras $\langle\Phi^+|_{25}/\sqrt2$ and $\langle\Phi^+|_{46}/\sqrt2$. Their contraction leaves $\Phi^+_{13}/8$. The herald [probability](probability-theory.md#probability) is therefore $1/64$ per ideal three-pair input, or $1/16$ conditional on both parity-routing filters having succeeded. This distinction prevents renormalizing away the optical [postselection](quantum-measurement.md#postselection) cost.

##### Bell swapping visibility under random labels

↑ **Parent:** [Entanglement swapping](#entanglement-swapping)

Suppose independent resource pairs have [density matrices](density-matrix.md) $v_j|\Phi^+\rangle\langle\Phi^+|+(1-v_j)I_4/4$. An ideal complete [Bell-basis measurement](#bell-basis-measurement), followed by outcome-dependent [Pauli gates](quantum-circuit.md#pauli-gate), produces a chosen [Bell state](bell-state.md) with white-noise visibility $v_1v_2$: either white-noise input makes the remote pair maximally mixed. If the reported label is reliable with probability $q$ and otherwise uniformly random, averaging the erroneous corrections makes that branch maximally mixed too, so $v_{\rm out}=v_1v_2q$. A second independent detector of the same quality during [quantum teleportation](#quantum-teleportation) adds another factor $q$ to the teleported [Bloch vector](density-matrix.md#bloch-vector).

#### Qudit teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A sender and receiver share $n^{-1/2}\sum_j|j j\rangle$. The sender measures the input and their resource half in the [generalized Bell basis](quantum-theory.md#generalized-bell-basis). Outcome $(r,s)$ gives the receiver $X^sZ^{-r}|\chi\rangle/n$, with probability $1/n^2$. After [classical communication](quantum-information-theory.md#classical-communication) of the outcome, the correction $Z^rX^{-s}$ restores the unknown [quantum state](quantum-system.md#quantum-state). The same calculation preserves correlations with a reference, as in [teleportation as an identity channel on a reference](#teleportation-as-an-identity-channel-on-a-reference).

#### Teleportation as an identity channel on a reference

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Ideal corrected [quantum teleportation](#quantum-teleportation) transfers an input system to the receiver while preserving its entire joint [density operator](density-matrix.md) with an arbitrary reference. Expand a joint [pure state](quantum-theory.md#pure-state) as $\sum_j|j\rangle|r_j\rangle$. Every teleportation branch acts with the same known correction on each system basis vector and does nothing to the reference vectors; undoing that correction restores the complete sum. Linearity extends the result to mixed states. The sender's measured carrier no longer retains the original reference correlations.

#### One-bit teleportation

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

Apply a [Controlled-Z gate](quantum-theory.md#controlled-z-gate) to input $a|0\rangle+b|1\rangle$ and a fresh $|+\rangle$ [quantum ancilla](quantum-information-theory.md#quantum-ancilla). Measuring the input in the [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) basis at angle $\alpha$, with outcome $s$, leaves the unnormalized output

$$
\frac1{\sqrt2}\left(a|+\rangle+(-1)^se^{i\alpha}b|-\rangle\right)=\frac1{\sqrt2}X^sJ(\alpha)|\psi\rangle.
$$

Each branch has [probability](probability-theory.md#probability) $1/2$, independently of the input. The logical output is $J(\alpha)|\psi\rangle$ with known [Pauli frame](quantum-circuit.md#pauli-frame) $X^s$; the input [qubit](quantum-system.md#qubit) has been measured, so this does not clone it.

##### Pauli-frame propagation along a measurement wire

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

With [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) vectors $(|0\rangle+(-1)^s e^{i\eta}|1\rangle)/\sqrt2$, the gate in [one-bit teleportation](#one-bit-teleportation) is $U(\eta)=H\operatorname{diag}(1,e^{-i\eta})=J(-\eta)$. Direct multiplication gives $U(\eta)Z=XU(\eta)$ and $U(\eta)X=e^{-i\eta}ZU(-\eta)$. Moving a [Pauli frame](quantum-circuit.md#pauli-frame) through this gate therefore exchanges its $X$ and $Z$ exponents and reverses the angle if the old $X$ exponent is one, as displayed up to [global phase](quantum-system.md#global-phase). A measurement outcome $s$ adds a further $X^s$ factor. This calculation supplies adaptive angle choices and the final classical output-bit correction of a linear [cluster state](topological-quantum-matter.md#cluster-state) computation.

##### Graph-state preparation of a computational-basis input

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

A two-vertex [graph state](quantum-circuit.md#graph-state) starts with two $|+\rangle$ states joined by a [Controlled-Z gate](quantum-theory.md#controlled-z-gate). Measuring the first vertex in the $X$ basis leaves the second in $X^sH|+\rangle=X^s|0\rangle$, where $s$ is the measurement outcome. Thus a known zero input can be supplied to a measurement wire using only a graph-state resource and a known [Pauli frame](quantum-circuit.md#pauli-frame). This preparation link precedes the links implementing the desired logical [J gate](#j-gate-in-measurement-based-quantum-computation); later measurement angles and output-bit corrections absorb its byproduct.

##### Heralded Pauli X correction using controlled-Z and measurements

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

Two angle-zero [one-bit teleportations](#one-bit-teleportation) with outcomes $p,q$ implement $X^qH X^pH=X^qZ^p$ on an arbitrary input, up to [global phase](quantum-system.md#global-phase). A [Controlled-Z gate](quantum-theory.md#controlled-z-gate) with a fixed $|1\rangle$ [quantum ancilla](quantum-information-theory.md#quantum-ancilla) implements $Z$, so $Z^p$ removes the known $Z$ factor. The result is $X^q$ up to phase. With probability one half the desired [Pauli X gate](quantum-theory.md#pauli-x-gate) is applied; otherwise the input is unchanged. Repeating until $q=1$ gives an exact heralded correction with two attempts on average and almost-sure termination. It has no finite worst-case measurement count. A [Pauli frame](quantum-circuit.md#pauli-frame) avoids this repeat-until-success procedure when only logical action or classical output statistics are required.

##### J gate in measurement-based quantum computation

↑ **Parent:** [One-bit teleportation](#one-bit-teleportation)

For the printed equatorial-basis convention,

$$
J(\alpha)=\frac1{\sqrt2}\begin{pmatrix}1&e^{i\alpha}\\1&-e^{i\alpha}\end{pmatrix}=H\operatorname{diag}(1,e^{i\alpha}).
$$

It is the [Hadamard gate](quantum-theory.md#hadamard-gate) after a [phase gate](quantum-theory.md#phase-gate). The identities $J(\alpha)Z=XJ(\alpha)$ and $J(\alpha)X=e^{i\alpha}ZJ(-\alpha)$ follow by multiplying their matrices. For $\alpha=0,\pi/2$ these are [Clifford gates](quantum-circuit.md#clifford-gate). In particular $J(-\pi/2)=XJ(\pi/2)$, permitting a sign change of the measurement angle to be absorbed into a [Pauli frame](quantum-circuit.md#pauli-frame).

###### J-gate phase-error operator norm

↑ **Parent:** [J gate in measurement-based quantum computation](#j-gate-in-measurement-based-quantum-computation)

The [J gate](#j-gate-in-measurement-based-quantum-computation) is $J(\alpha)=HP(\alpha)$, where $P(\alpha)=\operatorname{diag}(1,e^{i\alpha})$: the [phase gate](quantum-theory.md#phase-gate) acts first and the [Hadamard gate](quantum-theory.md#hadamard-gate) acts second. Unitary invariance of the [operator norm](continuous-dual-space.md#operator-norm) reduces its angle error to the single nonzero diagonal difference of the [phase gate](quantum-theory.md#phase-gate). Its norm is $|e^{i\delta}-1|=2|\sin(\delta/2)|\leq|\delta|$. The [quantum circuit gate-error telescoping bound](quantum-circuit.md#quantum-circuit-gate-error-telescoping-bound) then makes an angle tolerance of $\epsilon/k$ sufficient for $k$ such imperfect gates and exact other gates.

#### Bell-basis teleportation identity

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

For $|\beta_{xz}\rangle=(Z^zX^x\otimes I)|\beta_{00}\rangle$, an arbitrary qubit obeys

$$
|\alpha\rangle_C|\beta_{00}\rangle_{AB}
=\frac12\sum_{x,z\in\{0,1\}}
|\beta_{xz}\rangle_{CA}X^xZ^z|\alpha\rangle_B.
$$

A Bell-basis measurement reveals $(x,z)$, after which the receiver applies the inverse Pauli correction.

#### No-programming theorem

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

A deterministic finite-dimensional universal programmable quantum gate cannot implement every unitary exactly: programs for physically distinct unitaries would have to be mutually orthogonal, but a finite-dimensional program register contains only finitely many mutually orthogonal states.

This is a restriction on programmable [quantum circuits](quantum-circuit.md) and their [unitary operators](vector-space.md#unitary-operator), rather than a statement about the existence of classical program descriptions.

#### Teleportation with the psi-plus Bell state

↑ **Parent:** [Quantum teleportation](#quantum-teleportation)

When the shared resource is $|\Psi^+\rangle$, Bell outcomes $\Phi^+,\Phi^-,\Psi^+,\Psi^-$ leave the receiver with $X|\alpha\rangle,XZ|\alpha\rangle,|\alpha\rangle,Z|\alpha\rangle$, respectively, up to global phases.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (139)

- [Bell basis](quantum-theory.md#bell-basis)
- [Bell-basis conversion circuit](quantum-theory.md#bell-basis-conversion-circuit)
- [Bell-basis measurement](#bell-basis-measurement)
- [Bell correlations versus a classical mixture](quantum-information-theory.md#bell-correlations-versus-a-classical-mixture)
- [Bell-label Hamming distance and bit errors](#bell-label-hamming-distance-and-bit-errors)
- [Bell pair](#bell-pair)
- [Bell state analyzer](#bell-state-analyzer)
- [Bell-state nondemolition measurement](#bell-state-nondemolition-measurement)
- [Bell swapping visibility under random labels](#bell-swapping-visibility-under-random-labels)
- [Bell twirling followed by triplet symmetrization](density-matrix.md#bell-twirling-followed-by-triplet-symmetrization)
- [Bipartite quantum system](quantum-mechanics.md#bipartite-quantum-system)
- [Bouwmeester quantum teleportation experiment](#bouwmeester-quantum-teleportation-experiment)
- [CHSH Tsirelson bound](foundations-of-quantum-mechanics.md#chsh-tsirelson-bound)
- [Classical communication lower bound for exact qubit teleportation](#classical-communication-lower-bound-for-exact-qubit-teleportation)
- [Computational-basis intercept-resend attack](computer-science.md#computational-basis-intercept-resend-attack)
- [Coplanar qubit realization of the chained Bell inequality](foundations-of-quantum-mechanics.md#coplanar-qubit-realization-of-the-chained-bell-inequality)
- [Deterministic two-qubit entanglement dilution](#deterministic-two-qubit-entanglement-dilution)
- [Entanglement-assisted discrimination of a Pauli basis](quantum-information-theory.md#entanglement-assisted-discrimination-of-a-pauli-basis)
- [Entanglement-assisted nondemolition parity measurement](quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement)
- [Entangling gate](quantum-circuit.md#entangling-gate)
- [Generalized Bell state](quantum-theory.md#generalized-bell-state)
- [Global cloning fidelity](quantum-theory.md#global-cloning-fidelity)
- [Heralded Bell-pair projection with two polarization parity filters](#heralded-bell-pair-projection-with-two-polarization-parity-filters)
- [Local flag correction of a Bell-state phase mixture](#local-flag-correction-of-a-bell-state-phase-mixture)
- [Localizing a Bell pair from a GHZ state](quantum-theory.md#localizing-a-bell-pair-from-a-ghz-state)
- [LOCC discrimination of four Bell states using two copies](quantum-theory.md#locc-discrimination-of-four-bell-states-using-two-copies)
- [One-bit remote preparation of real qubit states](quantum-information-theory.md#one-bit-remote-preparation-of-real-qubit-states)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/quantum-information.md#1/f/i/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/quantum-information.md#2/d/ii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/quantum-information.md#3/a/ii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#1/c/i/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#1/c/ii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#1/d/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#2/b/ii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#3/c/ii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/quantum-information.md#3/d/i/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information.md#1/b/i/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information.md#2/b/iii/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information.md#3/b/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/quantum-information.md#3/d/iii/solution)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2017.md#3/e/solution)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2021.md#2/a/solution)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2021.md#2/b/solution)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2021.md#3/c/iv/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8.md#7/1/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8.md#7/2/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8.md#7/a/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8.md#7/b/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2005/7-and-8.md#8/2/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/7.md#1/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2006/7.md#3/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2008/8.md#2/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2009/8.md#1/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/8.md#1/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/8.md#2/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2015.md#7/b/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2015.md#8/a/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2015.md#8/c/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2017.md#4/a/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2017.md#4/d/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2017.md#5/b/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2019.md#6/c/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021.md#5/a/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021.md#6/c/solution)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2021.md#6/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-58.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-50.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/a/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/a/4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-66.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57.md#3/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323.md#3/iii/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#10d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#10c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#10c/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#15d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323.md#1/b/i/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323.md#4/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1.md#10d/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#10d/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#15d/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#15d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4.md#10d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#10e/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3.md#10e/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2.md#35a/e/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1.md#section-c/c10/solution)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2016/paper-1.md#1/solution)
- [Solution](past-exam-of-the-quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford/2009.md#b/6/solution)
- [Solution](past-exam-of-the-quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford/2010.md#b/6/solution)
- [Solution](past-exam-of-the-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford/2009.md#3/solution)
- [Solution](past-exam-of-the-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford/2010.md#3/solution)
- [Solution](past-exam-of-the-short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford/2015.md#s3/3/4/solution)
- [Perfect two-basis discrimination would allow superluminal signalling](quantum-theory.md#perfect-two-basis-discrimination-would-allow-superluminal-signalling)
- [Polarization CHSH count model](foundations-of-quantum-mechanics.md#polarization-chsh-count-model)
- [Polarization correlations of the Psi-plus Bell state](#polarization-correlations-of-the-psi-plus-bell-state)
- [Polarization entanglement](#polarization-entanglement)
- [Quantum information theory](quantum-information-theory.md)
- [Qubit transpose map](quantum-information-theory.md#qubit-transpose-map)
- [Reflected real-basis CHSH strategy](foundations-of-quantum-mechanics.md#reflected-real-basis-chsh-strategy)
- [Remote preparation in conjugate bases](quantum-theory.md#remote-preparation-in-conjugate-bases)
- [Single-local-gate Bell readout information](#single-local-gate-bell-readout-information)
- [Superdense coding](#superdense-coding)
- [Two excited atoms in a resonant Tavis-Cummings mode](tensor-product-of-quantum-systems.md#two-excited-atoms-in-a-resonant-tavis-cummings-mode)
- [Two-outcome LOCC dilution of a Bell pair](#two-outcome-locc-dilution-of-a-bell-pair)
- [Two-pair component of polarization-entangled down-conversion](optics.md#two-pair-component-of-polarization-entangled-down-conversion)
- [Two-qubit Werner state](density-matrix.md#two-qubit-werner-state)
- [Universal NOT gate](quantum-information-theory.md#universal-not-gate)
