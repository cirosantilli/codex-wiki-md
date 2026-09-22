# Quantum information

↑ **Parent:** [2023](../2023.md)

Source paper: [https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1)

Solutions to all three questions.[Printed pp. 2–4, Questions 1–3; the cover identifies Trinity Term 2023](../../quantum-information-theory.md#quantum-information-examination-paper-a16608w1-2023) A product such as $|01\rangle$ abbreviates a [tensor product of quantum systems](../../tensor-product-of-quantum-systems.md), with system labels ordered as indicated. Operations in a written sequence are applied from left to right in time; in an operator product, the rightmost operator acts first.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
    - [iii](#3/d/iii)
      - [Solution](#3/d/iii/solution)

## 1

↑ **Parent:** [Quantum information](quantum-information.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A [density matrix](../../density-matrix.md) is a complex $d\times d$ [Hermitian matrix](../../hilbert-space.md#hermitian-operator) that is [positive semidefinite](../../quadratic-form.md#positive-semidefinite-matrix) and has unit [trace](../../linear-algebra.md#matrix-trace):

$$
\boxed{\rho=\rho^\dagger,\qquad v^\dagger\rho v\geq0\ \text{for every }v\in\mathbb C^d,\qquad\operatorname{Tr}\rho=1.}
$$

Equivalently, its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are nonnegative and sum to one, with an [orthonormal basis](../../inner-product.md#orthonormal-basis) of [eigenvectors](../../linear-operator-theory.md#eigenvector).[§1.1.2, printed pp. 17–18, equations (1.94)–(1.97)](../../physics-bibliography.md#the-theory-of-quantum-information-by-john-watrous/mathematical-preliminaries)

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

A [basic measurement](../../quantum-measurement.md#basic-measurement) is specified by an [orthonormal basis](../../inner-product.md#orthonormal-basis) $\{|b_j\rangle\}_{j=0}^{d-1}$. The [Born rule](../../wave-function.md#born-rule) for the [density matrix](../../density-matrix.md) $\rho$ gives the outcome [probabilities](../../probability-theory.md#probability)

$$
\boxed{p(j)=\langle b_j|\rho|b_j\rangle=\operatorname{Tr}\bigl(\rho|b_j\rangle\langle b_j|\bigr).}
$$

These [probabilities](../../probability-theory.md#probability) are nonnegative by [positive semidefiniteness](../../quadratic-form.md#positive-semidefinite-matrix) and sum to one by the [resolution of the identity](../../inner-product.md#resolution-of-the-identity) and unit [trace](../../linear-algebra.md#matrix-trace). In the [computational basis](../../quantum-theory.md#computational-basis), the answers are simply the diagonal entries $\rho_{jj}$.[§2.3, Definition 2.34, measurement probabilities](../../physics-bibliography.md#the-theory-of-quantum-information-by-john-watrous/basic-notions-of-quantum-information)

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Expand the [density matrix](../../density-matrix.md) of the [Bell state](../../bell-state.md) and take the [partial trace](../../quantum-theory.md#partial-trace) over Alice's [qubit](../../quantum-system.md#qubit):

$$
|\phi_+\rangle\langle\phi_+|=\frac12\sum_{j,k=0}^1|j\rangle\langle k|_A\otimes|j\rangle\langle k|_B,
\qquad
\rho_B=\frac12\sum_{j,k=0}^1\langle k|j\rangle|j\rangle\langle k|.
$$

The [orthonormality](../../inner-product.md#orthonormal-set) of the [computational basis](../../quantum-theory.md#computational-basis) removes the off-diagonal terms. Thus Bob's [reduced density matrix](../../bell-state.md#reduced-density-matrix) is the [maximally mixed state](../../density-matrix.md#maximally-mixed-state)

$$
\boxed{\rho_B=\frac12\bigl(|0\rangle\langle0|+|1\rangle\langle1|\bigr)=\frac I2.}
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Write the proposed [quantum state ensemble](../../density-matrix.md#quantum-state-ensemble) as $\{(|u\rangle,p),(|v\rangle,1-p)\}$ with normalized [pure states](../../quantum-theory.md#pure-state), so that

$$
\frac I2=p|u\rangle\langle u|+(1-p)|v\rangle\langle v|.
$$

Taking the [expectation values](../../quantum-system.md#expectation-value) in $|u\rangle$ and $|v\rangle$, and setting $c=|\langle u|v\rangle|^2$, gives

$$
\frac12=p+(1-p)c\geq p,
\qquad
\frac12=pc+1-p\geq1-p.
$$

Consequently $p\leq1/2$ and $p\geq1/2$. Substitution then gives $c=0$. The two [pure states](../../quantum-theory.md#pure-state) are therefore [orthogonal](../../inner-product.md#orthogonal-vectors), with equal [probabilities](../../probability-theory.md#probability):

$$
\boxed{p=\frac12,\qquad |v\rangle=|u^\perp\rangle\ \text{up to a global phase}.}
$$

Conversely, any [orthonormal basis](../../inner-product.md#orthonormal-basis) of a [qubit](../../quantum-system.md#qubit) has projectors summing to $I$, so such a [quantum state ensemble](../../density-matrix.md#quantum-state-ensemble) does give $I/2$. This proves the characterization of [two-state ensembles of a maximally mixed qubit](../../density-matrix.md#two-state-ensembles-of-a-maximally-mixed-qubit).

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Alice uses [conjugate-basis steering of a Bell pair](../../foundations-of-quantum-mechanics.md#conjugate-basis-steering-of-a-bell-pair). Write the desired [orthonormal basis](../../inner-product.md#orthonormal-basis) for Bob as $|\psi\rangle=a|0\rangle+b|1\rangle$ and $|\psi^\perp\rangle=c|0\rangle+d|1\rangle$. Entrywise [complex conjugation](../../complex-analysis.md#complex-conjugation) in the [computational basis](../../quantum-theory.md#computational-basis) gives Alice's [orthonormal basis](../../inner-product.md#orthonormal-basis)

$$
|\overline\psi\rangle=\overline a|0\rangle+\overline b|1\rangle,
\qquad
|\overline{\psi^\perp}\rangle=\overline c|0\rangle+\overline d|1\rangle.
$$

For either $|u\rangle$ in Bob's chosen [orthonormal basis](../../inner-product.md#orthonormal-basis), the corresponding unnormalized conditional [quantum state](../../quantum-system.md#quantum-state) is

$$
(\langle\overline u|_A\otimes I_B)|\phi_+\rangle_{AB}
=\frac1{\sqrt2}\sum_{j=0}^1\langle\overline u|j\rangle|j\rangle_B
=\frac{|u\rangle_B}{\sqrt2}.
$$

Its squared [norm](../../normed-vector-space.md#norm) is $1/2$. Thus **Alice measures in the complex-conjugate basis**, obtaining the required Bob [pure states](../../quantum-theory.md#pure-state) with [probability](../../probability-theory.md#probability) $1/2$ each. Averaging over Alice's undisclosed outcome leaves Bob's [density matrix](../../density-matrix.md) equal to $I/2$, consistent with the [no-communication theorem](../../bell-state.md#no-communication-theorem).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use [deterministic two-qubit entanglement dilution](../../bell-state.md#deterministic-two-qubit-entanglement-dilution), retaining the specified complex [probability amplitudes](../../wave-function.md#probability-amplitude). Alice implements a [quantum instrument](../../quantum-measurement.md#quantum-instrument) on $A$ with [Kraus operators](../../quantum-information-theory.md#kraus-operator)

$$
M_0=\begin{pmatrix}\alpha&0\\0&\beta\end{pmatrix},
\qquad
M_1=\begin{pmatrix}\beta&0\\0&\alpha\end{pmatrix}.
$$

The [Kraus representation](../../quantum-information-theory.md#kraus-representation) completeness condition holds even for complex $\alpha,\beta$:

$$
M_0^\dagger M_0+M_1^\dagger M_1=(|\alpha|^2+|\beta|^2)I=I.
$$

To realize this using the permitted [quantum gates](../../quantum-circuit.md#quantum-logic-gate) and a [basic measurement](../../quantum-measurement.md#basic-measurement), Alice initializes an [ancilla qubit](../../quantum-information-theory.md#ancilla-qubit) $C$ to $|0\rangle$. Conditional on her [computational-basis state](../../quantum-theory.md#computational-basis-state) being $j$, she applies to $C$ the [unitary matrix](../../linear-operator-theory.md#unitary-matrix)

$$
V_0=\begin{pmatrix}\alpha&-\overline\beta\\\beta&\overline\alpha\end{pmatrix},
\qquad
V_1=\begin{pmatrix}\beta&-\overline\alpha\\\alpha&\overline\beta\end{pmatrix}.
$$

Each has [orthonormal](../../inner-product.md#orthonormal-set) columns. Therefore $W=|0\rangle\langle0|_A\otimes V_0+|1\rangle\langle1|_A\otimes V_1$ is a [unitary gate](../../quantum-circuit.md#quantum-logic-gate), with

$$
W\bigl(|u\rangle_A|0\rangle_C\bigr)
=M_0|u\rangle_A|0\rangle_C+M_1|u\rangle_A|1\rangle_C.
$$

A [computational-basis measurement](../../quantum-theory.md#quantum-measurement-in-the-computational-basis) of $C$ implements the desired [quantum instrument](../../quantum-measurement.md#quantum-instrument). Its two unnormalized branches on $AB$ are

$$
(M_0\otimes I)|\phi_+\rangle
=\frac{\alpha|00\rangle+\beta|11\rangle}{\sqrt2},
\qquad
(M_1\otimes I)|\phi_+\rangle
=\frac{\beta|00\rangle+\alpha|11\rangle}{\sqrt2}.
$$

Each has [probability](../../probability-theory.md#probability) $1/2$. Alice sends her outcome $m$ as one classical [bit](../../information-theory.md#bit). For $m=0$, both parties keep their [qubits](../../quantum-system.md#qubit) unchanged. For $m=1$, both apply a [Pauli X gate](../../quantum-theory.md#pauli-x-gate), giving

$$
(X\otimes X)(\beta|00\rangle+\alpha|11\rangle)
=\alpha|00\rangle+\beta|11\rangle.
$$

Thus **both outcomes produce the exact target using one classical bit and local operations**. The construction includes $\alpha=0$ or $\beta=0$ and arbitrary [relative quantum phases](../../quantum-system.md#relative-quantum-phase); it requires no [quantum channel](../../quantum-information-theory.md#quantum-channel) between the parties.

## 2

↑ **Parent:** [Quantum information](quantum-information.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In the ordered [computational basis](../../quantum-theory.md#computational-basis) $|0\rangle,|1\rangle$, the [Pauli X gate](../../quantum-theory.md#pauli-x-gate), [Pauli Y gate](../../quantum-theory.md#pauli-y-gate), [Pauli Z gate](../../quantum-theory.md#pauli-z-gate), [Hadamard gate](../../quantum-theory.md#hadamard-gate) and [T gate](../../quantum-theory.md#t-gate) are

$$
\boxed{\begin{aligned}
X&=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
Y=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\quad
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\\
H&=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},\quad
T=\begin{pmatrix}1&0\\0&e^{i\pi/4}\end{pmatrix}.
\end{aligned}}
$$

In the ordered two-[qubit](../../quantum-system.md#qubit) [computational basis](../../quantum-theory.md#computational-basis) $|00\rangle,|01\rangle,|10\rangle,|11\rangle$, with the first [qubit](../../quantum-system.md#qubit) controlling the second, the [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) is

$$
\boxed{\operatorname{CNOT}_{1\to2}=\begin{pmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{pmatrix}.}
$$

Here the [T gate](../../quantum-theory.md#t-gate) uses the conventional representative with first diagonal entry one; another common representative differs only by a [global phase](../../quantum-system.md#global-phase).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Initialize one [qubit](../../quantum-system.md#qubit) in $|0\rangle$, then apply a [Hadamard gate](../../quantum-theory.md#hadamard-gate), a [T gate](../../quantum-theory.md#t-gate), and a [Hadamard gate](../../quantum-theory.md#hadamard-gate), in that temporal order. Defining the [Pauli X eigenstates](../../quantum-mechanics.md#pauli-x-eigenstate) $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$, the successive [quantum states](../../quantum-system.md#quantum-state) are

$$
|0\rangle\xrightarrow{H}|+\rangle
\xrightarrow{T}\frac{|0\rangle+e^{i\pi/4}|1\rangle}{\sqrt2}
\xrightarrow{H}\boxed{\frac{|+\rangle+e^{i\pi/4}|-\rangle}{\sqrt2}.}
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Initialize three [qubits](../../quantum-system.md#qubit) in $|000\rangle$. Apply a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on the first, then [controlled-NOT gates](../../quantum-theory.md#controlled-not-gate) $1\to2$ and $1\to3$:

$$
|000\rangle\longmapsto\frac{|000\rangle+|100\rangle}{\sqrt2}
\longmapsto\frac{|000\rangle+|111\rangle}{\sqrt2}.
$$

Apply the [T gate](../../quantum-theory.md#t-gate) twice to the first [qubit](../../quantum-system.md#qubit). Because $T^2=\operatorname{diag}(1,i)$, the resulting [GHZ state](../../quantum-theory.md#greenberger-horne-zeilinger-state) with the specified [relative quantum phase](../../quantum-system.md#relative-quantum-phase) is

$$
\boxed{T_1^2\operatorname{CNOT}_{1\to3}\operatorname{CNOT}_{1\to2}H_1|000\rangle
=\frac{|000\rangle+i|111\rangle}{\sqrt2}.}
$$

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Initialize two [qubits](../../quantum-system.md#qubit) in $|00\rangle$. A [Hadamard gate](../../quantum-theory.md#hadamard-gate) on the first followed by a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) $1\to2$ prepares the [Bell state](../../bell-state.md) $|\phi_+\rangle$. The permitted [T gates](../../quantum-theory.md#t-gate) and [Hadamard gates](../../quantum-theory.md#hadamard-gate) implement the needed [Pauli gates](../../quantum-circuit.md#pauli-gate) exactly:

$$
Z=T^4,\qquad X=HT^4H.
$$

Apply $T_1^4$, followed by $H_2,T_2,T_2,T_2,T_2,H_2$. These are a [Pauli Z gate](../../quantum-theory.md#pauli-z-gate) on the first [qubit](../../quantum-system.md#qubit) and a [Pauli X gate](../../quantum-theory.md#pauli-x-gate) on the second, giving

$$
\frac{|00\rangle+|11\rangle}{\sqrt2}
\xrightarrow{Z_1}\frac{|00\rangle-|11\rangle}{\sqrt2}
\xrightarrow{X_2}\boxed{\frac{|01\rangle-|10\rangle}{\sqrt2}.}
$$

Every operation is in the allowed gate set; no [quantum measurement](../../quantum-measurement.md) or probabilistic branch is needed.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use [three-way qutrit sign-flip discrimination](../../quantum-information-theory.md#three-way-qutrit-sign-flip-discrimination). Prepare the [qutrit](../../quantum-system.md#qutrit) in the [uniform superposition state](../../quantum-circuit.md#uniform-superposition-state)

$$
|s\rangle=\frac{|0\rangle+|1\rangle+|2\rangle}{\sqrt3}.
$$

For an unknown label $j\in\{0,1,2\}$, the supplied [unitary operator](../../vector-space.md#unitary-operator) is $U_j=I-2|j\rangle\langle j|$. Apply it once and then apply the known [inversion about the mean](../../quantum-theory.md#inversion-about-the-mean)

$$
D=2|s\rangle\langle s|-I
=\frac13\begin{pmatrix}-1&2&2\\2&-1&2\\2&2&-1\end{pmatrix}.
$$

Since $D^\dagger=D$ and $D^2=I$, this is an allowed [unitary transformation](../../vector-space.md#unitary-operator). Using $\langle s|j\rangle=1/\sqrt3$ gives

$$
DU_j|s\rangle
=D\left(|s\rangle-\frac2{\sqrt3}|j\rangle\right)
=-\frac13|s\rangle+\frac2{\sqrt3}|j\rangle
=\frac{5|j\rangle-\sum_{k\ne j}|k\rangle}{3\sqrt3}.
$$

Perform a [computational-basis measurement](../../quantum-theory.md#quantum-measurement-in-the-computational-basis) and guess that its outcome is the unknown label. The [Born rule](../../wave-function.md#born-rule) gives

$$
\boxed{\Pr(\text{correct}\mid U_j)=\left|\frac5{3\sqrt3}\right|^2=\frac{25}{27}.}
$$

Each incorrect outcome has [probability](../../probability-theory.md#probability) $1/27$, verifying normalization. The success [probability](../../probability-theory.md#probability) is $25/27$ separately for every label, so no assumption about their prior [probabilities](../../probability-theory.md#probability) is needed.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

We prove the [one-query constancy obstruction for phase oracles](../../theoretical-computer-science.md#one-query-constancy-obstruction-for-phase-oracles) while allowing arbitrary [quantum ancillas](../../quantum-information-theory.md#quantum-ancilla). By [purification of a density operator](../../density-matrix.md#purification-of-a-density-operator), the [quantum state](../../quantum-system.md#quantum-state) immediately before the sole query can be taken as

$$
|\Psi\rangle=\sum_{x=0}^{M-1}|x\rangle|a_x\rangle,
\qquad p_x=\langle a_x|a_x\rangle,
\qquad\sum_xp_x=1.
$$

The [ancilla](../../quantum-information-theory.md#quantum-ancilla) vectors need not be normalized or [orthogonal](../../inner-product.md#orthogonal-vectors). Classical randomness and earlier [quantum measurements](../../quantum-measurement.md) can be included in additional [ancillas](../../quantum-information-theory.md#quantum-ancilla); allowing access to these systems only gives the proposed algorithm more power.

For the zero [constant function](../../function.md#constant-function), the [phase oracle](../../theoretical-computer-science.md#phase-oracle) is $I$, leaving $|\Psi\rangle$ unchanged. For each $j$, consider the [Boolean function](../../analysis-of-boolean-functions.md#boolean-function) that is one at $j$ and zero elsewhere. Since $M>2$, it is nonconstant, and its [phase oracle](../../theoretical-computer-science.md#phase-oracle) produces

$$
|\Psi_j\rangle=|\Psi\rangle-2|j\rangle|a_j\rangle,
\qquad\langle\Psi|\Psi_j\rangle=1-2p_j.
$$

Any later fixed [unitary transformation](../../vector-space.md#unitary-operator) preserves these [inner products](../../inner-product.md). An arbitrary final [quantum measurement](../../quantum-measurement.md) cannot distinguish the constant output from each nonconstant output with certainty unless they are [orthogonal](../../inner-product.md#orthogonal-vectors), by [perfect discrimination of pure states requires orthogonality](../../quantum-measurement.md#perfect-discrimination-of-pure-states-requires-orthogonality). Explicitly, an accepting [POVM](../../quantum-measurement.md#positive-operator-valued-measure) effect $E$ would satisfy $E|\Psi\rangle=|\Psi\rangle$ and $E|\Psi_j\rangle=0$, forcing $\langle\Psi|\Psi_j\rangle=0$.

Therefore exact classification requires $p_j=1/2$ for every $j$. Summing gives

$$
\boxed{1=\sum_{j=0}^{M-1}p_j=\frac M2,}
$$

which contradicts $M>2$. Thus **one query cannot decide constancy with certainty**. The other [constant function](../../function.md#constant-function) gives $-I$, differing only by a [global phase](../../quantum-system.md#global-phase), so it does not change the argument. For comparison, $M=2$ permits $p_0=p_1=1/2$; the impossibility arises from demanding the test work for every nonconstant [Boolean function](../../analysis-of-boolean-functions.md#boolean-function).

## 3

↑ **Parent:** [Quantum information](quantum-information.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A bipartite [pure state](../../quantum-theory.md#pure-state) is **entangled exactly when it is not a product state**: there are no normalized [quantum states](../../quantum-system.md#quantum-state) $|u\rangle_A,|v\rangle_B$ such that

$$
|\psi\rangle_{AB}=|u\rangle_A\otimes|v\rangle_B.
$$

Equivalently, its [Schmidt rank](../../von-neumann-entropy.md#schmidt-rank) exceeds one, or either [reduced density matrix](../../bell-state.md#reduced-density-matrix) is a [mixed state](../../density-matrix.md#mixed-state). This definition concerns [quantum entanglement](../../bell-state.md#entangled-state) across the specified division into systems $A$ and $B$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An [entangling gate](../../quantum-circuit.md#entangling-gate) is a [unitary transformation](../../vector-space.md#unitary-operator) $U$ on two [quantum systems](../../quantum-system.md) for which **at least one pure product input has an entangled output**:

$$
\boxed{\exists\,|u\rangle_A,|v\rangle_B:\quad
U(|u\rangle_A\otimes|v\rangle_B)\ \text{is entangled}.}
$$

It need not create [quantum entanglement](../../bell-state.md#entangled-state) on every [product state](../../bell-state.md#product-state). For example, the [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) leaves $|00\rangle$ a [product state](../../bell-state.md#product-state) but maps $|+\rangle|0\rangle$ to a [Bell state](../../bell-state.md), so it is an [entangling gate](../../quantum-circuit.md#entangling-gate).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

The sign factor separates as $(-1)^{x+y}=(-1)^x(-1)^y$. Consequently the [quantum state](../../quantum-system.md#quantum-state) factors into a [tensor product of quantum systems](../../tensor-product-of-quantum-systems.md):

$$
\frac12\sum_{x,y=0}^1(-1)^{x+y}|x\rangle|y\rangle
=\left(\frac{|0\rangle-|1\rangle}{\sqrt2}\right)\otimes\left(\frac{|0\rangle-|1\rangle}{\sqrt2}\right)
=\boxed{|-\rangle\otimes|-\rangle.}
$$

It is a [product state](../../bell-state.md#product-state), so **it is not entangled**.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

Grouping by the first [qubit](../../quantum-system.md#qubit) gives

$$
\frac12\bigl(|00\rangle+|01\rangle+|10\rangle-|11\rangle\bigr)
=\frac{|0\rangle|+\rangle+|1\rangle|-\rangle}{\sqrt2}.
$$

The vectors on both sides form [orthonormal bases](../../inner-product.md#orthonormal-basis), so this is a [Schmidt decomposition](../../von-neumann-entropy.md#schmidt-decomposition) with two nonzero [Schmidt coefficients](../../von-neumann-entropy.md#schmidt-coefficient) $1/\sqrt2$. Hence **the state is maximally entangled**. Independently, its coefficient [matrix](../../vector-space.md#matrix) has [determinant](../../multilinear-algebra.md#determinant)

$$
\det\left[\frac12\begin{pmatrix}1&1\\1&-1\end{pmatrix}\right]=-\frac12\ne0,
$$

which excludes a [product state](../../bell-state.md#product-state) by the [two-qubit product-state determinant criterion](../../bell-state.md#two-qubit-product-state-determinant-criterion). Each [reduced density matrix](../../bell-state.md#reduced-density-matrix) is $I/2$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

Alice holds the input [qubit](../../quantum-system.md#qubit) $Q$ in $|\psi\rangle_Q=a|0\rangle+b|1\rangle$ and her half $A$ of a shared [Bell pair](../../bell-state.md#bell-pair) $|\phi_+\rangle_{AB}$; Bob holds $B$. Alice applies a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) $Q\to A$, then a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on $Q$. In the system order $Q,A,B$, the initial [quantum state](../../quantum-system.md#quantum-state) is

$$
\frac1{\sqrt2}\left(a|000\rangle+a|011\rangle+b|100\rangle+b|111\rangle\right).
$$

After these two [quantum gates](../../quantum-circuit.md#quantum-logic-gate), direct expansion yields the [quantum teleportation](../../bell-state.md#quantum-teleportation) identity

$$
\frac12\Bigl[
|00\rangle_{QA}(a|0\rangle+b|1\rangle)_B
+|01\rangle_{QA}(b|0\rangle+a|1\rangle)_B
+|10\rangle_{QA}(a|0\rangle-b|1\rangle)_B
+|11\rangle_{QA}(-b|0\rangle+a|1\rangle)_B
\Bigr]
=\frac12\sum_{m,n=0}^1|mn\rangle_{QA}X_B^nZ_B^m|\psi\rangle_B.
$$

Alice performs [computational-basis measurements](../../quantum-theory.md#quantum-measurement-in-the-computational-basis) on $Q,A$, and sends the two classical [bits](../../information-theory.md#bit) $m,n$ to Bob. Each outcome has [probability](../../probability-theory.md#probability) $1/4$, independently of the input [pure state](../../quantum-theory.md#pure-state). Bob applies the indicated [Pauli gates](../../quantum-circuit.md#pauli-gate): first $X^n$, then $Z^m$, so his total correction is $Z^mX^n$. In every branch,

$$
\boxed{Z^mX^nX^nZ^m|\psi\rangle=|\psi\rangle.}
$$

This proves exact [quantum teleportation](../../bell-state.md#quantum-teleportation) using one [Bell pair](../../bell-state.md#bell-pair) and two classical [bits](../../information-theory.md#bit). Alice's original [qubit](../../quantum-system.md#qubit) has been measured; the protocol transfers the [quantum state](../../quantum-system.md#quantum-state) without leaving her another copy.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Write the arbitrary initial [pure state](../../quantum-theory.md#pure-state) as

$$
|\chi\rangle_{QR}=|0\rangle_Q|r_0\rangle_R+|1\rangle_Q|r_1\rangle_R,
\qquad\langle r_0|r_0\rangle+\langle r_1|r_1\rangle=1.
$$

The reference vectors need not be normalized or [orthogonal](../../inner-product.md#orthogonal-vectors). By [linearity](../../vector-space.md#linearity), the same [quantum teleportation](../../bell-state.md#quantum-teleportation) calculation, with the [identity operator](../../vector-space.md#identity-operator) on $R$, gives the post-gate [quantum state](../../quantum-system.md#quantum-state)

$$
\frac12\sum_{m,n=0}^1|mn\rangle_{QA}
\left[(X_B^nZ_B^m)\otimes I_R\right]
\left(|0\rangle_B|r_0\rangle_R+|1\rangle_B|r_1\rangle_R\right).
$$

Thus each outcome still has [probability](../../probability-theory.md#probability) $1/4$. Bob's [Pauli gate](../../quantum-circuit.md#pauli-gate) correction leaves the normalized joint [quantum state](../../quantum-system.md#quantum-state)

$$
\boxed{|\chi\rangle_{BR}=|0\rangle_B|r_0\rangle_R+|1\rangle_B|r_1\rangle_R.}
$$

All operations act trivially on $R$, so the result is independent of its holder or location. This establishes [teleportation as an identity channel on a reference](../../bell-state.md#teleportation-as-an-identity-channel-on-a-reference), preserving [quantum entanglement](../../bell-state.md#entangled-state) with the untouched reference. Since every corrected branch is the same, discarding the classical outcomes also leaves the required joint [density matrix](../../density-matrix.md).

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

Combine the hypothetical protocol with [superdense coding](../../bell-state.md#superdense-coding). Before a message is chosen, Alice and Bob share a further [Bell pair](../../bell-state.md#bell-pair) $|\phi_+\rangle_{QR}$, with $Q$ at Alice and $R$ at Bob, in addition to any resources needed for the hypothetical [quantum teleportation](../../bell-state.md#quantum-teleportation) protocol. To encode two classical [bits](../../information-theory.md#bit) $u,v$, Alice applies the [Pauli gates](../../quantum-circuit.md#pauli-gate) $Z_Q^uX_Q^v$, preparing

$$
|\beta_{uv}\rangle_{QR}=(Z_Q^uX_Q^v\otimes I_R)|\phi_+\rangle_{QR}.
$$

The four choices are the four mutually [orthogonal](../../inner-product.md#orthogonal-vectors) [Bell states](../../bell-state.md). Alice now uses the hypothetical protocol to teleport $Q$ to Bob using only one classical [bit](../../information-theory.md#bit). Its assumed preservation of the joint [quantum state](../../quantum-system.md#quantum-state) gives Bob both $B$ and $R$ in

$$
|\beta_{uv}\rangle_{BR}=(Z_B^uX_B^v\otimes I_R)|\phi_+\rangle_{BR}.
$$

Bob performs a [Bell-basis measurement](../../bell-state.md#bell-basis-measurement). Explicitly, a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) $B\to R$, followed by a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on $B$, gives

$$
\boxed{(H_B\otimes I_R)\operatorname{CNOT}_{B\to R}|\beta_{uv}\rangle_{BR}=|u\rangle_B|v\rangle_R.}
$$

A [computational-basis measurement](../../quantum-theory.md#quantum-measurement-in-the-computational-basis) therefore recovers **both message bits with certainty after only one transmitted classical bit**. The initial [Bell pairs](../../bell-state.md#bell-pair) are shared before the message is chosen and carry no message themselves. This proves the [classical communication lower bound for exact qubit teleportation](../../bell-state.md#classical-communication-lower-bound-for-exact-qubit-teleportation): a perfect protocol preserving an external reference needs at least two transmitted classical [bits](../../information-theory.md#bit).

## ↑ Ancestors (8)

1. [2023](../2023.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
