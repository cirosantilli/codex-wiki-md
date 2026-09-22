# Quantum information

↑ **Parent:** [2022](../2022.md)

Source paper: [https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1)

Solutions to all three questions.[Cover dated 3 June 2022; printed pp. 2–7, Questions 1–3](../../quantum-information-theory.md#quantum-information-examination-paper-a16608w1-2022) System labels specify the order of each [tensor product of quantum systems](../../tensor-product-of-quantum-systems.md). In an operator product the rightmost operator acts first. In Question 3(d), the stated fidelity is the [squared quantum fidelity](../../quantum-information-theory.md#squared-quantum-fidelity) of the full two-[qubit](../../quantum-system.md#qubit) output with the desired two-copy [pure state](../../quantum-theory.md#pure-state).

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [basic measurement](../../quantum-measurement.md#basic-measurement) of a finite-dimensional [quantum system](../../quantum-system.md) is specified by an [orthonormal basis](../../inner-product.md#orthonormal-basis) $\{|b_j\rangle\}_j$ of its [Hilbert space](../../hilbert-space.md). For a normalized input [pure state](../../quantum-theory.md#pure-state) $|\chi\rangle$, the [Born rule](../../wave-function.md#born-rule) gives

$$
\boxed{p_j=|\langle b_j|\chi\rangle|^2,\qquad
|\chi_j\rangle=\frac{|b_j\rangle\langle b_j|\chi\rangle}{\sqrt{p_j}}
\quad(p_j>0).}
$$

The [post-measurement state](../../quantum-measurement.md#post-measurement-state) is therefore $|b_j\rangle$ up to a [global phase](../../quantum-system.md#global-phase). An outcome of zero [probability](../../probability-theory.md#probability) has no conditional [post-measurement state](../../quantum-measurement.md#post-measurement-state). For a general input [density matrix](../../density-matrix.md) $\rho$, the same [basic measurement](../../quantum-measurement.md#basic-measurement) has $p_j=\langle b_j|\rho|b_j\rangle$ and conditional [density matrix](../../density-matrix.md) $|b_j\rangle\langle b_j|$ whenever $p_j>0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the [Pauli X eigenstates](../../quantum-mechanics.md#pauli-x-eigenstate) $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$ and $\cos\theta+i\sin\theta=e^{i\theta}$. Their [probability amplitudes](../../wave-function.md#probability-amplitude) are

$$
\langle\pm|\phi\rangle=\frac{\sqrt2\pm e^{i\theta}}{\sqrt6}.
$$

The [Born rule](../../wave-function.md#born-rule) gives

$$
\boxed{\Pr(+)=\frac12+\frac{\sqrt2}{3}\cos\theta,\qquad
\Pr(-)=\frac12-\frac{\sqrt2}{3}\cos\theta.}
$$

The two [probabilities](../../probability-theory.md#probability) sum to one. Their dependence on the [relative quantum phase](../../quantum-system.md#relative-quantum-phase) is the [quantum interference](../../quantum-system.md#quantum-interference) between the two components in the [computational basis](../../quantum-theory.md#computational-basis).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

If Alice's [basic measurement](../../quantum-measurement.md#basic-measurement) returns a normalized vector $|u\rangle_A$, form Bob's unnormalized conditional vector

$$
|\widetilde\chi_u\rangle_B=(\langle u|_A\otimes I_B)|\chi\rangle_{AB}.
$$

The [Born rule](../../wave-function.md#born-rule) and normalization give

$$
\boxed{p_u=\|\widetilde\chi_u\|^2,\qquad
|\chi_u\rangle_B=\frac{|\widetilde\chi_u\rangle_B}{\sqrt{p_u}}\quad(p_u>0).}
$$

The joint [post-measurement state](../../quantum-measurement.md#post-measurement-state) is $|u\rangle_A\otimes|\chi_u\rangle_B$. For $|u\rangle_A=\alpha|0\rangle_A+\beta|1\rangle_A$ with real coefficients and $\alpha^2+\beta^2=1$, contraction of the [Bell state](../../bell-state.md) gives

$$
(\langle u|\otimes I)|\phi_+\rangle
=\frac{\alpha|0\rangle+\beta|1\rangle}{\sqrt2},
\qquad p_u=\frac12.
$$

Thus **Bob's normalized conditional state is $\alpha|0\rangle_B+\beta|1\rangle_B$**. For complex coefficients the contraction instead contains their [complex conjugates](../../complex-analysis.md#complex-conjugate); this is the same conjugation underlying [conjugate-basis steering of a Bell pair](../../foundations-of-quantum-mechanics.md#conjugate-basis-steering-of-a-bell-pair).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Let $p_{ab}$ denote the conditional winning [probability](../../probability-theory.md#probability) in the [CHSH game](../../foundations-of-quantum-mechanics.md#chsh-game). With both settings zero, [computational-basis measurements](../../quantum-theory.md#quantum-measurement-in-the-computational-basis) of the [Bell state](../../bell-state.md) always agree, so $p_{00}=1$. When just one setting is one, Bob's conditional [pure state](../../quantum-theory.md#pure-state) from part (i), or the corresponding calculation with Alice and Bob exchanged, gives agreement [probability](../../probability-theory.md#probability) $\cos^2\theta$. Hence $p_{01}=p_{10}=\cos^2\theta$.

For $a=b=1$, winning requires different output [bits](../../information-theory.md#bit). Alice obtains each of her two outcomes with [probability](../../probability-theory.md#probability) $1/2$. Given her first outcome, Bob's desired overlap is

$$
\langle f_1(\theta)|e_0(\theta)\rangle=2\sin\theta\cos\theta=\sin2\theta;
$$

given her second outcome, the other desired overlap is $\langle f_0(\theta)|e_1(\theta)\rangle=-\sin2\theta$. Thus $p_{11}=\sin^2(2\theta)$. Averaging over the four equally likely inputs gives

$$
\boxed{p_{\mathrm{win}}(\theta)=\frac{1+2\cos^2\theta+\sin^2(2\theta)}4
=\frac{3+\cos2\theta-\cos^2(2\theta)}4.}
$$

The maximum winning [probability](../../probability-theory.md#probability) for noncommunicating classical players is $3/4$, the game form of the [CHSH inequality](../../foundations-of-quantum-mechanics.md#chsh-inequality). Setting $t=\cos2\theta$, strict improvement requires $t-t^2>0$, or $0<t<1$. On the stipulated interval this gives

$$
\boxed{0<\theta<\frac\pi4.}
$$

The endpoints give equality with the classical bound. Within this [reflected real-basis CHSH strategy](../../foundations-of-quantum-mechanics.md#reflected-real-basis-chsh-strategy), the maximum is $13/16$ at $t=1/2$, namely $\theta=\pi/6$; this follows by completing the square in $t$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use [entanglement-assisted discrimination of a Pauli basis](../../quantum-information-theory.md#entanglement-assisted-discrimination-of-a-pauli-basis). Define the known single-[qubit](../../quantum-system.md#qubit) [unitary operator](../../vector-space.md#unitary-operator) $V$ by $V|0\rangle=|\psi\rangle$ and $V|1\rangle=|\psi^\perp\rangle$. Prepare the device input $A$ and a reference [ancilla qubit](../../quantum-information-theory.md#ancilla-qubit) $R$ in

$$
|\Omega\rangle_{AR}=(V_A\otimes I_R)|\phi_+\rangle
=\frac{|\psi\rangle_A|0\rangle_R+|\psi^\perp\rangle_A|1\rangle_R}{\sqrt2}.
$$

Apply the unknown device once to $A$, then apply the known inverse $V^\dagger$ to $A$. Since

$$
V^\dagger U_0V=I,\quad V^\dagger U_1V=Z,\quad
V^\dagger U_2V=X,\quad V^\dagger U_3V=iY,
$$

the possible two-[qubit](../../quantum-system.md#qubit) outputs are

$$
\begin{aligned}
U_0:&\quad (|00\rangle+|11\rangle)/\sqrt2,\\
U_1:&\quad (|00\rangle-|11\rangle)/\sqrt2,\\
U_2:&\quad (|01\rangle+|10\rangle)/\sqrt2,\\
U_3:&\quad (|01\rangle-|10\rangle)/\sqrt2.
\end{aligned}
$$

These are the four mutually [orthogonal](../../inner-product.md#orthogonal-vectors) [Bell states](../../bell-state.md). A [Bell-basis measurement](../../bell-state.md#bell-basis-measurement) therefore identifies the device with certainty. Explicitly, apply a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) $A\to R$, then a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on $A$, followed by [computational-basis measurements](../../quantum-theory.md#quantum-measurement-in-the-computational-basis). The readouts $00,10,01,11$ identify $U_0,U_1,U_2,U_3$, respectively. Thus **one use of the device and one reference qubit suffice**.

## 2

↑ **Parent:** [Quantum information](quantum-information.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For normalized vector representatives in the same [Hilbert space](../../hilbert-space.md), two [pure states](../../quantum-theory.md#pure-state) are $\varepsilon$-close in [pure-state norm distance](../../quantum-theory.md#pure-state-norm-distance) when

$$
\boxed{\bigl\||\psi\rangle-|\phi\rangle\bigr\|_2\leq\varepsilon.}
$$

Here $\|\cdot\|_2$ is the [Euclidean norm](../../normed-vector-space.md#euclidean-norm) of the coefficient vector in any [orthonormal basis](../../inner-product.md#orthonormal-basis). Equivalently, $2-2\operatorname{Re}\langle\psi|\phi\rangle\leq\varepsilon^2$. If the convention identifies vector representatives differing by a [global phase](../../quantum-system.md#global-phase), first minimize over that phase, giving $\min_\gamma\||\psi\rangle-e^{i\gamma}|\phi\rangle\|_2=\sqrt{2-2|\langle\psi|\phi\rangle|}$; the vector-norm convention above specifies the representatives.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Two [unitary transformations](../../vector-space.md#unitary-operator) $U,V$ on the same [Hilbert space](../../hilbert-space.md) are $\varepsilon$-close in [operator-norm distance between unitary gates](../../quantum-circuit.md#operator-norm-distance-between-unitary-gates) when

$$
\boxed{\|U-V\|_{\mathrm{op}}
=\sup_{\|\psi\|_2=1}\bigl\|U|\psi\rangle-V|\psi\rangle\bigr\|_2\leq\varepsilon.}
$$

Thus their outputs are $\varepsilon$-close in [pure-state norm distance](../../quantum-theory.md#pure-state-norm-distance) for every normalized input. This is an [operator norm](../../continuous-dual-space.md#operator-norm) condition, stronger than checking only one chosen input. If [global phase](../../quantum-system.md#global-phase) is disregarded for the whole operation, use $\min_\gamma\|U-e^{i\gamma}V\|_{\mathrm{op}}$ instead, with one phase chosen for the operator rather than separately for each input.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

An [entangling gate](../../quantum-circuit.md#entangling-gate) is a [unitary operator](../../vector-space.md#unitary-operator) on two [quantum systems](../../quantum-system.md) for which **some pure product input is mapped to an entangled state**:

$$
\boxed{\exists\,|u\rangle_A,|v\rangle_B:\quad
U(|u\rangle_A\otimes|v\rangle_B)\ \text{is entangled}.}
$$

It need not create [quantum entanglement](../../bell-state.md#entangled-state) from every [product state](../../bell-state.md#product-state). For example, a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) entangles $|+\rangle|0\rangle$ but leaves $|00\rangle$ a [product state](../../bell-state.md#product-state).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

**The gate set is universal.** Since the [Hadamard gate](../../quantum-theory.md#hadamard-gate) satisfies $H^\dagger=H$ and $H^2=I$, the supplied $U$ is a [unitary operator](../../vector-space.md#unitary-operator), and

$$
U^2=\frac{(I-iH)^2}{2}=-iH.
$$

Two applications of $U$ therefore realize a [Hadamard gate](../../quantum-theory.md#hadamard-gate) up to a [global phase](../../quantum-system.md#global-phase). Together with the supplied [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) and [T gate](../../quantum-theory.md#t-gate), this simulates the given [universal quantum gate set](../../quantum-circuit.md#universal-quantum-gate-set).

An exact matrix representative of $H$ can also be synthesized if desired. Put $A=U^2=-iH$ and $S=T^2$. Direct multiplication gives $(AS)^6=-iI$, hence

$$
\boxed{(AS)^{18}A=H.}
$$

This finite product uses only $U$ and $T$, so the conclusion does not rely on discarding a [global phase](../../quantum-system.md#global-phase).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**The gate set is not universal.** The displayed two-[qubit](../../quantum-system.md#qubit) [matrix](../../vector-space.md#matrix) is the [SWAP gate](../../quantum-theory.md#swap-gate):

$$
W(|u\rangle\otimes|v\rangle)=|v\rangle\otimes|u\rangle.
$$

Both $V$ and the [Hadamard gate](../../quantum-theory.md#hadamard-gate) act on one [qubit](../../quantum-system.md#qubit). Thus every gate preserves a fully factored [product state](../../bell-state.md#product-state), and induction gives the same property for every [quantum circuit](../../quantum-circuit.md) built from them. This is the [product-state obstruction to SWAP universality](../../quantum-theory.md#product-state-obstruction-to-swap-universality).

For a quantitative obstruction to even approximate universality, every two-[qubit](../../quantum-system.md#qubit) [product state](../../bell-state.md#product-state) has squared overlap at most $1/2$ with a [Bell state](../../bell-state.md). Indeed, for normalized coefficient vectors $u,v$,

$$
|\langle\phi_+|u\otimes v\rangle|^2
=\frac{|u_0v_0+u_1v_1|^2}{2}\leq\frac12
$$

by the [Cauchy-Schwarz inequality](../../probability-and-statistics.md#cauchy-schwarz-inequality). A [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) acting on $|+\rangle|0\rangle$ would instead produce that [Bell state](../../bell-state.md), so these circuits cannot approximate all [unitary transformations](../../vector-space.md#unitary-operator). The fact that $V^2=e^{-i\pi/8}T$ supplies a [T gate](../../quantum-theory.md#t-gate) up to [global phase](../../quantum-system.md#global-phase) does not supply an [entangling gate](../../quantum-circuit.md#entangling-gate).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Use the [entanglement-assisted promised equality protocol](../../theoretical-computer-science.md#entanglement-assisted-promised-equality-protocol). Alice applies the [phase oracle](../../theoretical-computer-science.md#phase-oracle) $O_x|i\rangle=(-1)^{x_i}|i\rangle$ on $A$, and Bob applies $O_y|i\rangle=(-1)^{y_i}|i\rangle$ on $B$. These are [unitary operators](../../vector-space.md#unitary-operator) because their diagonal entries have [modulus](../../complex-analysis.md#modulus) one. After Alice sends $A$ to Bob, the joint [pure state](../../quantum-theory.md#pure-state) is

$$
|\Omega_{xy}\rangle=\frac1{\sqrt n}\sum_{i=0}^{n-1}(-1)^{x_i+y_i}|ii\rangle.
$$

Let $|\Omega\rangle=n^{-1/2}\sum_i|ii\rangle$ be the original [maximally entangled state](../../quantum-theory.md#maximally-entangled-state). If $d=d_H(x,y)$ is the [Hamming distance](../../coding-theory.md#hamming-distance), then

$$
\langle\Omega|\Omega_{xy}\rangle
=\frac1n\sum_i(-1)^{x_i+y_i}
=\frac{n-d-d}{n}=1-\frac{2d}{n}.
$$

Bob performs the [projective measurement](../../quantum-measurement.md#projective-measurement) with projectors $P=|\Omega\rangle\langle\Omega|$ and $I-P$. Under the promise,

$$
\boxed{d=0\implies\Pr(P)=1,\qquad
d=n/2\implies\Pr(P)=0.}
$$

He declares equal strings for the first outcome and distance $n/2$ for the other. This is exact because the promised outputs occupy [orthogonal](../../inner-product.md#orthogonal-vectors) subspaces. A [basic measurement](../../quantum-measurement.md#basic-measurement) also suffices: extend $|\Omega\rangle$ to an [orthonormal basis](../../inner-product.md#orthonormal-basis) and group all its other outcomes together. Alice transmits one $n$-dimensional system, realizable using $\lceil\log_2n\rceil$ [qubits](../../quantum-system.md#qubit); $n$ need not be a power of two.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Use [Hadamard conjugation of a controlled gate](../../quantum-theory.md#hadamard-conjugation-of-a-controlled-gate) to obtain the [Controlled-Z gate](../../quantum-theory.md#controlled-z-gate):

$$
CZ=(I\otimes H)\operatorname{CNOT}_{1\to2}(I\otimes H)
=\operatorname{diag}(1,1,1,-1).
$$

Conjugating by [Pauli X gates](../../quantum-theory.md#pauli-x-gate) on both [qubits](../../quantum-system.md#qubit) moves its negative entry from $|11\rangle$ to $|00\rangle$:

$$
(X\otimes X)CZ(X\otimes X)=I-2|00\rangle\langle00|.
$$

Finally $(H\otimes H)|00\rangle=|+\rangle|+\rangle=|e_0\rangle$, so a [two-qubit diffusion circuit](../../quantum-theory.md#two-qubit-diffusion-circuit) is

$$
\boxed{C=(H\otimes H)(X\otimes X)(I\otimes H)
\operatorname{CNOT}_{1\to2}(I\otimes H)(X\otimes X)(H\otimes H)=-W.}
$$

In temporal order, apply [Hadamard gates](../../quantum-theory.md#hadamard-gate) on both [qubits](../../quantum-system.md#qubit), [Pauli X gates](../../quantum-theory.md#pauli-x-gate) on both, a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on the second, a [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) $1\to2$, a [Hadamard gate](../../quantum-theory.md#hadamard-gate) on the second, [Pauli X gates](../../quantum-theory.md#pauli-x-gate) on both, then [Hadamard gates](../../quantum-theory.md#hadamard-gate) on both. Every gate is permitted. The overall minus sign is the allowed [global phase](../../quantum-system.md#global-phase), so this implements the required [inversion about the mean](../../quantum-theory.md#inversion-about-the-mean) for [Grover search algorithm](../../quantum-theory.md#grover-s-algorithm).

## 3

↑ **Parent:** [Quantum information](quantum-information.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The two conditions on a [density matrix](../../density-matrix.md) are **positive semidefiniteness and unit trace**:

$$
\boxed{\rho\geq0,\qquad\operatorname{Tr}\rho=1.}
$$

Here [positive semidefinite](../../quadratic-form.md#positive-semidefinite-matrix) includes being a [Hermitian matrix](../../hilbert-space.md#hermitian-operator), with $v^\dagger\rho v\geq0$ for every vector $v$. Equivalently, a [density matrix](../../density-matrix.md) is [Hermitian](../../hilbert-space.md#hermitian-operator) with nonnegative [eigenvalues](../../linear-operator-theory.md#eigenvalue) summing to one.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The [Pauli Z gate](../../quantum-theory.md#pauli-z-gate) gives a **rotation through $\pi$ about the $z$ axis** of the [Bloch sphere](../../density-matrix.md#bloch-sphere). In [Bloch vector](../../density-matrix.md#bloch-vector) coordinates,

$$
\boxed{(r_x,r_y,r_z)\longmapsto(-r_x,-r_y,r_z).}
$$

For example, this follows from $ZXZ=-X$, $ZYZ=-Y$ and $ZZZ=Z$ in the [Pauli matrix](../../algebra.md#pauli-matrices) expansion $\rho=(I+r_xX+r_yY+r_zZ)/2$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Since $H=(X+Z)/\sqrt2$, the [Hadamard gate](../../quantum-theory.md#hadamard-gate) is, up to a [global phase](../../quantum-system.md#global-phase), the [rotation gate](../../quantum-circuit.md#rotation-gate)

$$
e^{-i\pi(X+Z)/(2\sqrt2)}=-iH.
$$

Thus its [Bloch sphere](../../density-matrix.md#bloch-sphere) action is a **rotation through $\pi$ about the axis $(1,0,1)/\sqrt2$**, halfway between the positive $x$ and $z$ axes:

$$
\boxed{(r_x,r_y,r_z)\longmapsto(r_z,-r_y,r_x).}
$$

The identities $HXH=Z$, $HYH=-Y$ and $HZH=X$ verify this [Bloch vector](../../density-matrix.md#bloch-vector) transformation directly.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

**The state is separable.** The [identity matrix](../../vector-space.md#identity-matrix) resolves into the four projectors of the [computational basis](../../quantum-theory.md#computational-basis), giving the explicit [quantum state ensemble](../../density-matrix.md#quantum-state-ensemble)

$$
\boxed{\frac{I_4}{4}=\frac14\sum_{i,j=0}^1
\bigl(|i\rangle\langle i|\bigr)_A\otimes\bigl(|j\rangle\langle j|\bigr)_B
=\frac{I_2}{2}\otimes\frac{I_2}{2}.}
$$

Each member is a [pure state](../../quantum-theory.md#pure-state) that is a [product state](../../bell-state.md#product-state), so this is a [separable quantum state](../../quantum-information-theory.md#separable-quantum-state) by its defining decomposition.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

**The state is separable.** The off-diagonal terms of the two [Bell state](../../bell-state.md) projectors have opposite signs and cancel:

$$
\boxed{\frac12|\phi_+\rangle\langle\phi_+|+\frac12|\phi_-\rangle\langle\phi_-|
=\frac12|00\rangle\langle00|+\frac12|11\rangle\langle11|.}
$$

This is a [quantum state ensemble](../../density-matrix.md#quantum-state-ensemble) of two [pure states](../../quantum-theory.md#pure-state) that are [product states](../../bell-state.md#product-state), with [probability](../../probability-theory.md#probability) $1/2$ each, establishing a [separable quantum state](../../quantum-information-theory.md#separable-quantum-state). Its correlations are classical; an ensemble decomposition into [entangled states](../../bell-state.md#entangled-state) does not itself establish [quantum entanglement](../../bell-state.md#entangled-state) of the [density matrix](../../density-matrix.md).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

For input $|0\rangle_S$, the [controlled-NOT gate](../../quantum-theory.md#controlled-not-gate) fixes $|00\rangle_{SC}$, which is the ideal two-copy [pure state](../../quantum-theory.md#pure-state). Thus its [global cloning fidelity](../../quantum-theory.md#global-cloning-fidelity) is $F_0=1$. For input $|+\rangle_S$, the actual output is the [Bell state](../../bell-state.md) $|\phi_+\rangle$, whereas the desired output is $|++\rangle$. Their overlap is

$$
\langle++|\phi_+\rangle=\frac1{\sqrt2},\qquad F_+=\frac12.
$$

With the given equal input [probabilities](../../probability-theory.md#probability),

$$
\boxed{F_0=1,\qquad F_+=\frac12,\qquad
\overline F=\frac12\left(1+\frac12\right)=\frac34.}
$$

These values use the specified [squared quantum fidelity](../../quantum-information-theory.md#squared-quantum-fidelity) for the full output, rather than a one-copy marginal fidelity.

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

Assume perfect cloning of both specified [pure states](../../quantum-theory.md#pure-state). Allowing irrelevant output [global phases](../../quantum-system.md#global-phase), this would require

$$
U|00\rangle=e^{i\alpha}|00\rangle,
\qquad U|+0\rangle=e^{i\beta}|++\rangle.
$$

A [unitary operator](../../vector-space.md#unitary-operator) preserves [inner products](../../inner-product.md), and therefore their magnitudes. But the input overlap and required output overlap have different magnitudes:

$$
\boxed{|\langle00|+0\rangle|=\frac1{\sqrt2}
\ne\frac12=|\langle00|++\rangle|.}
$$

This contradiction proves that **no such two-qubit unitary exists**, without assuming the [no-cloning theorem](../../quantum-theory.md#no-cloning-theorem).

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

Construct an [economical two-state quantum cloner](../../quantum-theory.md#economical-two-state-quantum-cloner) by moving both actual outputs slightly toward one another relative to the two desired copies. Set $|a\rangle=|00\rangle$ and $|b\rangle=|++\rangle$. Their overlap is $1/2$, so their sum and difference yield the [orthonormal](../../inner-product.md#orthonormal-set) vectors

$$
|u\rangle=\frac{|a\rangle+|b\rangle}{\sqrt3},\qquad
|v\rangle=|a\rangle-|b\rangle.
$$

The desired outputs have the symmetric expressions

$$
|a\rangle=\cos\frac\pi6|u\rangle+\sin\frac\pi6|v\rangle,
\qquad
|b\rangle=\cos\frac\pi6|u\rangle-\sin\frac\pi6|v\rangle.
$$

Choose the actual outputs to be

$$
|c_0\rangle=\cos\frac\pi8|u\rangle+\sin\frac\pi8|v\rangle,
\qquad
|c_+\rangle=\cos\frac\pi8|u\rangle-\sin\frac\pi8|v\rangle.
$$

They are normalized and satisfy

$$
\langle c_0|c_+\rangle=\cos\frac\pi4=\frac1{\sqrt2}
=\langle00|+0\rangle.
$$

Consequently the prescription $|00\rangle\mapsto|c_0\rangle$, $|+0\rangle\mapsto|c_+\rangle$ preserves the [Gram matrix](../../inner-product.md#gram-matrix) of the two inputs and defines a [linear isometry](../../hilbert-space.md#linear-isometry-of-hilbert-spaces) on their span. The [unitary extension of a finite-dimensional isometry](../../hilbert-space.md#unitary-extension-of-a-finite-dimensional-isometry) gives a [unitary operator](../../vector-space.md#unitary-operator) on the same four-dimensional, two-[qubit](../../quantum-system.md#qubit) [Hilbert space](../../hilbert-space.md); no extra workspace is required.

For an explicit full-space construction, define $c=\cos(\pi/8)$, $s=\sin(\pi/8)$ and the [orthonormal basis](../../inner-product.md#orthonormal-basis)

$$
|p\rangle=c|00\rangle+s|10\rangle,\qquad
|m\rangle=s|00\rangle-c|10\rangle,\qquad |01\rangle,\ |11\rangle.
$$

Choose two further [orthonormal](../../inner-product.md#orthonormal-set) vectors perpendicular to $u,v$,

$$
|w\rangle=\frac{|01\rangle-|10\rangle}{\sqrt2},\qquad
|t\rangle=\frac{|01\rangle+|10\rangle-2|11\rangle}{\sqrt6}.
$$

Then

$$
U=|u\rangle\langle p|+|v\rangle\langle m|
+|w\rangle\langle01|+|t\rangle\langle11|
$$

maps one [orthonormal basis](../../inner-product.md#orthonormal-basis) to another and is therefore [unitary](../../vector-bundle.md#unitary-connection). Since $|00\rangle=c|p\rangle+s|m\rangle$ and $|+0\rangle=c|p\rangle-s|m\rangle$, it has exactly the required two outputs.

Finally,

$$
\langle a|c_0\rangle=\langle b|c_+\rangle
=\cos\frac\pi6\cos\frac\pi8+\sin\frac\pi6\sin\frac\pi8
=\cos\frac\pi{24}.
$$

Both inputs therefore have the same [global cloning fidelity](../../quantum-theory.md#global-cloning-fidelity), and so does their average:

$$
\boxed{F_0=F_+=\overline F=\cos^2\frac\pi{24}\approx0.9829629131.}
$$

This proves the requested existence with a two-[qubit](../../quantum-system.md#qubit) [unitary gate](../../quantum-circuit.md#quantum-logic-gate).

## ↑ Ancestors (8)

1. [2022](../2022.md)
2. [Past exam of the computer science course of the University of Oxford](../../past-exam-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
4. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
5. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
6. [University of Oxford](../../university-of-oxford.md)
7. [List of universities](../../README.md#list-of-universities)
8. [Codex Wiki](../../README.md)
