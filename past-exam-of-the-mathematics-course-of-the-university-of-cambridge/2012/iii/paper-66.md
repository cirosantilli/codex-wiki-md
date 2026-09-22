# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_66.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $|0\rangle=|\uparrow_z\rangle$ and $|1\rangle=|\downarrow_z\rangle$. The [total-spin sector](../../../quantum-mechanics.md#total-spin-sector) with spin zero consists of the [spin singlet state](../../../bell-state.md#spin-singlet-state) $|\Psi^-\rangle=(|01\rangle-|10\rangle)/\sqrt2$, not the whole subspace with zero $z$ component. These must be distinguished: the [Bell state](../../../bell-state.md) $|\Psi^+\rangle$ has zero $z$ component but total spin one.

There are two meanings of verification to separate here. A one-pair [entanglement-assisted statistical singlet verification](../../../quantum-measurement.md#entanglement-assisted-statistical-singlet-verification) is possible: choose a shared random axis from $x,y,z$, measure that axis's two-spin parity by the meter circuit below, and accept anticorrelation. An $x$ or $y$ test uses local basis changes before and after the computational-axis circuit. The singlet always passes and is unchanged. Averaging the three acceptance projectors gives

$$
\Omega=\frac13\sum_{j=x,y,z}\frac{I-\sigma_j\otimes\sigma_j}{2}
=P_s+\frac13(I-P_s).
$$

Every triplet state passes with probability $1/3$, so a failure excludes the singlet, while repeated tests on independently prepared copies can give statistical confidence. A single pass does not certify the singlet with certainty.

**Exact single-shot verification cannot be implemented with just one shared Bell pair.** Here exact verification means a yes outcome with probability one on the [spin singlet state](../../../bell-state.md#spin-singlet-state), zero on its orthogonal complement, and preservation of the singlet on yes. If that stronger meaning is intended, the question needs an extra resource. The [Bell-pair cost of exact nondemolition singlet verification](../../../quantum-measurement.md#bell-pair-cost-of-exact-nondemolition-singlet-verification) gives a short proof. For a fully resolved tuple $\mu,\nu$ of local measurement records, contraction of the shared $|\Phi^+\rangle$ gives a system [Kraus operator](../../../quantum-information-theory.md#kraus-operator)

$$
K_{\mu\nu}=\frac1{\sqrt2}\left(A_{\mu0}\otimes B_{\nu0}+A_{\mu1}\otimes B_{\nu1}\right).
$$

Local ancillas and locally adaptive operations are included in these operators. Refining any unobserved local environment gives the same form, so the [operator Schmidt rank](../../../von-neumann-entropy.md#operator-schmidt-rank) is at most two. On each nonzero yes branch, zero false positives forces $K_{\mu\nu}$ to vanish on the entire triplet subspace, and singlet preservation forces

$$
K_{\mu\nu}=c_{\mu\nu}P_s,\qquad
P_s=\frac14(I\otimes I-X\otimes X-Y\otimes Y-Z\otimes Z).
$$

The four [Pauli matrices](../../../algebra.md#pauli-matrices), including the identity, are an orthogonal operator basis. Thus $P_s$ has [operator Schmidt rank](../../../von-neumann-entropy.md#operator-schmidt-rank) four, contradicting the rank-two bound. At least one yes branch is nonzero because the singlet must pass with certainty. Shared classical randomness cannot evade this branchwise argument.

With **two shared Bell pairs**, an explicit corrected protocol is available. On the first meter pair, apply local system-to-meter [CNOT gates](../../../quantum-theory.md#controlled-not-gate) and measure both meters in the computational basis. If their records are $u,v$, the [Kraus operator](../../../quantum-information-theory.md#kraus-operator) is $P_z/\sqrt2$, where $z=(-1)^{u\oplus v}$ and $P_z=(I+zZ_AZ_B)/2$. On the second pair, measure $X_AX_B$ by the same circuit conjugated with local [Hadamard gates](../../../quantum-theory.md#hadamard-gate) on the system. The two parities commute, and their joint projectors are the four [Bell-state nondemolition measurement](../../../bell-state.md#bell-state-nondemolition-measurement) projectors. The singlet is exactly the outcome $(z,x)=(-1,-1)$ and remains unchanged. Local interactions and readouts fit within the stated interval; the combined verdict becomes available only after the records are compared by [classical communication](../../../quantum-information-theory.md#classical-communication).

This corrected exact protocol resolves the triplet into three [Bell states](../../../bell-state.md). It preserves the singlet and every [Bell state](../../../bell-state.md), but generally destroys triplet superpositions. A binary [Lüders rule](../../../quantum-measurement.md#luders-rule) measurement preserving all triplet coherence is a different operation: it violates the [singlet-triplet measurement causality obstruction](../../../quantum-theory.md#singlet-triplet-measurement-causality-obstruction). The one-pair protocol used below measures a single parity and supplies the statistical test above; it does not give exact single-shot singlet verification.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the nonnegative representative of reduction modulo four. The four product [eigenstates](../../../quantum-mechanics.md#eigenstate) and [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\begin{array}{c|rrrr}
\text{state}&|00\rangle&|01\rangle&|10\rangle&|11\rangle\\
\text{eigenvalue}&2&0&0&2
\end{array}
$$

because $-2\equiv2\pmod4$. Consequently the observable is **$I+Z_AZ_B$**. It has the even sector $\operatorname{span}\{|00\rangle,|11\rangle\}$ with value two and the odd sector $\operatorname{span}\{|01\rangle,|10\rangle\}$ with value zero.

The [entanglement-assisted nondemolition parity measurement](../../../quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement) needs just the single shared $|\Phi^+\rangle$ provided in the question. Apply $\operatorname{CNOT}_{A\to d_1}$ and $\operatorname{CNOT}_{B\to d_2}$. For a computational-basis input $|a b\rangle$, the meter becomes

$$
\frac{|a b\rangle_d+|1\oplus a,1\oplus b\rangle_d}{\sqrt2}.
$$

Measuring the meters gives $u\oplus v=a\oplus b$. For an arbitrary coherent system input, its conditional [Kraus operator](../../../quantum-information-theory.md#kraus-operator) is

$$
K_{uv}=\frac1{\sqrt2}P_{u\oplus v},\qquad
P_p=\frac{I+(-1)^pZ_AZ_B}{2}.
$$

It preserves every superposition within the measured sector, so this realizes the [Lüders rule](../../../quantum-measurement.md#luders-rule) for the two degenerate [eigenvalues](../../../linear-operator-theory.md#eigenvalue). The answer is **two for equal meter bits, zero for unequal meter bits**. Each individual meter bit is uniform; only later comparison reveals the parity, respecting [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling). This construction is independent of the defective one-pair singlet-verification request in part (a).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use one shared $|\Phi^+\rangle$ pair to measure $Z_AZ_B$, and the other to measure $X_AX_B$. The latter [entanglement-assisted nondemolition parity measurement](../../../quantum-measurement.md#entanglement-assisted-nondemolition-parity-measurement) is obtained by applying [Hadamard gates](../../../quantum-theory.md#hadamard-gate) to both system [qubits](../../../quantum-mechanics.md#qubit) before and after the $Z$-parity circuit. Since $ZX=-XZ$ at each site, the two minus signs cancel, giving $[Z_AZ_B,X_AX_B]=0$.

The [Bell states](../../../bell-state.md) have joint [eigenvalues](../../../linear-operator-theory.md#eigenvalue)

$$
\begin{array}{c|rrrr}
\text{state}&\Phi^+&\Phi^-&\Psi^+&\Psi^-\\
Z_AZ_B&+1&+1&-1&-1\\
X_AX_B&+1&-1&+1&-1
\end{array}
$$

and are therefore distinguished uniquely by the two meter parities. For records $(u,v)$ and $(r,s)$, the combined [Kraus operator](../../../quantum-information-theory.md#kraus-operator) is

$$
K_{uvrs}=\frac12P_{z,x},\qquad
P_{z,x}=\frac14(I+zZ_AZ_B)(I+xX_AX_B),
\quad z=(-1)^{u\oplus v},\quad x=(-1)^{r\oplus s}.
$$

Each $P_{z,x}$ is the rank-one projector onto the corresponding [Bell state](../../../bell-state.md). This is a [Bell-state nondemolition measurement](../../../bell-state.md#bell-state-nondemolition-measurement): an input [Bell state](../../../bell-state.md) remains exactly that state for every possible local record. The local circuits can be scheduled without communication; the identity of the [Bell state](../../../bell-state.md) is known only when the classical records are brought together. **Two parity bits distinguish all four Bell states without disturbing them.**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Interpret the requested measurement as distinguishing all four stated orthogonal [eigenstates](../../../quantum-mechanics.md#eigenstate), hence as their rank-one [projective measurement](../../../quantum-measurement.md#projective-measurement). If they have indistinguishable degenerate [eigenvalues](../../../linear-operator-theory.md#eigenvalue), this assumption need not hold; the identity observable, for example, cannot reveal the basis and gives no contradiction.

Let Bob initially prepare $|0\rangle_B$. Alice encodes a bit by preparing $|0\rangle_A$ or $|1\rangle_A$, without changing Bob's initial [reduced density matrix](../../../bell-state.md#reduced-density-matrix). If Alice prepares zero, the global input is the first [eigenstate](../../../quantum-mechanics.md#eigenstate), so nondemolition leaves Bob in $|0\rangle$ with certainty. If Alice prepares one, the rank-one [Lüders rule](../../../quantum-measurement.md#luders-rule), after discarding the outcome, dephases Bob in the rotated basis

$$
|u\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle,
\qquad |v\rangle=\sin\theta|0\rangle-\cos\theta|1\rangle.
$$

His output is $\rho_B=\cos^2\theta|u\rangle\langle u|+\sin^2\theta|v\rangle\langle v|$. A computational-basis measurement then gives

$$
\boxed{\Pr_B(1\mid A=0)=0,\qquad
\Pr_B(1\mid A=1)=2\sin^2\theta\cos^2\theta=\tfrac12\sin^2(2\theta).}
$$

It is positive for every $0<\theta\leq\pi/4$. Repeating the experiment would transmit Alice's choice across a spacelike interval, violating [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling). The [controlled-basis measurement causality obstruction](../../../quantum-theory.md#controlled-basis-measurement-causality-obstruction) therefore excludes the entire nonzero interval, including $\pi/4$.

At **$\theta=0$**, the basis is the computational product basis, up to an irrelevant sign on the fourth vector. Alice and Bob each measure $Z$ locally, then compare their results later. Each product [eigenstate](../../../quantum-mechanics.md#eigenstate) is preserved. Thus being a product basis is insufficient for an instantaneous [quantum nondemolition measurement](../../../quantum-measurement.md#quantum-nondemolition-measurement): a remote party's choice of which local basis is measured can still cause signalling.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Quantum teleportation](../../../bell-state.md#quantum-teleportation) transfers the [quantum state](../../../quantum-mechanics.md#quantum-state) of an unknown [qubit](../../../quantum-mechanics.md#qubit) from a sender's carrier to a receiver's carrier. It also transfers correlations with any external reference. It does not determine classical amplitudes or send the original particle.

The standard deterministic protocol consumes **one shared maximally entangled Bell pair and two classical bits** from Alice to Bob. Alice performs a local [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement) on the input and her half of the pair; Bob applies the corresponding local [Pauli gate](../../../quantum-circuit.md#pauli-gate). The classical message is essential: before receiving it, Bob has the outcome-averaged [density operator](../../../quantum-theory.md#density-matrix) $I/2$ and cannot recover or detect the unknown state. The original input is consumed by the measurement, so [quantum teleportation](../../../bell-state.md#quantum-teleportation) is compatible with the [no-cloning theorem](../../../quantum-theory.md#no-cloning-theorem).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write the arbitrary joint [pure state](../../../quantum-theory.md#pure-state) of the input $A$ and an external reference $R$ as

$$
|\Omega\rangle_{AR}=|0\rangle_A|r_0\rangle_R+|1\rangle_A|r_1\rangle_R,
\qquad \langle r_0|r_0\rangle+\langle r_1|r_1\rangle=1.
$$

The reference vectors need not be normalized or orthogonal. Share $|\Phi^+\rangle_{aB}$. Label Alice's [Bell states](../../../bell-state.md) by

$$
|\beta_{rs}\rangle_{Aa}
=\frac1{\sqrt2}\sum_{j=0}^1(-1)^{rj}|j\rangle_A|j\oplus s\rangle_a,
\qquad r,s\in\{0,1\}.
$$

Projecting onto this [Bell basis](../../../quantum-theory.md#bell-basis) gives the unnormalized state

$$
{}_{Aa}\langle\beta_{rs}|\left(|\Omega\rangle_{AR}|\Phi^+\rangle_{aB}\right)
=\frac12(X_B^sZ_B^r\otimes I_R)|\Omega\rangle_{BR}.
$$

Each outcome has probability $1/4$. Alice sends $(r,s)$ and Bob applies **$Z_B^rX_B^s$**, reversing the two [Pauli gates](../../../quantum-circuit.md#pauli-gate). The final state is exactly $|\Omega\rangle_{BR}$ for every outcome. In particular all input [entanglement](../../../bell-state.md#entangled-state) and other correlations with $R$ now belong to $B$, while the reference marginal is unchanged. This is [teleportation as an identity channel on a reference](../../../bell-state.md#teleportation-as-an-identity-channel-on-a-reference).

Conditioned on the record, Alice's two measured carriers are in $|\beta_{rs}\rangle$ and factor from $BR$. Thus $A$ no longer retains its original correlations with $R$. There is no second copy, even when the teleported [qubit](../../../quantum-mechanics.md#qubit) was initially [entangled](../../../bell-state.md#entangled-state) with a larger system.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The root $\omega$ must be a **primitive $n$th root of unity**, for example $e^{2\pi i/n}$. The printed statement merely says $n$th root; that is insufficient. With $n=2$ and $\omega=1$, the states with $r=0$ and $r=1$ coincide. More generally, a root of order $d<n$ repeats the $r$ labels modulo $d$. For $n=1$ the construction is trivial.

For a [primitive root of unity](../../../algebra.md#primitive-root-of-unity), the [generalized Bell basis](../../../quantum-theory.md#generalized-bell-basis) obeys

$$
\langle\psi_{rs}|\psi_{r's'}\rangle
=\delta_{ss'}\frac1n\sum_{j=0}^{n-1}\omega^{j(r'-r)}
=\delta_{ss'}\delta_{rr'}.
$$

The last equality follows from the finite [geometric series](../../../real-analysis.md#geometric-series): a nonzero exponent difference modulo $n$ has sum zero, while zero difference has sum $n$. There are $n^2$ orthonormal vectors in an $n^2$-dimensional [Hilbert space](../../../hilbert-space.md), so they form a complete basis.

For [qudit teleportation](../../../bell-state.md#qudit-teleportation), Alice's input is $|\chi\rangle_U=\sum_jc_j|j\rangle$. Alice and Bob share $|\psi_{00}\rangle_{aB}=n^{-1/2}\sum_k|k k\rangle$. Define the [qudit shift and phase operators](../../../quantum-mechanics.md#qudit-shift-and-phase-operators) by $X|j\rangle=|j+1\rangle$ and $Z|j\rangle=\omega^j|j\rangle$. Alice measures $Ua$ in the [generalized Bell basis](../../../quantum-theory.md#generalized-bell-basis). On outcome $(r,s)$, Bob's unnormalized state is

$$
\frac1n\sum_jc_j\omega^{-rj}|j+s\rangle_B
=\frac1nX^sZ^{-r}|\chi\rangle_B.
$$

All outcomes have probability $1/n^2$. Alice communicates $(r,s)$ and Bob applies

$$
\boxed{Z^rX^{-s},}
$$

which restores $|\chi\rangle$ exactly. The protocol consumes one maximally entangled pair of $n$-level systems, a local $n^2$-outcome measurement, and a classical message with $n^2$ possibilities. For a fixed-length binary encoding, $\lceil\log_2 n^2\rceil$ bits suffice. No measurement depends on the unknown amplitudes.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Bob uses [qudit teleportation](../../../bell-state.md#qudit-teleportation) to teleport his carrier $B_1$ to Clare through the pair $B_2C$. This transfers Bob's entanglement with Alice to Clare. Explicitly, Bob performs a [generalized Bell basis](../../../quantum-theory.md#generalized-bell-basis) measurement on $B_1B_2$. Contraction of the two initial pairs gives

$$
{}_{B_1B_2}\langle\psi_{rs}|
\left(|\psi_{00}\rangle_{AB_1}|\psi_{00}\rangle_{B_2C}\right)
=\frac1{n\sqrt n}\sum_j\omega^{-rj}|j\rangle_A|j+s\rangle_C
=\frac1n(I_A\otimes X_C^sZ_C^{-r})|\psi_{00}\rangle_{AC}.
$$

The probability is $1/n^2$ for each outcome. Bob sends $(r,s)$ to Clare, who applies $Z_C^rX_C^{-s}$. **Alice and Clare then share $|\psi_{00}\rangle_{AC}$ with certainty.** This is [entanglement swapping](../../../bell-state.md#entanglement-swapping); neither an additional entangled pair nor a quantum transmission during the protocol is required.

The two initial pairs are consumed, and Bob's measured carriers cease to be entangled with $AC$. Without Bob's classical record, averaging the possible [generalized Bell states](../../../quantum-theory.md#generalized-bell-state) leaves $AC$ maximally mixed. Thus the conditional [entanglement swapping](../../../bell-state.md#entanglement-swapping) does not supply faster-than-light communication.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [EPR criterion of reality](../../../quantum-theory.md#epr-criterion-of-reality) proposes that a quantity has an element of physical reality when its value can be predicted with certainty without disturbing the system. It is a sufficient criterion, not a claim that every uncertain prediction is unreal. In the original locality argument, measuring one member of a separated correlated pair allows such a prediction for the other, whose physical condition is assumed unaffected by the remote choice.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Combining the [EPR criterion of reality](../../../quantum-theory.md#epr-criterion-of-reality) with perfect predictive correlations and locality motivates pre-existing values for the locally selectable observables. The general [local hidden-variable theory](../../../quantum-theory.md#local-hidden-variable-theory) additionally assumes a complete shared variable $\lambda$ and conditional factorization

$$
p(A,B\mid a,b,\lambda)=p_A(A\mid a,\lambda)p_B(B\mid b,\lambda),
\qquad \rho(\lambda\mid a,b)=\rho(\lambda).
$$

The second condition is [measurement independence](../../../quantum-theory.md#measurement-independence). The reality criterion alone does not prove this factorization for arbitrary imperfect correlations: it motivates the local completion whose consequences are being tested.

A [deterministic local hidden-variable model](../../../quantum-theory.md#deterministic-local-hidden-variable-model) may be used without loss of generality by putting local random seeds into $\lambda$. For each $\lambda$, write its setting responses as $A,A',B,B'\in\{-1,1\}$. Integrating with the same setting-independent distribution and using the [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives

$$
\begin{aligned}
|E(a,b)-E(a,b')|+|E(a',b)+E(a',b')|
&\leq\int d\lambda\,\rho(\lambda)
\left(|A(B-B')|+|A'(B+B')|\right)\\
&=\int d\lambda\,\rho(\lambda)
\left(|B-B'|+|B+B'|\right)=2.
\end{aligned}
$$

Exactly one of $B-B'$ and $B+B'$ vanishes and the other has magnitude two. Hence the requested **CHSH bound is two**. No assumption about the spacelike quantum state enters this local-model derivation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The equal mixture of $|\Phi^+\rangle$ and $|\Phi^-\rangle$ cancels their off-diagonal coherence, leaving the [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state)

$$
\rho(0)=\frac12|00\rangle\langle00|+\frac12|11\rangle\langle11|.
$$

A trivial [LHV model](../../../quantum-theory.md#local-hidden-variable-theory) chooses a shared random bit $j$, uniformly zero or one, and prepares both local [qubits](../../../quantum-mechanics.md#qubit) in $|j\rangle$. Each party uses the local [Born rule](../../../quantum-mechanics.md#born-rule) for its own chosen spin direction, with independent local random seeds if a deterministic description is desired. This reproduces the entire joint measurement distribution, not merely the $z$-axis correlation.

Since the state has an explicit [local hidden-variable theory](../../../quantum-theory.md#local-hidden-variable-theory) for these local measurements, **it cannot violate the CHSH inequality**, by the derivation in part (b). Classical correlation of the shared preparation bit is sufficient; the cancellation of coherence removes the [entanglement](../../../bell-state.md#entangled-state).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

This is the [dephased Bell-state mixture](../../../bell-state.md#dephased-bell-state-mixture) with coherence parameter $2x$. The [Pauli correlation tensor](../../../quantum-theory.md#pauli-correlation-tensor) is

$$
T_{ij}=\operatorname{Tr}[\rho(x)\,\sigma_i\otimes\sigma_j],
\qquad T=\operatorname{diag}(2x,-2x,1),
$$

so spin measurements along unit vectors have $E(\mathbf a,\mathbf b)=\mathbf a^TT\mathbf b$. Choose

$$
\mathbf a=\mathbf e_z,\qquad \mathbf a'=\mathbf e_x,\qquad
\mathbf b=\frac{\mathbf e_z+2x\mathbf e_x}{\sqrt{1+4x^2}},\qquad
\mathbf b'=\frac{-\mathbf e_z+2x\mathbf e_x}{\sqrt{1+4x^2}}.
$$

Then $E(a,b)-E(a,b')=2/\sqrt{1+4x^2}$ and $E(a',b)+E(a',b')=8x^2/\sqrt{1+4x^2}$. The [CHSH inequality](../../../quantum-theory.md#chsh-inequality) expression is therefore

$$
\boxed{S(x)=2\sqrt{1+4x^2}>2\quad\text{for every }0<x\leq\tfrac12.}
$$

These axes also attain the [CHSH optimum from the correlation tensor](../../../quantum-theory.md#chsh-optimum-from-the-correlation-tensor), since the two largest [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of $T^TT$ are $1$ and $4x^2$. At $x=1/2$ the value is $2\sqrt2$; at $x=0$ the explicit [LHV model](../../../quantum-theory.md#local-hidden-variable-theory) in part (c) applies. Thus **exactly $0<x\leq1/2$ has correlations incompatible with a local hidden-variable description**.

Arbitrarily small positive coherence suffices in this particular one-parameter family, with optimally chosen axes; the violation above two tends to zero quadratically as $x\to0$. This does not imply that every entangled mixed state violates a [CHSH inequality](../../../quantum-theory.md#chsh-inequality).

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

All time-dependent [Hamiltonian operators](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) are multiples of the same fixed operator, so they commute and their [time-ordered exponential](../../../perturbative-quantum-field-theory.md#time-ordered-exponential) reduces to an ordinary exponential. Let $P_1=(I-Z_S)/2$. With $\hbar=1$ and the given unit coupling integral,

$$
U=\exp\left[-\frac{i\pi}{2}P_1\otimes(I-X_D)\right]
=P_0\otimes I+P_1\otimes e^{-i\pi(I-X_D)/2}.
$$

Since $X_D^2=I$,

$$
e^{-i\pi(I-X_D)/2}
=e^{-i\pi/2}\left[\cos(\pi/2)I+i\sin(\pi/2)X_D\right]=X_D.
$$

Thus

$$
\boxed{U=P_0\otimes I+P_1\otimes X_D,\qquad
U|s,d\rangle=|s,d\oplus s\rangle.}
$$

It is exactly the [CNOT gate](../../../quantum-theory.md#controlled-not-gate) with $S$ controlling $D$, with no residual relative phase. Acting on $(c_0|0\rangle+c_1|1\rangle)_S|0\rangle_D$ correlates the system basis label with the apparatus label, producing $c_0|00\rangle+c_1|11\rangle$ as required.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In the [Hadamard basis](../../../quantum-theory.md#hadamard-basis), $X_D$ is diagonal with projectors $Q_\pm=(I\pm X_D)/2$. Rewrite the same [CNOT gate](../../../quantum-theory.md#controlled-not-gate) in the original tensor-factor order $S\otimes D$ as

$$
\boxed{U=I_S\otimes Q_+ + Z_S\otimes Q_-.}
$$

Expanding $P_0\otimes I+P_1\otimes X_D$ verifies this identity directly. Now $Z_S|+\rangle=|-\rangle$ and $Z_S|-\rangle=|+\rangle$, so $Z_S$ is $\widetilde X_S$ in the complementary basis. If $D$ is plus, the identity acts on $S$; if $D$ is minus, its sign-basis label flips. Hence $D$ is the control and $S$ the target in this basis.

Equivalently,

$$
(H\otimes H)\operatorname{CNOT}_{S\to D}(H\otimes H)
=\operatorname{CNOT}_{D\to S}.
$$

This [CNOT control reversal in the Hadamard basis](../../../quantum-theory.md#cnot-control-reversal-in-the-hadamard-basis) concerns the matrix in changed local bases, rather than a physical exchange of the two carriers.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Hadamard basis](../../../quantum-theory.md#hadamard-basis) changes the [Pauli matrices](../../../algebra.md#pauli-matrices) by $Z_S=\widetilde X_S$ and $X_D=\widetilde Z_D$. Thus, keeping tensor factors ordered as $S,D$, the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) is

$$
\boxed{H_{\rm int}(t)=\frac{\pi g(t)}4
(I_S-\widetilde X_S)\otimes(I_D-\widetilde Z_D).}
$$

If $D$ has new-basis label plus, the second factor vanishes. If $D$ has label minus, the integrated generator on $S$ is $\pi(I-\widetilde X_S)/2$, whose exponential is $\widetilde X_S$ by part (a). The generator therefore has the same controlled form with $D$ as control in the complementary bases.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

To use $S$ as the apparatus, prepare it in the ready state **$|+\rangle_S$** and later read it in the [Hadamard basis](../../../quantum-theory.md#hadamard-basis). For an arbitrary input $\alpha|+\rangle_D+\beta|-\rangle_D$, part (b) gives

$$
|+\rangle_S(\alpha|+\rangle_D+\beta|-\rangle_D)
\longmapsto
\alpha|+\rangle_S|+\rangle_D+\beta|-\rangle_S|-\rangle_D.
$$

The two apparatus states are orthogonal, so its readout measures the corresponding projectors on $D$ and preserves each input [eigenstate](../../../quantum-mechanics.md#eigenstate). The observable is

$$
\boxed{X_D=\widetilde Z_D,}
$$

with outcomes $+1$ and $-1$. This is the [measurement direction of a CNOT interaction](../../../quantum-theory.md#measurement-direction-of-a-cnot-interaction) in the complementary basis.

The ready state and readout basis matter. Keeping $S$ in the original $|0\rangle_S$ would make the old-basis controlled gate act as the identity on $D$, producing no record. Thus the same interaction can serve either measurement direction, with different apparatus preparation and pointer readout; the [Hamiltonian operator](../../../quantum-mechanics.md#hamiltonian-quantum-mechanics) alone does not assign an intrinsic system/apparatus role.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
