# Quantum error correction

↑ **Parent:** [Quantum theory](quantum-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quantum_error_correction)

Quantum error correction encodes logical states into a larger Hilbert space so that a specified family of physical errors can be detected and reversed.

**Table of contents**

- [Quantum error-correcting code](#quantum-error-correcting-code)
- [Logical qubit](#logical-qubit)
- [Concatenated quantum error-correcting code](#concatenated-quantum-error-correcting-code)
  - [Five-qubit concatenation threshold](#five-qubit-concatenation-threshold)
- [Five-qubit error correcting code](#five-qubit-error-correcting-code)
  - [Five-qubit stabilizer syndrome table](#five-qubit-stabilizer-syndrome-table)
- [Quantum error detection](#quantum-error-detection)
  - [Correction implies detection at twice the weight](#correction-implies-detection-at-twice-the-weight)
- [Nondegenerate quantum error-correcting code](#nondegenerate-quantum-error-correcting-code)
  - [Quantum Hamming bound](#quantum-hamming-bound)
    - [Perfect quantum error-correcting code](#perfect-quantum-error-correcting-code)
- [Distance of a quantum error-correcting code](#distance-of-a-quantum-error-correcting-code)
  - [Correctable Pauli error radius](#correctable-pauli-error-radius)
  - [Quantum Singleton bound](#quantum-singleton-bound)
  - [Quantum erasure correction](#quantum-erasure-correction)
- [Linearity of coherent quantum error correction](#linearity-of-coherent-quantum-error-correction)
- [Knill--Laflamme condition](#knill-laflamme-condition)
  - [Necessity of the Knill-Laflamme condition](#necessity-of-the-knill-laflamme-condition)
  - [Constructive recovery from the Knill-Laflamme condition](#constructive-recovery-from-the-knill-laflamme-condition)
- [Stabilizer code](#stabilizer-code)
  - [Symplectic representation of a stabilizer code](#symplectic-representation-of-a-stabilizer-code)
  - [CSS code](#css-code)
    - [Nested-code CSS syndrome recovery](#nested-code-css-syndrome-recovery)
  - [Centralizer of a stabilizer group](#centralizer-of-a-stabilizer-group)
  - [Local correctability of a stabilizer code](#local-correctability-of-a-stabilizer-code)
    - [Pauli error criterion for a stabilizer code](#pauli-error-criterion-for-a-stabilizer-code)
  - [Dressed stabilizer under a weak local perturbation](#dressed-stabilizer-under-a-weak-local-perturbation)
  - [Distance of a stabilizer code](#distance-of-a-stabilizer-code)
  - [Error syndrome](#error-syndrome)
    - [Stabilizer-syndrome coset](#stabilizer-syndrome-coset)
  - [Phase-flip repetition code](#phase-flip-repetition-code)
    - [Logical Hadamard convention for a phase-flip repetition code](#logical-hadamard-convention-for-a-phase-flip-repetition-code)
    - [Logical failure of the three-qubit phase-flip repetition code](#logical-failure-of-the-three-qubit-phase-flip-repetition-code)
    - [Phase-flip protection by Hadamard conjugation](#phase-flip-protection-by-hadamard-conjugation)
    - [Majority-vote decoding of a repetition code](#majority-vote-decoding-of-a-repetition-code)
  - [Bit-flip repetition code](#bit-flip-repetition-code)
    - [Coherent syndrome extraction for the three-qubit repetition code](#coherent-syndrome-extraction-for-the-three-qubit-repetition-code)
      - [Timed bit flip during repetition-code syndrome extraction](#timed-bit-flip-during-repetition-code-syndrome-extraction)
        - [Exact encoded-state failure with a faulty parity check](#exact-encoded-state-failure-with-a-faulty-parity-check)
  - [Concatenated phase-and-bit-flip repetition code](#concatenated-phase-and-bit-flip-repetition-code)
    - [Shor code](#shor-code)
      - [Shor-code phase-flip syndrome](#shor-code-phase-flip-syndrome)
  - [Steane code](#steane-code)
    - [Nondegenerate phase-flip correction in the Steane code](#nondegenerate-phase-flip-correction-in-the-steane-code)
  - [Color code](#color-code)
    - [String operator in a topological code](#string-operator-in-a-topological-code)
  - [Surface code](#surface-code)
    - [Surface code on a chain of spheres](#surface-code-on-a-chain-of-spheres)
    - [Surface-code decoding as a random-bond Ising model](#surface-code-decoding-as-a-random-bond-ising-model)
    - [Ground-state splitting of a surface-code cylinder](#ground-state-splitting-of-a-surface-code-cylinder)
    - [Toric code](#toric-code)
      - [Surface-code anyon model](#surface-code-anyon-model)

## Quantum error-correcting code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

A quantum error-correcting code is a subspace encoding a logical [Hilbert space](hilbert-space.md), together with a specified family of noise operators that a common recovery [quantum channel](quantum-information-theory.md#quantum-channel) reverses on every encoded state. A K-dimensional code carries $\log_2K$ logical qubits. For a code projector $P$, correctability is characterized by the [Knill--Laflamme condition](#knill-laflamme-condition); code distance is defined by the smallest undetectable operator weight, not merely by the number of generators.

## Logical qubit

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

A [logical qubit](#logical-qubit) is a two-dimensional encoded quantum subsystem with chosen orthonormal logical basis states $|0_L\rangle,|1_L\rangle$. An encoding [linear isometry](hilbert-space.md#linear-isometry-of-hilbert-spaces) sends $\alpha|0\rangle+\beta|1\rangle$ to $\alpha|0_L\rangle+\beta|1_L\rangle$. In a [concatenated quantum error-correcting code](#concatenated-quantum-error-correcting-code), one level's [logical qubit](#logical-qubit) supplies one [qubit](quantum-mechanics.md#qubit) of the next outer code.

## Concatenated quantum error-correcting code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

A concatenated quantum code replaces each physical [qubit](quantum-mechanics.md#qubit) of an outer code by a [logical qubit](#logical-qubit) of an inner code. Correction proceeds from inner blocks to outer blocks. For independent errors and ideal correction, a logical-error map $f$ iterates as $p_{\ell+1}=f(p_\ell)$. This recursion describes the code/channel model and does not by itself include errors in encoding and recovery gates.

// Target: quantum-error-correction.bigb

### Five-qubit concatenation threshold

↑ **Parent:** [Concatenated quantum error-correcting code](#concatenated-quantum-error-correcting-code)

Assume independent physical-error [probability](probability-theory.md#probability) $p$, correction of zero or one errors, and failure on every block with at least two errors. The failure map is $f(p)=1-(1-p)^5-5p(1-p)^4$. Factoring $f(p)-p$ gives $p(1-p)(4p^3-11p^2+9p-1)$. The unique interior threshold is the root of $4p^3-11p^2+9p-1=0$. Below it concatenation decreases the failure [probability](probability-theory.md#probability) toward zero. Two levels give $f(f(p))=1000p^4+O(p^5)$, compared with $10p^2+O(p^3)$ at one level.

// Target: quantum-information-theory.bigb

## Five-qubit error correcting code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Five-qubit_error_correcting_code)

The five-qubit code encodes one logical [qubit](quantum-mechanics.md#qubit) into five physical [qubits](quantum-mechanics.md#qubit) and corrects an arbitrary error on one physical [qubit](quantum-mechanics.md#qubit). In a nondegenerate realization, the identity and fifteen one-qubit [Pauli operators](quantum-circuit.md#pauli-operator) take the two-dimensional code into sixteen mutually orthogonal syndrome subspaces, filling the 32-dimensional physical [Hilbert space](hilbert-space.md).

// Target: quantum-error-correction.bigb

### Five-qubit stabilizer syndrome table

↑ **Parent:** [Five-qubit error correcting code](#five-qubit-error-correcting-code)

The four commuting independent [stabilizer generators](quantum-circuit.md#stabilizer-generator) define a two-dimensional [stabilizer code](#stabilizer-code). The identity and fifteen single-site [Pauli errors](quantum-circuit.md#pauli-operator) have sixteen distinct four-bit [error syndromes](#error-syndrome), so their two-dimensional images form an [orthogonal direct sum](vector-space.md#orthogonal-direct-sum) of the physical space. This proves nondegenerate single-site correction and the [perfect quantum error-correcting code](#perfect-quantum-error-correcting-code) property. The operators $X^{\otimes5}$ and $Z^{\otimes5}$ commute with the stabilizer and anticommute with each other. Multiplying $X^{\otimes5}$ by $XZZXI$ gives, up to phase, $IYYIX$, a nontrivial weight-three logical operator, proving distance exactly three.

## Quantum error detection

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

A code with [orthogonal projector](hilbert-space.md#orthogonal-projection) $P$ detects an error $E$ when its compression to the code is scalar. A [projective measurement](quantum-measurement.md#projective-measurement) of $P$ then either flags departure from the code or, on a successful code-space outcome, leaves the logical state unchanged up to normalization. This includes harmless scalar errors, even though they need not produce a nonzero [error syndrome](#error-syndrome). Detectability extends by linearity to the span of a set of errors. Every [Pauli operator](quantum-circuit.md#pauli-operator) of weight less than the [quantum code distance](#distance-of-a-quantum-error-correcting-code) is detectable.

### Correction implies detection at twice the weight

↑ **Parent:** [Quantum error detection](#quantum-error-detection)

Split the support of a [Pauli operator](quantum-circuit.md#pauli-operator) of weight at most $2t$ into two sets of size at most $t$. It is, up to a scalar phase, $E_a^\dagger E_b$ for two errors in the correctable family. The [Knill--Laflamme condition](#knill-laflamme-condition) makes its compression to the code scalar, which is [quantum error detection](#quantum-error-detection). Expansion in the Pauli basis extends the assertion to every operator supported on at most $2t$ [qubits](quantum-mechanics.md#qubit). The number $t$ counts affected qubits, not the cardinality of an arbitrary selected family of errors.

## Nondegenerate quantum error-correcting code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

For a specified correctable set of distinct [Pauli operators](quantum-circuit.md#pauli-operator) modulo phase, a nondegenerate code has mutually orthogonal error images $E\mathcal X$. Equivalently, the matrix in the [Knill--Laflamme condition](#knill-laflamme-condition) is diagonal for that Pauli error set. Each error therefore requires a separate syndrome subspace of dimension equal to the logical code dimension. Degenerate codes can have distinct errors with the same action on the code and do not satisfy this orthogonality counting argument.

### Quantum Hamming bound

↑ **Parent:** [Nondegenerate quantum error-correcting code](#nondegenerate-quantum-error-correcting-code)

For unknown-location [Pauli operators](quantum-circuit.md#pauli-operator) of weight at most $t$, there are $N(t)=\sum_{j=0}^t3^j\binom nj$ physically distinct errors modulo phase, including the identity. A [nondegenerate quantum code](#nondegenerate-quantum-error-correcting-code) assigns them mutually orthogonal error-image subspaces, each of dimension $2^k$, within the $2^n$-dimensional physical [Hilbert space](hilbert-space.md). Hence $N(t)2^k\leq2^n$. The hypothesis of nondegeneracy is essential to this dimension count.

#### Perfect quantum error-correcting code

↑ **Parent:** [Quantum Hamming bound](#quantum-hamming-bound)

A [nondegenerate quantum code](#nondegenerate-quantum-error-correcting-code) is perfect at correction radius $t$ if its distinct correctable [Pauli error](quantum-circuit.md#pauli-operator) images exhaust the physical [Hilbert space](hilbert-space.md). Each image has dimension $2^k$, and their [orthogonal direct sum](vector-space.md#orthogonal-direct-sum) is the whole $2^n$-dimensional space precisely when the [quantum Hamming bound](#quantum-hamming-bound) is an equality. This perfectness concerns unknown-location errors of weight at most $t$; it does not imply correction of every higher-weight error.

## Distance of a quantum error-correcting code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

An $[[n,k,d]]$ [quantum error correction](quantum-error-correction.md) code is a $2^k$-dimensional subspace of $n$ [qubits](quantum-mechanics.md#qubit). Its distance $d$ is the minimum weight of a [Pauli operator](quantum-circuit.md#pauli-operator) $E$ for which $PEP$ is not a scalar multiple of the code projector $P$. Thus every operator supported on fewer than $d$ qubits has scalar compression to the code, by expansion in the Pauli basis. This definition includes degenerate codes; a low-weight operator acting as a scalar does not reduce the distance.

### Correctable Pauli error radius

↑ **Parent:** [Distance of a quantum error-correcting code](#distance-of-a-quantum-error-correcting-code)

The guaranteed radius is the largest integer $t$ for which all unknown-location [Pauli operators](quantum-circuit.md#pauli-operator) of weight at most $t$ can be corrected together. Pairwise products have weight at most $2t$, so $2t<d$ suffices by the [Knill--Laflamme condition](#knill-laflamme-condition). Conversely, split a minimum-weight undetectable Pauli operator between two subsets of its support. If $d\leq2t$, this gives two errors of weight at most $t$ whose pairwise product violates that condition. Consequently $d$ is either $2t+1$ or $2t+2$; parity cannot be recovered from $t$ alone.

### Quantum Singleton bound

↑ **Parent:** [Distance of a quantum error-correcting code](#distance-of-a-quantum-error-correcting-code)

For a code carrying $k>0$ logical [qubits](quantum-mechanics.md#qubit), two disjoint subsets $A,B$ of $d-1$ physical qubits are each correctable erasures. Purify the maximally mixed logical input using a reference $R$, and call the remaining physical subsystem $C$. Erasure decoupling gives $S(RA)=S(R)+S(A)$ and $S(RB)=S(R)+S(B)$. Purity and [Subadditivity of Von Neumann entropy](von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) imply $2S(R)\leq2S(C)$, hence $k\leq n-2(d-1)$. If two such disjoint subsets would not fit, partition the entire physical system into two correctable subsets; purity and decoupling then force $S(R)=0$, a contradiction. Thus the partition used in the proof is justified independently of the bound.

### Quantum erasure correction

↑ **Parent:** [Distance of a quantum error-correcting code](#distance-of-a-quantum-error-correcting-code)

Errors on a known subset of $m$ [qubits](quantum-mechanics.md#qubit) are correctable by a distance-$d$ code whenever $m<d$. Every product $E_a^\dagger E_b$ of errors supported on that subset still has support in the same subset, so its compression is scalar. The [Knill--Laflamme condition](#knill-laflamme-condition) therefore supplies one recovery for every channel on that subset. Equivalently, erasing the subset leaks no logical information to it: if a reference is maximally entangled with the encoded logical system, its joint [density operator](quantum-theory.md#density-matrix) with the erased subsystem is a [product state](bell-state.md#product-state).

## Linearity of coherent quantum error correction

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)

Suppose fixed unitary encoding and recovery correct each error $E_j$ by mapping every logical input $|\psi\rangle$ to $|\psi\rangle\otimes|\eta_j\rangle$. The syndrome vector can be taken independent of the logical input: applying linearity to basis inputs and their equal superposition forces their syndrome vectors to agree. Hence an error $E=\sum_jc_jE_j$ is mapped to $|\psi\rangle\otimes\sum_jc_j|\eta_j\rangle$. If $E$ is unitary, this final syndrome vector is normalized and the circuit corrects $E$. Orthogonality of the syndrome states is not needed for the linear-span argument; it is a separate condition concerning distinguishability of errors.

<h2 id="knill-laflamme-condition">Knill--Laflamme condition</h2>

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Knill--Laflamme_condition)

A code projector $P$ corrects errors $\{E_a\}$ exactly when $PE_a^\dagger E_bP=C_{ab}P$ for every pair.

### Necessity of the Knill-Laflamme condition

↑ **Parent:** [Knill--Laflamme condition](#knill-laflamme-condition)

If a common recovery [quantum channel](quantum-information-theory.md#quantum-channel) with [Kraus operators](quantum-information-theory.md#kraus-operator) $R_\mu$ restores every pure code state after each error $E_a$, then each vector $R_\mu E_a|\psi\rangle$ is parallel to $|\psi\rangle$. [Linearity](vector-space.md#linearity) on basis vectors and their pairwise superpositions forces $R_\mu E_aP=c_{\mu a}P$, with the scalar independent of the logical state. Insert $\sum_\mu R_\mu^\dagger R_\mu=I$ between two error operators to obtain the displayed [Knill--Laflamme condition](#knill-laflamme-condition). This proves necessity without presuming an orthogonal syndrome description of recovery.

### Constructive recovery from the Knill-Laflamme condition

↑ **Parent:** [Knill--Laflamme condition](#knill-laflamme-condition)

The matrix $C$ in the [Knill--Laflamme condition](#knill-laflamme-condition) is positive semidefinite, since $v^\dagger Cv$ is the squared norm of $\sum_av_aE_a|\psi\rangle$ for any normalized code state. Diagonalizing it gives linear combinations $F_j$ with $PF_j^\dagger F_lP=c_j\delta_{jl}P$. For $c_j>0$, $V_j=F_jP/\sqrt{c_j}$ is an isometry of the code into an error-image subspace, and these subspaces are orthogonal. Measuring their projectors and applying $V_j^\dagger$ recovers the logical state. Complete the operation arbitrarily on the orthogonal complement to obtain a [quantum channel](quantum-information-theory.md#quantum-channel). This construction corrects every noise map whose [Kraus operators](quantum-information-theory.md#kraus-operator) lie in the specified error span, including coherent superpositions of error operators.

## Stabilizer code

↑ **Parent:** [Quantum error correction](quantum-error-correction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stabilizer_code)

A stabilizer code is the common positive eigenspace of a commuting subgroup of the Pauli group.

### Symplectic representation of a stabilizer code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

A [stabilizer group](quantum-circuit.md#stabilizer-group) with $r$ independent generators maps injectively to an r-dimensional isotropic subspace of the [binary symplectic space of Pauli labels](quantum-circuit.md#binary-symplectic-space-of-pauli-labels). For generator rows $(A\mid B)$, commutation is $AB^T+BA^T=0$ over $\mathbb F_2$. Its [stabilizer subspace](quantum-circuit.md#stabilizer-subspace) has dimension $2^{n-r}$. The labels of the [centralizer of a stabilizer group](#centralizer-of-a-stabilizer-group) form $L^\perp$; labels in $L^\perp\setminus L$ act as nontrivial logical Pauli operators.

### CSS code

↑ **Parent:** [Stabilizer code](#stabilizer-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/CSS_code)

For binary [linear codes](coding-theory.md#linear-code) $C_2\subseteq C_1\subseteq\mathbb F_2^N$, the CSS code has basis $|x+C_2\rangle=|C_2|^{-1/2}\sum_{y\in C_2}|x+y\rangle$ for $x\in C_1/C_2$. Its X stabilizers come from $C_2$ and its Z stabilizers from the [dual code](coding-theory.md#dual-code) $C_1^\perp$; their commutation follows from orthogonality. For positive logical dimension, $d_X=\min\{\operatorname{wt}(x):x\in C_1\setminus C_2\}$ and $d_Z=\min\{\operatorname{wt}(z):z\in C_2^\perp\setminus C_1^\perp\}$, with [quantum code distance](#distance-of-a-quantum-error-correcting-code) $d=\min(d_X,d_Z)$. Thus arbitrary errors on at most $\lfloor(d-1)/2\rfloor$ [qubits](quantum-mechanics.md#qubit) are correctable. Stabilizer errors are harmless even if their weight is small; the distances exclude them.

#### Nested-code CSS syndrome recovery

↑ **Parent:** [CSS code](#css-code)

For binary [linear codes](coding-theory.md#linear-code) $C\subseteq C'$, the coset superpositions of the [CSS code](#css-code) have $X$ checks labelled by $C$ and $Z$ checks by $(C')^\perp$. A bit-error pattern $a$ gives the classical [syndrome](coding-theory.md#syndrome) for $C'$, and a phase-error pattern $b$ gives the syndrome for the [dual code](coding-theory.md#dual-code) $C^\perp$. Errors with $2t_X<\min_{a\in C'\setminus C}\operatorname{wt}(a)$ and $2t_Z<\min_{b\in C^\perp\setminus(C')^\perp}\operatorname{wt}(b)$ are jointly correctable. Every pairwise Pauli-error product either anticommutes with a check, giving zero code compression, or its low-weight components belong to the stabilizer and give scalar compression. Thus the [Knill--Laflamme condition](#knill-laflamme-condition) covers coherent superpositions and [quantum channels](quantum-information-theory.md#quantum-channel) as well as definite bit and phase errors.

### Centralizer of a stabilizer group

↑ **Parent:** [Stabilizer code](#stabilizer-code)

The Pauli centralizer $C(S)$ consists of Pauli operators commuting with every stabilizer. Elements of $C(S)\setminus S$, modulo stabilizers and phases, are the nontrivial logical Pauli operators.

### Local correctability of a stabilizer code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

If every pairwise product $E_a^\dagger E_b$ has weight below the code distance, it cannot be a nontrivial logical operator. The Knill--Laflamme conditions then hold for the whole error set.

#### Pauli error criterion for a stabilizer code

↑ **Parent:** [Local correctability of a stabilizer code](#local-correctability-of-a-stabilizer-code)

Let $S$ exclude $-I$, let $C(S)$ be its Pauli centralizer, and let $\mathcal Z=\{\pm I,\pm iI\}$. A set of [Pauli errors](quantum-circuit.md#pauli-operator) is jointly correctable exactly when every product $E_a^\dagger E_b$ belongs to $\mathcal ZS$ or lies outside $C(S)$. Outside the centralizer its code compression is zero by anticommutation; in $\mathcal ZS$ it acts as a scalar. A centralizing operator outside $\mathcal ZS$ has zero trace on the code but is unitary there, so cannot be scalar. This gives precisely the [Knill--Laflamme condition](#knill-laflamme-condition). Scalar phases must be retained when formulating the group criterion.

### Dressed stabilizer under a weak local perturbation

↑ **Parent:** [Stabilizer code](#stabilizer-code)

Quasi-adiabatic continuation carries each stabilizer to a quasi-local conserved operator for the perturbed low-energy space. Bare Pauli errors are then only approximately correctable because the dressed operators have exponentially small non-Pauli tails.

### Distance of a stabilizer code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

The distance is the minimum weight of a Pauli operator that preserves the code space but acts nontrivially on its logical information.

### Error syndrome

↑ **Parent:** [Stabilizer code](#stabilizer-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error_syndrome)

An error syndrome records which stabilizer generators commute or anticommute with an error.

#### Stabilizer-syndrome coset

↑ **Parent:** [Error syndrome](#error-syndrome)

Two Pauli errors have the same stabilizer syndrome exactly when their product lies in the centralizer of the stabilizer group. Thus a syndrome identifies a coset $E_sC(S)$, while logical operators inside that coset remain indistinguishable.

### Phase-flip repetition code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

The $n$-qubit phase-flip repetition code is stabilized by $X_jX_{j+1}$ and has codewords $|+\rangle^{\otimes n}$ and $|-\rangle^{\otimes n}$. It has logical operators $\overline Z=X_1$ and $\overline X=Z_1\cdots Z_n$, so its distance against phase flips is $n$.

#### Logical Hadamard convention for a phase-flip repetition code

↑ **Parent:** [Phase-flip repetition code](#phase-flip-repetition-code)

The codewords $|+++\rangle,|---\rangle$ have residual logical [Pauli X gate](quantum-theory.md#pauli-x-gate) after an uncorrectable two- or three-site phase error. Precede their encoding by a logical [Hadamard gate](quantum-theory.md#hadamard-gate) and follow decoding by its inverse. Since $HXH=Z$, the same error now acts as a logical [Pauli Z gate](quantum-theory.md#pauli-z-gate). Explicitly the encoded coefficients are $(\alpha+\beta)/\sqrt2$ and $(\alpha-\beta)/\sqrt2$ for an input $\alpha|0\rangle+\beta|1\rangle$. This convention matters when translating physical phase errors into a claimed decoded phase-error channel.

#### Logical failure of the three-qubit phase-flip repetition code

↑ **Parent:** [Phase-flip repetition code](#phase-flip-repetition-code)

The [phase-flip repetition code](#phase-flip-repetition-code) with codewords $|+++\rangle,|---\rangle$ corrects any one physical [Pauli Z gate](quantum-theory.md#pauli-z-gate) error. Its two adjacent-pair [error syndromes](#error-syndrome) cannot distinguish an error pattern from its three-bit complement. Minimum-weight recovery therefore leaves no residual error at weight zero or one, and leaves $Z_1Z_2Z_3$ at weight two or three. This residual operator exchanges the codewords, so inverse encoding gives a logical [Pauli X gate](quantum-theory.md#pauli-x-gate). For independent physical phase errors of probability $\epsilon$, the decoded [quantum channel](quantum-information-theory.md#quantum-channel) is $(1-p_L)\rho+p_LX\rho X$, where $p_L=3\epsilon^2(1-\epsilon)+\epsilon^3$. For $0<\epsilon<1/2$, $\epsilon-p_L=\epsilon(1-\epsilon)(1-2\epsilon)>0$.

#### Phase-flip protection by Hadamard conjugation

↑ **Parent:** [Phase-flip repetition code](#phase-flip-repetition-code)

Insert [Hadamard gates](quantum-theory.md#hadamard-gate) on every data qubit immediately after encoding by a [bit-flip repetition code](#bit-flip-repetition-code) and immediately before its bit-flip detection and recovery. The intervening physical error is thereby conjugated by $H^{\otimes n}$, and $HZH=X$ turns a single [Pauli Z gate](quantum-theory.md#pauli-z-gate) error into a single bit flip for the original correction circuit. The encoded logical codewords are now $|+\rangle^{\otimes n}$ and $|-\rangle^{\otimes n}$. The syndrome ancillas and the final inverse encoding stay unchanged. This protects against phase flips in the new basis; it does not simultaneously correct arbitrary bit flips in the physical basis.

#### Majority-vote decoding of a repetition code

↑ **Parent:** [Phase-flip repetition code](#phase-flip-repetition-code)

For independent errors of probability $p<1/2$, maximum-likelihood decoding of a repetition code chooses the lower-weight error compatible with the syndrome. This is majority voting, with threshold $p_c=1/2$ and exponentially vanishing logical-error probability below threshold.

### Bit-flip repetition code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

The $m$-qubit bit-flip repetition code is obtained from the [phase-flip repetition code](#phase-flip-repetition-code) by interchanging $X$ and $Z$. It is stabilized by $Z_jZ_{j+1}$ and has logical operators $\overline X=X_1\cdots X_m$ and $\overline Z=Z_1$.

#### Coherent syndrome extraction for the three-qubit repetition code

↑ **Parent:** [Bit-flip repetition code](#bit-flip-repetition-code)

Encode $u|0\rangle+v|1\rangle$ as $u|000\rangle+v|111\rangle$. Four [controlled-NOT gates](quantum-theory.md#controlled-not-gate) copy the displayed two data parities into initially zero [quantum ancillas](quantum-information-theory.md#quantum-ancilla). No logical amplitude is measured. The [error syndromes](#error-syndrome) $00,01,10,11$ correspond respectively to no bit flip and bit flips on data qubits $1,2,3$. Conditional [Toffoli gates](quantum-theory.md#toffoli-gate), with temporary [Pauli X gates](quantum-theory.md#pauli-x-gate) implementing zero-valued controls, undo the indicated error. Inverse encoding yields the original logical state and a separate syndrome state. A phase flip has zero bit-flip syndrome and remains as a logical phase error; this three-qubit code is not a general single-qubit-error code.

##### Timed bit flip during repetition-code syndrome extraction

↑ **Parent:** [Coherent syndrome extraction for the three-qubit repetition code](#coherent-syndrome-extraction-for-the-three-qubit-repetition-code)

Suppose the first ancilla records parity $q_2\oplus q_3$, then a fault of value $f$ flips $q_2$, and the second ancilla records parity $q_1\oplus q_2$. For incoming bit-error pattern $e$, the observed [error syndrome](#error-syndrome) is the displayed pair, while the final data error before recovery is $d=e\oplus(0,f,0)$. When $f=1$, the observed syndrome differs from the actual data syndrome by $(1,0)$. Applying the usual minimum-weight recovery leaves a nonzero syndrome, so the state is outside the code space even when the channel itself made no error. This is a timing-dependent failure of this simple extraction circuit, not a general obstruction to fault-tolerant [quantum error correction](quantum-error-correction.md).

###### Exact encoded-state failure with a faulty parity check

↑ **Parent:** [Timed bit flip during repetition-code syndrome extraction](#timed-bit-flip-during-repetition-code-syndrome-extraction)

For independent channel bit flips of probability $p$ and the specified extraction fault of probability $q$, require recovery of an arbitrary input in the original encoded subspace. Every extraction-fault event leaves nonzero [error syndrome](#error-syndrome); without that fault, channel errors are corrected exactly at weight zero or one. Thus success probability is $(1-q)[(1-p)^3+3p(1-p)^2]$. Compared with a single unencoded bit-flip channel, strict improvement for $0<p<1/2$ requires $q<p(1-2p)/[(1-p)(1+2p)]$. A different decoder or an added later ideal recovery changes the performance criterion and must be specified separately.

### Concatenated phase-and-bit-flip repetition code

↑ **Parent:** [Stabilizer code](#stabilizer-code)

Replacing every qubit of an $n$-qubit [phase-flip repetition code](#phase-flip-repetition-code) by an $m$-qubit [bit-flip repetition code](#bit-flip-repetition-code) gives a code with logical $Z$- and $X$-operator weights $m$ and $n$, respectively, and hence distance $\min(m,n)$.

#### Shor code

↑ **Parent:** [Concatenated phase-and-bit-flip repetition code](#concatenated-phase-and-bit-flip-repetition-code)

The nine-qubit Shor code encodes one logical [qubit](quantum-mechanics.md#qubit) with basis vectors $|0_L\rangle=|G_+\rangle^{\otimes3}$ and $|1_L\rangle=|G_-\rangle^{\otimes3}$, where $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. Six adjacent $Z$-pair [stabilizer generators](quantum-circuit.md#stabilizer-generator) locate a single bit flip within a block, while $X_1\cdots X_6$ and $X_4\cdots X_9$ diagnose which block has had its relative phase changed. Together they correct every single-qubit [Pauli operator](quantum-circuit.md#pauli-operator), hence every single-qubit error by the [Pauli expansion of a quantum error](quantum-circuit.md#pauli-expansion-of-a-quantum-error).

A [Pauli Z gate](quantum-theory.md#pauli-z-gate) on qubit four has phase-check eigenvalues $(-1,-1)$ and leaves all six $Z$-pair checks positive. Applying $Z_4$ restores the state. The same phase syndrome arises from $Z_5$ or $Z_6$; these have the same action on the code since their pairwise products are stabilizers. This is a degeneracy, not a failure of correction.

##### Shor-code phase-flip syndrome

↑ **Parent:** [Shor code](#shor-code)

Group the nine physical [qubits](quantum-mechanics.md#qubit) into three blocks and write $B_r$ for the product of three [Pauli X gates](quantum-theory.md#pauli-x-gate) in block $r$. The commuting [stabilizer generators](quantum-circuit.md#stabilizer-generator) $B_1B_2$ and $B_2B_3$ have eigenvalue $+1$ on both logical codewords. A [Pauli Z gate](quantum-theory.md#pauli-z-gate) in blocks one, two or three gives syndromes $(-,+)$, $(-,-)$ or $(+,-)$ respectively. Apply a Z gate to any one qubit of the indicated block to recover the logical state. Z errors at distinct locations within a block act identically on the code, so this correction is degenerate.

### Steane code

↑ **Parent:** [Stabilizer code](#stabilizer-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Steane_code)

The Steane code is a seven-qubit CSS stabilizer code encoding one logical qubit with distance three.

#### Nondegenerate phase-flip correction in the Steane code

↑ **Parent:** [Steane code](#steane-code)

Write the [Steane code](#steane-code) basis as uniform [quantum superpositions](quantum-mechanics.md#quantum-superposition) over a binary [linear code](coding-theory.md#linear-code) $D$ and a disjoint coset $t+D$, where $D$ is the even-weight part of the length-seven [Hamming code](coding-theory.md#hamming-code). For $Z(w)=\bigotimes_{j=1}^7Z_j^{w_j}$, diagonal [Pauli Z gates](quantum-theory.md#pauli-z-gate) cannot connect the two cosets. Within coset $t_a+D$, the overlap is

$$
\langle\psi_a|Z(w)|\psi_a\rangle=(-1)^{w\cdot t_a}|D|^{-1}\sum_{x\in D}(-1)^{w\cdot x}.
$$

If $w\notin D^\perp$, translation by a word $x_0\in D$ with $w\cdot x_0=1$ negates this sum, so it vanishes. Since the [dual code](coding-theory.md#dual-code) $D^\perp$ is the length-seven [Hamming code](coding-theory.md#hamming-code) of minimum [Hamming distance](coding-theory.md#hamming-distance) three, every nonzero $w$ of [Hamming weight](coding-theory.md#hamming-weight) one or two has vanishing overlap. Taking $u,v$ from $\{0,e_1,\ldots,e_7\}$ proves the displayed identity. The eight two-dimensional error images are [orthogonal](linear-algebra.md#orthogonal-vectors), so their [projective measurement](quantum-measurement.md#projective-measurement) determines the [error syndrome](#error-syndrome) without revealing the logical state; applying the identified [phase flip](quantum-theory.md#pauli-z-gate) again recovers every code state. This proves [nondegenerate quantum error-correcting code](#nondegenerate-quantum-error-correcting-code) behaviour for the identity and all single-site [phase flips](quantum-theory.md#pauli-z-gate), including their coherent linear span.

### Color code

↑ **Parent:** [Stabilizer code](#stabilizer-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Color_code)

A color code places qubits on a three-colorable lattice and assigns X-type and Z-type stabilizers to each colored plaquette.

#### String operator in a topological code

↑ **Parent:** [Color code](#color-code)

A string operator creates excitations at its endpoints. Multiplying by a successive segment moves an endpoint because the shared intermediate excitation is toggled twice.

### Surface code

↑ **Parent:** [Stabilizer code](#stabilizer-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Surface_code)

The surface code is a topological stabilizer code whose electric and magnetic excitations are bosons with mutual-semion braiding.

#### Surface code on a chain of spheres

↑ **Parent:** [Surface code](#surface-code)

Join $n$ spheres pole to pole and draw $m$ longitude edges on each sphere. Qubits on edges, two-edge face $Z$ stabilizers, and vertex $X$ stabilizers realize the concatenated phase-and-bit-flip repetition code. A pole-to-pole path has weight $n$, while a dual equatorial cut has weight $m$.

#### Surface-code decoding as a random-bond Ising model

↑ **Parent:** [Surface code](#surface-code)

For independent bit flips, summing the probabilities of all error chains in one syndrome and logical class equals, up to a class-independent factor, the partition function of a random-bond [Ising model](statistical-physics.md#ising-model). A reference error fixes bond signs and products of star stabilizers become Ising spin configurations.

#### Ground-state splitting of a surface-code cylinder

↑ **Parent:** [Surface code](#surface-code)

On a cylinder with equal anyon-condensing boundaries, the two topological ground states split only through a virtual string implementing a logical operator. A perturbation of strength $h$ produces a splitting of order $J$ times a path-counting factor times $(|h|/J)^d$, where $d$ is the shortest supported logical-string length.

#### Toric code

↑ **Parent:** [Surface code](#surface-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Toric_code)

The toric code has commuting star and plaquette stabilizers. Its electric and magnetic excitations are bosons with mutual-semion statistics, and their fusion is a fermion.

##### Surface-code anyon model

↑ **Parent:** [Toric code](#toric-code)

The surface-code anyons are $1,e,m,f=e\times m$. They obey $e^2=m^2=f^2=1$; $e$ and $m$ are bosons with mutual full-braiding phase $-1$, while their composite $f$ is a fermion.

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory.md)
2. [Branches of physics](physics.md#branches-of-physics)
3. [Physics](physics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Distance of a quantum error-correcting code](#distance-of-a-quantum-error-correcting-code)
- [Timed bit flip during repetition-code syndrome extraction](#timed-bit-flip-during-repetition-code-syndrome-extraction)
