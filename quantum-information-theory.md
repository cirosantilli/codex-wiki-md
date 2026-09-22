# Quantum information theory

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_information_theory)

Quantum information theory studies information processing with quantum states, measurements, channels, entanglement, and quantum entropy.

**Table of contents**

- [Quantum random access code](#quantum-random-access-code)
  - [Optimal three-to-one qubit random access code](#optimal-three-to-one-qubit-random-access-code)
- [Classical communication](#classical-communication)
- [Remote state preparation](#remote-state-preparation)
  - [Asymptotic remote state preparation by block indexing](#asymptotic-remote-state-preparation-by-block-indexing)
  - [Heralded remote preparation of an arbitrary qubit](#heralded-remote-preparation-of-an-arbitrary-qubit)
    - [One-bit heralding of a remote state preparation block](#one-bit-heralding-of-a-remote-state-preparation-block)
  - [Two-bit remote state preparation on a graph-state path](#two-bit-remote-state-preparation-on-a-graph-state-path)
  - [One-bit remote preparation of real qubit states](#one-bit-remote-preparation-of-real-qubit-states)
- [Schumacher compression](#schumacher-compression)
  - [Memoryless quantum information source](#memoryless-quantum-information-source)
  - [Quantum typical subspace](#quantum-typical-subspace)
    - [Typical subspace theorem](#typical-subspace-theorem)
  - [Reliable quantum source compression](#reliable-quantum-source-compression)
    - [Typical-subspace compression with a failure flag](#typical-subspace-compression-with-a-failure-flag)
      - [Average pure-source fidelity after typical projection](#average-pure-source-fidelity-after-typical-projection)
    - [Finite-dimensional quantum compression converse](#finite-dimensional-quantum-compression-converse)
- [Classical-quantum state](#classical-quantum-state)
  - [Entropy of a classical-quantum state](#entropy-of-a-classical-quantum-state)
  - [Holevo quantity](#holevo-quantity)
    - [Holevo quantity under a quantum channel](#holevo-quantity-under-a-quantum-channel)
    - [Holevo's theorem](#holevo-s-theorem)
      - [One-shot classical-quantum coding converse](#one-shot-classical-quantum-coding-converse)
- [Measure-and-prepare channel](#measure-and-prepare-channel)
  - [Measurement channel](#measurement-channel)
    - [Conditional input ensemble after a local measurement](#conditional-input-ensemble-after-a-local-measurement)
- [Fidelity of quantum states](#fidelity-of-quantum-states)
  - [Pure-state trace distance and fidelity identity](#pure-state-trace-distance-and-fidelity-identity)
  - [Unitary invariance of trace distance and fidelity](#unitary-invariance-of-trace-distance-and-fidelity)
  - [Squared quantum fidelity](#squared-quantum-fidelity)
  - [Joint concavity of quantum fidelity](#joint-concavity-of-quantum-fidelity)
  - [Monotonicity of quantum fidelity under partial trace](#monotonicity-of-quantum-fidelity-under-partial-trace)
  - [Pure-state gentle measurement bound](#pure-state-gentle-measurement-bound)
- [Coherent information](#coherent-information)
  - [Mutual information and coherent information identity](#mutual-information-and-coherent-information-identity)
  - [Coherent information upper bound by input entropy](#coherent-information-upper-bound-by-input-entropy)
  - [Coherent information as an environment conditional entropy](#coherent-information-as-an-environment-conditional-entropy)
  - [Data-processing inequality for coherent information](#data-processing-inequality-for-coherent-information)
  - [Anti-degradable quantum channel](#anti-degradable-quantum-channel)
- [Joint convexity of quantum relative entropy](#joint-convexity-of-quantum-relative-entropy)
- [Quantum ancilla](#quantum-ancilla)
  - [Ancilla qubit](#ancilla-qubit)
- [Positive linear map](#positive-linear-map)
  - [Positivity (linear maps)](#positivity-linear-maps)
  - [Decomposable positive map](#decomposable-positive-map)
    - [Størmer-Woronowicz decomposability theorem](#stormer-woronowicz-decomposability-theorem)
  - [k-reduction map](#k-reduction-map)
  - [Completely positive map](#completely-positive-map)
    - [Quantum operation](#quantum-operation)
    - [Stinespring representation of a completely positive map](#stinespring-representation-of-a-completely-positive-map)
    - [Kraus representation](#kraus-representation)
      - [Trace-preserving and unital Kraus conditions](#trace-preserving-and-unital-kraus-conditions)
      - [Kraus operator](#kraus-operator)
    - [Choi matrix](#choi-matrix)
      - [Spectral Kraus decomposition](#spectral-kraus-decomposition)
      - [Choi state](#choi-state)
      - [Choi reconstruction formula](#choi-reconstruction-formula)
    - [Quantum channel](#quantum-channel)
      - [Memoryless quantum channel](#memoryless-quantum-channel)
        - [Quantum erasure channel](#quantum-erasure-channel)
          - [Entanglement-assisted capacity of a quantum erasure channel](#entanglement-assisted-capacity-of-a-quantum-erasure-channel)
        - [Entanglement-assisted classical capacity](#entanglement-assisted-classical-capacity)
      - [Amplitude damping channel](#amplitude-damping-channel)
        - [Unitary dilation of amplitude damping](#unitary-dilation-of-amplitude-damping)
        - [Entanglement fidelity of amplitude damping](#entanglement-fidelity-of-amplitude-damping)
        - [Bloch-vector map of amplitude damping](#bloch-vector-map-of-amplitude-damping)
          - [Repeated amplitude damping limit](#repeated-amplitude-damping-limit)
      - [Holevo capacity](#holevo-capacity)
        - [Superadditivity of Holevo capacity](#superadditivity-of-holevo-capacity)
        - [Additivity of Holevo capacity](#additivity-of-holevo-capacity)
          - [Holevo-capacity additivity for entanglement-breaking channels](#holevo-capacity-additivity-for-entanglement-breaking-channels)
        - [Product-input classical-capacity converse](#product-input-classical-capacity-converse)
      - [Classical capacity of a quantum channel](#classical-capacity-of-a-quantum-channel)
        - [Holevo-Schumacher-Westmoreland theorem](#holevo-schumacher-westmoreland-theorem)
      - [Random unitary channel](#random-unitary-channel)
        - [Heisenberg-Weyl operator](#heisenberg-weyl-operator)
          - [Heisenberg-Weyl twirling channel](#heisenberg-weyl-twirling-channel)
        - [Pauli channel](#pauli-channel)
          - [Quantum bit-flip channel](#quantum-bit-flip-channel)
            - [Average pure-qubit fidelity of a bit-flip channel](#average-pure-qubit-fidelity-of-a-bit-flip-channel)
          - [Quantum depolarizing channel](#quantum-depolarizing-channel)
            - [Entanglement-assisted capacity of a qubit depolarizing channel](#entanglement-assisted-capacity-of-a-qubit-depolarizing-channel)
              - [High-noise capacity ratio for qubit depolarization](#high-noise-capacity-ratio-for-qubit-depolarization)
            - [Depolarizing noise weight above one](#depolarizing-noise-weight-above-one)
            - [Pauli-mixture parametrization of qubit depolarization](#pauli-mixture-parametrization-of-qubit-depolarization)
            - [Holevo capacity of a qubit depolarizing channel](#holevo-capacity-of-a-qubit-depolarizing-channel)
              - [Product-input block bound for a qubit depolarizing channel](#product-input-block-bound-for-a-qubit-depolarizing-channel)
          - [Phase-flip channel](#phase-flip-channel)
            - [Iterated phase-flip channel](#iterated-phase-flip-channel)
          - [Dephasing channel](#dephasing-channel)
            - [Complex environment overlap in qubit dephasing](#complex-environment-overlap-in-qubit-dephasing)
      - [Unital quantum channel](#unital-quantum-channel)
        - [Eigenvalue mixing matrix of a unital quantum channel](#eigenvalue-mixing-matrix-of-a-unital-quantum-channel)
          - [Spectral majorization under a unital quantum channel](#spectral-majorization-under-a-unital-quantum-channel)
        - [Werner–Holevo channel](#werner-holevo-channel)
      - [Strictly contractive quantum channel](#strictly-contractive-quantum-channel)
      - [Primitive quantum channel](#primitive-quantum-channel)
      - [Stinespring dilation](#stinespring-dilation)
      - [Entanglement fidelity](#entanglement-fidelity)
        - [Entanglement fidelity bound by state fidelity](#entanglement-fidelity-bound-by-state-fidelity)
        - [Quantum Fano inequality](#quantum-fano-inequality)
        - [Kraus formula for entanglement fidelity](#kraus-formula-for-entanglement-fidelity)
        - [Operation fidelity](#operation-fidelity)
      - [Lindblad equation](#lindblad-equation)
        - [Lindblad dissipator](#lindblad-dissipator)
        - [Lindblad operator](#lindblad-operator)
        - [Lindbladian](#lindbladian)
          - [Finite-dimensional Lindbladians have stationary states](#finite-dimensional-lindbladians-have-stationary-states)
          - [Lindbladian gap](#lindbladian-gap)
          - [Unique stationary state of a Lindbladian](#unique-stationary-state-of-a-lindbladian)
        - [Quantum Trajectory Theory](#quantum-trajectory-theory)
          - [Dark state of a Lindblad equation](#dark-state-of-a-lindblad-equation)
- [Quantum de Finetti theorem](#quantum-de-finetti-theorem)
  - [Mean-field ansatz from the quantum de Finetti theorem](#mean-field-ansatz-from-the-quantum-de-finetti-theorem)
- [Separable quantum state](#separable-quantum-state)
  - [Separable positive operator](#separable-positive-operator)
  - [Positive-map separability criterion](#positive-map-separability-criterion)
  - [Entanglement witness](#entanglement-witness)
  - [Partial transpose](#partial-transpose)
    - [Partial transpose of a maximally entangled projector](#partial-transpose-of-a-maximally-entangled-projector)
    - [Positive partial transpose](#positive-partial-transpose)
      - [PPT maximally entangled overlap bound](#ppt-maximally-entangled-overlap-bound)
    - [Trace-adjoint identity for partial transpose](#trace-adjoint-identity-for-partial-transpose)
  - [Positive partial transpose criterion](#positive-partial-transpose-criterion)
  - [Entanglement-breaking channel](#entanglement-breaking-channel)
    - [Separable Choi-state criterion for entanglement breaking](#separable-choi-state-criterion-for-entanglement-breaking)
    - [Rank-one Kraus representation of an entanglement-breaking channel](#rank-one-kraus-representation-of-an-entanglement-breaking-channel)
- [Isotropic quantum state](#isotropic-quantum-state)
- [Swap operator](#swap-operator)
- [Pretty good measurement](#pretty-good-measurement)
- [Quantum state discrimination](#quantum-state-discrimination)
- [Quantum binary hypothesis testing](#quantum-binary-hypothesis-testing)
  - [Binary test for quantum decoding success](#binary-test-for-quantum-decoding-success)
  - [Quantum channel discrimination](#quantum-channel-discrimination)
    - [Diamond norm of the transposition map](#diamond-norm-of-the-transposition-map)
  - [Holevo–Helstrom theorem](#holevo-helstrom-theorem)
    - [Equal-prior discrimination of qubit states](#equal-prior-discrimination-of-qubit-states)
- [Entanglement monogamy](#entanglement-monogamy)
  - [Coffman--Kundu--Wootters inequality](#coffman-kundu-wootters-inequality)
  - [Entanglement area law](#entanglement-area-law)
    - [Tensor-network area-law bound](#tensor-network-area-law-bound)
- [Werner state](#werner-state)
- [Ancilla bit](#ancilla-bit)

## Quantum random access code

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_random_access_code)

An encoding stores $n$ classical bits in $m$ [qubits](quantum-mechanics.md#qubit) so that a receiver who later chooses a bit index can recover that bit with a specified success probability. The sender cannot tailor the encoding to the unknown requested index. This task permits approximate recovery of any one bit rather than simultaneous recovery of all bits, and must specify whether additional communication, shared randomness, or [entanglement](bell-state.md#entangled-state) is allowed.

### Optimal three-to-one qubit random access code

↑ **Parent:** [Quantum random access code](#quantum-random-access-code)

Encode signs $s_j=(-1)^{b_j}$ by the unit [Bloch vector](quantum-theory.md#bloch-vector) $(s_1,s_2,s_3)/\sqrt3$. Perform the requested [Pauli measurement](quantum-theory.md#measurement-of-a-pauli-observable) and interpret a positive outcome as zero. Every input and index has success $p_*$. To prove optimality, write each binary-measurement difference as $D_j=t_jI+v_j\cdot\sigma$, where positivity gives $|v_j|\le1-|t_j|$. Averaging over all eight inputs cancels the $t_j$ terms. For any encoding vectors of norm at most one, the average success is at most $1/2+(1/48)\sum_s|\sum_js_jv_j|$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds the sum by $8\sqrt{\sum_j|v_j|^2}\le8\sqrt3$, proving the optimum even for mixed encodings and general binary measurements. The constant-success construction also maximizes worst-case success.

## Classical communication

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

Classical communication transmits a distinguishable classical record, such as measurement bits, between parties. In [quantum teleportation](bell-state.md#quantum-teleportation) it tells the receiver which local correction to apply. [Quantum no-signalling](quantum-theory.md#quantum-no-signalling) prevents shared [entanglement](bell-state.md#entangled-state) alone from transmitting the record. A classical message cannot propagate across a spacelike separation in a relativistic protocol.

## Remote state preparation

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

Remote state preparation uses a shared [entangled state](bell-state.md#entangled-state), local [measurement in quantum measurements](quantum-measurement.md) and classical communication to prepare a state known to the sender at the receiver. The sender can tailor the measurement to the desired state, so restricted state families can require less communication than [quantum teleportation](bell-state.md#quantum-teleportation). A real great-circle family of [qubit](quantum-mechanics.md#qubit) states admits [one-bit remote preparation of real qubit states](#one-bit-remote-preparation-of-real-qubit-states).

### Asymptotic remote state preparation by block indexing

↑ **Parent:** [Remote state preparation](#remote-state-preparation)

Prepare independent candidate blocks by [one-bit heralding of a remote state preparation block](#one-bit-heralding-of-a-remote-state-preparation-block), but send only the first successful block's index. Success eventually occurs with [probability](probability-theory.md#probability) one; a [prefix code for a rare geometric success](coding-theory.md#prefix-code-for-a-rare-geometric-success) uses at most $n+e/(e-1)$ expected [bits](information-theory.md#bit) per block. The expected [singlet state](quantum-mechanics.md#singlet-state) consumption is $n2^n$. Alternatively, limiting the number of trials to $n2^n$ gives failure [probability](probability-theory.md#probability) at most $e^{-n}$ and a fixed message length $n+\log_2n+O(1)$. Both versions approach one classical [bit](information-theory.md#bit) per remotely prepared [qubit](quantum-mechanics.md#qubit) in their respective expected-length or high-success senses.

// Target: quantum-theory.bigb

### Heralded remote preparation of an arbitrary qubit

↑ **Parent:** [Remote state preparation](#remote-state-preparation)

For a target [pure state](quantum-theory.md#pure-state) $|\psi\rangle$ of a [qubit](quantum-mechanics.md#qubit), choose its orthogonal complement so that

$$
|\Psi^-\rangle=\frac{|\psi\rangle|\psi^\perp\rangle-|\psi^\perp\rangle|\psi\rangle}{\sqrt2}.
$$

Measuring the sender's half of this [singlet state](quantum-mechanics.md#singlet-state) in that basis leaves the receiver in $|\psi\rangle$ when the sender obtains $|\psi^\perp\rangle$. The outcome has [probability](probability-theory.md#probability) one half. One classical success flag heralds the exact preparation without conveying the target's classical description.

// Target: quantum-theory.bigb

#### One-bit heralding of a remote state preparation block

↑ **Parent:** [Heralded remote preparation of an arbitrary qubit](#heralded-remote-preparation-of-an-arbitrary-qubit)

Apply [heralded remote preparation of an arbitrary qubit](#heralded-remote-preparation-of-an-arbitrary-qubit) independently to $n$ shared [singlet states](quantum-mechanics.md#singlet-state). The sender reports one [bit](information-theory.md#bit) indicating whether every local outcome was successful. A positive flag certifies that the receiver's block is the desired product of $n$ [pure states](quantum-theory.md#pure-state); its [probability](probability-theory.md#probability) is $2^{-n}$. A negative flag need not identify which states failed, since the whole block can be discarded.

// Target: algebra.bigb

### Two-bit remote state preparation on a graph-state path

↑ **Parent:** [Remote state preparation](#remote-state-preparation)

Alice holds the first two qubits and Bob the third of a [three-vertex graph-state wire](quantum-circuit.md#three-vertex-graph-state-wire). Alice measures at $\alpha$ and $(-1)^r\beta$, with outcomes $r,s$, and sends these two bits. Bob applies $Z^rX^s$, the inverse of the known [Pauli frame](quantum-circuit.md#pauli-frame) $X^sZ^r$, obtaining $U(\beta)U(\alpha)|+\rangle$ up to [global phase](quantum-mechanics.md#global-phase). Bob need not know the angles. Every branch succeeds, with branch probability $1/4$, and no postselection is needed. Alice's measurements and Bob's corrections constitute [local operations and classical communication](bell-state.md#local-operations-and-classical-communication) on the previously shared entangled resource.

### One-bit remote preparation of real qubit states

↑ **Parent:** [Remote state preparation](#remote-state-preparation)

For $|\alpha_\theta\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle$, Alice measures her half of a [Bell state](bell-state.md) in the real basis $\{|\alpha_\theta\rangle,|\beta_\theta\rangle\}$, with $|\beta_\theta\rangle=-\sin\theta|0\rangle+\cos\theta|1\rangle$. Bob receives one outcome bit and applies $I$ or $iY$. Since $iY|\beta_\theta\rangle=|\alpha_\theta\rangle$ for every $\theta$, the preparation is exact and the correction is independent of the unknown parameter.

## Schumacher compression

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schumacher_compression)

Schumacher compression is quantum source coding into the typical subspace of $\rho^{\otimes n}$. Asymptotically reliable compression is possible at every qubit rate above the [Von Neumann entropy](von-neumann-entropy.md) $S(\rho)$.

### Memoryless quantum information source

↑ **Parent:** [Schumacher compression](#schumacher-compression)

A pure-state source emits independent states from a fixed [quantum state ensemble](quantum-theory.md#quantum-state-ensemble). Its average block [density operator](quantum-theory.md#density-matrix) is the tensor power of the one-use average. Unassisted [reliable quantum source compression](#reliable-quantum-source-compression) preserves the emitted quantum states, rather than only their classical labels. [Schumacher compression](#schumacher-compression) gives the optimum asymptotic qubit rate $S(\rho)$ for such a source, with every larger rate achievable. Nonorthogonal equally likely pure states need not have entropy one: their classical labels have entropy one but their average density operator can have lower [Von Neumann entropy](von-neumann-entropy.md).

### Quantum typical subspace

↑ **Parent:** [Schumacher compression](#schumacher-compression)

For a [density operator](quantum-theory.md#density-matrix) $\pi=\sum_iq_i|\phi_i\rangle\langle\phi_i|$, the quantum typical subspace is spanned by product eigenvectors of $\pi^{\otimes n}$ whose eigenvalues $q_{i_1}\cdots q_{i_n}$ satisfy

$$
\left|-\frac1n\log_2(q_{i_1}\cdots q_{i_n})-S(\pi)\right|\leq\varepsilon.
$$

It applies the classical [weakly typical sequence](information-theory.md#weakly-typical-sequence) definition to the spectrum. If $P_\varepsilon^{(n)}$ is its [orthogonal projection](hilbert-space.md#orthogonal-projection), then

$$
\dim\mathcal T_\varepsilon^{(n)}\leq2^{n(S(\pi)+\varepsilon)},\qquad
\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})\longrightarrow1.
$$

The first statement follows from the [typical-set cardinality bounds](information-theory.md#typical-set-cardinality-bounds), and the second from the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers). This subspace holds nearly all the source probability while using exponentially fewer dimensions than the whole space when $S(\pi)<\log_2d$.

#### Typical subspace theorem

↑ **Parent:** [Quantum typical subspace](#quantum-typical-subspace)

For each fixed $\delta>0$, the [quantum typical subspace](#quantum-typical-subspace) projector selects eigenvalues of $\pi^{\otimes n}$ between $2^{-n(S(\pi)+\delta)}$ and $2^{-n(S(\pi)-\delta)}$. Its probability tends to one by the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) for the spectral information variable. If its probability is at least $1-\epsilon$, its dimension is between $(1-\epsilon)2^{n(S(\pi)-\delta)}$ and $2^{n(S(\pi)+\delta)}$. These statements give the size and concentration estimates behind [Schumacher compression](#schumacher-compression).

### Reliable quantum source compression

↑ **Parent:** [Schumacher compression](#schumacher-compression)

A quantum source-compression scheme has encoding and decoding [quantum channels](#quantum-channel) with compressed space $\mathcal K_n$ and rate $\limsup_n n^{-1}\log_2\dim\mathcal K_n$. For a pure-state source ensemble, average reliability means that the mean squared [quantum fidelity](#fidelity-of-quantum-states) after decoding tends to one. A stronger coherent criterion is $F_e(\pi^{\otimes n},\mathcal D_n\circ\mathcal E_n)\to1$, where [entanglement fidelity](#entanglement-fidelity) also tests a purification reference. Encoding the [quantum typical subspace](#quantum-typical-subspace) achieves both criteria above $S(\pi)$. [Schumacher's original quantum coding paper](https://doi.org/10.1103/PhysRevA.51.2738) establishes quantum source coding.

#### Typical-subspace compression with a failure flag

↑ **Parent:** [Reliable quantum source compression](#reliable-quantum-source-compression)

Measure the [quantum typical subspace](#quantum-typical-subspace) projector $\Pi$. Encode its successful sector isometrically and reserve one orthogonal compressed flag for failure; decode the flag to a fixed state. The composite channel is $\mathcal N_n(\tau)=\Pi\tau\Pi+\operatorname{Tr}[(I-\Pi)\tau]|\varphi_0\rangle\langle\varphi_0|$. It is trace preserving. The [Kraus formula for entanglement fidelity](#kraus-formula-for-entanglement-fidelity) gives the displayed lower bound, while convexity of the square gives the same bound for average pure-source fidelity. One flag adds only a vanishing asymptotic rate overhead.

##### Average pure-source fidelity after typical projection

↑ **Parent:** [Typical-subspace compression with a failure flag](#typical-subspace-compression-with-a-failure-flag)

For a [quantum state ensemble](quantum-theory.md#quantum-state-ensemble) of pure vectors and an [orthogonal projection](hilbert-space.md#orthogonal-projection) $P$, measure $\{P,I-P\}$, preserve the successful subspace, and decode failure to a fixed normalized vector $\varphi$. The resulting [quantum channel](#quantum-channel) is $\Lambda(X)=PXP+\operatorname{Tr}[(I-P)X]|\varphi\rangle\langle\varphi|$. For $\alpha_k=\|P\psi_k\|$, its [squared quantum fidelity](#squared-quantum-fidelity) on the $k$th source vector is $\alpha_k^4+(1-\alpha_k^2)|\langle\psi_k|\varphi\rangle|^2$. The inequality $a^2\geq2a-1$ on $[0,1]$ proves the displayed average bound. It depends only on the source density operator's weight in $P$ and does not require the emitted vectors to be orthogonal.

#### Finite-dimensional quantum compression converse

↑ **Parent:** [Reliable quantum source compression](#reliable-quantum-source-compression)

If encoding and decoding [quantum channels](#quantum-channel) factor through a $k$-dimensional space, their composite [Kraus operators](#kraus-operator) all have [matrix rank](vector-space.md#matrix-rank) at most $k$. The [rank bound for a weighted operator trace](compact-operator.md#rank-bound-for-a-weighted-operator-trace) and the [Kraus formula for entanglement fidelity](#kraus-formula-for-entanglement-fidelity) imply

$$
F_e(\rho,\mathcal D\mathcal C)\leq\sum_{j<k}\lambda_j(\rho).
$$

Thus high [operation fidelity](#operation-fidelity) requires the leading $k$ [eigenvalues](linear-operator-theory.md#eigenvalue) of the source [density operator](quantum-theory.md#density-matrix) to carry almost all its probability. The bound applies to arbitrary completely positive trace-preserving encoders and decoders.

## Classical-quantum state

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

A classical-quantum state has block-diagonal form $\rho_{XB}=\sum_xp_x|x\rangle\langle x|\otimes\rho_x$. Its entropy is $H(p)+\sum_xp_xS(\rho_x)$.

### Entropy of a classical-quantum state

↑ **Parent:** [Classical-quantum state](#classical-quantum-state)

The [classical-quantum state](#classical-quantum-state) is block diagonal. If $\lambda_{xj}$ are the eigenvalues of $\rho_x$, its eigenvalues are $p_x\lambda_{xj}$. Inserting these into the definition of [Von Neumann entropy](von-neumann-entropy.md) gives the displayed sum of classical [Shannon entropy](information-theory.md#information-entropy) and mean conditional quantum entropy. Its [quantum mutual information](von-neumann-entropy.md#quantum-mutual-information) is therefore the [Holevo quantity](#holevo-quantity) $S(\sum_xp_x\rho_x)-\sum_xp_xS(\rho_x)$.

### Holevo quantity

↑ **Parent:** [Classical-quantum state](#classical-quantum-state)

For an ensemble $\{p_x,\rho_x\}$ with average $\bar\rho$, the Holevo quantity is $\chi=S(\bar\rho)-\sum_xp_xS(\rho_x)=I(X:B)$ of the associated [classical-quantum state](#classical-quantum-state).

#### Holevo quantity under a quantum channel

↑ **Parent:** [Holevo quantity](#holevo-quantity)

Attach an orthogonal classical label register to an ensemble. Its [quantum mutual information](von-neumann-entropy.md#quantum-mutual-information) with the quantum system equals the ensemble [Holevo quantity](#holevo-quantity). A local [quantum channel](#quantum-channel) changes the ensemble states but preserves their labels and probabilities. [Data processing for quantum mutual information](von-neumann-entropy.md#data-processing-for-quantum-mutual-information) then proves that the output [Holevo quantity](#holevo-quantity) cannot exceed the input value.

<h4 id="holevo-s-theorem">Holevo's theorem</h4>

↑ **Parent:** [Holevo quantity](#holevo-quantity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Holevo's_theorem)

The classical mutual information obtained by any measurement of a quantum ensemble is at most its [Holevo quantity](#holevo-quantity). This follows from the [data-processing inequality for quantum relative entropy](von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) applied to the measurement channel.

##### One-shot classical-quantum coding converse

↑ **Parent:** [Holevo's theorem](#holevo-s-theorem)

For $k$ equiprobable quantum code states with average decoding error $\epsilon<1$, [data-processing inequality for quantum relative entropy](von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) applied to the [binary test for quantum decoding success](#binary-test-for-quantum-decoding-success) gives

$$
I(X:Q)\geq(1-\epsilon)\log_2k-h_2(\epsilon)-\epsilon\log_2(1-1/k)\geq(1-\epsilon)\log_2k-1
$$

for $k\geq2$. Here $h_2$ is [binary entropy](information-theory.md#binary-entropy). The case $k=1$ is trivial. Taking the supremum over allowed input distributions yields a code-size bound in terms of the largest [Holevo quantity](#holevo-quantity); at $\epsilon=1$ the undivided inequality is vacuous.

## Measure-and-prepare channel

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

A measure-and-prepare channel measures a POVM $\{M_x\}$ and outputs a prescribed state $\sigma_x$: $T(\rho)=\sum_x\operatorname{Tr}(M_x\rho)\sigma_x$. Such channels are exactly the [entanglement-breaking channels](#entanglement-breaking-channel).

### Measurement channel

↑ **Parent:** [Measure-and-prepare channel](#measure-and-prepare-channel)

A measurement channel writes a [POVM](quantum-measurement.md#positive-operator-valued-measure)'s outcome into an orthogonal classical register:

$$
\Phi(X)=\sum_a\operatorname{Tr}(E_aX)|a\rangle\langle a|.
$$

For any input [orthonormal basis](linear-algebra.md#orthonormal-basis) $|j\rangle$, the [Kraus operators](#kraus-operator) $K_{a,j}=|a\rangle\langle j|\sqrt{E_a}$ realize this map and satisfy $\sum_{a,j}K_{a,j}^\dagger K_{a,j}=I$. It is therefore a trace-preserving [completely positive map](#completely-positive-map).

#### Conditional input ensemble after a local measurement

↑ **Parent:** [Measurement channel](#measurement-channel)

For a bipartite input [density operator](quantum-theory.md#density-matrix) $\rho^x_{AC}$ and a [POVM](quantum-measurement.md#positive-operator-valued-measure) $\{E_y\}$ on $A$, let $q(y|x)=\operatorname{Tr}[(E_y\otimes I)\rho^x]$. For $q(y|x)>0$, the conditioned input on $C$ is

$$
\rho_C^{x,y}=\frac{\operatorname{Tr}_A[(\sqrt{E_y}\otimes I)\rho^x(\sqrt{E_y}\otimes I)]}{q(y|x)}.
$$

Its positivity follows from the positive sandwich before the [partial trace](quantum-theory.md#partial-trace). A [quantum channel](#quantum-channel) on $C$ acts on these conditional [density operators](quantum-theory.md#density-matrix) even if the original input is an [entangled state](bell-state.md#entangled-state).

## Fidelity of quantum states

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fidelity_of_quantum_states)

In the unsquared convention, quantum fidelity is $F(\rho,\sigma)=\operatorname{Tr}\sqrt{\sqrt\rho\sigma\sqrt\rho}$. It equals the minimum classical Bhattacharyya coefficient over all POVMs.

### Pure-state trace distance and fidelity identity

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

For pure states $\rho=|\psi\rangle\langle\psi|$ and $\sigma=|\varphi\rangle\langle\varphi|$, the unsquared [quantum fidelity](#fidelity-of-quantum-states) is $F=|\langle\psi|\varphi\rangle|$. In their two-dimensional span, $\rho-\sigma$ has [trace](linear-algebra.md#matrix-trace) zero and [determinant](linear-algebra.md#determinant) $-(1-F^2)$, hence [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm\sqrt{1-F^2}$. Its [trace norm](functional-analysis.md#trace-norm) is twice the positive [eigenvalue](linear-operator-theory.md#eigenvalue), giving [trace distance](quantum-theory.md#trace-distance) $D=\sqrt{1-F^2}$.

// Target: quantum-information-theory.bigb

### Unitary invariance of trace distance and fidelity

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

For any unitary $U$, the unique [positive square root of an operator](hilbert-space.md#positive-square-root-of-an-operator) obeys $\sqrt{UAU^\dagger}=U\sqrt A U^\dagger$. Conjugating the [positive operators](hilbert-space.md#positive-operator) appearing in [trace distance](quantum-theory.md#trace-distance) and [quantum fidelity](#fidelity-of-quantum-states) therefore conjugates their square roots. Cyclicity of the [trace](linear-algebra.md#matrix-trace) removes the unitary factors, proving invariance of both quantities under simultaneous unitary transformations of the states.

// Target: quantum-information-theory.bigb

### Squared quantum fidelity

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

This is the square of the [unsquared quantum fidelity](#fidelity-of-quantum-states), another common convention for fidelity. If one state is $|\psi\rangle\langle\psi|$, it equals $\langle\psi|\sigma|\psi\rangle$. For two pure states it equals $|\langle\psi|\varphi\rangle|^2$. The ensemble average used in pure-state quantum source coding is normally the average of this overlap probability; the convention must be stated when comparing fidelity formulas.

### Joint concavity of quantum fidelity

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

In the unsquared convention, $F(\sum_xp_x\rho_x,\sum_xp_x\sigma_x)\geq\sum_xp_xF(\rho_x,\sigma_x)$. Use [Uhlmann's theorem](quantum-theory.md#uhlmann-s-theorem) to choose component purifications with nonnegative maximizing overlaps, and then construct matching [flagged purifications of a quantum ensemble](quantum-theory.md#flagged-purification-of-a-quantum-ensemble). Their overlap is the weighted sum on the right; the fidelity of the mixtures maximizes over all such overlaps.

### Monotonicity of quantum fidelity under partial trace

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

Discarding a subsystem cannot decrease unsquared [quantum fidelity](#fidelity-of-quantum-states): $F(\rho_A,\sigma_A)\geq F(\rho_{AB},\sigma_{AB})$. Maximizing purifications of the joint states are also candidates for purifications of the marginals, with the discarded subsystem included in the reference. [Uhlmann's theorem](quantum-theory.md#uhlmann-s-theorem) then proves the inequality. Information loss makes the two states at least as similar.

### Pure-state gentle measurement bound

↑ **Parent:** [Fidelity of quantum states](#fidelity-of-quantum-states)

If $M$ is a [positive contraction](hilbert-space.md#positive-contraction) and $p=\langle\psi|M^2|\psi\rangle>0$, the normalized successful [post-measurement state](quantum-measurement.md#post-measurement-state) is $M|\psi\rangle/\sqrt p$. Since $M^2\leq M$,

$$
F\left(|\psi\rangle\langle\psi|,\frac{M|\psi\rangle\langle\psi|M}{p}\right)^2
=\frac{\langle\psi|M|\psi\rangle^2}{p}\geq p.
$$

A likely outcome therefore preserves a pure input well in [quantum fidelity](#fidelity-of-quantum-states) when its measurement operator is positive. Positivity excludes a hidden unitary rotation that could otherwise change the state even for an outcome of probability one.

## Coherent information

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coherent_information)

For a channel output $Q$ and complementary environment output $E$, coherent information is $I_c(\Lambda,\rho)=S(Q)-S(E)=-H(R|Q)$ for a purification reference $R$.

### Mutual information and coherent information identity

↑ **Parent:** [Coherent information](#coherent-information)

For a purified input with reference $R$ and channel output $B$, $I(R:B)=S(R)+S(B)-S(RB)=S(\rho)+I_c(\Lambda,\rho)$. The reference entropy is fixed through subsequent channels. Thus [data-processing inequality for coherent information](#data-processing-inequality-for-coherent-information) immediately implies [data processing for quantum mutual information](von-neumann-entropy.md#data-processing-for-quantum-mutual-information) between that reference and successive outputs.

### Coherent information upper bound by input entropy

↑ **Parent:** [Coherent information](#coherent-information)

In a purified [Stinespring dilation](#stinespring-dilation), [coherent information](#coherent-information) satisfies $I_c=S(RE)-S(E)=S(\rho)-I(R:E)$. Nonnegativity of [quantum mutual information](von-neumann-entropy.md#quantum-mutual-information) implies $I_c\leq S(\rho)$. Equality means that the reference and environment are uncorrelated, so the environment learns nothing about the purified input reference.

### Coherent information as an environment conditional entropy

↑ **Parent:** [Coherent information](#coherent-information)

Purify the input on $RA$ and dilate a channel by $A\to BE$. The joint state $RBE$ is pure, so complementary entropies obey $S(B)=S(RE)$ and $S(RB)=S(E)$. Therefore [coherent information](#coherent-information) is $I_c=S(B)-S(RB)=S(R\mid E)=-S(R\mid B)$. The positive environment conditional entropy and negative receiving-system conditional entropy are two equivalent forms.

### Data-processing inequality for coherent information

↑ **Parent:** [Coherent information](#coherent-information)

A [quantum channel](#quantum-channel) on the receiving system cannot increase [coherent information](#coherent-information): $I(A\rangle B)_\rho\geq I(A\rangle B^{\prime})_\sigma$. Dilate the channel to a [linear isometry of Hilbert spaces](hilbert-space.md#linear-isometry-of-hilbert-spaces) $B\to B^{\prime}E$. The difference is $I(A:E|B^{\prime})$ of the dilated state, nonnegative by [Strong subadditivity of Von Neumann entropy](von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy).

### Anti-degradable quantum channel

↑ **Parent:** [Coherent information](#coherent-information)

A quantum channel is anti-degradable when its receiver output can be simulated from the complementary environment output. Data processing then forces every coherent information to be nonpositive, and no-cloning prevents perfect quantum transmission.

## Joint convexity of quantum relative entropy

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

Quantum relative entropy obeys $D(\sum_ip_i\rho_i\|\sum_ip_i\sigma_i)\leq\sum_ip_iD(\rho_i\|\sigma_i)$. It follows by applying data processing to flagged block-diagonal states and discarding the flag.

## Quantum ancilla

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

A quantum ancilla is an auxiliary quantum system introduced to assist a state preparation, measurement, or channel use. Applying a channel to one part of an entangled system can reveal behavior invisible to inputs without an ancilla.

### Ancilla qubit

↑ **Parent:** [Quantum ancilla](#quantum-ancilla)

An [ancilla qubit](#ancilla-qubit) is a two-dimensional [quantum ancilla](#quantum-ancilla). It is the quantum version of an [ancilla bit](#ancilla-bit); an auxiliary quantum register can contain several such qubits.

## Positive linear map

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

A positive linear map sends every [positive semidefinite matrix](linear-algebra.md#positive-semidefinite-matrix) to a positive semidefinite matrix. Positivity need not persist after tensoring with the identity map on an ancillary system; requiring that stronger property gives a [completely positive map](#completely-positive-map).

### Positivity (linear maps)

↑ **Parent:** [Positive linear map](#positive-linear-map)

A [linear map](vector-space.md#linear-map) between ordered [vector spaces](vector-space.md) is positive if it carries the positive cone of the domain into the positive cone of the codomain. For function spaces this means $f\geq0\Longrightarrow Tf\geq0$. A [Feller semigroup](functional-analysis.md#feller-semigroup) consists of such positive maps on continuous functions.

### Decomposable positive map

↑ **Parent:** [Positive linear map](#positive-linear-map)

A decomposable positive map between complex matrix algebras has the form $\Phi=\Phi_1+\Phi_2\circ T$, where $\Phi_1,\Phi_2$ are [completely positive maps](#completely-positive-map) and $T$ is the [matrix transpose](vector-space.md#transpose). Such a map cannot detect a [positive partial transpose](#positive-partial-transpose) entangled state: applying it to one subsystem gives a sum of two positive operators.

<h4 id="stormer-woronowicz-decomposability-theorem">Størmer-Woronowicz decomposability theorem</h4>

↑ **Parent:** [Decomposable positive map](#decomposable-positive-map)

Every [positive linear map](#positive-linear-map) between $M_2(\mathbb C)$ and $M_2(\mathbb C)$, or between $M_2(\mathbb C)$ and $M_3(\mathbb C)$ in either direction, is a [decomposable positive map](#decomposable-positive-map). The low-dimensional result is the ingredient that makes the [positive partial transpose criterion](#positive-partial-transpose-criterion) sufficient in two-qubit and qubit-qutrit systems. [Woronowicz's low-dimensional positive-map paper](https://doi.org/10.1016/0034-4877(76)90038-0) establishes the $M_2$ to $M_3$ case; taking adjoints gives the reverse direction.

### k-reduction map

↑ **Parent:** [Positive linear map](#positive-linear-map)

The $k$-reduction map is $\Lambda_k(X)=k\operatorname{Tr}(X)I-X$. It remains positive when tensored with the identity on pure inputs of Schmidt rank at most $k$, making it a witness for Schmidt number greater than $k$.

### Completely positive map

↑ **Parent:** [Positive linear map](#positive-linear-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Completely_positive_map)

A linear map $\Phi$ between matrix algebras is completely positive when $\Phi\otimes\operatorname{id}_r$ is positive for every ancillary dimension $r$. In finite dimensions this is equivalent to positivity of its [Choi matrix](#choi-matrix) and to the existence of a [Kraus representation](#kraus-representation).

#### Quantum operation

↑ **Parent:** [Completely positive map](#completely-positive-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_operation)

A [completely positive map](#completely-positive-map) with $\sum_\alpha K_\alpha^\dagger K_\alpha\leq I$ is a trace-nonincreasing quantum operation, representing an outcome branch with its probability retained in the trace. A deterministic [quantum channel](#quantum-channel) has equality and is trace preserving. Dividing a branch output by its trace gives a conditional state but generally produces a nonlinear update; that normalization is not part of the linear quantum operation.

#### Stinespring representation of a completely positive map

↑ **Parent:** [Completely positive map](#completely-positive-map)

In finite dimensions, a [completely positive map](#completely-positive-map) has the form $\mathcal N(X)=\operatorname{Tr}_E(VXV^\dagger)$ for $V:\mathcal H_Q\to\mathcal H_{Q\prime}\otimes\mathcal H_E$. From a [Kraus representation](#kraus-representation) take $V=\sum_jK_j\otimes|j\rangle$. The observable-picture adjoint is $\mathcal N^\dagger(Y)=V^\dagger(Y\otimes I_E)V$. A general completely positive map need not have isometric $V$; it is a [linear isometry of Hilbert spaces](hilbert-space.md#linear-isometry-of-hilbert-spaces) precisely when the map is trace preserving.

#### Kraus representation

↑ **Parent:** [Completely positive map](#completely-positive-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kraus_representation)

Every finite-dimensional completely positive map has $T(\rho)=\sum_jK_j\rho K_j^\dagger$. It is trace preserving exactly when $\sum_jK_j^\dagger K_j=I$.

##### Trace-preserving and unital Kraus conditions

↑ **Parent:** [Kraus representation](#kraus-representation)

For a [Kraus representation](#kraus-representation) $\Phi(X)=\sum_kA_kXA_k^\dagger$, trace preservation is equivalent to the first identity, by cyclicity of the trace. The second says $\Phi(I)=I$, namely unitality, and is a distinct constraint. For $0<\gamma<1$, the [amplitude damping channel](#amplitude-damping-channel) has operators $A_0=\operatorname{diag}(1,\sqrt{1-\gamma})$ and $A_1=\sqrt\gamma|0\rangle\langle1|$ and is trace-preserving but not unital. Taking the adjoints as Kraus operators instead gives a unital completely positive map whose output trace on $|0\rangle\langle0|$ is $1+\gamma$.

##### Kraus operator

↑ **Parent:** [Kraus representation](#kraus-representation)

The operators $K_j$ in a [Kraus representation](#kraus-representation) are Kraus operators. For a measurement outcome $i$, its associated Kraus operators determine both the outcome probability and the conditional post-measurement state.

#### Choi matrix

↑ **Parent:** [Completely positive map](#completely-positive-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Choi_matrix)

For normalized maximally entangled $|\phi\rangle=d^{-1/2}\sum_j|jj\rangle$, the Choi matrix of $T$ is $C_T=(T\otimes\operatorname{id})(|\phi\rangle\langle\phi|)$. Choi's theorem says $T$ is completely positive exactly when $C_T\geq0$.

##### Spectral Kraus decomposition

↑ **Parent:** [Choi matrix](#choi-matrix)

Use the unnormalized [Choi matrix](#choi-matrix) $J(\Phi)=(\Phi\otimes\mathrm{id})(|\widetilde\Psi\rangle\langle\widetilde\Psi|)$, which has trace $d$ for a channel. A positive such matrix has a spectral decomposition with vectors $v_k=\sqrt{\lambda_k}u_k$. In paired bases define the [Kraus operator](#kraus-operator) $A_k$ by $(A_k)_{ij}=(v_k)_{ij}$, so $v_k=(A_k\otimes I)\sum_j|j\rangle|j\rangle$. Partial contraction with a [conjugate index vector](quantum-theory.md#conjugate-index-vector) gives $A_k|\phi\rangle$, hence $\Phi(|\phi\rangle\langle\phi|)=\sum_kA_k|\phi\rangle\langle\phi|A_k^\dagger$. Rank-one projectors span the operator space, proving the [Kraus representation](#kraus-representation) on all inputs. Trace preservation is equivalent to $\sum_kA_k^\dagger A_k=I$. This construction needs at most $\operatorname{rank}J$ nonzero Kraus operators.

##### Choi state

↑ **Parent:** [Choi matrix](#choi-matrix)

A channel's Choi state is its normalized [Choi matrix](#choi-matrix),

$$
C_\Lambda=(\Lambda\otimes\operatorname{id})(|\Phi_d\rangle\langle\Phi_d|),\qquad
|\Phi_d\rangle=\frac1{\sqrt d}\sum_i|ii\rangle.
$$

It is a [density operator](quantum-theory.md#density-matrix) and satisfies $\operatorname{Tr}_{\rm out}C_\Lambda=I_{\rm in}/d$. Some authors use an unnormalized [Choi matrix](#choi-matrix) of trace $d$, so reconstruction factors depend on the convention.

##### Choi reconstruction formula

↑ **Parent:** [Choi matrix](#choi-matrix)

With normalized [Choi state](#choi-state) $C_\Lambda$ and the output factor first,

$$
\Lambda(X)=d\operatorname{Tr}_{\rm in}[C_\Lambda(I_{\rm out}\otimes X^T)].
$$

Expand $C_\Lambda=d^{-1}\sum_{i,j}\Lambda(|i\rangle\langle j|)\otimes|i\rangle\langle j|$. The [partial trace](quantum-theory.md#partial-trace) multiplies each coefficient by $\operatorname{Tr}(|i\rangle\langle j|X^T)=X_{ij}$, reconstructing $\Lambda(X)$ by linearity.

#### Quantum channel

↑ **Parent:** [Completely positive map](#completely-positive-map)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_channel)

A quantum channel is a linear completely positive trace-preserving map between operator algebras.

##### Memoryless quantum channel

↑ **Parent:** [Quantum channel](#quantum-channel)

A memoryless quantum channel has independent identical noise on successive uses, described by the tensor-power map $\Phi^{\otimes n}$. This factorization does not restrict the encoder to product inputs: one can feed an [entangled state](bell-state.md#entangled-state) across uses. A block code with equally likely messages $m$ chooses states $\rho_m$ and a decoder [POVM](quantum-measurement.md#positive-operator-valued-measure) $(D_m)$. Its average error is $1-|\mathcal M|^{-1}\sum_m\operatorname{Tr}[D_m\Phi^{\otimes n}(\rho_m)]$, and its rate is $n^{-1}\log_2|\mathcal M|$. The [classical capacity of a quantum channel](#classical-capacity-of-a-quantum-channel) allows such entangled block inputs; the one-use [Holevo capacity](#holevo-capacity) gives the product-input capacity and requires regularization in general.

###### Quantum erasure channel

↑ **Parent:** [Memoryless quantum channel](#memoryless-quantum-channel)

A quantum erasure channel transmits an input state unchanged with probability $1-p$ and replaces it by an orthogonal, recognizable erasure flag with probability $p$. Its output space has one more dimension than the input. This is a [quantum channel](#quantum-channel) for $0\le p\le1$ and preserves all input coherences on the nonerased branch.

###### Entanglement-assisted capacity of a quantum erasure channel

↑ **Parent:** [Quantum erasure channel](#quantum-erasure-channel)

For input dimension $D$, an input of entropy $S(\rho)$ gives output entropy $h_2(p)+(1-p)S(\rho)$ and reference-output entropy $h_2(p)+pS(\rho)$. These follow from [entropy of an orthogonal quantum mixture](von-neumann-entropy.md#entropy-of-an-orthogonal-quantum-mixture) and purity of the input purification. Thus the [quantum mutual information](von-neumann-entropy.md#quantum-mutual-information) is $2(1-p)S(\rho)$, maximized at $\rho=I_D/D$. The [entanglement-assisted classical capacity](#entanglement-assisted-classical-capacity) is consequently $2(1-p)\log_2D$ bits per use; for a binary input it is $2(1-p)$.

###### Entanglement-assisted classical capacity

↑ **Parent:** [Memoryless quantum channel](#memoryless-quantum-channel)

This is the supremum of reliable classical bits per use of a [memoryless quantum channel](#memoryless-quantum-channel) when sender and receiver share unlimited prior [quantum entanglement](bell-state.md#entangled-state). If $|\psi_\rho\rangle_{RA}$ purifies the input, let $\omega_{RB}=(\operatorname{id}_R\otimes\mathcal N)(|\psi_\rho\rangle\langle\psi_\rho|)$. The single-letter capacity formula is $\max_\rho[S(\rho)+S(\mathcal N(\rho))-S(\omega_{RB})]$, the maximum [quantum mutual information](von-neumann-entropy.md#quantum-mutual-information) between reference and output. The preshared resource is independent of the message.

##### Amplitude damping channel

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Amplitude_damping_channel)

A zero-temperature energy-relaxation channel transfers the excited population of a [qubit](quantum-mechanics.md#qubit) to its ground state. Its [Kraus operators](#kraus-operator) are $A_0=\operatorname{diag}(1,\sqrt{1-p})$ and $A_1=\sqrt p|0\rangle\langle1|$ for $0\leq p\leq1$. They satisfy $\sum_jA_j^\dagger A_j=I$. The excited population is multiplied by $1-p$ and coherences by $\sqrt{1-p}$. For nonzero $p$, it is not a [unital quantum channel](#unital-quantum-channel).

###### Unitary dilation of amplitude damping

↑ **Parent:** [Amplitude damping channel](#amplitude-damping-channel)

With the environment initially in $|0\rangle$, take $U$ to fix $|00\rangle$ and $|11\rangle$, and rotate the span of $|10\rangle,|01\rangle$ by the displayed action and $U|01\rangle=\sqrt{1-p}|01\rangle-\sqrt p|10\rangle$. This is a [unitary operator](vector-space.md#unitary-operator). Its environment matrix elements $\langle0|_EU|0\rangle_E$ and $\langle1|_EU|0\rangle_E$ are the [Kraus operators](#kraus-operator) of the [amplitude damping channel](#amplitude-damping-channel). Tracing out the environment multiplies the excited population by $1-p$, transfers the remainder to the ground state, and multiplies off-diagonal entries by $\sqrt{1-p}$.

###### Entanglement fidelity of amplitude damping

↑ **Parent:** [Amplitude damping channel](#amplitude-damping-channel)

The [Kraus formula for entanglement fidelity](#kraus-formula-for-entanglement-fidelity) applies to any input, including mixed qubit states. For the [amplitude damping channel](#amplitude-damping-channel), the diagonal Kraus trace is $[1+s_z+\sqrt{1-p}(1-s_z)]/2$ and the jump Kraus trace has squared modulus $p(s_x^2+s_y^2)/4$. Summing them gives the formula. Ground-state inputs have unit [entanglement fidelity](#entanglement-fidelity); excited-state inputs have fidelity $1-p$.

###### Bloch-vector map of amplitude damping

↑ **Parent:** [Amplitude damping channel](#amplitude-damping-channel)

Applying the [amplitude damping channel](#amplitude-damping-channel) to the [Bloch vector](quantum-theory.md#bloch-vector) form of a qubit [density operator](quantum-theory.md#density-matrix) gives an affine map. Transverse components contract by $\sqrt{1-p}$; the longitudinal component contracts by $1-p$ and shifts toward the ground-state north pole. Reading the entries of the output [density operator](quantum-theory.md#density-matrix) proves the map. The displacement distinguishes this channel from centered depolarization.

###### Repeated amplitude damping limit

↑ **Parent:** [Bloch-vector map of amplitude damping](#bloch-vector-map-of-amplitude-damping)

Under repeated identical [amplitude damping channels](#amplitude-damping-channel), all excited population eventually relaxes to the ground state for any fixed $0<p\leq1$. The [Bloch vector](quantum-theory.md#bloch-vector) approaches $(0,0,1)$. For $p=1$ the limit is reached in one action, while $p=0$ is the identity channel and preserves every input. Keeping the zero-damping endpoint separate prevents an incorrect universal relaxation claim.

##### Holevo capacity

↑ **Parent:** [Quantum channel](#quantum-channel)

The Holevo capacity of a [quantum channel](#quantum-channel) is the maximum one-use output [Holevo quantity](#holevo-quantity),

$$
\chi^*(\Lambda)=\max_{\{p_x,\rho_x\}}
\left[S\left(\sum_xp_x\Lambda(\rho_x)\right)-\sum_xp_xS(\Lambda(\rho_x))\right].
$$

It is the unassisted classical communication limit for [product state](bell-state.md#product-state) encodings with collective output measurements. Arbitrary entangled inputs require the regularized expression in the [Holevo-Schumacher-Westmoreland theorem](#holevo-schumacher-westmoreland-theorem).

###### Superadditivity of Holevo capacity

↑ **Parent:** [Holevo capacity](#holevo-capacity)

Take independent ensembles for two [quantum channels](#quantum-channel) and their Cartesian product ensemble. The [Von Neumann entropy](von-neumann-entropy.md) of a tensor product is the sum of the two entropies, both for its average output and for each labelled output. Thus its [Holevo quantity](#holevo-quantity) is the sum of the two individual quantities. Taking ensembles arbitrarily close to each supremum proves the displayed inequality without requiring maximizing ensembles to exist. It does not assert additivity for arbitrary channels.

###### Additivity of Holevo capacity

↑ **Parent:** [Holevo capacity](#holevo-capacity)

A channel's [Holevo capacity](#holevo-capacity) is additive with another channel when their joint capacity equals the sum of the individual capacities. If this holds with every other channel, the channel's tensor powers have capacity $n\chi^*(\Lambda)$ and regularization does not increase its unassisted [classical capacity of a quantum channel](#classical-capacity-of-a-quantum-channel). Additivity is a special property, not a general rule for quantum channels.

###### Holevo-capacity additivity for entanglement-breaking channels

↑ **Parent:** [Additivity of Holevo capacity](#additivity-of-holevo-capacity)

Every [entanglement-breaking channel](#entanglement-breaking-channel) $\mathcal E$ has additive [Holevo capacity](#holevo-capacity) with every finite-dimensional [quantum channel](#quantum-channel) $\mathcal N$. A [measure-and-prepare channel](#measure-and-prepare-channel) factorization exposes a classical measurement outcome. The [quantum mutual information balance identity](von-neumann-entropy.md#quantum-mutual-information-balance-identity) and [data processing for quantum mutual information](von-neumann-entropy.md#data-processing-for-quantum-mutual-information) then bound the joint output [Holevo quantity](#holevo-quantity) by the sum of the individual capacities, using the [conditional input ensemble after a local measurement](#conditional-input-ensemble-after-a-local-measurement) for the other channel. Independent product ensembles attain the reverse inequality.

###### Product-input classical-capacity converse

↑ **Parent:** [Holevo capacity](#holevo-capacity)

For a code with [product state](bell-state.md#product-state) inputs to $n$ uses of a memoryless [quantum channel](#quantum-channel), [Subadditivity of Von Neumann entropy](von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) bounds its output [Holevo quantity](#holevo-quantity) by $n\chi^*(\Lambda)$. The [Holevo bound](#holevo-s-theorem) and [Fano's inequality](information-theory.md#fano-s-inequality) then give, for asymptotic rate $R$, average and hence maximum error at least $1-\chi^*(\Lambda)/R$ in the limit inferior. In particular, no code above that rate can have vanishing maximum error, even with a collective decoder measurement.

##### Classical capacity of a quantum channel

↑ **Parent:** [Quantum channel](#quantum-channel)

The unassisted classical capacity is the supremum of classical bit rates achievable with asymptotically vanishing message error. It allows entanglement among different channel inputs, but no preshared sender-receiver entanglement. The [Holevo-Schumacher-Westmoreland theorem](#holevo-schumacher-westmoreland-theorem) gives its regularized entropy expression.

###### Holevo-Schumacher-Westmoreland theorem

↑ **Parent:** [Classical capacity of a quantum channel](#classical-capacity-of-a-quantum-channel)

For a finite-dimensional memoryless [quantum channel](#quantum-channel),

$$
C(\Lambda)=\lim_{n\to\infty}\frac1n\chi^*(\Lambda^{\otimes n}).
$$

The [Holevo bound](#holevo-s-theorem) controls information obtainable from an output ensemble, while collective decoding makes rates below the corresponding coding expression achievable. The [Holevo capacity](#holevo-capacity) needs regularization because input states can be entangled across channel uses. [Watrous's channel-coding chapter](https://cs.uwaterloo.ca/~watrous/TQI/TQI.8.pdf) states and develops the classical-capacity theorem.

##### Random unitary channel

↑ **Parent:** [Quantum channel](#quantum-channel)

A random unitary channel has $T(\rho)=\sum_jp_jU_j\rho U_j^\dagger$. Its Choi matrix is a convex combination of maximally entangled pure states.

###### Heisenberg-Weyl operator

↑ **Parent:** [Random unitary channel](#random-unitary-channel)

On a $d$-dimensional [Hilbert space](hilbert-space.md), let $X|j\rangle=|j+1\bmod d\rangle$ and $Z|j\rangle=e^{2\pi ij/d}|j\rangle$. The $d^2$ unitaries $W_{k,m}=X^kZ^m$ form an orthogonal operator basis under the [Hilbert-Schmidt inner product](compact-operator.md#hilbert-schmidt-inner-product).

###### Heisenberg-Weyl twirling channel

↑ **Parent:** [Heisenberg-Weyl operator](#heisenberg-weyl-operator)

Averaging conjugation by all [Heisenberg-Weyl operators](#heisenberg-weyl-operator) completely depolarizes a system:

$$
\frac1{d^2}\sum_{k,m}W_{k,m}AW_{k,m}^\dagger=(\operatorname{Tr}A)\frac Id.
$$

Summing over phases $Z^m$ kills off-diagonal matrix elements, and averaging shifts $X^k$ makes all diagonal elements equal. Acting on subsystem $B$ of a bipartite operator gives $(\operatorname{Tr}_BA)\otimes I_B/d$. This identity turns [joint convexity of quantum relative entropy](#joint-convexity-of-quantum-relative-entropy) into monotonicity under [partial trace](quantum-theory.md#partial-trace).

###### Pauli channel

↑ **Parent:** [Random unitary channel](#random-unitary-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pauli_channel)

A one-qubit Pauli channel applies $I,\sigma_x,\sigma_y,\sigma_z$ with probabilities $p_0,p_x,p_y,p_z$. It maps a Bloch vector diagonally by independently contracting or reversing its three components.

###### Quantum bit-flip channel

↑ **Parent:** [Pauli channel](#pauli-channel)

A bit-flip channel applies the [Pauli X gate](quantum-theory.md#pauli-x-gate) with [probability](probability-theory.md#probability) $p$ and does nothing otherwise. If the classical error outcome is not recorded, its output is the convex mixture $\mathcal E_p(\rho)=(1-p)\rho+pX\rho X$, not a coherent superposition of the two alternatives.

// Target: quantum-information-theory.bigb

###### Average pure-qubit fidelity of a bit-flip channel

↑ **Parent:** [Quantum bit-flip channel](#quantum-bit-flip-channel)

For pure input $|\psi\rangle$, squared [quantum fidelity](#fidelity-of-quantum-states) after the bit-flip channel is $(1-p)+p|\langle\psi|X|\psi\rangle|^2$. The last factor is the square of the input's Bloch $x$ component. Rotational symmetry of the [uniform pure-qubit average](quantum-theory.md#uniform-pure-qubit-average) gives $\langle r_x^2\rangle=1/3$, because $r_x^2+r_y^2+r_z^2=1$. Hence the average squared fidelity is $1-2p/3$. Averaging an unsquared fidelity or over a different ensemble gives a different quantity.

// Target: quantum-mechanics.bigb

###### Quantum depolarizing channel

↑ **Parent:** [Pauli channel](#pauli-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_depolarizing_channel)

A qubit depolarizing channel shrinks every [Bloch vector](quantum-theory.md#bloch-vector) by the same factor: $\Lambda_p(\rho)=p\rho+(1-p)I/2$. In this retention-parameter convention it is completely positive for $-1/3\leq p\leq1$; the usual mixture of unchanged and fully randomized states uses $0\leq p\leq1$.

###### Entanglement-assisted capacity of a qubit depolarizing channel

↑ **Parent:** [Quantum depolarizing channel](#quantum-depolarizing-channel)

For the [quantum depolarizing channel](#quantum-depolarizing-channel) applying the identity with probability $1-p$ and each nonidentity [Pauli operator](quantum-circuit.md#pauli-operator) with probability $p/3$, the entanglement-assisted classical capacity is the displayed number of [bits](information-theory.md#bit) per use. Here $H_4$ is [Shannon entropy](information-theory.md#information-entropy) of the four listed probabilities. Its unassisted product-state capacity is $1-h_2(2p/3)$. Both vanish at $p=3/4$. If $q$ instead denotes replacement by $I/2$, then $p=3q/4$ and complete depolarization is at $q=1$. [The original entanglement-assisted capacity paper](https://arxiv.org/abs/quant-ph/9904023) gives the depolarizing-channel formula.

###### High-noise capacity ratio for qubit depolarization

↑ **Parent:** [Entanglement-assisted capacity of a qubit depolarizing channel](#entanglement-assisted-capacity-of-a-qubit-depolarizing-channel)

With [Bloch vector](quantum-theory.md#bloch-vector) retention $\eta\to0$, the unassisted product-state capacity of a [quantum depolarizing channel](#quantum-depolarizing-channel) is $\eta^2/(2\ln2)+O(\eta^4)$. Its entanglement-assisted capacity is $3\eta^2/(2\ln2)+O(\eta^3)$, obtained by expanding [Shannon entropy](information-theory.md#information-entropy) around the uniform four-outcome distribution. Consequently their limiting ratio is three, independent of the linear noise-parameter convention.

###### Depolarizing noise weight above one

↑ **Parent:** [Quantum depolarizing channel](#quantum-depolarizing-channel)

The displayed qubit [quantum channel](#quantum-channel) is completely positive for $0\leq q\leq4/3$. Indeed its [Pauli channel](#pauli-channel) probabilities are $1-3q/4$ for the identity and $q/4$ for each nonidentity Pauli operator. In the range $q>1$ the coefficient $1-q$ is negative, so the displayed expression is not a convex mixture of the unchanged and maximally mixed states, even though the Pauli representation is a valid [random unitary channel](#random-unitary-channel). Its [Bloch vector](quantum-theory.md#bloch-vector) is contracted and reversed by the factor $1-q$. The [Holevo capacity of a qubit depolarizing channel](#holevo-capacity-of-a-qubit-depolarizing-channel) remains $1-h_2(q/2)$ throughout this interval.

###### Pauli-mixture parametrization of qubit depolarization

↑ **Parent:** [Quantum depolarizing channel](#quantum-depolarizing-channel)

If the identity is applied with probability $p$ and the three nonidentity [Pauli operators](quantum-circuit.md#pauli-operator) each with probability $(1-p)/3$, the [Bloch vector](quantum-theory.md#bloch-vector) retention factor is $(4p-1)/3$. Thus complete depolarization occurs at $p=1/4$, not at zero. The [Holevo capacity of a qubit depolarizing channel](#holevo-capacity-of-a-qubit-depolarizing-channel) becomes $1-h_2((2p+1)/3)$ in this identity-probability parametrization.

###### Holevo capacity of a qubit depolarizing channel

↑ **Parent:** [Quantum depolarizing channel](#quantum-depolarizing-channel)

For the retention parameter $p$, the [Holevo capacity](#holevo-capacity) is

$$
\chi^*(\Lambda_p)=1-h_2\left(\frac{1+p}2\right).
$$

Every output has [Von Neumann entropy](von-neumann-entropy.md) at least the value on a pure input, $h_2((1+p)/2)$. Two equiprobable orthogonal pure inputs attain this minimum entropy individually and have maximally mixed average output, attaining the bound. [Additivity of Holevo capacity](#additivity-of-holevo-capacity) makes the unassisted [classical capacity of a quantum channel](#classical-capacity-of-a-quantum-channel) equal to this value. [King's depolarizing-channel capacity paper](https://arxiv.org/abs/quant-ph/0204172) proves additivity with an arbitrary other channel.

###### Product-input block bound for a qubit depolarizing channel

↑ **Parent:** [Holevo capacity of a qubit depolarizing channel](#holevo-capacity-of-a-qubit-depolarizing-channel)

For $\Phi(\rho)=p\rho+(1-p)I/2$, every output qubit has [Von Neumann entropy](von-neumann-entropy.md) at least $h((1-p)/2)$. A product input therefore has output entropy at least $n h((1-p)/2)$. The average output has entropy at most $n$, so its [Holevo quantity](#holevo-quantity) is bounded by the displayed expression. This allows correlated classical message labels and joint output measurements, but requires product quantum inputs. The [Holevo bound](#holevo-s-theorem) and [Fano's inequality](information-theory.md#fano-s-inequality) turn it into the corresponding asymptotic rate bound.

###### Phase-flip channel

↑ **Parent:** [Pauli channel](#pauli-channel)

The phase-flip channel is $\Lambda_p(\rho)=(1-p)\rho+p\sigma_z\rho\sigma_z$. It multiplies the $x$ and $y$ components of the Bloch vector by $1-2p$ and leaves the $z$ component fixed.

###### Iterated phase-flip channel

↑ **Parent:** [Phase-flip channel](#phase-flip-channel)

Independent successive applications of the [phase-flip channel](#phase-flip-channel) $D_\epsilon(\rho)=(1-\epsilon)\rho+\epsilon Z\rho Z$ preserve diagonal entries and multiply off-diagonal entries by $(1-2\epsilon)^n$. Hence $D_\epsilon^n=D_{\epsilon_n}$ with the displayed parameter, for nonnegative integers $n$. If $0<\epsilon<1/2$, the limit is the [completely dephasing channel](quantum-measurement.md#rank-one-dephasing), equivalently a [nonselective projective measurement](quantum-measurement.md#nonselective-projective-measurement) in the [computational basis](quantum-theory.md#computational-basis). A time-interval law can be iterated this way only under the memoryless composition assumption.

###### Dephasing channel

↑ **Parent:** [Pauli channel](#pauli-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dephasing_channel)

A dephasing channel suppresses off-diagonal density-matrix entries in a preferred basis while preserving populations. Complete dephasing is identical to a projective measurement in that basis with its outcome discarded.

###### Complex environment overlap in qubit dephasing

↑ **Parent:** [Dephasing channel](#dephasing-channel)

An environment interaction preserving the computational populations multiplies a qubit's upper off-diagonal density entry by $\overline c$. A real [phase-flip channel](#phase-flip-channel) representation exists for every input precisely when $c$ is real, with probability $(1-c)/2$. For $c=re^{i\varphi}$, the channel is a [phase-flip channel](#phase-flip-channel) of probability $(1-r)/2$ followed by the diagonal [unitary operator](vector-space.md#unitary-operator) $\operatorname{diag}(1,e^{i\varphi})$. The coherent phase cannot be discarded just because the populations are unchanged.

##### Unital quantum channel

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unital_quantum_channel)

A quantum channel is unital when $T(I)=I$. Every random unitary channel is unital, while the converse fails in dimension at least three.

###### Eigenvalue mixing matrix of a unital quantum channel

↑ **Parent:** [Unital quantum channel](#unital-quantum-channel)

Choose input eigenvectors $u_i$ and output eigenvectors $v_j$ for a [unital quantum channel](#unital-quantum-channel). Positivity makes the displayed entries nonnegative. Trace preservation makes every column sum one; unitality makes every row sum one. Thus $A$ is a [doubly stochastic matrix](vector-space.md#doubly-stochastic-matrix) and the output spectrum satisfies $s=Ar$. The mixing matrix need not be a matrix of squared overlaps of a single unitary, even though its row and column constraints are the same.

###### Spectral majorization under a unital quantum channel

↑ **Parent:** [Eigenvalue mixing matrix of a unital quantum channel](#eigenvalue-mixing-matrix-of-a-unital-quantum-channel)

A [unital quantum channel](#unital-quantum-channel) mixes its input spectrum with a [doubly stochastic matrix](vector-space.md#doubly-stochastic-matrix), so its output spectrum satisfies the [majorization](vector-space.md#majorization) relation with its input spectrum. The reverse inequality is generally false: a [pure state](quantum-theory.md#pure-state) can be sent to a maximally mixed state. The direction expresses the fact that unital noise can make eigenvalues more uniform. Equality of the two spectra is possible, for example under a unitary channel.

<h6 id="werner-holevo-channel">Werner–Holevo channel</h6>

↑ **Parent:** [Unital quantum channel](#unital-quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Werner–Holevo_channel)

The Werner–Holevo channel is $T(\rho)=(\operatorname{Tr}(\rho)I-\rho^T)/(d-1)$. Its normalized Choi matrix is the maximally mixed state on the antisymmetric subspace.

##### Strictly contractive quantum channel

↑ **Parent:** [Quantum channel](#quantum-channel)

A quantum channel is strictly contractive in trace distance when it reduces the distance between every pair of distinct density operators by a uniform factor smaller than one.

##### Primitive quantum channel

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_quantum_channel)

A finite-dimensional quantum channel is primitive when some power maps every nonzero positive operator to a positive-definite operator. Equivalently, eigenvalue one is simple and no other eigenvalue lies on the unit circle.

##### Stinespring dilation

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stinespring_dilation)

A Stinespring dilation represents a quantum channel by an isometry $V=\sum_iK_i\otimes|i\rangle$ followed by tracing out the environment.

##### Entanglement fidelity

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_fidelity)

For a purification $|\Psi_\rho\rangle_{RA}$, the entanglement fidelity of a channel $\Lambda$ is

$$
F_e(\rho,\Lambda)=
\langle\Psi_\rho|(\operatorname{id}_R\otimes\Lambda)
(|\Psi_\rho\rangle\langle\Psi_\rho|)
|\Psi_\rho\rangle.
$$

It is independent of the chosen purification.

###### Entanglement fidelity bound by state fidelity

↑ **Parent:** [Entanglement fidelity](#entanglement-fidelity)

In the [unsquared quantum fidelity](#fidelity-of-quantum-states) convention, the fidelity between a purification and its channel output is the square root of [entanglement fidelity](#entanglement-fidelity). Tracing out the purifying reference leaves the input and output marginals. [Monotonicity of quantum fidelity under partial trace](#monotonicity-of-quantum-fidelity-under-partial-trace) therefore gives the bound. Preserving an input marginal is a weaker requirement than preserving its correlations with a reference.

###### Quantum Fano inequality

↑ **Parent:** [Entanglement fidelity](#entanglement-fidelity)

For a [quantum channel](#quantum-channel) on a $d\geq2$ dimensional system, purify the input to $|\Psi\rangle_{QR}$ and set $\sigma=(\mathcal N\otimes\operatorname{id})(|\Psi\rangle\langle\Psi|)$. Its [entanglement fidelity](#entanglement-fidelity) $F_e=\langle\Psi|\sigma|\Psi\rangle$ satisfies $S(\sigma)\leq h(F_e)+(1-F_e)\log_2(d^2-1)$. This is the [entropy bound from overlap with a pure state](von-neumann-entropy.md#entropy-bound-from-overlap-with-a-pure-state) in dimension $d^2$. For a trivial one-dimensional system the output entropy is zero.

###### Kraus formula for entanglement fidelity

↑ **Parent:** [Entanglement fidelity](#entanglement-fidelity)

If $\{K_a\}$ is any [Kraus representation](#kraus-representation) of a [quantum channel](#quantum-channel) $\Lambda$, then

$$
F_e(\rho,\Lambda)=\sum_a|\operatorname{Tr}(\rho K_a)|^2.
$$

For a [purification of a density operator](quantum-theory.md#purification-of-a-density-operator), each branch overlap is $\langle\Psi_\rho|(I\otimes K_a)|\Psi_\rho\rangle=\operatorname{Tr}(\rho K_a)$. Summing the squared branch overlaps gives [entanglement fidelity](#entanglement-fidelity).

###### Operation fidelity

↑ **Parent:** [Entanglement fidelity](#entanglement-fidelity)

In the unsquared [quantum fidelity](#fidelity-of-quantum-states) convention, operation fidelity compares a [purification of a density operator](quantum-theory.md#purification-of-a-density-operator) with its image under a [quantum channel](#quantum-channel) acting on the source subsystem:

$$
F_{\rm op}(\Lambda,\rho)=F\bigl(|\Psi_\rho\rangle\langle\Psi_\rho|,(\operatorname{id}\otimes\Lambda)(|\Psi_\rho\rangle\langle\Psi_\rho|)\bigr).
$$

Its square is [entanglement fidelity](#entanglement-fidelity). Thus this convention is distinct from the squared quantity $F_e$; the two should not be installed as synonyms.

##### Lindblad equation

↑ **Parent:** [Quantum channel](#quantum-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lindblad_equation)

A Markovian continuous-time quantum channel obeys

$$
\dot\rho=-i[H,\rho]+\sum_\alpha\left(L_\alpha\rho L_\alpha^\dagger-\frac12\{L_\alpha^\dagger L_\alpha,\rho\}\right).
$$

###### Lindblad dissipator

↑ **Parent:** [Lindblad equation](#lindblad-equation)

A [Lindblad dissipator](#lindblad-dissipator) is the non-Hamiltonian generator associated with a [Lindblad operator](#lindblad-operator) $V$. It preserves the [trace](linear-algebra.md#matrix-trace) because cyclicity gives $\operatorname{Tr}(V\rho V^\dagger)=\operatorname{Tr}(V^\dagger V\rho)$, cancelling the two [anticommutator](vector-space.md#anticommutator) terms. It preserves Hermiticity and satisfies $\mathcal D[V](I)=[V,V^\dagger]$; it need not preserve the identity or the [purity of a density operator](quantum-theory.md#purity-of-a-density-operator).

###### Lindblad operator

↑ **Parent:** [Lindblad equation](#lindblad-equation)

The Lindblad operators $L_\alpha$ describe dissipative channels in a Markovian open-system evolution. Their normalization fixes the corresponding rates, and their representation is not unique.

###### Lindbladian

↑ **Parent:** [Lindblad equation](#lindblad-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lindbladian)

The Lindbladian $\mathcal L$ is the linear superoperator on density operators defined by the right-hand side of a [Lindblad equation](#lindblad-equation), so that $\dot\rho=\mathcal L(\rho)$.

###### Finite-dimensional Lindbladians have stationary states

↑ **Parent:** [Lindbladian](#lindbladian)

For any initial [density operator](quantum-theory.md#density-matrix), average its time-independent [Lindblad equation](#lindblad-equation) trajectory as $\bar\rho_T=T^{-1}\int_0^T\rho(t)\,dt$. These averages stay in the compact convex set of [density operators](quantum-theory.md#density-matrix). Along a convergent subsequence, $\mathcal L(\bar\rho_T)=(\rho(T)-\rho(0))/T\to0$, so the limit is stationary. Thus a finite-dimensional physical [Affine Bloch equation](quantum-theory.md#affine-bloch-equation) has at least one physical equilibrium, even though an arbitrary affine real equation can have none.

###### Lindbladian gap

↑ **Parent:** [Lindbladian](#lindbladian)

The Lindbladian gap is the smallest positive decay rate $-\operatorname{Re}\lambda$ among nonzero eigenvalues $\lambda$ of a relaxing Lindbladian. It controls the slowest asymptotic exponential approach to the stationary state.

###### Unique stationary state of a Lindbladian

↑ **Parent:** [Lindbladian](#lindbladian)

A finite-dimensional Lindbladian converges to one stationary state for every initial state exactly when zero is a simple eigenvalue and every other eigenvalue has strictly negative real part. A trivial commutant of the Hamiltonian and all jump operators and their adjoints is a standard irreducibility criterion leading to uniqueness under the usual finite-dimensional hypotheses.

###### Quantum Trajectory Theory

↑ **Parent:** [Lindblad equation](#lindblad-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_Trajectory_Theory)

A quantum-trajectory unravelling represents a [Lindblad equation](#lindblad-equation) as an ensemble of stochastic pure-state histories. In one jump unravelling, a state evolves between jumps under the non-Hermitian effective Hamiltonian $H_{\rm eff}=H-\frac i2\sum_\alpha L_\alpha^\dagger L_\alpha$, while a jump of type $\alpha$ sends it to a normalized multiple of $L_\alpha|\psi\rangle$.

###### Dark state of a Lindblad equation

↑ **Parent:** [Quantum Trajectory Theory](#quantum-trajectory-theory)

A pure stationary state is dark when every jump operator acts on it as a scalar, after an allowed shift of the jump operators, and the corresponding effective Hamiltonian preserves its ray. Every trajectory that reaches such a state remains on that same ray.

## Quantum de Finetti theorem

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_de_Finetti_theorem)

The quantum de Finetti theorem represents every infinitely exchangeable quantum state as a mixture of independent identically distributed product states. Finite versions approximate a fixed-size marginal of an $N$-exchangeable state by such a mixture with error tending to zero as $N$ grows.

### Mean-field ansatz from the quantum de Finetti theorem

↑ **Parent:** [Quantum de Finetti theorem](#quantum-de-finetti-theorem)

For a permutation-symmetric many-body problem with diverging coordination, finite-site reduced states approach mixtures of product states. Minimizing a local energy therefore reduces asymptotically to minimizing it over one-site density matrices, with separate one-site states allowed for distinct sublattices.

## Separable quantum state

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separable_quantum_state)

A bipartite state is separable when it is a convex combination $\sum_jp_j\rho_j^A\otimes\rho_j^B$ of product states; otherwise it is entangled.

### Separable positive operator

↑ **Parent:** [Separable quantum state](#separable-quantum-state)

A separable positive operator is a finite sum $\eta_{AB}=\sum_y\alpha_y\otimes\beta_y$ with both factors [positive operators](hilbert-space.md#positive-operator). If its [trace](linear-algebra.md#matrix-trace) is one, normalizing the nonzero factors gives a [separable quantum state](#separable-quantum-state). Conversely, a nonnegative scalar multiple of a [separable quantum state](#separable-quantum-state) is a separable positive operator.

### Positive-map separability criterion

↑ **Parent:** [Separable quantum state](#separable-quantum-state)

A finite-dimensional bipartite [density operator](quantum-theory.md#density-matrix) $\rho_{AB}$ is a [separable quantum state](#separable-quantum-state) exactly when $(\operatorname{id}_A\otimes\Phi)(\rho_{AB})\geq0$ for every [positive linear map](#positive-linear-map) from operators on $B$ to operators on $A$. In combination with the [Størmer-Woronowicz decomposability theorem](#stormer-woronowicz-decomposability-theorem), it makes the [positive partial transpose criterion](#positive-partial-transpose-criterion) sufficient for qubit-qutrit states. The criterion is established in [the Horodeckis' separability paper](https://arxiv.org/abs/quant-ph/9605038).

### Entanglement witness

↑ **Parent:** [Separable quantum state](#separable-quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_witness)

An entanglement witness is a [Hermitian operator](hilbert-space.md#hermitian-operator) $W$ such that $\operatorname{Tr}(W\rho)\geq0$ for every [separable quantum state](#separable-quantum-state) $\rho$, but $\operatorname{Tr}(W\sigma)<0$ for at least one [entangled state](bell-state.md#entangled-state) $\sigma$.

### Partial transpose

↑ **Parent:** [Separable quantum state](#separable-quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partial_transpose)

In a fixed product basis, the partial transpose on subsystem $B$ sends

$$
|i\rangle\langle j|\otimes|k\rangle\langle\ell|
\longmapsto
|i\rangle\langle j|\otimes|\ell\rangle\langle k|.
$$

It preserves Hermiticity and trace but need not preserve positivity on entangled inputs.

#### Partial transpose of a maximally entangled projector

↑ **Parent:** [Partial transpose](#partial-transpose)

For $|\Phi_d\rangle=d^{-1/2}\sum_j|jj\rangle$, the [partial transpose](#partial-transpose) of its [pure state](quantum-theory.md#pure-state) projector is $S/d$, where $S$ is the [swap operator](#swap-operator). Expand in matrix units: $|i\rangle\langle j|\otimes|i\rangle\langle j|$ becomes $|i\rangle\langle j|\otimes|j\rangle\langle i|$.

#### Positive partial transpose

↑ **Parent:** [Partial transpose](#partial-transpose)

A bipartite [density operator](quantum-theory.md#density-matrix) has positive partial transpose when $\rho^{T_B}\geq0$. Every [separable quantum state](#separable-quantum-state) has this property, since transposing one factor of a positive [product state](bell-state.md#product-state) preserves positivity and the separable sum preserves it as well. The property does not depend on which local basis defines the transpose.

##### PPT maximally entangled overlap bound

↑ **Parent:** [Positive partial transpose](#positive-partial-transpose)

Every [density operator](quantum-theory.md#density-matrix) $\sigma$ with [positive partial transpose](#positive-partial-transpose) has squared [quantum fidelity](#fidelity-of-quantum-states) at most $1/d$ with a fixed [maximally entangled state](quantum-theory.md#maximally-entangled-state) on $d\otimes d$. The [partial transpose of a maximally entangled projector](#partial-transpose-of-a-maximally-entangled-projector) and the [trace-adjoint identity for partial transpose](#trace-adjoint-identity-for-partial-transpose) express that squared overlap as $\operatorname{Tr}(S\sigma^{T_B})/d$. Since $\sigma^{T_B}$ is positive of [trace](linear-algebra.md#matrix-trace) one and the [swap operator](#swap-operator) has [operator norm](continuous-dual-space.md#operator-norm) one, [trace duality](compact-operator.md#trace-duality) gives the bound. A matching [product state](bell-state.md#product-state) attains equality.

#### Trace-adjoint identity for partial transpose

↑ **Parent:** [Partial transpose](#partial-transpose)

For bipartite operators $X,Y$ in a fixed product basis,

$$
\operatorname{Tr}(XY^{T_B})=\operatorname{Tr}(X^{T_B}Y).
$$

Expand both operators in products of matrix units. On the transposed factor, the identity is $\operatorname{Tr}(AT)=\operatorname{Tr}(A^TT^T)$; bilinearity gives the bipartite result. It allows a negative [partial transpose](#partial-transpose) eigenvector to define an [entanglement witness](#entanglement-witness).

### Positive partial transpose criterion

↑ **Parent:** [Separable quantum state](#separable-quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_partial_transpose_criterion)

Every separable state has positive partial transpose. The condition is also sufficient for separability on $2\otimes2$ and $2\otimes3$ systems.

### Entanglement-breaking channel

↑ **Parent:** [Separable quantum state](#separable-quantum-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement-breaking_channel)

A channel is entanglement breaking when applying it to one side of every bipartite state always produces a separable state. Equivalently, its Choi matrix is separable, and equivalently it has a measure-and-prepare representation.

#### Separable Choi-state criterion for entanglement breaking

↑ **Parent:** [Entanglement-breaking channel](#entanglement-breaking-channel)

A [quantum channel](#quantum-channel) is entanglement breaking exactly when its [Choi state](#choi-state) is a [separable quantum state](#separable-quantum-state). If $C_\Lambda=\sum_ap_a\sigma_a\otimes\tau_a$, the [Choi reconstruction formula](#choi-reconstruction-formula) gives a [measure-and-prepare channel](#measure-and-prepare-channel) with [POVM](quantum-measurement.md#positive-operator-valued-measure) $E_a=dp_a\tau_a^T$. Conversely, applying an entanglement-breaking channel to a [maximally entangled state](quantum-theory.md#maximally-entangled-state) produces a separable Choi state. [Horodecki, Shor and Ruskai's entanglement-breaking channel paper](https://arxiv.org/abs/quant-ph/0302031) develops the equivalences.

#### Rank-one Kraus representation of an entanglement-breaking channel

↑ **Parent:** [Entanglement-breaking channel](#entanglement-breaking-channel)

An [entanglement-breaking channel](#entanglement-breaking-channel) admits a [Kraus representation](#kraus-representation) with rank-one [Kraus operators](#kraus-operator) $K_j=|a_j\rangle\langle b_j|$. Its [Choi state](#choi-state) is a sum of positive [tensor-product operators](linear-algebra.md#tensor-product-operator), hence separable. Conversely, spectral decompositions of each prepared state and each [POVM](quantum-measurement.md#positive-operator-valued-measure) effect in a [measure-and-prepare channel](#measure-and-prepare-channel) produce rank-one Kraus operators. Trace preservation imposes $\sum_j\lVert a_j\rVert^2|b_j\rangle\langle b_j|=I$.

## Isotropic quantum state

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)

For two $d$-dimensional systems, an isotropic quantum state has the form

$$
\rho_p=p|\Phi^+\rangle\langle\Phi^+|+(1-p)\frac{I}{d^2},
$$

where $|\Phi^+\rangle=d^{-1/2}\sum_j|jj\rangle$ is a [maximally entangled state](quantum-theory.md#maximally-entangled-state). This parametrization is separable exactly when $p\leq1/(d+1)$.

The defining symmetry is $U\otimes\overline U$ invariance. This differs from the $U\otimes U$ invariance of a [Werner state](#werner-state); members above the displayed threshold are entangled.

## Swap operator

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Swap_operator)

The swap operator exchanges two tensor factors: $F(|\psi\rangle\otimes|\phi\rangle)=|\phi\rangle\otimes|\psi\rangle$. It has [eigenvalue](linear-operator-theory.md#eigenvalue) $+1$ on the symmetric subspace and $-1$ on the antisymmetric subspace, and the [partial transpose](#partial-transpose) of $|\Phi^+\rangle\langle\Phi^+|$ is $F/d$.

## Pretty good measurement

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pretty_good_measurement)

For ensemble $\{p_j,\rho_j\}$ with average $\bar\rho=\sum_jp_j\rho_j$, the pretty good measurement has $M_j=\bar\rho^{-1/2}p_j\rho_j\bar\rho^{-1/2}$ on the support of $\bar\rho$.

## Quantum state discrimination

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_state_discrimination)

[Quantum state discrimination](#quantum-state-discrimination) uses a [measurement in quantum mechanics](quantum-measurement.md) to identify which candidate [density operator](quantum-theory.md#density-matrix) was prepared. Minimum-error and unambiguous discrimination impose different objectives; [quantum binary hypothesis testing](#quantum-binary-hypothesis-testing) is the two-state case.

## Quantum binary hypothesis testing

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_binary_hypothesis_testing)

Quantum binary hypothesis testing chooses a two-outcome measurement to distinguish two candidate density operators, trading the probabilities of the two kinds of error.

### Binary test for quantum decoding success

↑ **Parent:** [Quantum binary hypothesis testing](#quantum-binary-hypothesis-testing)

For $k$ equiprobable quantum code states decoded by a [POVM](quantum-measurement.md#positive-operator-valued-measure) $\{E_m\}$, testing whether the classical message label agrees with the decoded output gives a joint binary [POVM](quantum-measurement.md#positive-operator-valued-measure) with $F_0=\sum_m|m\rangle\langle m|\otimes E_m$. Its acceptance probability is the decoding success $1-\epsilon$ on the joint [classical-quantum state](#classical-quantum-state) and $1/k$ on the product of its marginals. Applying [quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy) monotonicity to this test gives the [one-shot classical-quantum coding converse](#one-shot-classical-quantum-coding-converse).

### Quantum channel discrimination

↑ **Parent:** [Quantum binary hypothesis testing](#quantum-binary-hypothesis-testing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_channel_discrimination)

Quantum channel discrimination feeds a common input into one of several candidate [quantum channels](#quantum-channel) and measures the output. An entangled [quantum ancilla](#quantum-ancilla) permits inputs $\rho_{HR}$ and compares $(T_j\otimes\operatorname{id}_R)(\rho_{HR})$; optimal binary discrimination is governed by the [diamond norm](functional-analysis.md#diamond-norm) of the weighted channel difference.

#### Diamond norm of the transposition map

↑ **Parent:** [Quantum channel discrimination](#quantum-channel-discrimination)

For the [transposition map](vector-space.md#transpose) $\Theta:M_d\to M_d$, the [induced trace norm](functional-analysis.md#induced-trace-norm) is $\lVert\Theta\rVert_1=1$, while stabilization gives

$$
\lVert\Theta\rVert_\diamond=d.
$$

Thus an entangled [quantum ancilla](#quantum-ancilla) can amplify the distinguishability witnessed by transposition by a factor of $d$.

<h3 id="holevo-helstrom-theorem">Holevo–Helstrom theorem</h3>

↑ **Parent:** [Quantum binary hypothesis testing](#quantum-binary-hypothesis-testing)

For hypotheses $\rho_0,\rho_1$ with priors $p,1-p$, the optimal success probability is

$$
P_{\rm succ}^*=\frac12\left(1+\|p\rho_0-(1-p)\rho_1\|_1\right).
$$

An optimal measurement projects onto the positive and negative spectral subspaces of the weighted difference.

This is the minimum-error optimum in binary [quantum state discrimination](#quantum-state-discrimination).

#### Equal-prior discrimination of qubit states

↑ **Parent:** [Holevo–Helstrom theorem](#holevo-helstrom-theorem)

For equiprobable [qubit](quantum-mechanics.md#qubit) states with [Bloch vectors](quantum-theory.md#bloch-vector) $r,s$, their density-matrix difference is $(r-s)\cdot\sigma/2$, with [eigenvalues](linear-operator-theory.md#eigenvalue) $\pm|r-s|/2$. An effect $0\le E\le I$ declaring the first state yields success $1/2+\operatorname{Tr}[E(\rho_r-\rho_s)]/2$. Selecting its positive-eigenvalue eigenspace maximizes this [trace](linear-algebra.md#matrix-trace) and proves the displayed result. Measure along $r-s$ and attach the corresponding state labels; if the vectors coincide, no measurement improves on guessing.

## Entanglement monogamy

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_monogamy)

Entanglement monogamy limits how strongly one subsystem can be entangled with several independent partners.

<h3 id="coffman-kundu-wootters-inequality">Coffman--Kundu--Wootters inequality</h3>

↑ **Parent:** [Entanglement monogamy](#entanglement-monogamy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coffman--Kundu--Wootters_inequality)

For a pure state of three qubits, the squared concurrence obeys $C_{A:BC}^2\geq C_{AB}^2+C_{AC}^2$. In particular, if $A$ and $B$ form a maximally entangled pair, then $A$ has no entanglement with $C$.

### Entanglement area law

↑ **Parent:** [Entanglement monogamy](#entanglement-monogamy)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Entanglement_area_law)

An entanglement area law bounds the entropy of a region by a constant times the size of its boundary.

#### Tensor-network area-law bound

↑ **Parent:** [Entanglement area law](#entanglement-area-law)

If a bipartition cuts $n_\partial$ tensor-network bonds of dimension at most $\chi$, its Schmidt rank is at most $\chi^{n_\partial}$ and its [entanglement entropy](von-neumann-entropy.md#entanglement-entropy) is at most $n_\partial\log\chi$.

## Werner state

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Werner_state)

A [Werner state](#werner-state) is a bipartite [density operator](quantum-theory.md#density-matrix) invariant under $U\otimes U$ for every local [unitary operator](vector-space.md#unitary-operator) $U$. An [isotropic quantum state](#isotropic-quantum-state) instead has invariance under $U\otimes\overline U$; these are different families.

## Ancilla bit

↑ **Parent:** [Quantum information theory](quantum-information-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ancilla_bit)

An [ancilla bit](#ancilla-bit) is an auxiliary bit providing workspace in reversible computation. In a [quantum circuit](quantum-circuit.md), an [ancilla qubit](#ancilla-qubit) provides quantum workspace; a general [quantum ancilla](#quantum-ancilla) need not be a single bit.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)
