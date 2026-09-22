# Paper 325

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_325.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_325.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $q=(\mathbf q_1,\ldots,\mathbf q_N)$ denote the particle positions. In the [Ghirardi--Rimini--Weber model](../../../quantum-theory.md#ghirardi-rimini-weber-theory), the wavefunction obeys the ordinary [Schrödinger equation](../../../physics.md#schrodinger-equation)

$$
i\hbar\frac{\partial\psi}{\partial t}=H\psi
$$

between random collapses. Each particle $i$ has an independent [Poisson process](../../../probability-theory.md#poisson-process) of collapse times with rate $\lambda$. At such a time the state jumps according to

$$
\psi(q)\longmapsto
\frac{L_i(\mathbf X)\psi(q)}{\|L_i(\mathbf X)\psi\|},
\qquad
L_i(\mathbf X)=\frac{1}{(\pi r_C^2)^{3/4}}
\exp\left[-\frac{(\mathbf q_i-\mathbf X)^2}{2r_C^2}\right],
$$

where the random centre has [probability density](../../../quantum-mechanics.md#probability-density) $\|L_i(\mathbf X)\psi\|^2$. The normalization is arranged so that $\int d^3X\,L_i(\mathbf X)^2=I$.

The original GRW scales are approximately

$$
r_C\sim10^{-7}\ {\rm m},
\qquad
\lambda\sim10^{-16}\ {\rm s}^{-1}.
$$

An isolated microscopic particle is therefore exceedingly unlikely to collapse during a laboratory experiment. A macroscopic pointer containing about $N\sim10^{23}$ relevant particles has total collapse rate $N\lambda\sim10^7\ {\rm s}^{-1}$ and collapse time about $10^{-7}\ {\rm s}$. After a [measurement interaction](../../../quantum-measurement.md#measurement-interaction) correlates different microscopic outcomes with pointer positions separated by much more than $r_C$, one constituent's localization suppresses all incompatible pointer branches. This [GRW amplification mechanism](../../../quantum-theory.md#grw-amplification-mechanism) produces one definite macroscopic outcome with probabilities given by the [Born rule](../../../quantum-mechanics.md#born-rule), while leaving ordinary microscopic [unitary time evolution](../../../quantum-mechanics.md#unitary-time-evolution) almost unchanged.

For one spatial coordinate, average over the random centre of one collapse. The resulting [density operator](../../../quantum-theory.md#density-matrix) has position-space kernel

$$
\rho'(x,x')=
\exp\left[-\frac{(x-x')^2}{4r_C^2}\right]\rho(x,x').
$$

Its diagonal is unchanged, so $\langle x\rangle$ and $\langle x^2\rangle$ are unchanged. The first derivative of the Gaussian factor vanishes at $x=x'$, so $\langle p\rangle$ is also unchanged. Its second derivative does not vanish, and the [position representation of the momentum operator](../../../quantum-mechanics.md#position-representation-of-the-momentum-operator) gives

$$
\boxed{\langle p^2\rangle'
=\langle p^2\rangle+\frac{\hbar^2}{2r_C^2}}.
$$

In three dimensions the increase in total $\mathbf p^2$ is $3\hbar^2/(2r_C^2)$, corresponding to kinetic-energy increase $3\hbar^2/(4mr_C^2)$ per collapse. These are ensemble statements: conditioning on one specified collapse centre can shift the position moments. Repetition at rate $\lambda$ predicts [GRW spontaneous heating](../../../quantum-theory.md#grw-spontaneous-heating), so precision searches for anomalous bulk heating, spontaneous radiation, momentum diffusion, and loss of matter-wave interference test the model.

## 2

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The pure state $|\Psi\rangle_{AB}$ is [entangled](../../../bell-state.md#entangled-state) when it cannot be written as a [product state](../../../bell-state.md#product-state) $|a\rangle_A|b\rangle_B$, equivalently when its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) exceeds one. Its subsystem states are the [reduced density matrices](../../../bell-state.md#reduced-density-matrix)

$$
\rho_A=\operatorname{Tr}_B|\Psi\rangle\langle\Psi|,
\qquad
\rho_B=\operatorname{Tr}_A|\Psi\rangle\langle\Psi|,
$$

where the [partial trace](../../../quantum-theory.md#partial-trace) is characterized by $\operatorname{Tr}(M_A\rho_A)=\langle\Psi|M_A\otimes I_B|\Psi\rangle$ for every observable $M_A$.

Let Bob's measurement have [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $M_b$ satisfying $\sum_bM_b^\dagger M_b=I_B$. If Alice does not learn Bob's random outcome, her state after the measurement is

$$
\begin{aligned}
\rho'_A
&=\operatorname{Tr}_B\sum_b(I\otimes M_b)\rho_{AB}(I\otimes M_b^\dagger)\\
&=\operatorname{Tr}_B\left[\rho_{AB}
\left(I\otimes\sum_bM_b^\dagger M_b\right)\right]
=\rho_A.
\end{aligned}
$$

This [no-communication theorem](../../../bell-state.md#no-communication-theorem) means that Bob can change Alice's conditional state after she learns his outcome, but cannot change any local outcome distribution available to her alone. Standard [nonrelativistic quantum mechanics](../../../quantum-mechanics.md#nonrelativistic-quantum-mechanics) is therefore operationally compatible with the prohibition of [superluminal signalling](../../../special-relativity.md#faster-than-light-communication) in [special relativity](../../../special-relativity.md), despite its nonlocal conditional-state updates.

An exact nondisturbing state readout would destroy this protection if it reported the globally collapsed state on an absolute-time slice. For example, Alice and Bob may share [Bell states](../../../bell-state.md). At a prearranged time Bob encodes a bit by measuring his qubit in either the computational or [Hadamard basis](../../../quantum-theory.md#hadamard-basis). The usual projection postulate assigns Alice respectively one of $|0\rangle,|1\rangle$ or one of $|+\rangle,|-\rangle$. A device returning the exact pure state lets Alice identify which basis Bob chose without waiting for his outcome, producing a [superluminal signal](../../../special-relativity.md#faster-than-light-communication). Equivalently, Bob may choose whether to measure, and the device distinguishes the resulting proper pure state from the original improper maximally mixed local state.

A causal alternative is a [quantum state readout device](../../../quantum-theory.md#quantum-state-readout-device) located at a spacetime point $x$ that reports the [local quantum state under objective collapse](../../../quantum-theory.md#local-quantum-state-under-objective-collapse): take reduced states on spacelike hypersurfaces through $x$ and let those hypersurfaces approach the past [light cone](../../../special-relativity.md#light-cone) of $x$. The result includes localized collapses in $J^-(x)$ and excludes spacelike-separated collapses. This assumes a fixed [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime), localized collapse events, ordinary local unitary dynamics between them, and outputs that may control only operations in their causal future. The postulate is logically consistent because it adds a classical record of this local state without changing the state or any standard measurement probability. It also cannot support an indirect signalling algorithm. Inductively through the algorithm's events, every readout at $x$ depends only on operations, collapses, and earlier readouts in $J^-(x)$; any operation selected from that output lies in the readout's future light cone. Composing readouts, unitary evolutions, and measurements therefore never carries a controllable dependence outside a future light cone, so [relativistic causality](../../../special-relativity.md#relativistic-causality) is preserved.

## 3

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take $|L\rangle=|0\rangle$ and $|R\rangle=|1\rangle$. Initially the two masses are in the [product state](../../../bell-state.md#product-state)

$$
|\psi(0)\rangle=\frac12(|LL\rangle+|LR\rangle+|RL\rangle+|RR\rangle).
$$

The branch-dependent [Newtonian gravitational potential energy](../../../classical-mechanics.md#newtonian-gravitational-potential-energy) is $-Gm^2/d_{ab}$. Under the stated approximation, only the $|RL\rangle$ branch acquires an appreciable relative phase, so after time $t$,

$$
|\psi(t)\rangle\simeq
\frac12(|LL\rangle+|LR\rangle+e^{i\phi}|RL\rangle+|RR\rangle),
\qquad
\phi=\frac{Gm^2t}{\hbar d}.
$$

The determinant of its two-by-two coefficient matrix is $(1-e^{i\phi})/4$, which is nonzero unless $\phi$ is a multiple of $2\pi$. Thus the state generally has [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) two: the branch-dependent gravitational phase creates [gravitationally induced entanglement](../../../quantum-theory.md#gravitationally-induced-entanglement).

An [entanglement witness](../../../quantum-information-theory.md#entanglement-witness) has a bound obeyed by every [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) and violated by at least one entangled state. For a product state with [Bloch vectors](../../../quantum-theory.md#bloch-vector) $\mathbf r$ and $\mathbf s$,

$$
|\langle X\otimes Z+Y\otimes Y\rangle|
=|r_xs_z+r_ys_y|
\leq\sqrt{r_x^2+r_y^2}\sqrt{s_z^2+s_y^2}
\leq1
$$

by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Convexity gives the same bound for every separable mixed state. Consequently $W>1$ certifies entanglement; in conventional operator form, one of $I\mp(X\otimes Z+Y\otimes Y)$ has negative expectation whenever the absolute-value criterion is violated.

For the state above, direct use of the [Pauli matrices](../../../algebra.md#pauli-matrices) gives

$$
\langle X\otimes Z\rangle
=\langle Y\otimes Y\rangle
=\frac{\cos\phi-1}{2},
\qquad
W=1-\cos\phi.
$$

With the supplied values,

$$
\phi\simeq
\frac{(6.674\times10^{-11})(10^{-14})^2(10)}
{(1.054\times10^{-34})(2\times10^{-4})}
\simeq3.17,
$$

which is close to $\pi$. Hence $W\simeq2.00$, and to the nearest integer

$$
\boxed{W=2}.
$$

This is the operating principle of the [Bose--Marletto--Vedral experiment](../../../quantum-theory.md#bose-marletto-vedral-experiment).

## 4

↑ **Parent:** [Paper 325](paper-325.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) of an entangled pure two-qubit state has two nonzero terms. Absorb both complex phases into the local basis vectors and interchange the labels of the second qubit to obtain

$$
|\psi\rangle=c_0|\uparrow\rangle_1|\downarrow\rangle_2
+c_1|\downarrow\rangle_1|\uparrow\rangle_2,
\qquad
c_0,c_1>0,
\qquad
c_0^2+c_1^2=1.
$$

In this state the only nonzero same-axis two-qubit [Pauli correlators](../../../quantum-circuit.md#pauli-correlator) are

$$
\langle X\otimes X\rangle
=\langle Y\otimes Y\rangle=2c_0c_1,
\qquad
\langle Z\otimes Z\rangle=-1.
$$

All mixed-axis correlators vanish. Expanding $(\mathbf a\cdot\boldsymbol\sigma)\otimes(\mathbf b\cdot\boldsymbol\sigma)$ therefore gives

$$
\boxed{E(\mathbf a,\mathbf b)
=2c_0c_1(a_xb_x+a_yb_y)-a_zb_z}.
$$

For the four stated vectors this becomes

$$
E(\mathbf a,\mathbf b)=-\cos\beta,
\quad
E(\mathbf a,\mathbf b')=-\cos\beta',
\quad
E(\mathbf a',\mathbf b)=-2c_0c_1\sin\beta,
\quad
E(\mathbf a',\mathbf b')=-2c_0c_1\sin\beta'.
$$

It follows immediately that

$$
|E(\mathbf a,\mathbf b)-E(\mathbf a,\mathbf b')|
+|E(\mathbf a',\mathbf b)+E(\mathbf a',\mathbf b')|
=|\cos\beta-\cos\beta'|
+2c_0c_1|\sin\beta+\sin\beta'|.
$$

Every [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) obeys the corresponding [CHSH inequality](../../../quantum-theory.md#chsh-inequality) with upper bound two. Set $s=2c_0c_1>0$, choose $\beta'=\pi-\beta$, and take $\tan\beta=s$ with $0<\beta<\pi/2$. The displayed expression is then

$$
2(\cos\beta+s\sin\beta)=2\sqrt{1+s^2}>2.
$$

Thus every entangled pure two-qubit state has local measurement correlations that no separable state can reproduce, which is [Gisin's theorem](../../../quantum-theory.md#gisin-s-theorem). In an ideal [Bose--Marletto--Vedral experiment](../../../quantum-theory.md#bose-marletto-vedral-experiment), optimized local measurements can therefore witness any nonzero pure-state entanglement generated during the gravitational interaction. If gravity is the only interaction between the masses, such a violation shows that the mediator cannot be described by a purely classical local variable under the assumptions of the proposal; experimentally, control of [decoherence](../../../quantum-theory.md#quantum-decoherence) and nongravitational forces is essential to that inference.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
