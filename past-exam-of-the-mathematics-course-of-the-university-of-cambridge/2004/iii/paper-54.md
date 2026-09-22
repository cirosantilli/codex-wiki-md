# Paper 54

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper54.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper54.pdf)

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

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

By the [Schmidt decomposition theorem](../../../von-neumann-entropy.md#schmidt-decomposition), suitable [local unitary operations](../../../bell-state.md#local-unitary-operation) put the normalized [pure state](../../../quantum-theory.md#pure-state) into the form

$$
|\psi\rangle=\lambda_0|00\rangle+\lambda_1|11\rangle,\qquad \lambda_0,\lambda_1\geq0,\qquad \lambda_0^2+\lambda_1^2=1.
$$

It is [entangled](../../../bell-state.md#entangled-state) precisely when both [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are nonzero. Put $s=2\lambda_0\lambda_1$, so $0<s\leq1$ for the case of interest. The [Pauli operators](../../../quantum-circuit.md#pauli-operator)

$$
Z=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad X=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

satisfy $\langle Z\otimes Z\rangle=1$ and $\langle X\otimes X\rangle=s$ in this [pure state](../../../quantum-theory.md#pure-state): $Z\otimes Z$ fixes both basis terms, and $X\otimes X$ exchanges them.

Choose Alice's two [observables](../../../quantum-mechanics.md#observable) as $A_0=Z$, $A_1=X$, and Bob's as

$$
B_0=\frac{Z+sX}{\sqrt{1+s^2}},\qquad B_1=\frac{Z-sX}{\sqrt{1+s^2}}.
$$

These are valid dichotomic [projective measurements](../../../quantum-measurement.md#projective-measurement). Indeed, $XZ+ZX=0$ and $X^2=Z^2=I$, so $B_0^2=B_1^2=I$; each [observable](../../../quantum-mechanics.md#observable) has outcomes $\pm1$. For the [CHSH inequality](../../../quantum-theory.md#chsh-inequality) convention $|\langle A_0\otimes(B_0+B_1)+A_1\otimes(B_0-B_1)\rangle|\leq2$, the quantum value is

$$
\begin{aligned}
S&=\frac{2}{\sqrt{1+s^2}}\big(\langle Z\otimes Z\rangle+s\langle X\otimes X\rangle\big)\\
&=\boxed{2\sqrt{1+s^2}>2.}
\end{aligned}
$$

For the original [pure state](../../../quantum-theory.md#pure-state), conjugate these four [observables](../../../quantum-mechanics.md#observable) by the corresponding local [unitary operators](../../../vector-space.md#unitary-operator). Their outcomes and [Pauli correlators](../../../quantum-circuit.md#pauli-correlator) are unchanged, and each party still measures only their own [qubit](../../../quantum-mechanics.md#qubit). Thus **every entangled pure two-qubit state violates CHSH for suitable local measurements**, proving [Gisin's theorem](../../../quantum-theory.md#gisin-s-theorem) directly. The [CHSH axes for an entangled pure two-qubit state](../../../quantum-theory.md#chsh-axes-for-an-entangled-pure-two-qubit-state) approach a nonviolating configuration continuously as one [Schmidt coefficient](../../../von-neumann-entropy.md#schmidt-coefficient) tends to zero; the strict violation therefore need not be large for weak [entanglement](../../../bell-state.md#entangled-state).

## 2

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

There is a necessary distinction between a failure bound averaged over the unknown state, a worst-case bound, and a separate bound for each candidate state. The last interpretation is false: a forger can discard the inputs and always prepare $|\psi_0\rangle^{\otimes N}$. If the actual state is $|\psi_0\rangle$, every authenticity test passes with [probability](../../../probability-theory.md#probability) one. **The meaningful uniform statement concerns worst-case failure, or average failure under any fixed prior giving both states positive probability.** The PDF does not specify that prior; the argument below gives an explicit bound for either interpretation.

Put $c=|\langle\psi_0|\psi_1\rangle|\in(0,1)$. Any unconditional strategy producing $N$ output [qubits](../../../quantum-mechanics.md#qubit), including ancillas, adaptive [measurement in quantum measurements](../../../quantum-measurement.md) and correlated outputs, is a [quantum channel](../../../quantum-information-theory.md#quantum-channel) $\mathcal E$. Its inputs and ideal outputs are the [density operators](../../../quantum-theory.md#density-matrix)

$$
\sigma_i=\big(|\psi_i\rangle\langle\psi_i|\big)^{\otimes M},\qquad P_i=\big(|\psi_i\rangle\langle\psi_i|\big)^{\otimes N},\qquad \rho_i=\mathcal E(\sigma_i).
$$

The [projective measurements](../../../quantum-measurement.md#projective-measurement) on the different banknotes commute, and their all-pass effect is exactly $P_i$. Therefore the [probability](../../../probability-theory.md#probability) of at least one rejection, conditional on input $i$, is

$$
e_i=1-\operatorname{Tr}(P_i\rho_i).
$$

This remains true for entangled outputs; no independence of their individual test outcomes is assumed.

Use [trace distance](../../../quantum-theory.md#trace-distance) $D(\rho,\sigma)=\tfrac12\|\rho-\sigma\|_1$. The [pure-state trace distance and fidelity identity](../../../quantum-information-theory.md#pure-state-trace-distance-and-fidelity-identity) gives

$$
D(\sigma_0,\sigma_1)=\sqrt{1-c^{2M}},\qquad D(P_0,P_1)=\sqrt{1-c^{2N}}.
$$

For completeness, two pure-state projectors differ by a [matrix](../../../vector-space.md#matrix) with nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm\sqrt{1-|\langle u|v\rangle|^2}$, which proves this identity. Also the [pure-target upper bound on trace distance](../../../quantum-theory.md#pure-target-upper-bound-on-trace-distance) gives $D(\rho_i,P_i)\leq\sqrt{e_i}$. To see the mixed-state step, write $\rho_i=\sum_jq_j|u_j\rangle\langle u_j|$ and use [convexity](../../../real-analysis.md#convex-function) of the [trace norm](../../../functional-analysis.md#trace-norm) followed by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality):

$$
D(\rho_i,P_i)\leq\sum_jq_j\sqrt{1-\langle u_j|P_i|u_j\rangle}\leq\sqrt{1-\operatorname{Tr}(P_i\rho_i)}.
$$

Finally, [trace-distance contraction under quantum channels](../../../quantum-theory.md#trace-distance-contraction-under-quantum-channels) gives $D(\rho_0,\rho_1)\leq D(\sigma_0,\sigma_1)$. This follows from $D(\rho,\sigma)=\max_{0\leq E\leq I}\operatorname{Tr}[E(\rho-\sigma)]$: the adjoint channel is positive and unital, so its image of any effect $E$ is still an effect.

The [triangle inequality](../../../topological-analysis.md#triangle-inequality) now yields

$$
\begin{aligned}
\sqrt{1-c^{2N}}&\leq D(P_0,\rho_0)+D(\rho_0,\rho_1)+D(\rho_1,P_1)\\
&\leq\sqrt{e_0}+\sqrt{1-c^{2M}}+\sqrt{e_1}.
\end{aligned}
$$

Thus the [cloning failure bound from trace-distance contraction](../../../quantum-theory.md#cloning-failure-bound-from-trace-distance-contraction) is

$$
\sqrt{e_0}+\sqrt{e_1}\geq\Delta,\qquad \Delta=\sqrt{1-c^{2N}}-\sqrt{1-c^{2M}}>0,
$$

and in particular $\max(e_0,e_1)\geq\Delta^2/4$. For positive priors $\pi_0+\pi_1=1$, another [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
(\sqrt{e_0}+\sqrt{e_1})^2\leq(\pi_0e_0+\pi_1e_1)(\pi_0^{-1}+\pi_1^{-1}),
$$

so the average rejection [probability](../../../probability-theory.md#probability) satisfies

$$
\boxed{P_{\mathrm{fail}}=\pi_0e_0+\pi_1e_1\geq\pi_0\pi_1\Delta^2>p_0:=\tfrac12\pi_0\pi_1\Delta^2>0.}
$$

For equal priors, one may take $p_0=\Delta^2/8$; the same choice is a strict lower bound on worst-case rejection. This proves a quantitative version of the [no-cloning theorem](../../../quantum-theory.md#no-cloning-theorem) for the bank's all-pass test. It concerns an unconditional attempt: heralded success cannot be postselected while omitting failed attempts from the accounting.

## 3

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $q=|B|$ and choose $h$ uniformly from the finite family $H$. All bounds below must hold for every pair of distinct inputs $x,y\in A$.

A [universal hash family](../../../computer-science.md#universal-hash-family), also called universal2, satisfies $P[h(x)=h(y)]\leq1/q$. A [strongly universal hash family](../../../computer-science.md#strongly-universal-hash-family) satisfies

$$
P[h(x)=u,\ h(y)=v]=q^{-2}\quad\text{for every }u,v\in B.
$$

Thus the two outputs are independent and uniform; summing over $u=v$ gives the collision condition. An [almost strongly universal hash family](../../../computer-science.md#almost-strongly-universal-hash-family) permits a larger conditional guessing bound. In the $\varepsilon$-almost-strongly-universal convention used here,

$$
P[h(x)=u]=q^{-1},\qquad P[h(x)=u,\ h(y)=v]\leq\varepsilon/q,
$$

equivalently $P[h(y)=v\mid h(x)=u]\leq\varepsilon$. Necessarily $\varepsilon\geq1/q$, with $\varepsilon=1/q$ giving strong universality. Stating this normalization matters because the name alone does not specify the allowed forgery [probability](../../../probability-theory.md#probability).

Here is an explicit [polynomial almost strongly universal hashing](../../../computer-science.md#polynomial-almost-strongly-universal-hashing) construction and a one-use [message authentication](../../../computer-science.md#message-authentication) protocol. Use a publicly specified [finite field](../../../algebra.md#finite-field) $\mathbb F_q$, where $q=2^t$. Encode a fixed-length $n$-bit message as $L=\lceil n/t\rceil$ field elements $m_1,\ldots,m_L$, padding the final block in a fixed way. Both parties know the length, so this encoding is injective. They share independent uniform secret field elements $a,b$, requiring $2t$ shared secret bits. Define

$$
h_{a,b}(m)=b+\sum_{j=1}^{L}m_ja^j.
$$

For every message, the output is uniform because of $b$. For distinct messages $m,m'$ and prescribed tags $u,v$, the condition $h(m)=u$ determines exactly one value of $b$ for each $a$. The remaining condition is

$$
\sum_{j=1}^{L}(m'_j-m_j)a^j=v-u.
$$

Its left-hand side has a nonzero coefficient of positive degree, so subtracting the specified constant gives a nonzero [polynomial](../../../polynomial.md) of degree at most $L$. By the [root bound for a polynomial](../../../polynomial.md#lagrange-root-bound-over-a-field), there are at most $L$ possible field elements $a$. Consequently

$$
P[h(m)=u,h(m')=v]\leq L/q^2,
$$

and this is an $\varepsilon$-almost-strongly-universal family with $\varepsilon=L/q$, provided $L<q$. The powers start at one deliberately: a message coefficient at power zero could give a known constant tag shift, allowing a deterministic substitution.

Alice sends the message and its tag $u=h_{a,b}(m)$ over the public channel. Bob accepts only if his independently computed tag agrees. An attacker who has seen no tag guesses one with [probability](../../../probability-theory.md#probability) $1/q$. After seeing a valid pair $(m,u)$, an attacker substituting a different message $m'$ and any chosen tag $v$ succeeds with conditional [probability](../../../probability-theory.md#probability) at most $L/q$. This remains true when the choice of $m',v$ depends on the observed pair: the bound is uniform over all those choices. More explicitly, the observed tag leaves $a$ uniform because each possible $a$ has exactly one compatible secret mask $b$.

For a desired forgery bound $\eta$, choose $t=\lceil\log_2(n/\eta)\rceil$. Since $L\leq n$ and $q\geq n/\eta$, the substitution bound is at most $\eta$. The secret requirement is

$$
\boxed{2t=O(\log n+\log(1/\eta))\text{ bits},\qquad P(\text{substitution accepted})\leq L/2^t\leq\eta.}
$$

For a long message this is much shorter than its $n$ bits. This is [Wegman–Carter authentication](../../../computer-science.md#wegman-carter-authentication): a keyed hash plus a fresh secret [one-time pad](../../../coding-theory.md#one-time-pad) on the tag. It authenticates the message rather than concealing its contents. Use the key once for the guarantee just established; multiple authenticated messages require fresh masks and a reuse security analysis. Authenticate lengths and sequence identifiers too if variable lengths or replay protection are required.

## 4

↑ **Parent:** [Paper 54](paper-54.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Compute the honest one-qubit [density operators](../../../quantum-theory.md#density-matrix) in the [computational basis](../../../quantum-theory.md#computational-basis). Writing $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$ and $|u\rangle=(5|0\rangle+|1\rangle)/\sqrt{26}$, the two [quantum state ensembles](../../../quantum-theory.md#quantum-state-ensemble) give

$$
\begin{aligned}
\rho_0&=\tfrac12|0\rangle\langle0|+\tfrac14|+\rangle\langle+|+\tfrac14|1\rangle\langle1|=\begin{pmatrix}5/8&1/8\\1/8&3/8\end{pmatrix},\\
\rho_1&=\tfrac{13}{20}|u\rangle\langle u|+\tfrac7{20}|1\rangle\langle1|=\begin{pmatrix}5/8&1/8\\1/8&3/8\end{pmatrix}.
\end{aligned}
$$

The equality includes the off-diagonal coherence; comparing only the basis outcome probabilities would not suffice.

**The protocol is perfectly hiding against Bob when Alice is honest.** Independence of the honest preparations makes his full received [density operator](../../../quantum-theory.md#density-matrix) $\rho_0^{\otimes N}=\rho_1^{\otimes N}$. For any [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) $\{E_z\}$, including collective measurements and measurements using ancillas, the [Born rule](../../../quantum-mechanics.md#born-rule) gives the same outcome probabilities $\operatorname{Tr}(E_z\rho_0^{\otimes N})=\operatorname{Tr}(E_z\rho_1^{\otimes N})$. Thus no measurement supplies information about the committed bit.

**It is not binding against Alice.** Here is an explicit [ensemble-steering attack on quantum bit commitment](../../../computer-science.md#ensemble-steering-attack-on-quantum-bit-commitment). For each position, Alice prepares the normalized two-qubit [pure state](../../../quantum-theory.md#pure-state)

$$
|\Omega\rangle=\sqrt{\frac{13}{20}}|0\rangle_A|u\rangle_B+\sqrt{\frac7{20}}|1\rangle_A|1\rangle_B,
$$

retains $A$ and sends $B$. Its [partial trace](../../../quantum-theory.md#partial-trace) on $A$ is the honest common [density operator](../../../quantum-theory.md#density-matrix). She sends the $B$ halves of $N$ independent copies while retaining all the $A$ halves, and chooses her bit only at unveiling.

To open one, she makes a [projective measurement](../../../quantum-measurement.md#projective-measurement) of each retained [qubit](../../../quantum-mechanics.md#qubit) in the [computational basis](../../../quantum-theory.md#computational-basis). Outcome zero has [probability](../../../probability-theory.md#probability) $13/20$ and prepares Bob's state $|u\rangle$; outcome one has [probability](../../../probability-theory.md#probability) $7/20$ and prepares $|1\rangle$. She announces that list. It has exactly the honest bit-one distribution, and every declared-state test passes.

To open zero, she instead measures each retained [qubit](../../../quantum-mechanics.md#qubit) using a three-outcome [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) with effects $E_j=|v_j\rangle\langle v_j|$, where

$$
|v_0\rangle=\begin{pmatrix}2/\sqrt5\\-2/\sqrt{70}\end{pmatrix},\quad
|v_+\rangle=\begin{pmatrix}1/\sqrt5\\4/\sqrt{70}\end{pmatrix},\quad
|v_1\rangle=\begin{pmatrix}0\\\sqrt{5/7}\end{pmatrix}.
$$

All effects are positive. Their diagonal sums are $4/5+1/5=1$ and $4/70+16/70+5/7=1$, and the off-diagonal sum is zero, so $E_0+E_++E_1=I$. This establishes that the proposed [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) is physically valid.

To verify the conditional states directly, the coefficient [matrix](../../../vector-space.md#matrix) of $|\Omega\rangle$, with Bob's index as the row and Alice's as the column, is

$$
C=\begin{pmatrix}\sqrt{5/8}&0\\\sqrt{1/40}&\sqrt{7/20}\end{pmatrix}.
$$

A real rank-one effect $|v_j\rangle\langle v_j|$ on Alice's half gives the unnormalized Bob state vector $Cv_j$. For the three effects above,

$$
Cv_0=\sqrt{1/2}|0\rangle,\qquad Cv_+=\tfrac12|+\rangle,\qquad Cv_1=\tfrac12|1\rangle.
$$

Their squared norms are therefore $1/2,1/4,1/4$, exactly the honest bit-zero probabilities, and Bob's conditional [pure states](../../../quantum-theory.md#pure-state) are the corresponding declared states. Independent measurements on the retained halves produce the honest distribution of the entire list, so even checks on the declared frequencies do not defeat the attack. Every declared-state projector test again succeeds.

Alice can consequently unveil either bit with acceptance [probability](../../../probability-theory.md#probability) one, without having chosen it when sending the [qubits](../../../quantum-mechanics.md#qubit). This is the [Hughston–Jozsa–Wootters theorem](../../../quantum-theory.md#hughston-jozsa-wootters-theorem) mechanism implemented by an explicit measurement, rather than merely an appeal to the general impossibility of perfectly hiding and binding quantum [bit commitment](../../../computer-science.md#bit-commitment).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
