# Paper 325

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_325.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_325.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a bipartite [density operator](../../../quantum-theory.md#density-matrix) $\rho_{SA}$, the [reduced density matrix](../../../bell-state.md#reduced-density-matrix) of $S$ is

$$
\boxed{\rho_S=\operatorname{Tr}_A\rho_{SA}}.
$$

It is characterized by

$$
\operatorname{Tr}_S(M_S\rho_S)
=\operatorname{Tr}_{SA}[(M_S\otimes I_A)\rho_{SA}]
$$

for every observable $M_S$ on $S$. Equivalently, in any [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $\{|a_k\rangle\}$ of $A$, the [partial trace](../../../quantum-theory.md#partial-trace) is

$$
\rho_S=\sum_k(I_S\otimes\langle a_k|)\rho_{SA}
(I_S\otimes|a_k\rangle),
$$

and the result is independent of that basis.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let the apparatus begin in a ready state $|A_0\rangle$. An ideal unitary measurement interaction is defined on the relevant subspace by

$$
U(|e_i\rangle|A_0\rangle)=|e_i\rangle|i\rangle.
$$

Thus an initial $|\phi\rangle=\sum_i a_i|e_i\rangle$ evolves to the entangled state

$$
|\Psi\rangle=\sum_i a_i|e_i\rangle|i\rangle,
$$

and orthogonality of the pointer states gives

$$
\boxed{\rho_S=\operatorname{Tr}_A|\Psi\rangle\langle\Psi|
=\sum_i|a_i|^2|e_i\rangle\langle e_i|}.
$$

Before the interaction, the [Born rule](../../../quantum-mechanics.md#born-rule) gives

$$
\boxed{\Pr(P_{ij}=1)
=|\langle\psi_{ij}|\phi\rangle|^2
=\frac12|a_i+a_j|^2}.
$$

Afterward,

$$
\boxed{\Pr(P_{ij}=1)
=\operatorname{Tr}(P_{ij}\rho_S)
=\frac12(|a_i|^2+|a_j|^2)}.
$$

The missing cross term is the lost interference between the $i$ and $j$ branches. Entanglement with orthogonal pointer records therefore explains [quantum decoherence](../../../quantum-theory.md#quantum-decoherence) and the appearance of a classical mixture to the subsystem. It does not solve the [quantum measurement problem](../../../quantum-theory.md#measurement-problem): unitary evolution alone does not explain why one definite pointer value is observed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Einstein–Podolsky–Rosen criterion of reality](../../../quantum-theory.md#einstein-podolsky-rosen-criterion-of-reality) says that if a physical quantity can be predicted with certainty without disturbing a system, then an element of physical reality corresponds to that quantity.

Let $X_i,Y_i$ be Pauli measurements on particle $i$. The [GHZ state](../../../quantum-theory.md#greenberger-horne-zeilinger-state) in the question obeys

$$
X_1Y_2Y_3=+1,\qquad
Y_1X_2Y_3=+1,\qquad
Y_1Y_2X_3=+1
$$

with certainty. Each local outcome can therefore be predicted by spacelike-separated measurements on the other two particles. The EPR criterion assigns predetermined values $x_i,y_i\in\{-1,1\}$ satisfying those three equations. Multiplying them and using $y_i^2=1$ gives

$$
x_1x_2x_3=+1.
$$

Quantum theory instead predicts

$$
X_1X_2X_3|\psi_{\rm GHZ}\rangle=-|\psi_{\rm GHZ}\rangle,
$$

so a joint $X$ measurement has product $-1$ with certainty. The EPR elements of reality therefore contradict the quantum prediction, which is the [GHZ theorem](../../../quantum-theory.md#ghz-theorem) form of [Bell theorem](../../../quantum-theory.md#bell-theorem).

## 2

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The outputs satisfy

$$
a\mathbin\oplus b=xy,
$$

and each allowed pair occurs with probability $1/2$. This is a [Popescu–Rohrlich box](../../../quantum-theory.md#popescu-rohrlich-box). For either party, summing over the remote output gives a uniform local bit:

$$
P(a=0|x,y)=P(a=1|x,y)=\frac12,
$$

independently of $y$, and similarly for Bob independently of $x$. The device is therefore a [no-signalling box](../../../quantum-theory.md#no-signalling-box) and does not necessarily permit superluminal signalling, despite correlations stronger than quantum theory allows.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For input pairs other than $11$, either local output is the equiprobable ensemble $\{|+\rangle,|-\rangle\}$; for input $11$, it is $\{|0\rangle,|1\rangle\}$. Both ensembles have the same [density operator](../../../quantum-theory.md#density-matrix),

$$
\frac12(|+\rangle\langle+|+|-\rangle\langle-|)
=\frac12(|0\rangle\langle0|+|1\rangle\langle1|)
=\frac I2.
$$

Every local [measurement in quantum mechanics](../../../quantum-measurement.md) therefore has the same statistics for every remote input. The joint outputs have unusual correlations, but observing them requires the parties to compare results through an ordinary causal channel. Hence this device also does not necessarily allow superluminal signalling.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the stated pure product inputs, each local classical output is uniformly $c(\psi_X)$ or $c(\psi_X^\perp)$, independently of the remote bit and state. Those cases alone are therefore non-signalling.

The behavior on entangled inputs is not fixed by the specification, because a qubit entangled with another system has an [improper mixed state](../../../quantum-theory.md#improper-mixed-state) rather than its own pure state vector. A naive extension that reports a remotely steered pure-state decomposition would permit signalling: one party could choose a measurement basis on half of an entangled pair, and the other party's infinite-precision descriptions would distinguish the resulting ensembles even though they have the same reduced density matrix.

That extension is not forced. For example, the boxes may base outputs only on the [local quantum state under objective collapse](../../../quantum-theory.md#local-quantum-state-under-objective-collapse), or use a fixed ensemble determined solely by the local reduced density matrix; they may also reject inputs that are not pure local states. If one or both input qubits are entangled, such a local rule can output a description of the same local mixed state, a fixed basis ensemble for it, or a designated invalid-input result, all independently of spacelike-separated choices. The device therefore does not _necessarily_ allow superluminal signalling, although nonlocal pure-state-readout extensions would do so.

## 3

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For positions $\mathbf r_1,\mathbf r_2$, the two-particle [Schrödinger equation](../../../physics.md#schrodinger-equation) is

$$
\boxed{
i\hbar\frac{\partial\Psi}{\partial t}
=\left[-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)
-\frac{Gm^2}{|\mathbf r_1-\mathbf r_2|}\right]\Psi}.
$$

Neglecting packet spreading and writing $|a\rangle_i$ for $\psi_{ai}$, branchwise evolution gives

$$
|\Psi(t)\rangle\simeq\frac13\sum_{a,b=0}^2
\exp\left(\frac{iGm^2t}{\hbar d_{ab}}\right)
|a\rangle_1|b\rangle_2,
$$

up to local kinetic phases. This branch-dependent [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) produces [gravitationally induced entanglement](../../../quantum-theory.md#gravitationally-induced-entanglement).

Under the stated distance approximation, only the three branches $a=b$ acquire an appreciable common phase

$$
\phi=\frac{Gm^2t}{\hbar d}.
$$

The coefficient matrix is

$$
C=\frac13[J+(e^{i\phi}-1)I],
$$

where $J$ is the $3\times3$ all-ones matrix. The [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is

$$
\rho_1=CC^\dagger
=\frac19\left[(1+2\cos\phi)J
+2(1-\cos\phi)I\right].
$$

It equals $I/3$ when $\cos\phi=-1/2$, so the first maximally entangled state occurs at $\phi=2\pi/3$. Therefore

$$
\boxed{t_{\rm ent}
=\frac{2\pi\hbar d}{3Gm^2}
=\frac{hd}{3Gm^2}}
\simeq6.6\ {\rm s}.
$$

The state does not remain entangled for every $t>0$. Whenever $\phi=2\pi k$, all branch phases again agree and the state returns to its initial [product state](../../../bell-state.md#product-state). The revival period is

$$
\boxed{T=\frac{2\pi\hbar d}{Gm^2}
=\frac{hd}{Gm^2}\simeq19.7\ {\rm s}}.
$$

## 4

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

If Bob opens the trap, [Ehrenfest theorem](../../../quantum-mechanics.md#ehrenfest-theorem) gives branch-dependent Newtonian accelerations

$$
a_L\simeq\frac{Gm_A}{R^2},
\qquad
a_R\simeq\frac{Gm_A}{(R-d)^2},
$$

so, for $R\gg d$,

$$
\Delta a=a_R-a_L\simeq\frac{2Gm_A d}{R^3}.
$$

After time $t$, the centers of Bob's two conditional wave packets differ by

$$
\Delta x\simeq\frac12\Delta a\,t^2
\simeq\frac{Gm_A d}{R^3}t^2.
$$

For Alice's superposition, these distinguishable Bob states become entangled with $|L\rangle$ and $|R\rangle$; for Alice's mixture there was no initial coherence to entangle. Taking Bob's minimum packet width to be the [Planck length](../../../physics.md#planck-length) $\ell_P$, appreciable branch distinguishability begins when $\Delta x\sim\ell_P$, at

$$
\boxed{
t_{\rm ent}\sim
\sqrt{\frac{\ell_P R^3}{Gm_A d}}}.
$$

Keeping the trap closed suppresses this branch separation.

If $t_{\rm ent}<R/c$, Bob could choose whether to destroy Alice's local coherence before a light signal from his laboratory arrived. Any procedure by which Alice distinguished the coherent superposition from the mixture in less than $R/c$ would then enable superluminal signalling. The largest dangerous separation is determined parametrically by $t_{\rm ent}\sim R/c$, which gives

$$
R\sim\frac{Gm_A d}{c^2\ell_P}.
$$

Causality therefore requires

$$
T_A\gtrsim\frac Rc
\sim\frac{Gm_A d}{c^3\ell_P}.
$$

Using $Gm_P/c^2=\ell_P$ for the [Planck mass](../../../physics.md#planck-mass) $m_P$,

$$
\boxed{
T_A\gtrsim
\frac{m_A}{m_P}\frac dc}
$$

up to numerical factors.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
