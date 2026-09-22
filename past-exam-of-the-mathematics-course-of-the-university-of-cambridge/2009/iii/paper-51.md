# Paper 51

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper51.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper51.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The answer [qubit](../../../quantum-mechanics.md#qubit) enters the [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) in $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$, because the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) followed by the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) maps $|0\rangle$ to $|-\rangle$. Since $X|-\rangle=-|-\rangle$, [quantum phase kickback](../../../quantum-theory.md#phase-kickback) multiplies the $|xy\rangle$ component by $(-1)^{f(x,y)}$ and leaves the answer [qubit](../../../quantum-mechanics.md#qubit) unchanged. The two input [qubits](../../../quantum-mechanics.md#qubit) enter in the [uniform quantum superposition](../../../quantum-theory.md#uniform-quantum-superposition) $|++\rangle$. Thus

$$
\boxed{|\psi_{abcd}\rangle=\frac{(-1)^d}{2}\sum_{x,y\in\{0,1\}}(-1)^{axy+bx+cy}|xy\rangle\otimes|-\rangle.}
$$

Equivalently, using the [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) and the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate),

$$
|\psi_{abcd}\rangle=(-1)^d\bigl[C_Z^a(Z^b\otimes Z^c)|++\rangle\bigr]\otimes|-\rangle.
$$

Here the exponent in the phase may be evaluated as an ordinary integer, since its parity agrees with the [exclusive or](../../../computer-science.md#exclusive-or) expression. In particular, $d$ contributes only a [global phase](../../../quantum-mechanics.md#global-phase).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

When $a=0$, the first two [qubits](../../../quantum-mechanics.md#qubit) after the [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) are $(-1)^d Z^b|+\rangle\otimes Z^c|+\rangle$. The [Hadamard gate](../../../quantum-theory.md#hadamard-gate) obeys $HZ^t|+\rangle=|t\rangle$ for $t\in\{0,1\}$. Applying the [Walsh-Hadamard transform](../../../quantum-theory.md#walsh-hadamard-transform) therefore gives

$$
(H\otimes H\otimes I)|\psi_{0bcd}\rangle=(-1)^d|bc\rangle\otimes|-\rangle.
$$

Consequently the [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) has the deterministic outcomes

$$
\begin{array}{c|cccc}
\text{oracle}&f_{0001}&f_{0010}&f_{0100}&f_{0110}\\\hline
\text{outcome}&00&01&10&11
\end{array}
$$

These four distinct answers identify the four promised [Boolean quantum oracles](../../../quantum-theory.md#boolean-quantum-oracle) with **one query and certainty**. The constant term does not affect the [measurement in quantum mechanics](../../../quantum-measurement.md), because a [global phase](../../../quantum-mechanics.md#global-phase) does not change its [probabilities](../../../probability-theory.md#probability).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

All four promised functions have $a=1$. Use [quadratic Boolean phase cancellation](../../../quantum-theory.md#quadratic-boolean-phase-cancellation): apply a [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) to remove the phase $(-1)^{xy}$, then apply the [Walsh-Hadamard transform](../../../quantum-theory.md#walsh-hadamard-transform). With the rightmost gate acting first, choose

$$
\boxed{U=(H\otimes H)C_Z.}
$$

Because $C_Z^2=I$ and the [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) commutes with the [Pauli Z gates](../../../quantum-theory.md#pauli-z-gate),

$$
(U\otimes I)|\psi_{1bcd}\rangle=(-1)^d|bc\rangle\otimes|-\rangle.
$$

The [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) consequently produces

$$
\begin{array}{c|cccc}
\text{oracle}&f_{1000}&f_{1011}&f_{1101}&f_{1111}\\\hline
\text{outcome}&00&01&10&11
\end{array}
$$

Each answer occurs with [probability](../../../probability-theory.md#probability) one for its promised [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

In the ordered [computational basis](../../../quantum-theory.md#computational-basis) $00,01,10,11$, the first two [qubits](../../../quantum-mechanics.md#qubit) of $|\psi_{0000}\rangle$ have amplitudes $(1,1,1,1)/2$, while those of $|\psi_{1111}\rangle$ have amplitudes $(-1,1,1,1)/2$. Both have the same normalized answer [qubit](../../../quantum-mechanics.md#qubit) $|-\rangle$. Their [inner product](../../../linear-algebra.md#inner-product) is therefore

$$
\boxed{\langle\psi_{0000}|\psi_{1111}\rangle=\frac{-1+1+1+1}{4}=\frac12.}
$$

A common [unitary operator](../../../vector-space.md#unitary-operator) $U\otimes I$ preserves this nonzero [inner product](../../../linear-algebra.md#inner-product). To distinguish the alternatives with certainty using the prescribed [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis), their first-register outcome supports would have to be disjoint: every outcome possible under one alternative must be impossible under the other. Vectors with disjoint [computational basis](../../../quantum-theory.md#computational-basis) supports have zero [inner product](../../../linear-algebra.md#inner-product), contradicting its preservation. Thus **no such $U$ exists**. This is also an instance of [perfect discrimination of pure states requires orthogonality](../../../quantum-measurement.md#perfect-discrimination-of-pure-states-requires-orthogonality); allowing a more general [measurement in quantum mechanics](../../../quantum-measurement.md) would not rescue this pair of states. The obstruction concerns these prepared oracle-output states, rather than every conceivable oracle-query procedure.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

A classical query with known answer bit $z$ reveals exactly the one bit $f(x,y)$, since it returns $z\oplus f(x,y)$. For the four promised [Boolean functions](../../../combinatorics.md#boolean-function), the value table is

$$
\begin{array}{c|cccc}
(x,y)&1&y&x&x\oplus y\\\hline
00&1&0&0&0\\
01&1&1&0&1\\
10&1&0&1&1\\
11&1&1&1&0
\end{array}
$$

Every possible first query splits the four alternatives into one class of size one and another of size three. On the branch with three remaining alternatives, a second binary answer can separate at most two classes. At least two alternatives therefore still agree on that branch, regardless of how the second query was chosen adaptively. This [decision tree](../../../computer-science.md#decision-tree) argument proves that a procedure guaranteed to identify every alternative needs at least three queries in the worst case.

For sufficiency, query $00,01,10$. The three-bit answer strings for $1,y,x,x\oplus y$ are respectively $111,010,001,011$, which are all distinct. Hence **the exact classical worst-case query requirement is three**. Some individual branches can terminate sooner; the lower bound does not assert that every oracle requires three queries.

## 2

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $N=|A|$. For $N>1$, the unmarked [computational basis](../../../quantum-theory.md#computational-basis) vectors in $A$ give the normalized vector

$$
\boxed{|\omega\rangle=\frac1{\sqrt{N-1}}\sum_{x\in A\setminus\{a\}}|x\rangle
=\frac{\sqrt N|\psi_A\rangle-|a\rangle}{\sqrt{N-1}}.}
$$

Its norm is one and $\langle a|\omega\rangle=0$, so these two vectors form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) for $\mathcal V$. Splitting the [uniform superposition state](../../../quantum-circuit.md#uniform-superposition-state) into its marked and unmarked terms gives

$$
|\psi_A\rangle=\frac1{\sqrt N}|a\rangle+\sqrt{\frac{N-1}{N}}|\omega\rangle,
\qquad\boxed{\theta=\arcsin\frac1{\sqrt N}.}
$$

The nonnegative coefficients select the specified angle in $[0,\pi/2]$.

There is one degenerate boundary case: if $N=1$, then $|\psi_A\rangle=|a\rangle$ and $\mathcal V$ is one-dimensional. No vector in $\mathcal V$ can complete $|a\rangle$ to a two-element [orthonormal basis](../../../linear-algebra.md#orthonormal-basis). Thus the printed two-dimensional description needs $N>1$. For $N=1$ the search itself is already solved, with $\theta=\pi/2$ and no query.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $N>1$, use the [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $(|a\rangle,|\omega\rangle)$ from the preceding part. Both [reflection operators](../../../quantum-theory.md#reflection-operator) preserve $\mathcal V$, because their reflected vectors belong to it. With $s=\sin\theta$ and $c=\cos\theta$, their restricted [matrices](../../../vector-space.md#matrix) are

$$
V_{|a\rangle}=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\qquad
V_{|\psi_A\rangle}=I-2\begin{pmatrix}s^2&sc\\sc&c^2\end{pmatrix}
=\begin{pmatrix}\cos2\theta&-\sin2\theta\\-\sin2\theta&-\cos2\theta\end{pmatrix}.
$$

Multiplying in the specified order, including the overall minus sign, gives

$$
\boxed{G\big|_{\mathcal V}=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.}
$$

Equivalently,

$$
G\big|_{\mathcal V}=\cos2\theta\bigl(|a\rangle\langle a|+|\omega\rangle\langle\omega|\bigr)
+\sin2\theta\bigl(|a\rangle\langle\omega|-|\omega\rangle\langle a|\bigr).
$$

In particular, $G$ sends $\sin t|a\rangle+\cos t|\omega\rangle$ to $\sin(t+2\theta)|a\rangle+\cos(t+2\theta)|\omega\rangle$. This proves the [Grover rotation angle](../../../quantum-theory.md#grover-rotation-angle) description with the signs appropriate to these [reflection operators](../../../quantum-theory.md#reflection-operator).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $N\geq2$, induction using the [Grover rotation angle](../../../quantum-theory.md#grover-rotation-angle) gives

$$
G^k|\psi_A\rangle=\sin((2k+1)\theta)|a\rangle+\cos((2k+1)\theta)|\omega\rangle.
$$

The [quantum measurement in the computational basis](../../../quantum-theory.md#quantum-measurement-in-the-computational-basis) therefore returns $a$ with [probability](../../../probability-theory.md#probability) $\sin^2((2k+1)\theta)$. Since $0<\theta\leq\pi/4$, the first angle interval attaining the required success is

$$
\frac\pi2-\theta\ \leq\ (2k+1)\theta\ \leq\ \frac\pi2+\theta.
$$

The [first successful Grover iterate](../../../quantum-theory.md#first-successful-grover-iterate) is consequently

$$
\boxed{k_{\min}=\left\lceil\frac{\pi}{4\theta}-1\right\rceil
=\left\lceil\frac{\pi}{4\theta}\right\rceil-1.}
$$

Indeed, this is the first integer at or above the lower endpoint requirement $k\geq\pi/(4\theta)-1$. The inequality $\lceil t-1\rceil<t$ also implies $(2k_{\min}+1)\theta<\pi/2+\theta$, so this iterate cannot overshoot the first success interval. Every smaller nonnegative integer lies before that interval and fails the threshold. Finally, $\arcsin u>u$ for $0<u<1$, so

$$
\boxed{k_{\min}<\frac{\pi}{4\theta}<\frac{\pi\sqrt N}{4}.}
$$

For the singleton case $N=1$, measuring the initial state already returns $a$ with certainty, and $k_{\min}=0<\pi/4$. For $N=2$, the requested threshold is only $1/2$, so zero iterations already suffice. These boundary cases agree with the search guarantee.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

List the known distinct strings in $A$ as $a_0,\ldots,a_{N-1}$, where $N=2^m$, and use an $m$-[qubit](../../../quantum-mechanics.md#qubit) index [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla). Apply [Hadamard gates](../../../quantum-theory.md#hadamard-gate) to that register to prepare

$$
|0^n\rangle\otimes\frac1{\sqrt N}\sum_{j=0}^{N-1}|j\rangle.
$$

First, for each $j$ with $a_j\ne0^n$, apply the available [unitary operator](../../../vector-space.md#unitary-operator) that transposes $|0^n,j\rangle$ and $|a_j,j\rangle$. The pairs are disjoint because they have distinct index labels. Skip a transposition when the two vectors coincide. This produces

$$
\frac1{\sqrt N}\sum_j|a_j,j\rangle.
$$

Second, for each $j\ne0$, transpose $|a_j,j\rangle$ and $|a_j,0^m\rangle$. These pairs are disjoint because the data strings $a_j$ are distinct. No pair contains the term with $j=0$, and no later transposition moves an earlier output. The final state is exactly

$$
\boxed{\frac1{\sqrt N}\sum_j|a_j\rangle\otimes|0^m\rangle=|\psi_A\rangle\otimes|0^m\rangle.}
$$

This [clean subset superposition preparation](../../../quantum-theory.md#clean-subset-superposition-preparation) uses at most $N+(N-1)=2N-1$ of the given transpositions and $m$ [Hadamard gates](../../../quantum-theory.md#hadamard-gate). Since $m=O(\log_2 n)$, $N$ is polynomial in $n$; multiplying this count by the assumed polynomial size of each transposition gives a polynomial-size [quantum circuit](../../../quantum-circuit.md). The index [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) returns to zero, so the data register is a pure [uniform superposition state](../../../quantum-circuit.md#uniform-superposition-state), rather than a mixture obtained by discarding its index. The construction uses an available enumeration of the known subset; a membership oracle alone would not justify that enumeration.

## 3

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Using the printed measurement-vector convention, the [unitary operator](../../../vector-space.md#unitary-operator) is

$$
U(\theta)=\frac1{\sqrt2}\begin{pmatrix}1&e^{-i\theta}\\1&-e^{-i\theta}\end{pmatrix}
=H\operatorname{diag}(1,e^{-i\theta})=J(-\theta).
$$

Thus it is a [phase gate](../../../quantum-theory.md#phase-gate) followed by a [Hadamard gate](../../../quantum-theory.md#hadamard-gate), with angle sign opposite to the parameter in the catalogued [J gate](../../../bell-state.md#j-gate-in-measurement-based-quantum-computation). Its rows are the conjugate transposes of the orthonormal measurement vectors, so it is unitary. Right multiplication by the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) changes the sign of the second column, which is exactly the effect of left multiplication by the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate), exchanging the two rows. Explicitly,

$$
U(\theta)Z=\frac1{\sqrt2}\begin{pmatrix}1&-e^{-i\theta}\\1&e^{-i\theta}\end{pmatrix}=XU(\theta).
$$

Similarly, right multiplication by the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) exchanges columns, giving

$$
U(\theta)X=\frac1{\sqrt2}\begin{pmatrix}e^{-i\theta}&1\\-e^{-i\theta}&1\end{pmatrix}
=e^{-i\theta}Z\frac1{\sqrt2}\begin{pmatrix}1&e^{i\theta}\\1&-e^{i\theta}\end{pmatrix}.
$$

Therefore the exact identities, retaining the [global phase](../../../quantum-mechanics.md#global-phase) in the second one, are

$$
\boxed{U(\theta)Z=XU(\theta),\qquad U(\theta)X=e^{-i\theta}ZU(-\theta).}
$$

These supply [Pauli-frame propagation along a measurement wire](../../../bell-state.md#pauli-frame-propagation-along-a-measurement-wire).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write the normalized input [quantum state](../../../quantum-mechanics.md#quantum-state) as $|\psi\rangle=a|0\rangle+b|1\rangle$. The fresh [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) is $|+\rangle$, so the [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) creates

$$
a|0\rangle|+\rangle+b|1\rangle|-\rangle.
$$

Applying the measurement bra $\langle v_k(\theta)|$ to the first [qubit](../../../quantum-mechanics.md#qubit) leaves the unnormalized second-[qubit](../../../quantum-mechanics.md#qubit) vector

$$
|\widetilde\psi_k\rangle=\frac1{\sqrt2}\left(a|+\rangle+(-1)^k e^{-i\theta}b|-\rangle\right).
$$

Since $|+\rangle,|-\rangle$ form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis),

$$
\Pr(k)=\langle\widetilde\psi_k|\widetilde\psi_k\rangle
=\frac{|a|^2+|b|^2}{2}=\frac12.
$$

Also $U(\theta)|\psi\rangle=a|+\rangle+e^{-i\theta}b|-\rangle$, while the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) fixes $|+\rangle$ and changes the sign of $|-\rangle$. Dividing by the branch norm therefore gives

$$
\boxed{|\psi'_k\rangle=X^kU(\theta)|\psi\rangle,\qquad\Pr(k=0)=\Pr(k=1)=\frac12.}
$$

This is [one-bit teleportation](../../../bell-state.md#one-bit-teleportation) with the present positive-exponent measurement vectors; the transferred logical gate is $U(\theta)=J(-\theta)$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Label the chain [cluster state](../../../topological-quantum-matter.md#cluster-state) from top to bottom by $1,2,3,4$, and let $k,l,m$ be the phase-measurement outcomes on the first three vertices, with raw [computational basis](../../../quantum-theory.md#computational-basis) outcome $s$ on vertex four. Repeated [one-bit teleportation](../../../bell-state.md#one-bit-teleportation) leaves the last [qubit](../../../quantum-mechanics.md#qubit), up to [global phase](../../../quantum-mechanics.md#global-phase), in

$$
|\chi\rangle=X^mU(\gamma)X^lU(\beta)X^kU(\alpha)|+\rangle.
$$

This sequential description applies even though the whole [graph state](../../../quantum-circuit.md#graph-state) is prepared first: a later [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) acts only on unmeasured [qubits](../../../quantum-mechanics.md#qubit) and commutes with earlier single-[qubit](../../../quantum-mechanics.md#qubit) measurement operators. It can therefore be moved past those measurements for the purpose of calculating each conditional branch.

Take $\alpha=\theta$ and $\beta=0$, so $U(0)=H$. After the second measurement the logical state is

$$
X^lHX^kU(\theta)|+\rangle=X^lZ^kHU(\theta)|+\rangle.
$$

For binary $p,q$, the identities proved above imply the [Pauli-frame propagation along a measurement wire](../../../bell-state.md#pauli-frame-propagation-along-a-measurement-wire) rule

$$
U(\eta)X^pZ^q\simeq X^qZ^pU((-1)^p\eta),
$$

where $\simeq$ means equality up to [global phase](../../../quantum-mechanics.md#global-phase). Choose the third angle adaptively as $\gamma=(-1)^{l\oplus1}\phi$. Then $(-1)^l\gamma=-\phi$, and

$$
|\chi\rangle\simeq X^{m\oplus k}Z^lU(-\phi)HU(\theta)|+\rangle.
$$

Reading the target circuit in temporal order gives its premeasurement state

$$
|T\rangle=U(\phi)XHU(\theta)H|0\rangle
=e^{-i\phi}ZU(-\phi)HU(\theta)|+\rangle.
$$

Consequently

$$
|\chi\rangle\simeq X^{m\oplus k}Z^{l\oplus1}|T\rangle.
$$

The [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) changes only phases in the [computational basis](../../../quantum-theory.md#computational-basis), while the [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) exchanges its two measurement outcomes. Thus the explicit choices are

$$
\boxed{\alpha=\theta,\quad\beta=0,\quad\gamma=(-1)^{l\oplus1}\phi,\quad\delta=k\oplus m,\quad r=s\oplus k\oplus m.}
$$

Indeed, for every earlier outcome branch,

$$
\Pr(r=t\mid k,l,m)=|\langle t|T\rangle|^2\qquad(t=0,1).
$$

Hence averaging over the earlier random outcomes leaves exactly the target [probability distribution](../../../probability-theory.md#probability-distribution). This implements the desired [measurement-based quantum computation](../../../quantum-circuit.md#measurement-based-quantum-computation) without physically removing the final [Pauli frame](../../../quantum-circuit.md#pauli-frame).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\phi=j\pi/2$ for an integer $j$, and put $q=j\bmod2$. Use the fixed phase-measurement angles $(\theta,0,-\phi)$ and a fixed final [computational basis](../../../quantum-theory.md#computational-basis) measurement. Denote their outcomes by $k,l,m,s$. The adaptive construction would instead use $-\phi$ when $l=0$ and $+\phi$ when $l=1$.

For the printed measurement vectors,

$$
|v_t(\eta+j\pi)\rangle=|v_{t\oplus q}(\eta)\rangle.
$$

Therefore $+\phi$ and $-\phi$ define the same unordered pair of rank-one [linear projections](../../../vector-space.md#projection-linear-algebra); the labels are exchanged if and only if $q=1$. In the branch $l=1$, the outcome that would be called $m_{\mathrm{ad}}$ in the adaptive experiment is thus $m\oplus q$. In both branches,

$$
m_{\mathrm{ad}}=m\oplus ql.
$$

The output correction from the preceding part becomes

$$
\boxed{r=s\oplus k\oplus m\oplus ql.}
$$

If $j$ is even this reduces to $s\oplus k\oplus m$; if $j$ is odd an additional $l$ is included. This [equatorial measurement relabeling at Clifford angles](../../../quantum-measurement.md#equatorial-measurement-relabeling-at-clifford-angles) changes only the classical interpretation, not any physical measurement basis.

All four fixed single-[qubit](../../../quantum-mechanics.md#qubit) [projective measurements](../../../quantum-measurement.md#projective-measurement) act on different vertices, so their operators commute. They can be performed simultaneously, with the displayed classical correction applied afterward. The first angle $\theta$ may be arbitrary: it was never adaptive. Only the sign choice for the third angle needed to be replaced. Thus **the simulation is nonadaptive for every $\phi\in(\pi/2)\mathbb Z$**.

## 4

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For nonnegative integers $n$, assume the storage channel over successive intervals of length $\tau$ composes as $D_\epsilon^n$. This is the memoryless interpretation of the specified storage law. In the [computational basis](../../../quantum-theory.md#computational-basis), write the [density operator](../../../quantum-theory.md#density-matrix) as

$$
\rho=\begin{pmatrix}u&z\\\overline z&1-u\end{pmatrix}.
$$

Conjugation by the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) reverses the off-diagonal entries and leaves the diagonal entries unchanged, so

$$
D_\epsilon(\rho)=\begin{pmatrix}u&(1-2\epsilon)z\\(1-2\epsilon)\overline z&1-u\end{pmatrix}.
$$

After $n$ applications of the [phase-flip channel](../../../quantum-information-theory.md#phase-flip-channel), the multiplier is $(1-2\epsilon)^n$. Comparing with the multiplier $1-2\epsilon_n$ of a single [phase-flip channel](../../../quantum-information-theory.md#phase-flip-channel) gives

$$
\boxed{D_\epsilon^n=D_{\epsilon_n},\qquad\epsilon_n=\frac{1-(1-2\epsilon)^n}{2}.}
$$

For $n=0$ this gives the identity channel. Equivalently, composing two consecutive phase errors cancels them because $Z^2=I$, so their effective probability obeys $\epsilon_{n+1}=\epsilon+(1-2\epsilon)\epsilon_n$. The same expression solves this recurrence. The [iterated phase-flip channel](../../../quantum-information-theory.md#iterated-phase-flip-channel) formula presumes this composition law; specifying a channel at one time alone would not constrain a memory-bearing environment at later times.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Since $0<1-2\epsilon<1$, the off-diagonal multiplier of the [iterated phase-flip channel](../../../quantum-information-theory.md#iterated-phase-flip-channel) tends to zero. Thus

$$
\boxed{\lim_{n\to\infty}D_{\epsilon_n}(\rho)=\frac{\rho+Z\rho Z}{2}
=\begin{pmatrix}u&0\\0&1-u\end{pmatrix}.}
$$

Let $P_0=|0\rangle\langle0|$ and $P_1=|1\rangle\langle1|$ be the [computational basis](../../../quantum-theory.md#computational-basis) measurement projectors. The [nonselective projective measurement](../../../quantum-measurement.md#nonselective-projective-measurement) channel is

$$
P_0\rho P_0+P_1\rho P_1
=u|0\rangle\langle0|+(1-u)|1\rangle\langle1|,
$$

which is exactly the displayed limit. Its diagonal entries retain the original outcome [probabilities](../../../probability-theory.md#probability); the measurement outcome is ignored and the coherences are erased. The limiting evolution is therefore the [completely dephasing channel](../../../quantum-measurement.md#rank-one-dephasing).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Number the three data [qubits](../../../quantum-mechanics.md#qubit) from top to bottom. It suffices initially to follow a pure input $|\psi\rangle=a|0\rangle+b|1\rangle$; linearity will extend the result to every [density operator](../../../quantum-theory.md#density-matrix). The first two [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) create $a|000\rangle+b|111\rangle$. The first layer of [Hadamard gates](../../../quantum-theory.md#hadamard-gate) then encodes this as

$$
a|+++\rangle+b|---\rangle,
$$

the three-[qubit](../../../quantum-mechanics.md#qubit) [phase-flip repetition code](../../../quantum-error-correction.md#phase-flip-repetition-code). Let $e_i$ indicate whether a [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) occurred on data [qubit](../../../quantum-mechanics.md#qubit) $i$ during storage. The next layer of [Hadamard gates](../../../quantum-theory.md#hadamard-gate) uses $HZH=X$ and gives

$$
a|e_1e_2e_3\rangle+b|1\oplus e_1,1\oplus e_2,1\oplus e_3\rangle.
$$

The two initially zero syndrome [quantum ancillas](../../../quantum-information-theory.md#quantum-ancilla) receive the adjacent parities. In the diagram's top-to-bottom order, their [error syndrome](../../../quantum-error-correction.md#error-syndrome) is

$$
s_1=e_1\oplus e_2,\qquad s_2=e_2\oplus e_3.
$$

Both terms of the logical superposition have these same parities, so the syndrome is independent of $a,b$. Measuring it reveals no logical-state information.

At the marked position of $R$ in the printed circuit, there has already been another layer of [Hadamard gates](../../../quantum-theory.md#hadamard-gate) on the data. There is also a layer immediately after $R$. Thus a desired correction $X_i$ in the parity-extraction frame must be implemented as $R=Z_i$ at the actual recovery location, since $H^{\otimes3}Z_iH^{\otimes3}=X_i$. Choose the recovery according to

$$
\boxed{\begin{array}{c|c|c|c}
(s_1,s_2)&\text{weight-zero or one pattern}&\text{complementary pattern}&R\\\hline
00&000&111&I\\
10&100&011&Z_1\\
11&010&101&Z_2\\
01&001&110&Z_3
\end{array}}
$$

The two patterns on each row share a syndrome because complementing all three bits does not change either parity. For a weight-zero or one error, the recovery removes the entire error in the parity-extraction frame. The remaining state is $a|000\rangle+b|111\rangle$, and the two final [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) give $|\psi\rangle|00\rangle$.

For a weight-two or three error, minimum-weight recovery instead leaves all three bits flipped, giving $a|111\rangle+b|000\rangle$. The final [controlled-NOT gates](../../../quantum-theory.md#controlled-not-gate) send this to $(a|1\rangle+b|0\rangle)|00\rangle=X|\psi\rangle|00\rangle$. Consequently, for every input [density operator](../../../quantum-theory.md#density-matrix),

$$
\boxed{\rho'=\rho\quad(k=0,1),\qquad\rho'=X\rho X\quad(k=2,3).}
$$

The logical failure is a [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) after decoding, even though the stored physical errors were [Pauli Z gates](../../../quantum-theory.md#pauli-z-gate): $Z_1Z_2Z_3$ exchanges the two encoded codewords. This is the [logical failure of the three-qubit phase-flip repetition code](../../../quantum-error-correction.md#logical-failure-of-the-three-qubit-phase-flip-repetition-code).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Independent applications of the [phase-flip channel](../../../quantum-information-theory.md#phase-flip-channel) are a classical mixture of the eight physical [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) error patterns. A specified weight-$k$ pattern has [probability](../../../probability-theory.md#probability) $\epsilon^k(1-\epsilon)^{3-k}$. The recovery from the preceding part succeeds on weight zero and one, and yields the logical [Pauli X gate](../../../quantum-theory.md#pauli-x-gate) on weight two and three. There are three weight-two patterns and one weight-three pattern, so the logical failure probability is

$$
p_L=3\epsilon^2(1-\epsilon)+\epsilon^3=3\epsilon^2-2\epsilon^3.
$$

Averaging the corrected branches gives the complete decoded [quantum channel](../../../quantum-information-theory.md#quantum-channel)

$$
\boxed{\rho'=(1-3\epsilon^2+2\epsilon^3)\rho+(3\epsilon^2-2\epsilon^3)X\rho X.}
$$

In particular, the leading logical error is $3\epsilon^2$, rather than an error of first order in $\epsilon$. For the stated range,

$$
\epsilon-p_L=\epsilon(1-\epsilon)(1-2\epsilon)>0.
$$

Thus the failure probability is smaller than the physical error probability. The decoded channel is a bit-flip channel; it is not $D_{p_L}$, whose error operator would be $Z$. This distinction follows from the logical codeword exchange in the [phase-flip repetition code](../../../quantum-error-correction.md#phase-flip-repetition-code).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Take a normalized environment [quantum state](../../../quantum-mechanics.md#quantum-state)

$$
\boxed{|\psi_E\rangle=\sqrt{1-\epsilon}|0\rangle+\sqrt\epsilon|1\rangle.}
$$

The [Controlled-Z gate](../../../quantum-theory.md#controlled-z-gate) is symmetric between the two [qubits](../../../quantum-mechanics.md#qubit), so it can be written with the environment as the controlling system:

$$
C_Z=I\otimes|0\rangle\langle0|+Z\otimes|1\rangle\langle1|.
$$

Expanding the joint [density operator](../../../quantum-theory.md#density-matrix) after the interaction gives

$$
\begin{aligned}
C_Z(\rho\otimes|\psi_E\rangle\langle\psi_E|)C_Z
={}&(1-\epsilon)\rho\otimes|0\rangle\langle0|+\epsilon Z\rho Z\otimes|1\rangle\langle1|\\
&+\sqrt{\epsilon(1-\epsilon)}\bigl(\rho Z\otimes|0\rangle\langle1|+Z\rho\otimes|1\rangle\langle0|\bigr).
\end{aligned}
$$

In the [partial trace](../../../quantum-theory.md#partial-trace), the two off-diagonal environment operators have trace zero, while each diagonal projector has trace one. Hence

$$
\boxed{\operatorname{tr}_E\!\left[C_Z(\rho\otimes|\psi_E\rangle\langle\psi_E|)C_Z\right]
=(1-\epsilon)\rho+\epsilon Z\rho Z=D_\epsilon(\rho).}
$$

Equivalently, the [Kraus operators](../../../quantum-information-theory.md#kraus-operator) are $K_0=\sqrt{1-\epsilon}I$ and $K_1=\sqrt\epsilon Z$, and $K_0^\dagger K_0+K_1^\dagger K_1=I$. This explicit [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) describes the system's dephasing by discarding information in the environment. A fresh environment in this state at each storage interval also realizes the memoryless iteration used in part (a).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
