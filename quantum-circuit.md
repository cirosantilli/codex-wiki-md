# Quantum circuit

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_circuit)

A quantum circuit is a finite composition of quantum gates acting on quantum registers. Reading the diagram from input to output gives the order in which its unitary operations are applied.

**Table of contents**

- [Quantum circuit gate-error telescoping bound](#quantum-circuit-gate-error-telescoping-bound)
- [Depth-first quantum circuit path summation](#depth-first-quantum-circuit-path-summation)
- [Stoquastic circuit](#stoquastic-circuit)
  - [Stoquastic acceptance floor](#stoquastic-acceptance-floor)
- [Computational history state](#computational-history-state)
  - [Feynman-Kitaev Hamiltonian](#feynman-kitaev-hamiltonian)
    - [Gap above a degenerate history ground space](#gap-above-a-degenerate-history-ground-space)
    - [Input penalty of a history Hamiltonian](#input-penalty-of-a-history-hamiltonian)
  - [Nonlocal quantum clock](#nonlocal-quantum-clock)
  - [Unary quantum clock](#unary-quantum-clock)
    - [History-subspace propagation Hamiltonian](#history-subspace-propagation-hamiltonian)
      - [Gershgorin gap bound for an adiabatic history path](#gershgorin-gap-bound-for-an-adiabatic-history-path)
      - [Spectrum of a path propagation Hamiltonian](#spectrum-of-a-path-propagation-hamiltonian)
- [Quantum logic gate](#quantum-logic-gate)
  - [Two-qubit gate](#two-qubit-gate)
    - [Diagonal two-qubit phase entanglement criterion](#diagonal-two-qubit-phase-entanglement-criterion)
    - [Cartan decomposition of a two-qubit gate](#cartan-decomposition-of-a-two-qubit-gate)
- [Measurement-based quantum computation](#measurement-based-quantum-computation)
  - [Three-vertex graph-state wire](#three-vertex-graph-state-wire)
  - [Five-vertex graph-state circuit simulation](#five-vertex-graph-state-circuit-simulation)
  - [Four-cycle graph-state simulation of an entangle-and-measure circuit](#four-cycle-graph-state-simulation-of-an-entangle-and-measure-circuit)
  - [Measurement pattern](#measurement-pattern)
    - [Logical depth of a measurement pattern](#logical-depth-of-a-measurement-pattern)
      - [Two-layer measurement pattern for CNOT and x-axis rotations](#two-layer-measurement-pattern-for-cnot-and-x-axis-rotations)
      - [Nonadaptive Clifford measurement pattern](#nonadaptive-clifford-measurement-pattern)
        - [Nonadaptive Hadamard–CNOT measurement pattern](#nonadaptive-hadamard-cnot-measurement-pattern)
- [Quantum register](#quantum-register)
- [Rotation gate](#rotation-gate)
  - [Rotation about the x-axis](#rotation-about-the-x-axis)
  - [Rotation about the y-axis](#rotation-about-the-y-axis)
  - [Rotation about the z-axis](#rotation-about-the-z-axis)
- [Universal quantum gate set](#universal-quantum-gate-set)
  - [Solovay--Kitaev theorem](#solovay-kitaev-theorem)
- [Quantum state preparation](#quantum-state-preparation)
  - [Uniform coprime state for a semiprime](#uniform-coprime-state-for-a-semiprime)
  - [Uniform superposition state](#uniform-superposition-state)
  - [Hierarchical probability-distribution state preparation](#hierarchical-probability-distribution-state-preparation)
- [Quantum arithmetic](#quantum-arithmetic)
- [Pauli group](#pauli-group)
  - [Pauli-string commutation parity](#pauli-string-commutation-parity)
  - [Binary phase representation of a Pauli string](#binary-phase-representation-of-a-pauli-string)
    - [Binary symplectic space of Pauli labels](#binary-symplectic-space-of-pauli-labels)
      - [Isotropic subspace of a binary symplectic space](#isotropic-subspace-of-a-binary-symplectic-space)
    - [Controlled-Z update in the binary phase representation](#controlled-z-update-in-the-binary-phase-representation)
  - [Pauli frame](#pauli-frame)
  - [Pauli operator](#pauli-operator)
    - [Pauli decomposition of a qubit-environment isometry](#pauli-decomposition-of-a-qubit-environment-isometry)
    - [Weight of a Pauli operator](#weight-of-a-pauli-operator)
    - [Pauli expansion of a quantum error](#pauli-expansion-of-a-quantum-error)
    - [Pauli gate](#pauli-gate)
    - [Pauli correlator](#pauli-correlator)
  - [Stabilizer group](#stabilizer-group)
    - [Balanced spectrum of a nonidentity stabilizer](#balanced-spectrum-of-a-nonidentity-stabilizer)
    - [Stabilizer generator](#stabilizer-generator)
    - [Stabilizer state](#stabilizer-state)
      - [Stabilizer-state preparation](#stabilizer-state-preparation)
      - [Stabilizer tableau](#stabilizer-tableau)
      - [Graph state](#graph-state)
        - [Equatorial measurement of a graph-state leaf](#equatorial-measurement-of-a-graph-state-leaf)
        - [Computational-basis measurement of a graph-state vertex](#computational-basis-measurement-of-a-graph-state-vertex)
        - [Graph-state stabilizer generator](#graph-state-stabilizer-generator)
        - [Local complementation of a graph state](#local-complementation-of-a-graph-state)
    - [Stabilizer subspace](#stabilizer-subspace)
      - [Stabilizer-projector formula](#stabilizer-projector-formula)
  - [Clifford gate](#clifford-gate)
    - [Clifford circuit](#clifford-circuit)
      - [Gottesman--Knill theorem](#gottesman-knill-theorem)
        - [Extended Gottesman--Knill theorem](#extended-gottesman-knill-theorem)
      - [Clifford frame](#clifford-frame)
    - [Local Clifford operation](#local-clifford-operation)
    - [Strong classical simulation of a quantum circuit](#strong-classical-simulation-of-a-quantum-circuit)
      - [Heisenberg propagation of a Pauli observable through a Clifford circuit](#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit)
        - [Backward Pauli updates for Hadamard and phase gates](#backward-pauli-updates-for-hadamard-and-phase-gates)
    - [Weak classical simulation of a quantum circuit](#weak-classical-simulation-of-a-quantum-circuit)

## Quantum circuit gate-error telescoping bound

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

For two [quantum circuits](quantum-circuit.md) with corresponding unitary gates, their difference is a sum of terms containing one gate difference and exact or perturbed products on either side. Unitary invariance and the [triangle inequality](topological-analysis.md#triangle-inequality) for the [operator norm](continuous-dual-space.md#operator-norm) therefore bound the circuit difference by the sum of individual gate errors. Tensoring a gate with an identity leaves that norm unchanged. On a normalized input, the same bound controls the output vector distance with gate phases retained. This is a worst-case coherent bound; cancellation can make a particular circuit less sensitive, but cannot be assumed without further information.

## Depth-first quantum circuit path summation

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

Expand a [quantum circuit](quantum-circuit.md) [matrix element](vector-space.md#matrix-element) by inserting [computational basis](quantum-theory.md#computational-basis) resolutions between gates, then enumerate the intermediate strings depth first. The active stack stores one basis label and accumulator per [quantum circuit](quantum-circuit.md) layer, using polynomial space for polynomially many qubits and gates. Recompute entries rather than storing an exponential matrix or state vector. The output probability requires the [Born rule](quantum-mechanics.md#born-rule) sum of squared amplitude moduli.

## Stoquastic circuit

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

A [stoquastic circuit](#stoquastic-circuit) verifier uses reversible classical [quantum gates](#quantum-logic-gate), represented by [permutation matrices](vector-space.md#permutation-matrix), with zero and plus-state [ancilla qubits](quantum-information-theory.md#ancilla-qubit) and a final [Hadamard basis](quantum-theory.md#hadamard-basis) output measurement. A basis input remains an entrywise nonnegative state; a general [quantum witness](computer-science.md#quantum-witness) need not be a basis input. The resulting acceptance structure is used in [StoqMA](computer-science.md#stoqma).

### Stoquastic acceptance floor

↑ **Parent:** [Stoquastic circuit](#stoquastic-circuit)

If the output of a [stoquastic circuit](#stoquastic-circuit) is $|0\rangle|r_0\rangle+|1\rangle|r_1\rangle$ with nonnegative amplitudes, its plus-outcome probability is $1/2+\operatorname{Re}\langle r_0|r_1\rangle\geq1/2$. Basis [quantum witnesses](computer-science.md#quantum-witness) with zero and plus [ancilla qubits](quantum-information-theory.md#ancilla-qubit) always have this property. A soundness threshold below one half cannot hold for every such input.

## Computational history state

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

A [computational history state](#computational-history-state) coherently records a circuit's intermediate states with orthogonal clock labels: $(T+1)^{-1/2}\sum_{t=0}^T|\psi_t\rangle|c_t\rangle$. A propagation term penalizes a mismatch between adjacent time labels and the corresponding gate. With correct propagation, uniform coefficients form a zero-energy [ground state](quantum-mechanics.md#ground-state) within the history subspace.

### Feynman-Kitaev Hamiltonian

↑ **Parent:** [Computational history state](#computational-history-state)

A [Feynman-Kitaev Hamiltonian](#feynman-kitaev-hamiltonian) penalizes incorrect input initialization, disagreement between successive [quantum circuit](quantum-circuit.md) steps and clock labels, and optionally a rejecting output. Its propagation [quadratic form](linear-algebra.md#quadratic-form) is a sum of $\tfrac12\|\eta_t-U_t\eta_{t-1}\|^2$. Without output penalty, its zero-energy space consists of correctly initialized [computational history states](#computational-history-state). A [nonlocal quantum clock](#nonlocal-quantum-clock) makes the propagation formula simple but does not supply fixed qubit locality by itself.

#### Gap above a degenerate history ground space

↑ **Parent:** [Feynman-Kitaev Hamiltonian](#feynman-kitaev-hamiltonian)

After undoing [quantum circuit](quantum-circuit.md) propagation, the Hamiltonian without output penalty is $Q\otimes|0\rangle\langle0|+I\otimes E$. The common kernel is the valid input space times the uniform clock vector. On its orthogonal complement, the [smallest angle between two subspaces](hilbert-space.md#smallest-angle-between-two-subspaces) obeys $\cos\vartheta=\sqrt{T/(T+1)}$. The [Kitaev geometrical lemma](hilbert-space.md#kitaev-geometrical-lemma) and path gap $2/(T+1)^2$ give $\Delta\geq(T+1)^{-3}$. Degenerate valid [quantum witnesses](computer-science.md#quantum-witness) must be removed together when computing this angle.

#### Input penalty of a history Hamiltonian

↑ **Parent:** [Feynman-Kitaev Hamiltonian](#feynman-kitaev-hamiltonian)

The [input penalty of a history Hamiltonian](#input-penalty-of-a-history-hamiltonian) tests the prescribed [ancilla qubits](quantum-information-theory.md#ancilla-qubit) at clock time zero and leaves the [quantum witness](computer-science.md#quantum-witness) unrestricted. Zero [ancilla qubits](quantum-information-theory.md#ancilla-qubit) are tested by $|1\rangle\langle1|$, and plus [ancilla qubits](quantum-information-theory.md#ancilla-qubit) by $|-\rangle\langle-|$. Their sum $Q$ is positive and has positive integer [eigenvalues](linear-operator-theory.md#eigenvalue). Together with propagation, its kernel selects histories of valid initial data.

### Nonlocal quantum clock

↑ **Parent:** [Computational history state](#computational-history-state)

A [nonlocal quantum clock](#nonlocal-quantum-clock) records [quantum circuit](quantum-circuit.md) time in an abstract $T+1$ dimensional register. A binary encoding uses logarithmically many qubits, but transitions $|t\rangle\langle t-1|$ need not have bounded qubit locality. Extra diagonal penalties may exclude unused binary labels. A [unary quantum clock](#unary-quantum-clock) provides a different encoding for fixed-locality constructions.

### Unary quantum clock

↑ **Parent:** [Computational history state](#computational-history-state)

A [unary quantum clock](#unary-quantum-clock) represents step $t$ of a $T$-gate circuit by $|1\rangle^{\otimes t}|0\rangle^{\otimes(T-t)}$. Clock strings are orthogonal, and adjacent legal strings differ at one qubit. Local patterns around that change permit a [history-subspace propagation Hamiltonian](#history-subspace-propagation-hamiltonian) with bounded locality.

#### History-subspace propagation Hamiltonian

↑ **Parent:** [Unary quantum clock](#unary-quantum-clock)

In the orthonormal history basis $|e_t\rangle=|\psi_t\rangle|c_t\rangle$, circuit propagation restricts to $E=\frac12\sum_{t=1}^T(|e_t\rangle-|e_{t-1}\rangle)(\langle e_t|-\langle e_{t-1}|)$. This is a [Graph Laplacian](graph-theory.md#laplacian-matrix) on a path. Its uniform zero-energy vector is the [computational history state](#computational-history-state), while initialization restricts to $D=I-|e_0\rangle\langle e_0|$.

##### Gershgorin gap bound for an adiabatic history path

↑ **Parent:** [History-subspace propagation Hamiltonian](#history-subspace-propagation-hamiltonian)

For $M(s)=(1-s)D+sE$ in the unary history subspace, the first [Gershgorin disc](numerical-analysis.md#gershgorin-disc) lies in $[0,s]$ and every other disc has real part at least $1-s$. For $s<1/2$, the first disc is isolated and contains the unique [ground state](quantum-mechanics.md#ground-state) energy. Thus the [spectral gap](linear-operator-theory.md#spectral-gap) is at least $1-2s$, in particular at least $1/3$ for $s\leq1/3$.

##### Spectrum of a path propagation Hamiltonian

↑ **Parent:** [History-subspace propagation Hamiltonian](#history-subspace-propagation-hamiltonian)

For a path with $T+1$ vertices and edge weight $1/2$, the [eigenvalues](linear-operator-theory.md#eigenvalue) are $1-\cos[\pi k/(T+1)]$, $k=0,\ldots,T$. The corresponding coefficients are proportional to $\cos[\pi k(t+1/2)/(T+1)]$. The zero mode is uniform, and the [spectral gap](linear-operator-theory.md#spectral-gap) is at least $2/(T+1)^2$. The endpoint difference equations use reflecting ghost values, not periodic ones.

## Quantum logic gate

↑ **Parent:** [Quantum circuit](quantum-circuit.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_logic_gate)

A unitary operation on a fixed number of [qubits](quantum-mechanics.md#qubit) used as a component of a [quantum circuit](quantum-circuit.md). Examples include the [Hadamard gate](quantum-theory.md#hadamard-gate) and [Controlled-Z gate](quantum-theory.md#controlled-z-gate). Measurements are described separately by [measurement in quantum mechanics](quantum-measurement.md); a gate is a reversible operation on its full input state.

### Two-qubit gate

↑ **Parent:** [Quantum logic gate](#quantum-logic-gate)

A two-qubit gate is a [unitary operator](vector-space.md#unitary-operator) on two [qubit](quantum-mechanics.md#qubit) lines, extended by the identity on the others. It may be entangling, as a [CNOT gate](quantum-theory.md#controlled-not-gate) is, or a product of local operations. In a [Hamiltonian simulation](quantum-theory.md#hamiltonian-simulation) model allowing arbitrary two-qubit gates, the exponential of a Hermitian term supported on two lines counts as one such gate. Compiling it into a fixed discrete [universal quantum gate set](#universal-quantum-gate-set) introduces a separate approximation cost.

#### Diagonal two-qubit phase entanglement criterion

↑ **Parent:** [Two-qubit gate](#two-qubit-gate)

A diagonal [two-qubit gate](#two-qubit-gate) with entries $e^{i\phi_{jk}}$ is a product of local diagonal gates, up to [global phase](quantum-mechanics.md#global-phase), exactly when $\delta=0$ modulo $2\pi$. This follows by factoring the two-by-two array of phases; its determinant vanishes precisely in that case. If the determinant is nonzero, applying the gate to $|+\rangle\otimes|+\rangle$ produces an entangled state by the [two-qubit product-state determinant criterion](bell-state.md#two-qubit-product-state-determinant-criterion). In particular $\operatorname{diag}(-1,1,1,-1)=-Z\otimes Z$ is local, whereas $\operatorname{diag}(1,1,1,-1)$ is the entangling [Controlled-Z gate](quantum-theory.md#controlled-z-gate).

#### Cartan decomposition of a two-qubit gate

↑ **Parent:** [Two-qubit gate](#two-qubit-gate)

Every [two-qubit gate](#two-qubit-gate) has the displayed form with local elements of the [special unitary group](topological-group.md#special-unitary-group) and real interaction parameters. The three Pauli-product generators commute, so the central exponential is the product of three interactions. Local basis changes turn an [Ising coupling](control-theory.md#ising-coupling-of-two-qubits) into either of the other Pauli-product couplings. A fixed entangling controlled phase together with arbitrary local rotations can also synthesize each variable interaction, for example through two [CNOT gates](quantum-theory.md#controlled-not-gate) enclosing a variable $z$ rotation.

## Measurement-based quantum computation

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

Measurement-based quantum computation prepares an entangled resource [quantum state](quantum-mechanics.md#quantum-state), then applies single-[qubit](quantum-mechanics.md#qubit) [measurement in quantum measurements](quantum-measurement.md), potentially adapting later bases to earlier outcomes. [Pauli frame](#pauli-frame) tracking and classical outcome processing convert random physical branches into a specified logical computation. [Graph states](#graph-state) and [one-bit teleportation](bell-state.md#one-bit-teleportation) provide a concrete construction.

### Three-vertex graph-state wire

↑ **Parent:** [Measurement-based quantum computation](#measurement-based-quantum-computation)

A path [graph state](#graph-state) on three [qubits](quantum-mechanics.md#qubit) simulates two successive gates $U(\theta)=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta)$. Measure vertex one in the [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) basis $|v_r(\alpha)\rangle=(|0\rangle+(-1)^re^{i\alpha}|1\rangle)/\sqrt2$, then vertex two at angle $(-1)^r\beta$, obtaining bits $r,s$. Two [one-bit teleportations](bell-state.md#one-bit-teleportation) and $U(\theta)X=e^{-i\theta}ZU(-\theta)$ leave vertex three in $X^sZ^rU(\beta)U(\alpha)|+\rangle$, up to [global phase](quantum-mechanics.md#global-phase). A computational output bit $z$ is corrected to $z\oplus s$; the $Z$ factor affects only phase. Adaptive sign choice is required for general angles, although the final bit correction is purely classical.

### Five-vertex graph-state circuit simulation

↑ **Parent:** [Measurement-based quantum computation](#measurement-based-quantum-computation)

A [graph state](#graph-state) with edges $13,24,34,45$ simulates $J_2(\gamma)E_{12}(J_1(\alpha)\otimes J_2(\beta))$ on $|++\rangle$. Measure vertices 1 and 2 at angles $\alpha,\beta$, with results $s_1,s_2$, and vertex 4 at $(-1)^{s_2}\gamma$, with result $s_4$. [One-bit teleportation](bell-state.md#one-bit-teleportation) and [Pauli frame](#pauli-frame) propagation leave output frames $X_3^{s_1}Z_3^{s_2}$ and $X_5^{s_4\oplus s_1}Z_5^{s_2}$. Computational outputs are therefore corrected by $s_1$ and $s_4\oplus s_1$ respectively.

### Four-cycle graph-state simulation of an entangle-and-measure circuit

↑ **Parent:** [Measurement-based quantum computation](#measurement-based-quantum-computation)

Label a four-cycle $0-1-2-3-0$. Measure [vertex](graph.md#vertex-graph-theory) $0$ in the [computational basis](quantum-theory.md#computational-basis) with result $r$, then [vertex](graph.md#vertex-graph-theory) $1$ in the [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) basis at angle $\alpha$ with result $s$. [Graph-state vertex deletion](#computational-basis-measurement-of-a-graph-state-vertex) and [one-bit teleportation](bell-state.md#one-bit-teleportation) leave

$$
E_{23}X_2^{r\oplus s}J(\alpha)_2Z_3^r|++\rangle=X_2^{r\oplus s}Z_3^sE_{23}J(\alpha)_2|++\rangle.
$$

Final [computational basis](quantum-theory.md#computational-basis) measurements with raw results $d_2,d_3$ therefore simulate the ideal circuit $E_{23}J(\alpha)_2$ on $|++\rangle$ after the classical correction $k=d_2\oplus r\oplus s$, $l=d_3$. The output [probability distribution](probability-theory.md#probability-distribution) is correct in every prior branch; no physical [Pauli frame](#pauli-frame) correction is needed.

### Measurement pattern

↑ **Parent:** [Measurement-based quantum computation](#measurement-based-quantum-computation)

A measurement pattern specifies the resource [quantum state](quantum-mechanics.md#quantum-state), the measured [qubits](quantum-mechanics.md#qubit), their measurement bases, outcome-dependent basis choices and output corrections or classical relabellings. The dependence of a basis on earlier outcomes determines the [logical depth of a measurement pattern](#logical-depth-of-a-measurement-pattern). Preparing the resource and processing the final classical results are separate costs.

#### Logical depth of a measurement pattern

↑ **Parent:** [Measurement pattern](#measurement-pattern)

Logical measurement depth is the number of sequential measurement layers required by outcome-dependent basis choices. Depth one means all bases are fixed in advance, so the [measurement in quantum measurements](quantum-measurement.md) on distinct [qubits](quantum-mechanics.md#qubit) can be simultaneous. Classical output corrections may still depend on all outcomes. This does not assert depth-one graph-state preparation or constant-depth classical processing.

##### Two-layer measurement pattern for CNOT and x-axis rotations

↑ **Parent:** [Logical depth of a measurement pattern](#logical-depth-of-a-measurement-pattern)

An $R(\alpha)=J(\alpha)J(0)$ gadget with input [Pauli frame](#pauli-frame) $X^pZ^q$, angle-zero outcome $s$, and arbitrary-angle outcome $t$ uses angle $(-1)^{s\oplus q}\alpha$ and produces frame $X^{p\oplus t}Z^{q\oplus s}$. The [CNOT gate](quantum-theory.md#controlled-not-gate) gadget also updates its $Z$ frames without any dependence on incoming $X$ frames. Therefore all adaptive angle signs depend solely on angle-zero outcomes. Measure all those vertices first, compute every sign, and measure all remaining vertices in a second layer. The result is the desired logical circuit in a known [Pauli frame](#pauli-frame). Computational output measurements can share the second layer.

##### Nonadaptive Clifford measurement pattern

↑ **Parent:** [Logical depth of a measurement pattern](#logical-depth-of-a-measurement-pattern)

A path [graph state](#graph-state) simulates a sequence of [Clifford gates](#clifford-gate) $J(\alpha_j)$, $\alpha_j\in\{0,\pi/2\}$, using fixed [equatorial qubit measurement](quantum-measurement.md#equatorial-qubit-measurement) bases on successive path [vertices](graph.md#vertex-graph-theory). Let $s_j$ be raw outcomes, $t_j=2\alpha_j/\pi\in\{0,1\}$, and start the [Pauli frame](#pauli-frame) at $a_0=b_0=0$. Matrix commutation and $J(-\pi/2)=XJ(\pi/2)$ give

$$
a_j=s_j\oplus b_{j-1}\oplus t_ja_{j-1},\qquad b_j=a_{j-1}.
$$

Induction shows the final unmeasured state differs from the ideal circuit output by $X^{a_m}Z^{b_m}$, up to [global phase](quantum-mechanics.md#global-phase). A final [computational basis](quantum-theory.md#computational-basis) result $d$ is corrected to $d\oplus a_m$. All bases are fixed, and projectors on distinct [vertices](graph.md#vertex-graph-theory) commute, so all measurements, including the final one, can occur in a single layer. The frame recurrence is classical outcome processing, not quantum feed-forward.

<h6 id="nonadaptive-hadamard-cnot-measurement-pattern">Nonadaptive Hadamard–CNOT measurement pattern</h6>

↑ **Parent:** [Nonadaptive Clifford measurement pattern](#nonadaptive-clifford-measurement-pattern)

Compile each [CNOT gate](quantum-theory.md#controlled-not-gate) into a [Hadamard gate](quantum-theory.md#hadamard-gate), a [Controlled-Z gate](quantum-theory.md#controlled-z-gate), and another [Hadamard gate](quantum-theory.md#hadamard-gate) on its target. Every [one-bit teleportation](bell-state.md#one-bit-teleportation) implementing a [Hadamard gate](quantum-theory.md#hadamard-gate) uses a fixed angle-zero basis. A [Pauli frame](#pauli-frame) propagates by classical binary updates without changing a measurement basis. All internal measurements, and any fixed computational output measurements, therefore share one simultaneous layer. Resource preparation and classical processing are not included in this [logical measurement depth](#logical-depth-of-a-measurement-pattern).

## Quantum register

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

A quantum register is a named [tensor product](linear-algebra.md#tensor-product) factor of a [quantum circuit](quantum-circuit.md)'s [Hilbert space](hilbert-space.md), usually a collection of [qubits](quantum-mechanics.md#qubit). Registers separate data, control, output and workspace roles; [uncomputation](quantum-theory.md#uncomputation) returns workspace to a fixed [quantum state](quantum-mechanics.md#quantum-state) without destroying coherence in the data.

## Rotation gate

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

A one-qubit rotation gate is $R_\alpha(\theta)=e^{-i\theta\sigma_\alpha/2}$, where $\sigma_\alpha$ is a [Pauli matrix](algebra.md#pauli-matrices). It rotates the [Bloch vector](quantum-theory.md#bloch-vector) by angle $\theta$ about the corresponding axis.

### Rotation about the x-axis

↑ **Parent:** [Rotation gate](#rotation-gate)

The [rotation gate](#rotation-gate) about the [Pauli X gate](quantum-theory.md#pauli-x-gate) axis commutes with $X$. The [J gate](bell-state.md#j-gate-in-measurement-based-quantum-computation) convention gives $J(\alpha)J(0)=H\operatorname{diag}(1,e^{i\alpha})H=e^{i\alpha/2}R_x(\alpha)$, differing from the standard axis rotation only by [global phase](quantum-mechanics.md#global-phase).

### Rotation about the y-axis

↑ **Parent:** [Rotation gate](#rotation-gate)

The one-qubit [rotation gate](#rotation-gate)

$$
R_y(\theta)=\begin{pmatrix}\cos(\theta/2)&-\sin(\theta/2)\\\sin(\theta/2)&\cos(\theta/2)\end{pmatrix}
$$

satisfies $R_y(2\theta)|0\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle$ and $R_y(\alpha)R_y(\beta)=R_y(\alpha+\beta)$. The latter identity enables a [binary-angle implementation of a quantum variable rotation](quantum-theory.md#binary-angle-implementation-of-a-quantum-variable-rotation).

### Rotation about the z-axis

↑ **Parent:** [Rotation gate](#rotation-gate)

The one-qubit [rotation gate](#rotation-gate) is $R_z(\theta)=\operatorname{diag}(e^{-i\theta/2},e^{i\theta/2})$. It implements the two relative phases needed in [simulation of a computable diagonal Hamiltonian](quantum-theory.md#simulation-of-a-computable-diagonal-hamiltonian).

## Universal quantum gate set

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

A universal quantum gate set can approximate every finite-qubit [unitary operator](vector-space.md#unitary-operator) arbitrarily accurately using finite circuits over the set.

Universality is a property of a set of [quantum logic gates](#quantum-logic-gate): finite circuits from the set approximate arbitrary unitary transformations.

<h3 id="solovay-kitaev-theorem">Solovay--Kitaev theorem</h3>

↑ **Parent:** [Universal quantum gate set](#universal-quantum-gate-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solovay–Kitaev_theorem)

For a suitable finite inverse-closed [universal quantum gate set](#universal-quantum-gate-set), the Solovay--Kitaev theorem approximates a fixed-dimensional unitary to [operator norm](continuous-dual-space.md#operator-norm) error $\varepsilon$ with a gate sequence of length polynomial in $\log(1/\varepsilon)$.

## Quantum state preparation

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

Quantum state preparation constructs a circuit $B$ that maps a simple reference state to a desired state, $B|0^n\rangle=|\psi\rangle$. Efficient amplitude encoding requires structure or suitable oracle access to avoid reading exponentially many arbitrary amplitudes.

### Uniform coprime state for a semiprime

↑ **Parent:** [Quantum state preparation](#quantum-state-preparation)

For a [semiprime](number-theory.md#semiprime) $N=pq$ with distinct known primes, this [quantum state](quantum-mechanics.md#quantum-state) is uniform over the reduced residue classes. With $n$ binary digits in $N$, its fraction among all $2^n$ computational labels is $a=(p-1)(q-1)/2^n\geq1/4$. An [ancilla qubit](quantum-information-theory.md#ancilla-qubit) whose one probability is $1/(4a)$ dilutes the joint good probability to exactly $1/4$. A reversible range-and-[greatest common divisor](number-theory.md#greatest-common-divisor) predicate marks the good labels with [ancilla qubit](quantum-information-theory.md#ancilla-qubit) one, and a single [exact amplitude amplification](quantum-theory.md#exact-amplitude-amplification) iteration produces $|\xi_N\rangle|1\rangle$. Known prime factors provide the cardinality; the membership test itself needs only $N$. Polynomial gate complexity presumes ideal one-qubit rotations at the specified amplitudes.

### Uniform superposition state

↑ **Parent:** [Quantum state preparation](#quantum-state-preparation)

In an $N$-dimensional [computational basis](quantum-theory.md#computational-basis), the uniform superposition state is

$$
|s_N\rangle=\frac1{\sqrt N}\sum_{x=0}^{N-1}|x\rangle.
$$

Measurement in that basis gives the [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution). For $N=2^n$, [Hadamard gates](quantum-theory.md#hadamard-gate) prepare it from $|0^n\rangle$. Its reflection $2|s_N\rangle\langle s_N|-I$ is a [Grover diffusion operator](quantum-theory.md#grover-diffusion-operator).

### Hierarchical probability-distribution state preparation

↑ **Parent:** [Quantum state preparation](#quantum-state-preparation)

Hierarchical probability-distribution state preparation recursively bisects a classical probability distribution. At each level, a controlled rotation splits every parent interval's amplitude between its two children according to their conditional probabilities.

## Quantum arithmetic

↑ **Parent:** [Quantum circuit](quantum-circuit.md)

Quantum arithmetic implements a classical numerical function reversibly on computational-basis registers and therefore coherently on their superpositions. Temporary work values must be uncomputed to avoid unwanted entanglement.

## Pauli group

↑ **Parent:** [Quantum circuit](quantum-circuit.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pauli_group)

The $n$-qubit Pauli group consists of tensor products of $I,X,Y,Z$ multiplied by phases $\pm1$ or $\pm i$.

### Pauli-string commutation parity

↑ **Parent:** [Pauli group](#pauli-group)

For [tensor products](linear-algebra.md#tensor-product) of Pauli factors from $\{I,X,Y,Z\}$, let $k$ count the sites where both factors are nonidentity and different. Distinct nonidentity [Pauli matrices](algebra.md#pauli-matrices) anticommute, and equal or identity factors commute. Reversing the product site by site therefore gives $PQ=(-1)^kQP$. Thus two Pauli strings commute exactly when $k$ is even. The criterion applies to the perfect-correlation observables in the [GHZ theorem](quantum-theory.md#ghz-theorem).

### Binary phase representation of a Pauli string

↑ **Parent:** [Pauli group](#pauli-group)

Store a [Pauli group](#pauli-group) element with binary exponents $a_j,b_j$ and a phase exponent $s$ modulo four. This ordered $XZ$ convention uses $2n+2$ bits for $n$ [qubits](quantum-mechanics.md#qubit). Since $XZ=-iY$, phase factors are essential when converting to Hermitian [Pauli operators](#pauli-operator) and evaluating measurement probabilities.

#### Binary symplectic space of Pauli labels

↑ **Parent:** [Binary phase representation of a Pauli string](#binary-phase-representation-of-a-pauli-string)

Modulo scalar phases, the n-qubit [Pauli group](#pauli-group) is the additive space $\mathbb F_2^{2n}$, with label $(a,b)$ for $X^aZ^b$. Multiplication adds labels, and commutation contributes the sign $(-1)^{\omega}$. The displayed alternating form is nondegenerate. An isotropic subspace $L$ satisfies $L\subseteq L^\perp$, hence $\dim L\le n$; it labels commuting stabilizers.

##### Isotropic subspace of a binary symplectic space

↑ **Parent:** [Binary symplectic space of Pauli labels](#binary-symplectic-space-of-pauli-labels)

A subspace $L$ is isotropic when the symplectic pairing vanishes between every pair of its vectors. Its binary Pauli labels therefore commute. Nondegeneracy identifies the ambient space with its dual, so the map to $L^*$ is surjective and $\dim L^\perp=2n-\dim L$. Since $L\subseteq L^\perp$, it follows that $\dim L\le n$. This explains the maximum number of independent generators of a [stabilizer group](#stabilizer-group).

#### Controlled-Z update in the binary phase representation

↑ **Parent:** [Binary phase representation of a Pauli string](#binary-phase-representation-of-a-pauli-string)

Conjugation by a [Controlled-Z gate](quantum-theory.md#controlled-z-gate) leaves the $a$ bits unchanged and updates the displayed $b$ bits and phase, using the old bits. The phase occurs when the extra $Z$ from one line is moved past $X$ on the other line. These constant-size updates support [Heisenberg propagation of a Pauli observable through a Clifford circuit](#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit).

### Pauli frame

↑ **Parent:** [Pauli group](#pauli-group)

A Pauli frame is a classical record of known [Pauli operator](#pauli-operator) byproducts rather than their physical correction. A one-[qubit](quantum-mechanics.md#qubit) frame $X^aZ^b$ changes a [computational basis](quantum-theory.md#computational-basis) measurement label by $a$; $b$ changes only a phase. Conjugation by [Clifford gates](#clifford-gate) maps [Pauli operators](#pauli-operator) to [Pauli operators](#pauli-operator), so the frame can be updated by classical binary arithmetic throughout a [Clifford circuit](#clifford-circuit).

### Pauli operator

↑ **Parent:** [Pauli group](#pauli-group)

An $n$-qubit Pauli operator is a tensor product of single-qubit Pauli matrices, possibly multiplied by a phase. Hermitian Pauli operators have eigenvalues $+1$ and $-1$.

#### Pauli decomposition of a qubit-environment isometry

↑ **Parent:** [Pauli operator](#pauli-operator)

Every linear map from a [qubit](quantum-mechanics.md#qubit) into the [tensor product](linear-algebra.md#tensor-product) of that [qubit](quantum-mechanics.md#qubit) and an environment can be expanded in the [Pauli matrix](algebra.md#pauli-matrices) [orthonormal basis](linear-algebra.md#orthonormal-basis) of operators. If $V|0\rangle=|0\rangle|e_{00}\rangle+|1\rangle|e_{01}\rangle$ and $V|1\rangle=|0\rangle|e_{10}\rangle+|1\rangle|e_{11}\rangle$, then the four coefficient vectors are

$$
|e_0\rangle=\frac{|e_{00}\rangle+|e_{11}\rangle}{2},\quad
|e_1\rangle=\frac{|e_{01}\rangle+|e_{10}\rangle}{2},\quad
|e_2\rangle=\frac{i(|e_{10}\rangle-|e_{01}\rangle)}{2},\quad
|e_3\rangle=\frac{|e_{00}\rangle-|e_{11}\rangle}{2}.
$$

These environment vectors need not be orthogonal, so this is an operator expansion rather than a claim that the [quantum channel](quantum-information-theory.md#quantum-channel) is a classical [Pauli channel](quantum-information-theory.md#pauli-channel). Physical [isometries](riemannian-geometry.md#isometry) additionally preserve the [inner products](linear-algebra.md#inner-product) of the two input basis states.

#### Weight of a Pauli operator

↑ **Parent:** [Pauli operator](#pauli-operator)

The weight of a tensor-product [Pauli operator](#pauli-operator) is the number of nonidentity local factors; its global phase is ignored. Products satisfy $\operatorname{wt}(P^\dagger Q)\leq\operatorname{wt}(P)+\operatorname{wt}(Q)$ because their support is contained in the union of the two supports. The [quantum code distance](quantum-error-correction.md#distance-of-a-quantum-error-correcting-code) uses this weight to measure the smallest undetectable nontrivial action on logical information.

#### Pauli expansion of a quantum error

↑ **Parent:** [Pauli operator](#pauli-operator)

The tensor products of single-qubit [Pauli matrices](algebra.md#pauli-matrices) form an orthogonal basis of the operator space on $n$ [qubits](quantum-mechanics.md#qubit), so every linear error operator has a Pauli expansion. Using $X^aZ^b$, with scalar phases absorbed into the coefficients, its [computational basis](quantum-theory.md#computational-basis) action is $E|x\rangle=\sum_{a,b}c_{a,b}(-1)^{b\cdot x}|x+a\rangle$, with binary arithmetic. This describes coherent errors as well as individual Pauli errors; it does not assume that the noise is a probabilistic [Pauli channel](quantum-information-theory.md#pauli-channel). A physical noise map has [Kraus operators](quantum-information-theory.md#kraus-operator) of this form when the usual [quantum channel](quantum-information-theory.md#quantum-channel) description applies, for instance when the initial system and environment are uncorrelated.

#### Pauli gate

↑ **Parent:** [Pauli operator](#pauli-operator)

A Pauli gate applies a [Pauli matrix](algebra.md#pauli-matrices) as a [unitary operator](vector-space.md#unitary-operator) to a [qubit](quantum-mechanics.md#qubit). The [Pauli X gate](quantum-theory.md#pauli-x-gate), [Pauli Y gate](quantum-theory.md#pauli-y-gate) and [Pauli Z gate](quantum-theory.md#pauli-z-gate) are common correction operations in [quantum teleportation](bell-state.md#quantum-teleportation).

#### Pauli correlator

↑ **Parent:** [Pauli operator](#pauli-operator)

A Pauli correlator is the expectation value of a tensor product of [Pauli matrices](algebra.md#pauli-matrices), such as $\langle X\otimes Z\rangle$. It measures a specified correlation between qubit observables.

### Stabilizer group

↑ **Parent:** [Pauli group](#pauli-group)

A stabilizer group is an abelian subgroup of the [Pauli group](#pauli-group) that does not contain $-I$. Its simultaneous positive eigenspace is its stabilizer subspace.

#### Balanced spectrum of a nonidentity stabilizer

↑ **Parent:** [Stabilizer group](#stabilizer-group)

A [stabilizer group](#stabilizer-group) excludes $-I$, so each element squares to $I$ and is Hermitian; an imaginary-phase Pauli element would square to $-I$. A nonidentity stabilizer contains at least one nonidentity local [Pauli matrix](algebra.md#pauli-matrices) and has zero trace, since the trace of a tensor product is the product of local traces. Its eigenvalues are therefore $\pm1$ with equal multiplicities. This trace fact also gives $\dim\mathcal X_S=2^n/|S|$ from the [stabilizer-projector formula](#stabilizer-projector-formula).

#### Stabilizer generator

↑ **Parent:** [Stabilizer group](#stabilizer-group)

A set of stabilizer generators is an independent commuting family of Hermitian [Pauli operators](#pauli-operator) whose products form a [stabilizer group](#stabilizer-group).

#### Stabilizer state

↑ **Parent:** [Stabilizer group](#stabilizer-group)

A stabilizer state on $n$ qubits is the unique simultaneous positive eigenstate of a stabilizer group with $n$ independent generators.

##### Stabilizer-state preparation

↑ **Parent:** [Stabilizer state](#stabilizer-state)

Stabilizer-state preparation starts from a computational-basis state and applies a [Clifford circuit](#clifford-circuit), producing a [stabilizer state](#stabilizer-state).

##### Stabilizer tableau

↑ **Parent:** [Stabilizer state](#stabilizer-state)

A stabilizer tableau represents each Pauli generator by a binary row $[x_1\cdots x_n\mid z_1\cdots z_n]$, with one additional bit when its sign is retained. Clifford gates update these rows by arithmetic over $\mathbb F_2$.

##### Graph state

↑ **Parent:** [Stabilizer state](#stabilizer-state)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Graph_state)

For an undirected graph $G=(V,E)$, the graph state is

$$
|G\rangle=\prod_{(i,j)\in E}CZ_{ij}|+\rangle^{\otimes|V|}.
$$

###### Equatorial measurement of a graph-state leaf

↑ **Parent:** [Graph state](#graph-state)

Let $1$ be a leaf with neighbour $2$ and let the graph on the other [vertices](graph.md#vertex-graph-theory) be generated by the [Controlled-Z gate](quantum-theory.md#controlled-z-gate) product $E_{\mathrm{rest}}$. If the leaf has [Pauli Z gate](quantum-theory.md#pauli-z-gate) frame $Z_1^r$, measuring it at angle $\alpha$ with result $s$ applies [one-bit teleportation](bell-state.md#one-bit-teleportation) and leaves

$$
E_{\mathrm{rest}}\left(X_2^sJ(\alpha)_2Z_2^r|+\rangle_2\otimes|+\rangle_{\mathrm{other}}\right).
$$

Any known [Pauli Z gate](quantum-theory.md#pauli-z-gate) frames on other [vertices](graph.md#vertex-graph-theory) remain as additional factors before those [vertices](graph.md#vertex-graph-theory)' input states. The identity $J(\alpha)Z^r=X^rJ(\alpha)$ combines the leaf byproduct with the measurement result.

###### Computational-basis measurement of a graph-state vertex

↑ **Parent:** [Graph state](#graph-state)

For a [graph state](#graph-state) $|G\rangle=\prod_{ij\in E}CZ_{ij}|+\rangle^{\otimes|V|}$, measuring [vertex](graph.md#vertex-graph-theory) $v$ in the [computational basis](quantum-theory.md#computational-basis) with result $r$ gives the normalized state

$$
\left(\prod_{u\in N(v)}Z_u^r\right)|G-v\rangle.
$$

Each [Controlled-Z gate](quantum-theory.md#controlled-z-gate) from $v$ to a neighbour acts as $Z_u^r$ after projecting $v$ onto $|r\rangle$; all other [edges](graph-theory.md#edge-of-a-graph) remain unchanged. The projection contributes $1/\sqrt2$, so either result has [probability](probability-theory.md#probability) $1/2$. For a four-cycle, deleting one [vertex](graph.md#vertex-graph-theory) leaves a path and adds byproducts on its two endpoints.

###### Graph-state stabilizer generator

↑ **Parent:** [Graph state](#graph-state)

The graph-state stabilizer generator at vertex $v$ is $S_v=X_v\prod_{u\in N(v)}Z_u$. Two such generators commute because adjacent vertices contribute two Pauli anticommutations and nonadjacent vertices contribute none.

###### Local complementation of a graph state

↑ **Parent:** [Graph state](#graph-state)

Local complementation at a vertex $v$ toggles every edge between neighbors of $v$. It is implemented on graph states, up to global phase, by the local Clifford operator

$$
e^{-i\pi X_v/4}\prod_{u\in N(v)}e^{i\pi Z_u/4}.
$$

#### Stabilizer subspace

↑ **Parent:** [Stabilizer group](#stabilizer-group)

The stabilizer subspace of a commuting family $S$ of Hermitian Pauli operators is

$$
V_S=\{|\psi\rangle:S|\psi\rangle=|\psi\rangle\text{ for every }S\in\mathcal S\}.
$$

If there are $r$ independent generators on $n$ qubits, its dimension is $2^{n-r}$.

##### Stabilizer-projector formula

↑ **Parent:** [Stabilizer subspace](#stabilizer-subspace)

For a [stabilizer group](#stabilizer-group) $G=\langle g_1,\ldots,g_l\rangle$, the [orthogonal projector](hilbert-space.md#orthogonal-projection) onto its [stabilizer subspace](#stabilizer-subspace) is

$$
\Pi_G=\frac1{|G|}\sum_{g\in G}g
=\prod_{i=1}^l\frac{I+g_i}{2}.
$$

### Clifford gate

↑ **Parent:** [Pauli group](#pauli-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Clifford_gate)

A Clifford gate is a unitary operation that normalizes the [Pauli group](#pauli-group): conjugating any Pauli operator by it produces another Pauli operator. Hadamard, phase, and controlled-$Z$ gates generate the Clifford operations.

#### Clifford circuit

↑ **Parent:** [Clifford gate](#clifford-gate)

A Clifford circuit is composed entirely of Clifford gates. It maps Pauli operators to Pauli operators in the Heisenberg picture and stabilizer states to stabilizer states in the Schrödinger picture.

<h5 id="gottesman-knill-theorem">Gottesman--Knill theorem</h5>

↑ **Parent:** [Clifford circuit](#clifford-circuit)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gottesman–Knill_theorem)

The Gottesman--Knill theorem gives a classical polynomial-time simulation of quantum computations built from [stabilizer-state preparation](#stabilizer-state-preparation), [Clifford gates](#clifford-gate), and adaptive [Measurements of Pauli observables](quantum-theory.md#measurement-of-a-pauli-observable).

<h6 id="extended-gottesman-knill-theorem">Extended Gottesman--Knill theorem</h6>

↑ **Parent:** [Gottesman--Knill theorem](#gottesman-knill-theorem)

The extended Gottesman--Knill theorem allows arbitrary product-state inputs to a unitary Clifford circuit. Computational-basis output is weakly simulable for any number of measured qubits and strongly simulable for logarithmically many measured qubits.

##### Clifford frame

↑ **Parent:** [Clifford circuit](#clifford-circuit)

A Clifford frame records a known Clifford transformation classically instead of applying it physically. Updating the frame changes the Pauli observables used for later measurements while preserving the represented quantum computation.

#### Local Clifford operation

↑ **Parent:** [Clifford gate](#clifford-gate)

A local Clifford operation is a tensor product of one-qubit Clifford gates. On graph states, local Clifford operations implement graph transformations such as local complementation.

#### Strong classical simulation of a quantum circuit

↑ **Parent:** [Clifford gate](#clifford-gate)

A strong classical simulation computes a quantum circuit's specified output probabilities in classical polynomial time to the requested polynomial precision. This is stronger than weak simulation, which only samples from the output distribution.

##### Heisenberg propagation of a Pauli observable through a Clifford circuit

↑ **Parent:** [Strong classical simulation of a quantum circuit](#strong-classical-simulation-of-a-quantum-circuit)

To compute a single-qubit output probability of a [Clifford circuit](#clifford-gate), propagate its measured Pauli observable backward through the circuit. Every conjugation remains a tensor-product Pauli, whose expectation on a [product state](bell-state.md#product-state) factors into efficiently computable one-qubit expectations.

###### Backward Pauli updates for Hadamard and phase gates

↑ **Parent:** [Heisenberg propagation of a Pauli observable through a Clifford circuit](#heisenberg-propagation-of-a-pauli-observable-through-a-clifford-circuit)

For the [binary phase representation of a Pauli string](#binary-phase-representation-of-a-pauli-string), these local rules implement $P\mapsto U^\dagger P U$ for the [Hadamard gate](quantum-theory.md#hadamard-gate) and the phase gate $S=\operatorname{diag}(1,i)$. In particular $S^\dagger XS=-iXZ$, so the phase update differs in sign from forward conjugation. Use the old input bits, and reduce $s$ modulo four.

#### Weak classical simulation of a quantum circuit

↑ **Parent:** [Clifford gate](#clifford-gate)

A weak classical simulation samples in classical polynomial time from the output distribution of a quantum circuit, exactly or within a prescribed small total-variation distance.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (44)

- [Ancilla bit](quantum-information-theory.md#ancilla-bit)
- [BQP](computer-science.md#bqp)
- [Clean subset superposition preparation](quantum-theory.md#clean-subset-superposition-preparation)
- [Depth-first quantum circuit path summation](#depth-first-quantum-circuit-path-summation)
- [Exact quantum query complexity](computer-science.md#exact-quantum-query-complexity)
- [Feynman-Kitaev Hamiltonian](#feynman-kitaev-hamiltonian)
- [Gap above a degenerate history ground space](#gap-above-a-degenerate-history-ground-space)
- [Hamiltonian simulation](quantum-theory.md#hamiltonian-simulation)
- [No-programming theorem](bell-state.md#no-programming-theorem)
- [Nonlocal quantum clock](#nonlocal-quantum-clock)
- [Opposite-pair elimination for exact quantum balance testing](quantum-theory.md#opposite-pair-elimination-for-exact-quantum-balance-testing)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53.md#2/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-67.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61.md#4/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67.md#2/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324.md#3/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2.md#15c/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#15d/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324.md#3/b/solution)
- [QMA](computer-science.md#qma)
- [Quantum circuit gate-error telescoping bound](#quantum-circuit-gate-error-telescoping-bound)
- [Quantum complexity theory](computer-science.md#quantum-complexity-theory)
- [Quantum logic gate](#quantum-logic-gate)
- [Quantum query complexity](computer-science.md#quantum-query-complexity)
- [Quantum register](#quantum-register)
- [Qudit](quantum-mechanics.md#qudit)
- [Stoquastic Hamiltonian](quantum-theory.md#stoquastic-hamiltonian)
