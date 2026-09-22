# Measurement in quantum mechanics

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurement_in_quantum_mechanics)

A quantum measurement assigns probabilities to classical outcomes through positive operators that sum to the identity. A projective measurement uses mutually orthogonal projections.

**Table of contents**

- [Elitzur-Vaidman bomb tester](#elitzur-vaidman-bomb-tester)
  - [Repeated weak-rotation bomb-test efficiency](#repeated-weak-rotation-bomb-test-efficiency)
- [Measurement backaction](#measurement-backaction)
- [Perfect discrimination of pure states requires orthogonality](#perfect-discrimination-of-pure-states-requires-orthogonality)
- [Quantum nondemolition measurement](#quantum-nondemolition-measurement)
  - [Entanglement-assisted statistical singlet verification](#entanglement-assisted-statistical-singlet-verification)
  - [Bell-pair cost of exact nondemolition singlet verification](#bell-pair-cost-of-exact-nondemolition-singlet-verification)
  - [Entanglement-assisted nondemolition parity measurement](#entanglement-assisted-nondemolition-parity-measurement)
- [Antidistinguishable quantum states](#antidistinguishable-quantum-states)
- [Postselection](#postselection)
  - [Aharonov-Bergmann-Lebowitz rule](#aharonov-bergmann-lebowitz-rule)
    - [Context dependence of pre- and post-selected measurements](#context-dependence-of-pre-and-post-selected-measurements)
      - [N-box pre- and post-selection paradox](#n-box-pre-and-post-selection-paradox)
- [Measurement interaction](#measurement-interaction)
- [Generalized measurement postulate](#generalized-measurement-postulate)
  - [Nonselective quantum measurement](#nonselective-quantum-measurement)
  - [Selective quantum measurement](#selective-quantum-measurement)
  - [Positive operator-valued measure](#positive-operator-valued-measure)
    - [POVM–ensemble duality for the maximally mixed state](#povm-ensemble-duality-for-the-maximally-mixed-state)
    - [Pure positive operator-valued measure](#pure-positive-operator-valued-measure)
    - [Trine qubit POVM](#trine-qubit-povm)
    - [Informationally complete POVM](#informationally-complete-povm)
      - [Tetrahedral qubit POVM](#tetrahedral-qubit-povm)
    - [Binary rank-one qubit POVM](#binary-rank-one-qubit-povm)
- [Projective measurement](#projective-measurement)
  - [Completeness forces orthogonality of measurement projections](#completeness-forces-orthogonality-of-measurement-projections)
  - [Equatorial qubit measurement](#equatorial-qubit-measurement)
    - [Equatorial measurement relabeling at Clifford angles](#equatorial-measurement-relabeling-at-clifford-angles)
  - [Lüders rule](#luders-rule)
    - [Post-measurement state](#post-measurement-state)
    - [Nonselective projective measurement](#nonselective-projective-measurement)
      - [Pinching map](#pinching-map)
      - [Rank-one dephasing](#rank-one-dephasing)
        - [Relative-entropy identity for rank-one dephasing](#relative-entropy-identity-for-rank-one-dephasing)
        - [Support inclusion under rank-one dephasing](#support-inclusion-under-rank-one-dephasing)
- [Quantum state tomography](#quantum-state-tomography)
  - [Interferometric polarization tomography](#interferometric-polarization-tomography)
  - [Single-qubit process tomography](#single-qubit-process-tomography)
- [No information without disturbance](#no-information-without-disturbance)
  - [Quantum instrument](#quantum-instrument)
    - [Unitary dilation of a measurement instrument](#unitary-dilation-of-a-measurement-instrument)
    - [POVM does not determine the post-measurement state](#povm-does-not-determine-the-post-measurement-state)
    - [Local quantum operation](#local-quantum-operation)

## Elitzur-Vaidman bomb tester

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elitzur–Vaidman_bomb_tester)

A [photon](quantum-mechanics.md#photon) in a [quantum superposition](quantum-mechanics.md#quantum-superposition) of a safe path and an absorbing path can sometimes certify a live absorber without being absorbed. Recombination is chosen so that one output is impossible if the absorber is absent. A detection at that output is then an unambiguous successful test. The measurement back-action of a surviving live-absorber trial changes the interference pattern.

### Repeated weak-rotation bomb-test efficiency

↑ **Parent:** [Elitzur-Vaidman bomb tester](#elitzur-vaidman-bomb-tester)

For an [Elitzur-Vaidman bomb tester](#elitzur-vaidman-bomb-tester) using a rotation and its inverse, let $p$ be the probability of entering the absorbing path and $q=1-p$. Conditional on a live absorber, one trial has explosion probability $p$, successful safe identification probability $pq$, and inconclusive probability $q^2$. The inconclusive [projective measurement](#projective-measurement) resets the input, so summing a [geometric series](real-analysis.md#geometric-series) gives the displayed success probability after at most $N$ trials. Its limit is $q/(1+q)$, approaching one half as $p$ tends to zero through positive values. Exactly zero coupling produces no information.

## Measurement backaction

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

A [measurement in quantum mechanics](quantum-measurement.md) changes the conditional [density operator](quantum-theory.md#density-matrix), rather than merely revealing a pre-existing classical state. For an instrument with one operator $K_m$ per outcome, the displayed update occurs with [probability](probability-theory.md#probability) $\operatorname{Tr}(K_m\rho K_m^\dagger)$. Forgetting the outcome gives the corresponding [quantum channel](quantum-information-theory.md#quantum-channel). [Measurement-based quantum feedback](control-theory.md#measurement-based-quantum-feedback) must include this disturbance and the statistical information in the record.

## Perfect discrimination of pure states requires orthogonality

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

If a [positive operator-valued measure](#positive-operator-valued-measure) distinguishes normalized [pure states](quantum-theory.md#pure-state) $|u\rangle,|v\rangle$ with certainty, the effect $E$ for the first answer satisfies $\langle u|E|u\rangle=1$ and $\langle v|E|v\rangle=0$. Positivity of $E$ and $I-E$ implies $E|v\rangle=0$ and $E|u\rangle=|u\rangle$, because a positive operator with zero expectation annihilates the vector. Consequently $\langle u|v\rangle=\langle u|E|v\rangle=0$. Conversely, orthogonal states can be measured with their rank-one [linear projections](vector-space.md#projection-linear-algebra). A common [unitary operator](vector-space.md#unitary-operator) preserves this [inner product](linear-algebra.md#inner-product) and cannot remove the obstruction.

## Quantum nondemolition measurement

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_nondemolition_measurement)

An ideal measurement preserving the measured eigenspaces. In the projective setting, the selective instrument $\rho\mapsto P_j\rho P_j$ preserves every vector within outcome $j$, including coherence inside a degenerate eigenspace. Repeated measurements agree in the absence of intervening dynamics changing the measured quantity. Measuring a finer observable can destroy degeneracy coherence and need not realize the same [Lüders rule](#luders-rule) instrument.

### Entanglement-assisted statistical singlet verification

↑ **Parent:** [Quantum nondemolition measurement](#quantum-nondemolition-measurement)

Choose a shared random axis uniformly from $x,y,z$, perform its [entanglement-assisted nondemolition parity measurement](#entanglement-assisted-nondemolition-parity-measurement) with one [Bell pair](bell-state.md#bell-pair), and accept the anticorrelated parity. The [spin singlet state](bell-state.md#spin-singlet-state) always passes unchanged. The averaged acceptance operator is $\Omega=\sum_j(I-\sigma_j\otimes\sigma_j)/6=P_s+(I-P_s)/3$, so an orthogonal triplet state passes with probability one third. This is a statistical verifier with a nonzero acceptance gap, rather than an exact single-shot singlet-versus-triplet decision. The [Bell-pair cost of exact nondemolition singlet verification](#bell-pair-cost-of-exact-nondemolition-singlet-verification) concerns the stronger zero-error task.

### Bell-pair cost of exact nondemolition singlet verification

↑ **Parent:** [Quantum nondemolition measurement](#quantum-nondemolition-measurement)

Exact singlet verification accepts the [spin singlet state](bell-state.md#spin-singlet-state) with certainty, rejects every orthogonal state, and preserves the singlet on acceptance. Each nonzero accepting [Kraus operator](quantum-information-theory.md#kraus-operator) is then a scalar multiple of the singlet projector, whose [operator Schmidt rank](von-neumann-entropy.md#operator-schmidt-rank) is four. The [local Kraus rank bound from an entangled resource](von-neumann-entropy.md#local-kraus-rank-bound-from-an-entangled-resource) excludes a single shared [Bell pair](bell-state.md#bell-pair), which has [Schmidt rank](von-neumann-entropy.md#schmidt-rank) two. Two shared [Bell pairs](bell-state.md#bell-pair) suffice by a [Bell-state nondemolition measurement](bell-state.md#bell-state-nondemolition-measurement) followed by reporting whether its label is the singlet. This protocol may disturb triplet coherence. The rank bound concerns the resource [Schmidt rank](von-neumann-entropy.md#schmidt-rank), and is not an entropy lower bound of two bits for arbitrary resource states.

### Entanglement-assisted nondemolition parity measurement

↑ **Parent:** [Quantum nondemolition measurement](#quantum-nondemolition-measurement)

Share a [Bell state](bell-state.md) meter pair, apply local system-to-meter [CNOT gates](quantum-theory.md#controlled-not-gate), and measure each meter in the computational basis. The parity of the local meter records measures system $Z_AZ_B$ while preserving all coherence within either parity sector. The complete tuple of local records has [Kraus operator](quantum-information-theory.md#kraus-operator) $P_{u\oplus v}/\sqrt2$. Each local record is uniform, and the nonlocal result requires [local operations and classical communication](bell-state.md#local-operations-and-classical-communication) to compare records. A local [Hadamard gate](quantum-theory.md#hadamard-gate) conjugation supplies the corresponding $X_AX_B$ measurement.

## Antidistinguishable quantum states

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

A finite family of [quantum states](quantum-mechanics.md#quantum-state) is antidistinguishable if a [measurement in quantum mechanics](quantum-measurement.md) has labelled outcomes such that each outcome has zero probability for its corresponding state, while the outcomes form a complete [measurement in quantum mechanics](quantum-measurement.md). It can exclude a state without identifying which state was prepared. The [PBR exclusion measurement for zero and plus](quantum-theory.md#pbr-exclusion-measurement-for-zero-and-plus) supplies a four-state [projective measurement](#projective-measurement) example.

## Postselection

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

Postselection conditions a [measurement in quantum mechanics](quantum-measurement.md) on a specified outcome. If its branch acts by a [linear operator](vector-space.md#linear-operator) $K$ on a normalized input $|b\rangle$, its [probability](probability-theory.md#probability) is $\|K|b\rangle\|^2$, and its normalized output is $K|b\rangle/\|K|b\rangle\|$. This conditional state is defined only when the probability is nonzero. Physically unsuccessful trials are discarded; postselection is not a deterministic implementation of the nonlinear normalization map.

### Aharonov-Bergmann-Lebowitz rule

↑ **Parent:** [Postselection](#postselection)

For an ideal [projective measurement](#projective-measurement) with the [Lüders rule](#luders-rule), condition on both an initial [quantum state preparation](quantum-circuit.md#quantum-state-preparation) and a final successful [postselection](#postselection). Its outcome probabilities are proportional to $|\langle b|P_j|a\rangle|^2$, where $a$ is the forward-evolved initial state and $b$ the backward-evolved final state. The normalization must be nonzero. The expression is symmetric in these two boundary states, although its derivation uses the ordinary [Born rule](quantum-mechanics.md#born-rule) and conditional state update.

<h4 id="context-dependence-of-pre-and-post-selected-measurements">Context dependence of pre- and post-selected measurements</h4>

↑ **Parent:** [Aharonov-Bergmann-Lebowitz rule](#aharonov-bergmann-lebowitz-rule)

In the [ABL rule](#aharonov-bergmann-lebowitz-rule), probabilities depend on the full intermediate [measurement in quantum mechanics](quantum-measurement.md) instrument. A binary [Lüders rule](#luders-rule) [measurement in quantum mechanics](quantum-measurement.md) preserves coherence within its unresolved complement, whereas a fully resolved [projective measurement](#projective-measurement) removes it. Summing fine-grained probabilities after [measurement in quantum mechanics](quantum-measurement.md) does not generally reproduce the coarse-grained experiment. Different [postselection](#postselection) success rates are part of the distinction.

<h5 id="n-box-pre-and-post-selection-paradox">N-box pre- and post-selection paradox</h5>

↑ **Parent:** [Context dependence of pre- and post-selected measurements](#context-dependence-of-pre-and-post-selected-measurements)

For a uniform prestate in $N+1$ dimensions and poststate proportional to $\sum_{i=1}^N|i\rangle-(N-1)|N+1\rangle$, each binary question $P_i$ versus $I-P_i$ has conditional probability one for $i\leq N$. A fully resolved [measurement in quantum mechanics](quantum-measurement.md) instead assigns $1/D$ to each of the first $N$ outcomes and $(N-1)^2/D$ to the last. The [context dependence of pre- and post-selected measurements](#context-dependence-of-pre-and-post-selected-measurements) explains why these alternative certainties do not imply simultaneous properties.

## Measurement interaction

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

A measurement interaction correlates a measured system's alternatives with distinguishable states of an apparatus. Reading the apparatus then implements the associated [measurement in quantum mechanics](quantum-measurement.md).

## Generalized measurement postulate

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

A generalized quantum measurement is specified by operators $M_i$ satisfying $\sum_iM_i^\dagger M_i=I$. On input $\rho$, outcome $i$ has probability $\operatorname{Tr}(M_i^\dagger M_i\rho)$ and conditional state $M_i\rho M_i^\dagger/\operatorname{Tr}(M_i^\dagger M_i\rho)$.

### Nonselective quantum measurement

↑ **Parent:** [Generalized measurement postulate](#generalized-measurement-postulate)

A nonselective [measurement in quantum mechanics](quantum-measurement.md) averages over outcomes that are not read or not communicated. Its [quantum channel](quantum-information-theory.md#quantum-channel) is $\rho\mapsto\sum_iA_i\rho A_i^\dagger$, with $\sum_iA_i^\dagger A_i=I$. The completeness condition makes the channel trace preserving. The average equals $\sum_i p_i\rho_i$, where $\rho_i$ are the conditional states from a [selective quantum measurement](#selective-quantum-measurement). A [nonselective projective measurement](#nonselective-projective-measurement) is the special case in which the operators are orthogonal projectors.

### Selective quantum measurement

↑ **Parent:** [Generalized measurement postulate](#generalized-measurement-postulate)

A selective [measurement in quantum mechanics](quantum-measurement.md) conditions on a known outcome. For [Kraus operator](quantum-information-theory.md#kraus-operator) $A_i$, the [Born rule](quantum-mechanics.md#born-rule) gives $p_i=\operatorname{Tr}(A_i^\dagger A_i\rho)$ and the conditional [density operator](quantum-theory.md#density-matrix) is $A_i\rho A_i^\dagger/p_i$ when $p_i>0$. Conditioning changes the state and can change the conditional [reduced density matrix](bell-state.md#reduced-density-matrix) of a correlated remote system. That conditional state is available as such only to an observer with the outcome information.

### Positive operator-valued measure

↑ **Parent:** [Generalized measurement postulate](#generalized-measurement-postulate)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_operator-valued_measure)

A positive operator-valued measure is a family of positive operators $E_i$ satisfying $\sum_iE_i=I$. It determines measurement probabilities $\Pr(i)=\operatorname{Tr}(E_i\rho)$; choosing measurement operators with $E_i=M_i^\dagger M_i$ additionally determines state updates.

<h4 id="povm-ensemble-duality-for-the-maximally-mixed-state">POVM–ensemble duality for the maximally mixed state</h4>

↑ **Parent:** [Positive operator-valued measure](#positive-operator-valued-measure)

A [POVM](#positive-operator-valued-measure) $\{E_i\}$ in dimension $d$ corresponds to a [quantum state ensemble](quantum-theory.md#quantum-state-ensemble) with $p_i=\operatorname{Tr}(E_i)/d$ and $\rho_i=E_i/\operatorname{Tr}(E_i)$, omitting zero effects. Its average is the [maximally mixed state](quantum-theory.md#maximally-mixed-state) $I/d$. Conversely any ensemble with that average defines a POVM by $E_i=dp_i\rho_i$. These transformations are inverse. A [pure POVM](#pure-positive-operator-valued-measure) corresponds exactly to a pure-state ensemble decomposition of $I/d$.

#### Pure positive operator-valued measure

↑ **Parent:** [Positive operator-valued measure](#positive-operator-valued-measure)

A [POVM](#positive-operator-valued-measure) whose nonzero effects have rank one, $E_i=w_i|\psi_i\rangle\langle\psi_i|$, with normalized [pure states](quantum-theory.md#pure-state) and $w_i>0$. Completeness is $\sum_iw_i|\psi_i\rangle\langle\psi_i|=I$. This use of pure concerns effect rank, and does not mean an extremal point in the convex set of all POVMs.

#### Trine qubit POVM

↑ **Parent:** [Positive operator-valued measure](#positive-operator-valued-measure)

Choose three pure [qubit](quantum-mechanics.md#qubit) states whose unit [Bloch vectors](quantum-theory.md#bloch-vector) are coplanar, sum to zero and have pairwise angle $120$ degrees. The three effects $E_j=\frac23|\phi_j\rangle\langle\phi_j|$ sum to the identity, giving a [POVM](#positive-operator-valued-measure). If an input is the state orthogonal to $\phi_1$ or to $\phi_2$, outcome one excludes the first input and outcome two excludes the second. Each conclusive outcome has probability one half on its corresponding input; the third outcome is inconclusive with probability one half on either input. This gives [unambiguous quantum state discrimination](quantum-theory.md#unambiguous-quantum-state-discrimination), rather than identification on every trial.

#### Informationally complete POVM

↑ **Parent:** [Positive operator-valued measure](#positive-operator-valued-measure)

A [POVM](#positive-operator-valued-measure) is informationally complete if its outcome probabilities determine every input [density operator](quantum-theory.md#density-matrix) uniquely. Its effects must span the real space of Hermitian operators. For a qubit, normalization leaves at most $m-1$ independent probabilities from $m$ outcomes; an arbitrary [Bloch vector](quantum-theory.md#bloch-vector) has three real parameters, so one fixed informationally complete measurement requires at least four outcomes. Using several differently oriented binary measurements is a different experimental setting and can also perform [quantum state tomography](#quantum-state-tomography).

##### Tetrahedral qubit POVM

↑ **Parent:** [Informationally complete POVM](#informationally-complete-povm)

Choose the four unit [Bloch vectors](quantum-theory.md#bloch-vector) at the vertices of a [regular tetrahedron](geometry-and-topology.md#regular-tetrahedron), so $\sum_i\mathbf n_i=0$ and $\sum_i\mathbf n_i\mathbf n_i^T=4I/3$. The displayed four positive rank-one effects sum to $I$. On input $(I+\mathbf r\cdot\boldsymbol\sigma)/2$, their probabilities are $p_i=(1+\mathbf r\cdot\mathbf n_i)/4$, giving the reconstruction $\mathbf r=3\sum_i p_i\mathbf n_i$. This realizes the smallest fixed qubit [informationally complete POVM](#informationally-complete-povm).

#### Binary rank-one qubit POVM

↑ **Parent:** [Positive operator-valued measure](#positive-operator-valued-measure)

Two positive rank-one effects summing to $I$ in dimension two must be complementary [orthogonal projections](hilbert-space.md#orthogonal-projection). Write the first as $\alpha|\psi\rangle\langle\psi|$ with normalized $\psi$. The second has eigenvalues $1-\alpha$ and $1$, so its rank-one condition forces $\alpha=1$. The two unit [Bloch vectors](quantum-theory.md#bloch-vector) are antipodal, and this [POVM](#positive-operator-valued-measure) is a [projective measurement](#projective-measurement).

## Projective measurement

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

A projective measurement is specified by mutually orthogonal projections $P_i$ with $\sum_iP_i=I$. On a state $\rho$, outcome $i$ has probability $\operatorname{Tr}(P_i\rho)$.

This is the projection-valued special case of a [measurement in quantum mechanics](quantum-measurement.md); general POVM effects need not be projections.

### Completeness forces orthogonality of measurement projections

↑ **Parent:** [Projective measurement](#projective-measurement)

Let self-adjoint [orthogonal projections](hilbert-space.md#orthogonal-projection) $P_i$ sum to the identity. For $v$ in the range of $P_j$,

$$
\|v\|^2=\sum_i\langle v,P_iv\rangle=\sum_i\|P_iv\|^2.
$$

The $j$th term already equals $\|v\|^2$, so $P_iv=0$ for every $i\neq j$. Hence $P_iP_j=P_jP_i=0$ and the [projective measurement](#projective-measurement) operators commute.

// Target: quantum-theory.bigb

### Equatorial qubit measurement

↑ **Parent:** [Projective measurement](#projective-measurement)

The orthonormal [quantum states](quantum-mechanics.md#quantum-state) $|\alpha_s\rangle=(|0\rangle+(-1)^se^{-i\alpha}|1\rangle)/\sqrt2$, $s=0,1$, define an equatorial [projective measurement](#projective-measurement). The measured [observable](quantum-mechanics.md#observable) is $\cos\alpha\,X-\sin\alpha\,Y$, with [eigenvalue](linear-operator-theory.md#eigenvalue) $(-1)^s$. Thus $\alpha=0$ measures $X$, and $\alpha=\pi/2$ measures $-Y$ with these outcome labels. The sign convention matters when comparing different definitions of equatorial bases.

#### Equatorial measurement relabeling at Clifford angles

↑ **Parent:** [Equatorial qubit measurement](#equatorial-qubit-measurement)

For $|v_s(\eta)\rangle=(|0\rangle+(-1)^s e^{i\eta}|1\rangle)/\sqrt2$, adding $\pi$ exchanges the two outcomes of the same [projective measurement](#projective-measurement). At an angle $\phi=j\pi/2$, the choices $\phi$ and $-\phi$ therefore specify the same unordered pair of projectors: their labels differ by $j\bmod2$. An adaptive choice between these signs can be replaced by a fixed measurement and a classical label exchange. Together with [Pauli-frame propagation along a measurement wire](bell-state.md#pauli-frame-propagation-along-a-measurement-wire), this permits simultaneous measurements when all adaptive sign changes occur at these [Clifford gate](quantum-circuit.md#clifford-gate) angles.

<h3 id="luders-rule">Lüders rule</h3>

↑ **Parent:** [Projective measurement](#projective-measurement)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lüders_rule)

Conditional on outcome $i$ of a [projective measurement](#projective-measurement), the Lüders rule updates the state to

$$
\rho_i=\frac{P_i\rho P_i}{\operatorname{Tr}(P_i\rho)}.
$$

#### Post-measurement state

↑ **Parent:** [Lüders rule](#luders-rule)

The post-measurement state is the conditional quantum state after a specified measurement outcome. For a [projective measurement](#projective-measurement), it is given by the [Lüders rule](#luders-rule).

#### Nonselective projective measurement

↑ **Parent:** [Lüders rule](#luders-rule)

If the outcome of a projective measurement $\{P_i\}$ is discarded, its nonselective state update is the pinching channel

$$
\rho\longmapsto\sum_iP_i\rho P_i.
$$

It removes coherence between distinct measurement subspaces.

##### Pinching map

↑ **Parent:** [Nonselective projective measurement](#nonselective-projective-measurement)

For mutually orthogonal projectors summing to the identity, a pinching map discards coherences between their ranges while preserving each diagonal block. It is a [quantum channel](quantum-information-theory.md#quantum-channel) with [Kraus operators](quantum-information-theory.md#kraus-operator) $P_i$, and a [unital quantum channel](quantum-information-theory.md#unital-quantum-channel). A state is fixed by pinching exactly when it commutes with every projector.

##### Rank-one dephasing

↑ **Parent:** [Nonselective projective measurement](#nonselective-projective-measurement)

In an [orthonormal basis](linear-algebra.md#orthonormal-basis), rank-one dephasing is the [quantum channel](quantum-information-theory.md#quantum-channel) $\Delta(\rho)=\sum_i|\psi_i\rangle\langle\psi_i|\rho|\psi_i\rangle\langle\psi_i|$. It removes off-diagonal entries while preserving the basis probabilities. Its output [Von Neumann entropy](von-neumann-entropy.md) is their [Shannon entropy](information-theory.md#information-entropy), and the [relative-entropy identity for rank-one dephasing](#relative-entropy-identity-for-rank-one-dephasing) quantifies the entropy increase.

###### Relative-entropy identity for rank-one dephasing

↑ **Parent:** [Rank-one dephasing](#rank-one-dephasing)

Because $\log\Delta(\rho)$ is diagonal, $\operatorname{Tr}(\rho\log\Delta(\rho))=\operatorname{Tr}(\Delta(\rho)\log\Delta(\rho))$. Hence $D_{\mathrm{rel}}(\rho\|\Delta(\rho))=S(\Delta(\rho))-S(\rho)$. [Support inclusion under rank-one dephasing](#support-inclusion-under-rank-one-dephasing) handles zero probabilities, and [Klein's inequality](vector-space.md#klein-s-inequality) makes the difference nonnegative. Equality holds exactly when the state was already diagonal.

###### Support inclusion under rank-one dephasing

↑ **Parent:** [Rank-one dephasing](#rank-one-dephasing)

If $p_i=\langle\psi_i|\rho|\psi_i\rangle=0$, positivity gives $\sqrt\rho|\psi_i\rangle=0$, so the corresponding basis vector is in $\ker\rho$. Therefore $\ker\Delta(\rho)\subseteq\ker\rho$, and $\operatorname{supp}\rho\subseteq\operatorname{supp}\Delta(\rho)$. This makes the [quantum relative entropy](von-neumann-entropy.md#quantum-relative-entropy) of $\rho$ relative to its [rank-one dephasing](#rank-one-dephasing) finite.

## Quantum state tomography

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_state_tomography)

Quantum state tomography estimates enough expectation values on many identically prepared systems to reconstruct their [density operator](quantum-theory.md#density-matrix). A single ordinary specimen cannot provide arbitrarily many independent samples without disturbance.

### Interferometric polarization tomography

↑ **Parent:** [Quantum state tomography](#quantum-state-tomography)

A [polarizing beam splitter](optics.md#polarizing-beam-splitter) converts a [photon polarization](quantum-mechanics.md#photon-polarization) [qubit](quantum-mechanics.md#qubit) to two paths. Rotating one arm's [photon polarization](quantum-mechanics.md#photon-polarization) to match the other and recombining at a balanced [beam splitter](optics.md#beam-splitter) gives $P_1(\theta)=1/2+\operatorname{Re}(\alpha^*\beta e^{i\theta})$. Measurements at phases zero and $\pi/2$ recover the transverse [Bloch vector](quantum-theory.md#bloch-vector) components; direct counts in the two separated arms recover the population difference. All three components, rather than a fringe alone, determine an arbitrary [photon polarization](quantum-mechanics.md#photon-polarization) [density matrix](quantum-theory.md#density-matrix).

// Target: quantum-theory.bigb

### Single-qubit process tomography

↑ **Parent:** [Quantum state tomography](#quantum-state-tomography)

To identify the physical channel $\rho\mapsto V\rho V^\dagger$ of a single-[qubit](quantum-mechanics.md#qubit) [unitary gate](quantum-circuit.md#quantum-logic-gate), prepare each of the three positive [Pauli matrix](algebra.md#pauli-matrices) [eigenstates](quantum-mechanics.md#eigenstate) and estimate each output Pauli [expectation](probability-theory.md#expected-value). Their nine means are

$$
R_{ij}=\frac12\operatorname{Tr}(\sigma_iV\sigma_jV^\dagger),\qquad i,j\in\{x,y,z\}.
$$

They determine the [Bloch vector](quantum-theory.md#bloch-vector) [rotation](riemannian-geometry.md#rotation-mathematics) $\boldsymbol r\mapsto R\boldsymbol r$, hence the channel on all states. If two gates have the same channel, their relative unitary commutes with all three [Pauli matrices](algebra.md#pauli-matrices): commuting with $Z$ forces it diagonal and commuting with $X$ forces equal diagonal entries. Thus they differ by a scalar [global phase](quantum-mechanics.md#global-phase), proving uniqueness up to that phase. This procedure needs no controlled gate or [eigenstate](quantum-mechanics.md#eigenstate) of the unknown gate. Estimating its bounded measurement means to error $\epsilon$ with fixed confidence uses order $\epsilon^{-2}$ repetitions. It determines the relative [eigenphases](vector-space.md#eigenphase) but cannot determine an overall [eigenvalue](linear-operator-theory.md#eigenvalue) phase from uncontrolled gate access alone.

## No information without disturbance

↑ **Parent:** [Measurement in quantum mechanics](quantum-measurement.md)

If a [quantum instrument](#quantum-instrument) leaves every input state unchanged even after conditioning on its classical output, then its output distribution is independent of the input state. Thus an ordinary quantum process cannot learn arbitrary state information while preserving every state.

### Quantum instrument

↑ **Parent:** [No information without disturbance](#no-information-without-disturbance)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_instrument)

A quantum instrument associates each classical outcome with a completely positive trace-nonincreasing map; summing the outcome maps gives a [quantum channel](quantum-information-theory.md#quantum-channel). It specifies both outcome probabilities and conditional output states.

#### Unitary dilation of a measurement instrument

↑ **Parent:** [Quantum instrument](#quantum-instrument)

For [Kraus operators](quantum-information-theory.md#kraus-operator) satisfying $\sum_iA_i^\dagger A_i=I$, the map $V|\phi\rangle=\sum_iA_i|\phi\rangle\otimes|i\rangle$ is an [isometry](riemannian-geometry.md#isometry). Implement it by a [unitary operator](vector-space.md#unitary-operator) on the system and a [quantum ancilla](quantum-information-theory.md#quantum-ancilla), initially in an extra unused state $|0\rangle$. Projecting the output [quantum ancilla](quantum-information-theory.md#quantum-ancilla) onto $|i\rangle$ gives joint unnormalized state $A_i\rho A_i^\dagger\otimes|i\rangle\langle i|$. The outcome [probability](probability-theory.md#probability) is $\operatorname{Tr}(A_i\rho A_i^\dagger)$, and the conditional system state is $A_i\rho A_i^\dagger$ divided by this [probability](probability-theory.md#probability). The unused level can be merged into the first [orthogonal projection](hilbert-space.md#orthogonal-projection) without changing any outcome on the prepared state, giving a complete [projective measurement](#projective-measurement) with exactly the original outcome labels.

// Target: quantum-theory.bigb

#### POVM does not determine the post-measurement state

↑ **Parent:** [Quantum instrument](#quantum-instrument)

A [POVM](#positive-operator-valued-measure) fixes outcome probabilities, but a [quantum instrument](#quantum-instrument) additionally fixes the conditional output state. For computational-basis effects $E_y=|y\rangle\langle y|$, the operators $M_y=|y\rangle\langle y|$ leave the measured eigenstate as output, whereas $N_y=|0\rangle\langle y|$ reset every outcome to $|0\rangle$. Both have $M_y^\dagger M_y=N_y^\dagger N_y=E_y$. Thus a specification of effects alone cannot select a unique joint state that retains the measured quantum system.

#### Local quantum operation

↑ **Parent:** [Quantum instrument](#quantum-instrument)

A [local quantum operation](#local-quantum-operation) on one tensor-factor subsystem acts as $\Phi_A\otimes\operatorname{id}_B$, with $\Phi_A$ completely positive. An individual outcome branch can decrease trace, while the sum over outcomes of a normalized instrument preserves trace. The unselected operation consequently leaves the remote reduced state unchanged. In a local field algebra, Kraus operators inside one region and commuting with a distant observable give an analogous no-signalling statement. Locality of the operation must be established; an arbitrary globally defined projection is not automatically a physically local measurement.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (61)

- [Antidistinguishable quantum states](#antidistinguishable-quantum-states)
- [Context dependence of pre- and post-selected measurements](#context-dependence-of-pre-and-post-selected-measurements)
- [Entanglement monotone](bell-state.md#entanglement-monotone)
- [Logical depth of a measurement pattern](quantum-circuit.md#logical-depth-of-a-measurement-pattern)
- [Measurement backaction](#measurement-backaction)
- [Measurement-based quantum computation](quantum-circuit.md#measurement-based-quantum-computation)
- [Measurement interaction](#measurement-interaction)
- [N-box pre- and post-selection paradox](#n-box-pre-and-post-selection-paradox)
- [Nonselective quantum measurement](#nonselective-quantum-measurement)
- [Ontological model of a quantum system](quantum-theory.md#ontological-model-of-a-quantum-system)
- [Optimal stochastic conversion of a two-qubit pure state](bell-state.md#optimal-stochastic-conversion-of-a-two-qubit-pure-state)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-61.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-52.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/a/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53.md#4/b/protocol-2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-51.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-57.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#1/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#4/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#4/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#4/a/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#10d/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-323.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-325.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-325.md#4/b/solution)
- [Postselection](#postselection)
- [Projective measurement](#projective-measurement)
- [Pusey-Barrett-Rudolph theorem](quantum-theory.md#pusey-barrett-rudolph-theorem)
- [Quantum key distribution](computer-science.md#quantum-key-distribution)
- [Quantum logic gate](quantum-circuit.md#quantum-logic-gate)
- [Quantum state discrimination](quantum-information-theory.md#quantum-state-discrimination)
- [Reciprocal-state construction of unambiguous discrimination](quantum-theory.md#reciprocal-state-construction-of-unambiguous-discrimination)
- [Relativistic causality constraint on an ideal nonlocal measurement](quantum-theory.md#relativistic-causality-constraint-on-an-ideal-nonlocal-measurement)
- [Remote state preparation](quantum-information-theory.md#remote-state-preparation)
- [Selective quantum measurement](#selective-quantum-measurement)
- [Trace-distance-preserving binary measurement](quantum-theory.md#trace-distance-preserving-binary-measurement)
- [Two-outcome LOCC dilution of a Bell pair](bell-state.md#two-outcome-locc-dilution-of-a-bell-pair)
