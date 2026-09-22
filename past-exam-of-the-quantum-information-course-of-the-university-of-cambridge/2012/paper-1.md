# Paper 1

↑ **Parent:** [2012](../2012.md)

Source: [Cambridge examination PDF, physical pages 490–492; printed paper 250](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1).

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the [computational basis](../../quantum-theory.md#computational-basis) in the stated order and let the rightmost operation act first. The [controlled phase gate](../../quantum-theory.md#controlled-phase-gate) is $|0\rangle\langle0|\otimes I+|1\rangle\langle1|\otimes Z$. From the rotation definition,

$$
R_y(\theta)=\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix},\qquad
R_y(\pi/2)ZR_y(-\pi/2)=X.
$$

The control-zero block remains the identity, and the control-one block becomes $X$. Thus

$$
\boxed{R_y^{(2)}(\pi/2)U_{\rm CP}R_y^{(2)}(-\pi/2)=U_{\rm CNOT}.}
$$

This proves the relation for arbitrary [superpositions](../../vector-space.md#superposition-principle), rather than only for computational-basis probabilities.

For the second relation write $S=U_{\rm SW}^{1/2}$. Its central block is $\bigl(\begin{smallmatrix}a&b\\b&a\end{smallmatrix}\bigr)$, with $a=(1+i)/2$, $b=(1-i)/2$. Because $a^2=i/2$, $b^2=-i/2$ and $ab=1/2$, direct multiplication gives

$$
S R_z^{(1)}(\pi) S=\operatorname{diag}(-i,1,-1,i).
$$

Meanwhile $R_z^{(1)}(\pi/2)R_z^{(2)}(-\pi/2)=\operatorname{diag}(1,-i,i,1)$. Multiplying these diagonal matrices and the overall factor $i$ gives

$$
\boxed{iR_z^{(1)}(\pi/2)R_z^{(2)}(-\pi/2)S R_z^{(1)}(\pi)S
=\operatorname{diag}(1,1,1,-1)=U_{\rm CP}.}
$$

The supplied $S$ is indeed a [square root of the SWAP gate](../../quantum-theory.md#square-root-of-the-swap-gate): $S^2$ exchanges $|01\rangle$ and $|10\rangle$ while fixing the other basis states. It acts as one on the triplet subspace and as $i$ on the singlet subspace.

For an isotropic [exchange interaction](../../electromagnetism.md#exchange-interaction) with [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian) $H=J(t)\,\boldsymbol\sigma_1\cdot\boldsymbol\sigma_2/4$, define $\varphi=\int J(t)dt/\hbar$. Triplet and singlet energies differ by $J$, so

$$
U(\varphi)=e^{-i\varphi/4}(P_T+e^{i\varphi}P_S).
$$

An exchange pulse with $\varphi=\pi/2$ therefore implements $e^{-i\pi/8}S$. Two such pulses, interspersed with the specified local rotations, implement the [controlled phase gate](../../quantum-theory.md#controlled-phase-gate); the initial and final target rotations then turn it into a [CNOT gate](../../quantum-theory.md#controlled-not-gate). Their common overall phase has no effect on an isolated gate's outcome probabilities; a subsequently controlled version must keep track of conditional phases.

<a id="1/image-cnot-synthesis-from-two-square-root-of-swap-exchange-pulses-and-local-rotations-with-time-running-left-to-right"></a>
![](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2012/paper-1-exchange-cnot-circuit.png)

**[Figure 1](#1/image-cnot-synthesis-from-two-square-root-of-swap-exchange-pulses-and-local-rotations-with-time-running-left-to-right). CNOT synthesis from two square-root-of-SWAP exchange pulses and local rotations, with time running left to right**.

The construction converts a physically available two-spin interaction into a standard entangling gate, which together with arbitrary one-qubit rotations supplies [universal quantum computation](../../computer-science.md#universal-quantum-computation). Practical operation needs calibrated exchange pulse area and timing, individually controllable rotations, and reproducible phase references. Charge noise can change $J$; magnetic-field gradients add unwanted single-spin evolution, and anisotropic exchange modifies the assumed [Hamiltonian](../../hamiltonian-mechanics.md#hamiltonian). Pulses must suppress leakage into unwanted orbital states while finishing before excessive [decoherence](../../quantum-theory.md#quantum-decoherence). Readout, preparation, cross-talk and the extra operations in this decomposition all affect the achieved [quantum gate fidelity](../../quantum-information-theory.md#quantum-gate-fidelity). The algebraic identity alone does not establish a [fault-tolerant quantum computation](../../quantum-error-correction.md#fault-tolerant-quantum-computation) implementation.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Include Alice's detector and environment before taking a [partial trace](../../quantum-theory.md#partial-trace). Ideal measurement produces the global state

$$
|\Psi_1\rangle=\frac1{\sqrt2}\bigl(|01\rangle|d_{0A}E_{0A}\rangle-|10\rangle|d_{1A}E_{1A}\rangle\bigr).
$$

[Orthogonality](../../inner-product.md#orthogonal-vectors) of the two record states removes their cross terms from the reduced state of the particles:

$$
\boxed{\rho_{AB}^{(1)}=\frac12|01\rangle\langle01|+\frac12|10\rangle\langle10|
=\operatorname{diag}(0,1/2,1/2,0).}
$$

This [nonselective quantum measurement](../../quantum-measurement.md#nonselective-quantum-measurement) has changed the initially entangled singlet into a separable, classically anticorrelated reduced state. Its [entropy](../../entropy.md) is one bit, although the full particles-plus-records state is still pure under the assumed unitary dynamics. The [reduced density matrix](../../bell-state.md#reduced-density-matrix) is an [improper mixture](../../density-matrix.md#improper-mixture); tracing the environment does not by itself assert a literal collapse of that global state.

The [Born rule](../../wave-function.md#born-rule) gives Alice outcomes zero and one with equal [probability](../../probability-theory.md#probability). Conditional on a recorded result, the [selective quantum measurement](../../quantum-measurement.md#selective-quantum-measurement) assigns $|01\rangle$ or $|10\rangle$ to the particles. The unitary measurement coupling and orthogonal records explain [decoherence](../../quantum-theory.md#quantum-decoherence) in this basis; they do not supply an additional rule selecting a unique outcome. That is part of the [measurement problem](../../quantum-theory.md#measurement-problem). In a collapse postulate the individual outcome is stochastic; other interpretations account for outcome experience differently while retaining these operational probabilities.

When Bob makes the same kind of measurement, the global state becomes

$$
|\Psi_2\rangle=\frac1{\sqrt2}\bigl(
|01\rangle|d_{0A}E_{0A}\rangle|d_{1B}E_{1B}\rangle
-|10\rangle|d_{1A}E_{1A}\rangle|d_{0B}E_{0B}\rangle\bigr).
$$

Tracing both laboratories gives **the same reduced matrix**, $\rho_{AB}^{(2)}=\rho_{AB}^{(1)}$. Bob has added a correlated record, not restored the lost reduced coherence. If Alice's outcome is known, Bob's opposite outcome is certain in this ideal common basis. Without that record, his marginal is $I/2$, so his outcome remains equiprobable. Alice cannot choose her random result or use this [correlation](../../variance.md#pearson-correlation-coefficient) for faster-than-light signalling, consistently with [quantum no-signalling](../../quantum-theory.md#quantum-no-signalling).

These common-basis measurements alone do **not** distinguish quantum predictions from a local source sending opposite preassigned bits. To test that explanation, prepare fresh singlets and let the observers independently choose among incompatible measurement axes before recording each result. For singlet [spin](../../angular-momentum-operator.md#spin) measurements along unit vectors $\mathbf a,\mathbf b$, quantum mechanics predicts $E(\mathbf a,\mathbf b)=-\mathbf a\cdot\mathbf b$. The [CHSH inequality](../../foundations-of-quantum-mechanics.md#chsh-inequality) bounds $|S|\leq2$ for Bell-local models with measurement-independent settings. Choosing

$$
\mathbf a=\widehat z,\quad\mathbf a'=\widehat x,\quad
\mathbf b=(\widehat z+\widehat x)/\sqrt2,\quad
\mathbf b'=(\widehat z-\widehat x)/\sqrt2
$$

gives $S=E(\mathbf a,\mathbf b)+E(\mathbf a,\mathbf b')+E(\mathbf a',\mathbf b)-E(\mathbf a',\mathbf b')=-2\sqrt2$. A suitable [Bell test](../../foundations-of-quantum-mechanics.md#bell-test) constrains that class of explanations. Independently chosen settings, control of detection bias and separation of the measurement events matter when interpreting an actual experiment.

<a id="2/image-singlet-coherence-is-lost-from-the-reduced-density-matrix-after-a-local-unread-measurement-common-axis-anticorrelation-survives"></a>
![](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2012/paper-1-singlet-dephasing-correlation.png)

**[Figure 2](#2/image-singlet-coherence-is-lost-from-the-reduced-density-matrix-after-a-local-unread-measurement-common-axis-anticorrelation-survives). Singlet coherence is lost from the reduced density matrix after a local unread measurement; common-axis anticorrelation survives**.

If Alice first performs the fixed-axis irreversible measurement described above, the resulting [mixed state](../../density-matrix.md#mixed-state) has $E(\mathbf a,\mathbf b)=-a_zb_z$ and cannot supply that singlet violation. The incompatible settings must belong to the Bell measurement itself. Moreover, Bell violations do not choose among all interpretations of quantum mechanics: interpretations sharing the Born predictions remain observationally equivalent for this experiment. Objective-collapse modifications could instead require additional [interference](../../physical-optics.md#interference-wave-propagation) tests with specified departures from unitary dynamics.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [positive operator-valued measure](../../quantum-measurement.md#positive-operator-valued-measure) consists of [positive semidefinite](../../quadratic-form.md#positive-semidefinite-matrix) effects $E_r$ with $\sum_rE_r=I$. Its outcome probabilities are $p_r=\operatorname{Tr}(\rho E_r)$, which are nonnegative and sum to one. Unlike a [projective measurement](../../quantum-measurement.md#projective-measurement), its effects need not be mutually [orthogonal projections](../../hilbert-space.md#orthogonal-projection), and there can be more outcomes than the system's Hilbert-space dimension.

For example, choose three equatorial [Bloch vectors](../../density-matrix.md#bloch-vector) $\mathbf n_r$ separated by $120^\circ$ and set $E_r=(I+\mathbf n_r\cdot\boldsymbol\sigma)/3$. Each effect has [eigenvalues](../../linear-operator-theory.md#eigenvalue) zero and $2/3$, and the vectors sum to zero, so the three effects sum to $I$. This [trine qubit POVM](../../quantum-measurement.md#trine-qubit-povm) gives $p_r=(1+\mathbf s\cdot\mathbf n_r)/3$ for input [Bloch vector](../../density-matrix.md#bloch-vector) $\mathbf s$. It cannot be a three-outcome orthogonal [projective measurement](../../quantum-measurement.md#projective-measurement) on that [qubit](../../quantum-system.md#qubit).

A physical implementation can couple the system to an [ancilla](../../quantum-information-theory.md#quantum-ancilla) and projectively measure the enlarged system. More generally, operators $M_{r\alpha}$ implement an outcome with $E_r=\sum_\alpha M_{r\alpha}^\dagger M_{r\alpha}$; the normalized conditional state is $\sum_\alpha M_{r\alpha}\rho M_{r\alpha}^\dagger/p_r$. Thus a [POVM does not determine the post-measurement state](../../quantum-measurement.md#povm-does-not-determine-the-post-measurement-state): different [measurement instruments](../../quantum-measurement.md#quantum-instrument) can have the same outcome probabilities and different disturbance. [Generalized measurements](../../quantum-measurement.md#generalized-measurement-postulate) are useful for state discrimination and realistic detection, including explicitly modeled inconclusive outcomes.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

[Quantum cryptography](../../computer-science.md#quantum-cryptography) includes [quantum key distribution](../../computer-science.md#quantum-key-distribution), which establishes a shared secret key rather than transmitting an arbitrary plaintext directly. In [BB84](../../quantum-theory.md#bb84), Alice randomly prepares one of the two computational-basis or two complementary-basis [qubit](../../quantum-system.md#qubit) states; Bob randomly measures in either basis. They announce bases over an authenticated classical channel and retain the positions where their choices agree, about half in the ideal unbiased case. They test a subset for errors, reconcile the remaining strings, and apply [privacy amplification](../../computer-science.md#privacy-amplification) to remove a bounded eavesdropper's information. A protocol can abort when the observed data do not support a secret key.[1984 protocol; authors' later upload of the original proceedings contribution](../../physics-bibliography.md#quantum-cryptography-public-key-distribution-and-coin-tossing-by-charles-h-bennett-and-gilles-brassard)

Nonorthogonal states cannot be perfectly copied by a state-independent device, by the [no-cloning theorem](../../quantum-theory.md#no-cloning-theorem). An intercept-resend attacker who measures each signal in a random [BB84](../../quantum-theory.md#bb84) basis chooses the wrong basis half the time. On those sifted positions Bob has a one-half error [probability](../../probability-theory.md#probability), giving the ideal [BB84 intercept-resend error rate](../../quantum-theory.md#bb84-intercept-resend-error-rate) $1/4$. This simple calculation demonstrates detectable disturbance for that attack; it is not a complete security proof for arbitrary attacks.

Authentication is essential: otherwise an adversary can impersonate both participants. Error correction reveals information that must be included in the privacy budget, and losses, finite sample sizes, multiphoton emission and detector behavior belong in the security model. Entanglement-based variants can use Bell [correlations](../../variance.md#pearson-correlation-coefficient), but observing some entanglement or a Bell violation alone does not replace a quantitatively specified key-distillation protocol. The final key can subsequently be used in a suitable classical encryption scheme.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For [quantum teleportation](../../bell-state.md#quantum-teleportation), Alice holds an unknown input $|\psi\rangle_1$ and one member of a shared $|\Phi^+\rangle_{23}$ pair; Bob holds [qubit](../../quantum-system.md#qubit) 3. Alice applies a [CNOT gate](../../quantum-theory.md#controlled-not-gate) from 1 to 2 and a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on 1, then measures both in the [computational basis](../../quantum-theory.md#computational-basis). Expansion gives the [Bell-basis teleportation identity](../../bell-state.md#bell-basis-teleportation-identity)

$$
(H_1\otimes I)\operatorname{CNOT}_{1\to2}
(|\psi\rangle_1|\Phi^+\rangle_{23})
=\frac12\sum_{m,n=0}^1|mn\rangle_{12}X^nZ^m|\psi\rangle_3.
$$

Every outcome pair $(m,n)$ has [probability](../../probability-theory.md#probability) $1/4$, independently of the input. Alice sends these two classical bits, and Bob applies

$$
\boxed{Z^mX^n\,X^nZ^m|\psi\rangle=|\psi\rangle.}
$$

The order of the two corrections matters only by a global sign for the doubly nonzero outcome. The transformation also transfers entanglement with an untouched reference, because the identity is linear in the input amplitudes.

Before receiving the bits, Bob must average over all four Pauli-related states, obtaining $I/2$ for any input. Thus teleportation requires [classical communication](../../quantum-information-theory.md#classical-communication) and does not send information faster than light. The original input is consumed by Alice's measurement, so no second copy remains and the [no-cloning theorem](../../quantum-theory.md#no-cloning-theorem) is respected. Ideal [qubit](../../quantum-system.md#qubit) teleportation consumes one shared Bell pair and two classical bits, as well as local gates and measurements. Imperfect entanglement, gate error, detection error or lost classical records reduce practical fidelity; teleportation transfers the [quantum state](../../quantum-system.md#quantum-state), not the underlying material particle.

## ↑ Ancestors (11)

1. [2012](../2012.md)
2. [Past exam of the quantum information course of the University of Cambridge](../../past-exam-of-the-quantum-information-course-of-the-university-of-cambridge.md)
3. [Quantum Information course of the University of Cambridge](../../university-of-cambridge.md#quantum-information-course-of-the-university-of-cambridge)
4. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year 4 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-4-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
8. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
9. [University of Cambridge](../../university-of-cambridge.md)
10. [List of universities](../../README.md#list-of-universities)
11. [Codex Wiki](../../README.md)
