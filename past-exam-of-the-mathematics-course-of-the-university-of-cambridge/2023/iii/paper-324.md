# Paper 324

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_324.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_324.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
    - [iii](#2/c/iii)
      - [Solution](#2/c/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
    - [iii](#4/b/iii)
      - [Solution](#4/b/iii/solution)

## 1

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A [strong classical simulation of a quantum circuit](../../../quantum-circuit.md#strong-classical-simulation-of-a-quantum-circuit) computes any requested output probability

$$
p(y)=\Pr(Y=y),\qquad y\in\{0,1\}^k,
$$

in [polynomial time](../../../computer-science.md#polynomial-time), to the prescribed inverse-polynomial accuracy. A [weak classical simulation of a quantum circuit](../../../quantum-circuit.md#weak-classical-simulation-of-a-quantum-circuit) instead produces classical samples from the circuit's output distribution, with exact or suitably small total-variation error.

The [Extended Gottesman--Knill theorem](../../../quantum-circuit.md#extended-gottesman-knill-theorem) states that a unitary [Clifford circuit](../../../quantum-circuit.md#clifford-circuit) with an arbitrary [product state](../../../bell-state.md#product-state) input and final computational-basis measurements is weakly classically simulable. It is strongly simulable when only $O(\log n)$ output qubits are measured. Indeed, each joint output projector expands into $2^k$ [Pauli operators](../../../quantum-circuit.md#pauli-operator), and Clifford conjugation maps every such operator to another Pauli operator whose expectation factors over the input qubits. The factor $2^k$ is polynomial precisely for $k=O(\log n)$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Choose a [Clifford operation](../../../quantum-circuit.md#clifford-gate) $D$ with $D|0^n\rangle=|\sigma\rangle$ and absorb $D$ into the circuit. Push each subsequent Clifford gate forward through the computation. A computational-basis measurement made after a Clifford prefix $U$ becomes a [Pauli measurement](../../../quantum-theory.md#measurement-of-a-pauli-observable)

$$
Z_j\longmapsto U^\dagger Z_jU
$$

on the initial state, because Clifford conjugation preserves the [Pauli group](../../../quantum-circuit.md#pauli-group). Adaptivity merely makes the next Pauli depend on earlier classical outcomes.

It remains to eliminate the $n$ stabilizer qubits. Maintain their current [stabilizer group](../../../quantum-circuit.md#stabilizer-group). For a Pauli $P$ to be measured, there are two cases.


- If $P$ commutes with every stabilizer generator, its action on the one-dimensional stabilizer sector reduces to a Pauli operator on the remaining $t$ qubits, possibly with a known sign. Measure that effective Pauli on $|\rho\rangle$.
- If $P$ anticommutes with some stabilizer $S$, its outcome $\lambda\in\{+1,-1\}$ is uniformly random. Sample $\lambda$ for an ordinary measurement, or set $\lambda=+1$ when the original measurement is postselected. The Clifford operator


$$
V_\lambda=\frac{I+\lambda PS}{\sqrt2}
$$

maps the old stabilizer sector into the $\lambda$ eigenspace of $P$. Updating the Clifford frame by $V_\lambda$ removes this measurement while conjugating every later Pauli to another Pauli.

Iterating this procedure leaves an adaptive [Pauli-based computation](../../../quantum-theory.md#pauli-based-computation) on $|\rho\rangle$. The same classical outcomes determine every adaptive choice and final output, so this gives a [weak classical simulation](../../../quantum-circuit.md#weak-classical-simulation-of-a-quantum-circuit). Every postselected $Z$ outcome becomes either a fixed classical $+1$ branch or a postselected $+1$ Pauli measurement, as required.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Put $P_1=\sigma_1\otimes\sigma_2$ and $|\psi\rangle=|A\rangle^{\otimes2}$. After the first [Hadamard gate](../../../quantum-theory.md#hadamard-gate) and the two controlled Pauli gates, the joint state is

$$
\frac{|0\rangle|\psi\rangle+|1\rangle P_1|\psi\rangle}{\sqrt2}.
$$

The final Hadamard gate changes this to

$$
\frac12\left[
|0\rangle(I+P_1)|\psi\rangle
+|1\rangle(I-P_1)|\psi\rangle
\right].
$$

Conditioned on ancilla outcome $s\in\{0,1\}$, the normalized data state is therefore

$$
\boxed{
|\Psi_a\rangle=
\frac{[I+(-1)^sP_1]|A\rangle^{\otimes2}}
{\sqrt{2[1+(-1)^s\langle A|^{\otimes2}P_1|A\rangle^{\otimes2}]}}}.
$$

Write the input in the two [eigenspaces](../../../linear-operator-theory.md#eigenspace) of $P_1$ as

$$
|A\rangle^{\otimes2}=\alpha|p_+\rangle+\beta|p_-\rangle,
\qquad
P_1|p_\pm\rangle=\pm|p_\pm\rangle,
$$

where the displayed eigenstates are normalized. A direct PBC measurement gives

$$
|\Psi_b\rangle=
\begin{cases}
|p_+\rangle,&\text{outcome }+1,\\
|p_-\rangle,&\text{outcome }-1,
\end{cases}
$$

with probabilities $|\alpha|^2$ and $|\beta|^2$. Hence the ancilla circuit and the [Pauli measurement](../../../quantum-theory.md#measurement-of-a-pauli-observable) have identical outcome distributions and conditional data states after identifying the Pauli outcome with $(-1)^s$.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Use the standard [ancilla-assisted Pauli measurement](../../../quantum-theory.md#ancilla-assisted-pauli-measurement). To measure a Pauli $P$, reset the ancilla to $|0\rangle$, apply $H$, apply the controlled version of every nonidentity factor of $P$ with the ancilla as control, apply $H$ again, and measure the ancilla in the computational basis. The preceding calculation shows that outcome $s$ projects the data with

$$
\Pi_s(P)=\frac{I+(-1)^sP}{2}.
$$

First use this circuit with $P_1=Z\otimes I$, obtaining $s_1$. Since the measured ancilla is $|s_1\rangle$, apply the classically controlled correction $X^{s_1}$ to reset it to $|0\rangle$. Reuse it to measure $P_2=Z\otimes X$, obtaining $s_2$. All controlled Pauli gates and single-qubit corrections are [Clifford gates](../../../quantum-circuit.md#clifford-gate). Since $P_1P_2=P_2P_1$, the final data state is

$$
\boxed{
|\Psi_{\rm out}\rangle
=\frac{\Pi_{s_2}(P_2)\Pi_{s_1}(P_1)|A\rangle^{\otimes2}}
{\|\Pi_{s_2}(P_2)\Pi_{s_1}(P_1)|A\rangle^{\otimes2}\|}}.
$$

**Thus one resettable ancilla implements both measurements of the PBC without disturbing the already measured Pauli eigenvalue.**

## 2

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let the [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) of the Hermitian matrix be

$$
A=\sum_j\lambda_j|u_j\rangle\langle u_j|,
\qquad
|b\rangle=\sum_j\beta_j|u_j\rangle.
$$

The [HHL algorithm](../../../quantum-theory.md#hhl-algorithm) proceeds as follows.

[ Efficiently](https://ourbigbook.com/-/topic/efficiently) prepare the normalized amplitude encoding $|b\rangle$.  
[ Apply](https://ourbigbook.com/-/topic/apply) [quantum phase estimation](../../../quantum-theory.md#quantum-phase-estimation) to the simulated evolution $e^{iAt}$, producing an approximation of each eigenvalue:

$$
\sum_j\beta_j|u_j\rangle|\widetilde\lambda_j\rangle.
$$

[ Add](https://ourbigbook.com/-/topic/add) one ancilla and perform an eigenvalue-controlled rotation

$$
|\widetilde\lambda_j\rangle|0\rangle
\longmapsto
|\widetilde\lambda_j\rangle
\left(\sqrt{1-\frac{C^2}{\widetilde\lambda_j^2}}|0\rangle
+\frac{C}{\widetilde\lambda_j}|1\rangle\right),
$$

where $0<C\leq\min_j|\lambda_j|$.  
[ Uncompute](https://ourbigbook.com/-/topic/uncompute) the eigenvalue register. Conditional on measuring the ancilla as $1$, the system register is

$$
|x\rangle=
\frac{A^{-1}|b\rangle}{\|A^{-1}|b\rangle\|}
=\frac{\sum_j\beta_j\lambda_j^{-1}|u_j\rangle}
{\sqrt{\sum_j|\beta_j|^2|\lambda_j|^{-2}}}.
$$

The postselection probability can be increased with [amplitude amplification](../../../quantum-theory.md#amplitude-amplification).

The ingredients used here are efficient sparse [Hamiltonian simulation](../../../quantum-theory.md#hamiltonian-simulation) of $e^{iAt}$ and [quantum phase estimation](../../../quantum-theory.md#quantum-phase-estimation), which converts an eigenphase of that evolution into a binary approximation of $\lambda_j$. For sparsity $s$, condition number $\kappa$, and error $\epsilon$, the cost is polynomial in $s$, $\kappa$, $1/\epsilon$, and $\log N$ under the stated access assumptions.

Finally estimate $\langle x|M|x\rangle$ by repeated measurement of an efficient observable decomposition of $M$, or by a [Hadamard test](../../../quantum-theory.md#hadamard-test) when $M$ is unitary. A general efficiently block-encoded Hermitian $M$ can similarly be measured through its block encoding. Repetition and a [concentration inequality](../../../probability-inequality.md#concentration-inequality) give additive sampling error $O(1/\sqrt R)$ after $R$ independent preparations.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The essential requirement is an efficient [quantum state preparation](../../../quantum-circuit.md#quantum-state-preparation) circuit $B$ satisfying

$$
B|0^n\rangle=|b\rangle
=\frac1{\|b\|}\sum_{j=0}^{N-1}b_j|j\rangle.
$$

A standard sufficient promise is that $b$ has only $\operatorname{poly}(\log N)$ nonzero components, with their positions and values classically computable to the required precision in $\operatorname{poly}(\log N)$ time, and with efficiently computable normalization. More structured dense vectors are also allowed whenever cumulative weights or an equivalent data-access oracle permit amplitude encoding in polylogarithmic time. Without such a promise, merely loading $N$ arbitrary classical entries already costs $\Omega(N)$ and removes the claimed exponential dependence on dimension.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Use reversible [quantum arithmetic](../../../quantum-circuit.md#quantum-arithmetic) on an ancillary work register. On each computational-basis branch, compute

$$
|i\rangle|0\rangle|0\rangle
\longmapsto
|i\rangle|A_i\rangle|B_i\rangle
\longmapsto
|i\rangle|A_i\rangle|B_i\rangle|\theta_i\rangle,
$$

where

$$
f_i=\frac{A_i}{B_i},
\qquad
\theta_i=\arccos\sqrt{f_i}.
$$

Because the classical algorithms for $A_i$ and $B_i$ are efficient, they can be made reversible with polynomial overhead. Reversible division, square root, and inverse cosine to the retained binary precision likewise use $\operatorname{poly}(\log N)$ gates under the question's precision convention. Uncompute the $A_i$ and $B_i$ work registers, leaving

$$
\boxed{
|\widetilde\psi_m\rangle
=\sum_{i=0}^{2^m-1}\sqrt{p_i^{(m)}}|i\rangle|\theta_i\rangle}.
$$

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Suppose the angle register stores a fixed-point expansion $\theta_i=\sum_{r=1}^q\theta_{ir}2^{-r}\theta_{\max}$. Append a target qubit in $|0\rangle$. For each angle bit $	heta_{ir}$, apply to the target a controlled $R_y(2^{1-r}\theta_{\max})$. Rotations about the same axis commute, so their product is $R_y(2\theta_i)$ and

$$
|0\rangle\longmapsto
\cos\theta_i|0\rangle+\sin\theta_i|1\rangle.
$$

With $q=O(\operatorname{poly}\log N)$ retained bits, each controlled rotation decomposes into one- and two-qubit gates and the complete [quantum variable rotation](../../../quantum-theory.md#quantum-variable-rotation) has polylogarithmic size. Thus the required branchwise map is implemented coherently for every $i$.

<h4 id="2/c/iii">iii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/c/iii)

The ratio $f_i=A_i/B_i$ is the conditional probability that $X$ lies in the left half of interval $i$. After the controlled rotation and uncomputation of $|\theta_i\rangle$, append the rotation qubit to the interval label. The amplitudes become

$$
\sqrt{p_i^{(m)}f_i},|i0\rangle
+\sqrt{p_i^{(m)}(1-f_i)},|i1\rangle.
$$

But

$$
p_i^{(m)}f_i=p_{2i}^{(m+1)},
\qquad
p_i^{(m)}(1-f_i)=p_{2i+1}^{(m+1)}.
$$

Consequently one refinement step maps

$$
|\psi_m\rangle\longmapsto|\psi_{m+1}\rangle.
$$

Starting from $|\psi_1\rangle$ and repeating this [hierarchical probability-distribution state preparation](../../../quantum-circuit.md#hierarchical-probability-distribution-state-preparation) for $m=1,\ldots,n-1$ gives

$$
\boxed{|\psi_n\rangle
=\sum_{j=0}^{2^n-1}\sqrt{p_j^{(n)}}|j\rangle}.
$$

There are $n-1=O(\log N)$ refinement levels, each of polylogarithmic size by assumption.

## 3

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Let $\Pi_G$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto $G$. The two [reflection operators](../../../quantum-theory.md#reflection-operator) are

$$
I_{|\psi\rangle}=I-2|\psi\rangle\langle\psi|,
\qquad
I_G=I-2\Pi_G.
$$

The first fixes the hyperplane $|\psi\rangle^\perp$ and changes the sign of $|\psi\rangle$; the second fixes $G^\perp$ and changes the sign of $G$.

Write the normalized projections of $|\psi\rangle$ as

$$
|\psi\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle,
\qquad
|g\rangle\in G,
\quad |b\rangle\in G^\perp.
$$

The [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) states that for

$$
R=I_{|\psi\rangle}I_G
$$

one has, up to the irrelevant global sign $(-1)^k$,

$$
\boxed{R^k|\psi\rangle
=(-1)^k\left[
\sin((2k+1)\theta)|g\rangle
+\cos((2k+1)\theta)|b\rangle
\right]}.
$$

Thus every iteration increases the angle toward the good axis by $2\theta$ until the first overshoot.

For the proof, the plane $\operatorname{span}\{|g\rangle,|b\rangle\}$ is invariant. In its ordered basis,

$$
I_G=\begin{pmatrix}-1&0\\0&1\end{pmatrix},
\qquad
I_{|\psi\rangle}
=\begin{pmatrix}
\cos2\theta&-\sin2\theta\\
-\sin2\theta&-\cos2\theta
\end{pmatrix}.
$$

Their product is a planar rotation through $2\theta$ together with an overall sign. Applying that matrix $k$ times proves the formula, while components orthogonal to this plane never enter the initial state.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

If some integer $k$ obeys $(2k+1)\theta=\pi/2$, ordinary [amplitude amplification](../../../quantum-theory.md#amplitude-amplification) already gives $|g\rangle$ exactly. For a general known $\theta$, use [exact amplitude amplification](../../../quantum-theory.md#exact-amplitude-amplification). Choose $k$ so that

$$
\theta'=\frac{\pi}{4k+2}\leq\theta
$$

and put $c=\sin\theta'/\sin\theta\leq1$. Append an ancilla and coherently arrange that its designated good value has amplitude $c$ conditional on the original register being good. With the enlarged good subspace defined by

$$
f(x)=1\quad\text{and}\quad\text{ancilla}=0,
$$

the starting state's total good amplitude is $c\sin\theta=\sin\theta'$.

Apply the [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) $k$ times to this enlarged problem. Its final good amplitude is

$$
\sin((2k+1)\theta')=\sin\frac\pi2=1.
$$

The [Boolean quantum oracle](../../../quantum-theory.md#boolean-quantum-oracle) implements the reflection $I_G$ by phase kickback, and the known state-preparation circuit implements the reflection about the starting state by prepare--reflect--unprepare. A final computational-basis measurement therefore yields an $x$ with $f(x)=1$ with certainty.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

At trial $k$, the [amplitude amplification theorem](../../../quantum-theory.md#amplitude-amplification) gives success probability

$$
p_k=\sin^2((2k+1)\theta).
$$

Because the state is prepared afresh, the probability that the first success occurs at $k$ is

$$
\boxed{
\Pr(k^*=k)=p_k\prod_{j=0}^{k-1}(1-p_j)
=\sin^2((2k+1)\theta)
\prod_{j=0}^{k-1}\cos^2((2j+1)\theta)}.
$$

If one application of $R$ uses a constant number of oracle calls, reaching and performing trial $k$ costs a total of order $1+2+\cdots+k=\Theta(k^2)$ calls. Equivalently,

$$
\mathbb E C
=\Theta\left(
\sum_{k\geq1}k
\prod_{j=0}^{k-1}\cos^2((2j+1)\theta)
\right).
$$

For $k\theta\ll1$, use $\log\cos^2x=-x^2+O(x^4)$ and

$$
\sum_{j=0}^{k-1}(2j+1)^2=\frac{k(4k^2-1)}3
$$

to obtain

$$
\Pr(k^*\geq k)
=\exp\left[-\frac43\theta^2k^3+o(\theta^2k^3)\right].
$$

The first successful index is therefore typically $k^*=\Theta(\theta^{-2/3})$, and

$$
\boxed{\mathbb E C=\Theta(\theta^{-4/3})
=\Theta((n^*)^{4/3})},
$$

where $n^*=\Theta(1/\theta)$ is the first near-optimal Grover iteration count.

The last requested assertion in the official paper is false as printed. In fact, for small $\theta$, at least a constant fraction of the indices $j<n^*$ have $(2j+1)\theta\geq\pi/4$, and hence failure probability at most $1/2$. Consequently

$$
\boxed{\Pr(k^*\geq n^*)
=\prod_{j=0}^{n^*-1}\cos^2((2j+1)\theta)
\leq 2^{-c n^*}\longrightarrow0}
$$

for some constant $c>0$, rather than being bounded below by a positive constant. The reversed event $\Pr(k^*<n^*)$ does have a positive lower bound and in fact tends to one.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Now try only $k_i=2^i$. Since $n^*=2^N=\Theta(1/\theta)$, the total work through trial $N$ is the [geometric series](../../../real-analysis.md#geometric-series)

$$
\sum_{i=0}^N2^i=2^{N+1}-1=\Theta(n^*).
$$

For $i<N$, the success probabilities scale as

$$
p_i=\sin^2((2^{i+1}+1)\theta)
=O\left(\frac{4^i}{(n^*)^2}\right).
$$

Their sum is $O(1)$, so the product of their failure probabilities stays bounded away from zero: there is a constant probability of reaching the scale $k_N=n^*$. At that trial, the defining property of $n^*$ gives

$$
p_N=\sin^2((2n^*+1)\theta)=1-O(\theta^2),
$$

so almost all surviving runs stop there. Therefore

$$
\boxed{\mathbb E C=\Theta(n^*)=\Theta(1/\theta)}.
$$

The [geometric amplitude-amplification schedule](../../../quantum-theory.md#geometric-amplitude-amplification-schedule) is asymptotically better than the sequential schedule's $\Theta((n^*)^{4/3})$ calls and matches the usual Grover scaling up to a constant factor.

## 4

↑ **Parent:** [Paper 324](paper-324.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

A computational-basis vector $|x_1x_2x_3\rangle$ has eigenvalue $(-1)^{x_i+x_j}$ under $Z_iZ_j$. Simultaneous eigenvalue $+1$ for $Z_1Z_2$, $Z_2Z_3$, and $Z_1Z_3$ therefore requires

$$
x_1=x_2=x_3.
$$

The [stabilizer subspace](../../../quantum-circuit.md#stabilizer-subspace) is

$$
\boxed{V_S=\operatorname{span}\{|000\rangle,|111\rangle\}}.
$$

It is two-dimensional because the three displayed nonidentity stabilizers contain only two independent generators; indeed $(Z_1Z_2)(Z_2Z_3)=Z_1Z_3$.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

For the [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) $U=\operatorname{CNOT}_{12}$, propagation of the Pauli generators gives

$$
\boxed{
UX_1U^\dagger=X_1X_2,
\qquad UX_2U^\dagger=X_2,
\qquad UZ_1U^\dagger=Z_1,
\qquad UZ_2U^\dagger=Z_1Z_2}.
$$

Thus an $X$ on the control propagates forward to the target, while a $Z$ on the target propagates backward to the control.

Suppose $\widetilde V$ has the same four conjugation rules and put $W=U^\dagger\widetilde V$. Then $W$ commutes with $X_1,X_2,Z_1,Z_2$. These generators span the full two-qubit operator algebra, so its [commutant](../../../group-theory.md#centralizer) consists only of scalar multiples of the identity. Hence $W=e^{i\phi}I$ and

$$
\boxed{\widetilde V=e^{i\phi}U}.
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

Since the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) conjugates $X$ to $Z$,

$$
V_n=e^{i\pi(X\otimes X)/n},
\qquad
W_n=e^{i\pi(X\otimes Z)/n}.
$$

For $n=1$, each exponential is $-I$, so

$$
V_1W_1=I=e^{iA_1},
\qquad
\boxed{A_1=0}.
$$

For $n=2$,

$$
V_2=iX\otimes X,
\qquad
W_2=iX\otimes Z.
$$

Using $XZ=-iY$ gives

$$
V_2W_2=-I\otimes XZ=iI\otimes Y
=\exp\left(i\frac\pi2I\otimes Y\right),
$$

so one convenient logarithm is

$$
\boxed{A_2=\frac\pi2I\otimes Y}.
$$

Both products are [Clifford operations](../../../quantum-circuit.md#clifford-gate): the first is the identity and the second is a one-qubit [Pauli Y gate](../../../quantum-theory.md#pauli-y-gate) up to global phase.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

A [graph state](../../../quantum-circuit.md#graph-state) has computational-basis expansion

$$
|G\rangle=\frac1{2^{|V|/2}}
\sum_{x\in\{0,1\}^{|V|}}
(-1)^{\sum_{(r,s)\in E}x_rx_s}|x\rangle.
$$

For the path $G_A$ with edges $(1,2)$ and $(2,3)$,

$$
\boxed{
|G_A\rangle=\frac1{\sqrt8}(
|000\rangle+|001\rangle+|010\rangle-|011\rangle
+|100\rangle+|101\rangle-|110\rangle+|111\rangle)}.
$$

For the triangle $G_B$, the extra edge $(3,1)$ changes the phase whenever $x_1=x_3=1$, giving

$$
\boxed{
|G_B\rangle=\frac1{\sqrt8}(
|000\rangle+|001\rangle+|010\rangle-|011\rangle
+|100\rangle-|101\rangle-|110\rangle-|111\rangle)}.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

The [graph-state stabilizer generators](../../../quantum-circuit.md#graph-state-stabilizer-generator) of the path are

$$
S_1^A=X_1Z_2,
\qquad
S_2^A=Z_1X_2Z_3,
\qquad
S_3^A=Z_2X_3,
$$

and those of the triangle are

$$
S_1^B=X_1Z_2Z_3,
\qquad
S_2^B=Z_1X_2Z_3,
\qquad
S_3^B=Z_1Z_2X_3.
$$

Any pair of distinct generators has Pauli factors $X$ and $Z$ in exactly two common positions. Each such position contributes one minus sign on exchange, so the two signs cancel. Thus

$$
\boxed{[S_r^A,S_s^A]=[S_r^B,S_s^B]=0
\quad\text{for all }r,s}.
$$

This is the general commutativity mechanism for graph-state stabilizers associated with an undirected graph.

<h4 id="4/b/iii">iii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/b/iii)

If $S|\alpha\rangle=|\alpha\rangle$ and $|\beta\rangle=U|\alpha\rangle$, then

$$
(USU^\dagger)|\beta\rangle
=US|\alpha\rangle
=U|\alpha\rangle
=|\beta\rangle.
$$

Thus conjugating the state conjugates its entire [stabilizer group](../../../quantum-circuit.md#stabilizer-group).

The triangle $G_B$ is obtained from the path $G_A$ by [local complementation of a graph state](../../../quantum-circuit.md#local-complementation-of-a-graph-state) at vertex $2$, which toggles the edge between its neighbors $1$ and $3$. The corresponding [Local Clifford operation](../../../quantum-circuit.md#local-clifford-operation) is

$$
U_2=exp\left(-\frac{i\pi}{4}X_2\right)
\exp\left(\frac{i\pi}{4}Z_1\right)
\exp\left(\frac{i\pi}{4}Z_3\right).
$$

Direct conjugation gives

$$
U_2S_1^AU_2^\dagger=Y_1Y_2=S_1^BS_2^B,
$$



$$
U_2S_2^AU_2^\dagger=S_2^B,
$$



$$
U_2S_3^AU_2^\dagger=Y_2Y_3=S_2^BS_3^B.
$$

These three commuting operators generate exactly the same [stabilizer group](../../../quantum-circuit.md#stabilizer-group) as $S_1^B,S_2^B,S_3^B$. Therefore

$$
\boxed{|G_B\rangle=e^{i\phi}U_2|G_A\rangle}
$$

for an irrelevant global phase $e^{i\phi}$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
