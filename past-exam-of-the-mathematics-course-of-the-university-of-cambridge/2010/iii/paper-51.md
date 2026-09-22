# Paper 51

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper51.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper51.pdf)

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
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

[Quantum teleportation](../../../bell-state.md#quantum-teleportation) transfers an arbitrary unknown [qubit](../../../quantum-mechanics.md#qubit) state to a separated receiver while using [local operations and classical communication](../../../bell-state.md#local-operations-and-classical-communication), rather than sending that input qubit. Alice and Bob first share one [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) of two qubits, such as a [Bell pair](../../../bell-state.md#bell-pair); a shared [spin singlet state](../../../bell-state.md#spin-singlet-state) is equivalent after a known [local unitary operation](../../../bell-state.md#local-unitary-operation).

Alice performs a joint [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement) on the input qubit and her half of the pair. There are four possible outcomes. Bob's conditional qubit is the input state transformed by a known [Pauli operator](../../../quantum-circuit.md#pauli-operator) determined by that outcome. Alice sends the outcome as two classical bits, and Bob applies the inverse [Pauli operator](../../../quantum-circuit.md#pauli-operator). Thus **one shared Bell pair and two classical bits, together with local measurement and correction, transmit one unknown qubit exactly**. The entangled resource is consumed.

The procedure does not produce a classical description of the unknown amplitudes and does not leave a second copy at Alice, so it respects the [no-cloning theorem](../../../quantum-theory.md#no-cloning-theorem). Before receiving the classical outcome, Bob's [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is $I/2$, independent of the input; this respects the [no-communication theorem](../../../bell-state.md#no-communication-theorem). The next part proves the full identity-channel action, including inputs entangled with another system.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Label an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the $n$-dimensional [Hilbert space](../../../hilbert-space.md) by $j=0,\ldots,n-1$, with indices modulo $n$. Let

$$
\omega=e^{2\pi i/n},\qquad X|j\rangle=|j+1\rangle,\qquad Z|j\rangle=\omega^j|j\rangle.
$$

These are the shift and phase [Heisenberg-Weyl operators](../../../quantum-information-theory.md#heisenberg-weyl-operator). Alice holds the input $S$ and one half $A$ of the shared [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state)

$$
|\Phi_n\rangle_{AB}=\frac1{\sqrt n}\sum_{j=0}^{n-1}|j\rangle_A|j\rangle_B.
$$

She measures $SA$ in the [generalized Bell basis](../../../quantum-theory.md#generalized-bell-basis)

$$
|B_{pq}\rangle_{SA}=\frac1{\sqrt n}\sum_{j=0}^{n-1}\omega^{pj}|j\rangle_S|j+q\rangle_A,
\qquad p,q=0,\ldots,n-1.
$$

Its inner products are

$$
\langle B_{pq}|B_{p'q'}\rangle
=\delta_{qq'}\frac1n\sum_{j=0}^{n-1}\omega^{(p'-p)j}
=\delta_{pp'}\delta_{qq'}.
$$

There are $n^2$ orthonormal vectors in an $n^2$-dimensional space, so this is a complete [projective measurement](../../../quantum-measurement.md#projective-measurement).

For an unknown normalized state $|u\rangle=\sum_j u_j|j\rangle$, its contraction with measurement outcome $(p,q)$ gives Bob's unnormalized state

$$
\begin{aligned}
{}_{SA}\langle B_{pq}|\bigl(|u\rangle_S|\Phi_n\rangle_{AB}\bigr)
&=\frac1n\sum_j u_j\omega^{-pj}|j+q\rangle_B\\
&=\frac1nX^qZ^{-p}|u\rangle_B.
\end{aligned}
$$

Each outcome has [probability](../../../probability-theory.md#probability) $1/n^2$, independently of the input. Alice communicates the two $n$-valued labels, and Bob applies the ordered inverse

$$
\boxed{U_{pq}=Z^pX^{-q},\qquad
U_{pq}\left(\frac1nX^qZ^{-p}|u\rangle\right)=\frac1n|u\rangle.}
$$

The order matters because shift and phase operators do not generally commute. Normalizing the branch recovers the unknown state exactly, and all outcomes are corrected, so success is deterministic. The quantum resource is one maximally entangled pair of local dimension $n$. The classical resource is an $n^2$-valued message, with information content $2\log_2 n$ bits; $\lceil\log_2(n^2)\rceil$ ordinary bits suffice in fixed-length binary encoding.

This is faithful [qudit teleportation](../../../bell-state.md#qudit-teleportation) even for an input entangled with a reference $R$. Expand a joint pure state as $\sum_j|j\rangle_S|r_j\rangle_R$, without requiring the reference vectors to be orthogonal. The same contraction and correction act on each system basis vector, producing $n^{-1}\sum_j|j\rangle_B|r_j\rangle_R$. Thus the whole joint state, not just a reduced state, is preserved. Linearity extends the conclusion to mixed inputs. This is [teleportation as an identity channel on a reference](../../../bell-state.md#teleportation-as-an-identity-channel-on-a-reference).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

**Yes: deterministic entanglement swapping gives the required singlet.** Denote Bob's two local qubits by $B_1,B_2$. Known [local unitary operations](../../../bell-state.md#local-unitary-operation) first convert the two given [spin singlet states](../../../bell-state.md#spin-singlet-state) into $|\Phi^+\rangle_{AB_1}$ and $|\Phi^+\rangle_{B_2C}$. For example applying $ZX$ to the second qubit of a singlet gives $|\Phi^+\rangle$, where $X,Z$ are [Pauli operators](../../../quantum-circuit.md#pauli-operator).

Use the binary-labelled [Bell states](../../../bell-state.md)

$$
|B_{pq}\rangle=(I\otimes X^qZ^p)|\Phi^+\rangle,\qquad p,q\in\{0,1\}.
$$

They are $\Phi^+,\Phi^-,\Psi^+,\Psi^-$ for labels $(0,0),(1,0),(0,1),(1,1)$. Reordering registers to group Bob's qubits, direct expansion gives

$$
|\Phi^+\rangle_{AB_1}|\Phi^+\rangle_{B_2C}
=\frac12\sum_{p,q=0}^1|B_{pq}\rangle_{B_1B_2}|B_{pq}\rangle_{AC}.
$$

All four basis vectors are real in this convention; otherwise the paired expansion must account for complex conjugation. Bob performs the [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement) on $B_1B_2$. This joint operation is local to him, so it is allowed by [LOCC](../../../bell-state.md#local-operations-and-classical-communication). Each outcome occurs with probability $1/4$ and leaves $AC$ in the corresponding [Bell state](../../../bell-state.md).

Bob sends $(p,q)$ to Charlie. Charlie applies $Z^pX^{-q}$ to obtain $|\Phi^+\rangle_{AC}$, and then $XZ$ to obtain

$$
\boxed{|\Psi^-\rangle_{AC}=\frac{|01\rangle-|10\rangle}{\sqrt2}.}
$$

The correction works for every outcome, so no postselection or successful-outcome assumption is needed. This is [entanglement swapping](../../../bell-state.md#entanglement-swapping), equivalently teleportation of $B_1$ to $C$ while preserving its entanglement with $A$. If Bob's measurement result is ignored, the average $AC$ state is $I_4/4$; the protocol therefore does not supply entanglement usable without the classical outcome or violate the [no-communication theorem](../../../bell-state.md#no-communication-theorem).

## 2

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Introduce the orthonormal local vectors $|+\rangle=(|1\rangle+|2\rangle)/\sqrt2$ and $|-\rangle=(|1\rangle-|2\rangle)/\sqrt2$. Reexpressing the second state's factors in this basis gives its [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition)

$$
|\phi_2\rangle=\frac1{\sqrt3}|+\rangle_A|+\rangle_B+\sqrt{\frac23}|-\rangle_A|-\rangle_B.
$$

The squared [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are therefore $1/3,2/3$, whereas those of the first state are $1/2,1/2$.

To see directly why these distinguish the states, a [local unitary operation](../../../bell-state.md#local-unitary-operation) $U_A\otimes U_B$ changes the [reduced density matrix](../../../bell-state.md#reduced-density-matrix) to

$$
\rho_A' =\operatorname{Tr}_B[(U_A\otimes U_B)\rho_{AB}(U_A^\dagger\otimes U_B^\dagger)]
=U_A\rho_AU_A^\dagger.
$$

This is [local-unitary invariance of reduced-state spectra](../../../bell-state.md#local-unitary-invariance-of-reduced-state-spectra): the unitary on the traced subsystem cancels, and conjugation on $A$ leaves its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) unchanged. Here the reductions are

$$
\rho_A^{(1)}=\frac I2,\qquad
\rho_A^{(2)}=\frac13|+\rangle\langle+|+\frac23|-\rangle\langle-|
=\begin{pmatrix}1/2&-1/6\\-1/6&1/2\end{pmatrix}.
$$

Their spectra differ. Hence **no pair of local unitary operations carries the first state to the second**. More generally, normalized bipartite pure states are locally unitarily equivalent exactly when their squared Schmidt coefficients agree, including multiplicities; sufficiency follows by mapping one pair of Schmidt bases to the other.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

If the preparation label $i$ is sampled with probability $p_i$ but is not supplied to the experimenter, the [quantum state ensemble](../../../quantum-theory.md#quantum-state-ensemble) is represented by

$$
\boxed{\rho=\sum_{i=1}^n p_i|\psi_i\rangle\langle\psi_i|,\qquad
p_i\geq0,\quad\sum_i p_i=1.}
$$

For normalized states, this [density operator](../../../quantum-theory.md#density-matrix) is Hermitian, positive semidefinite and has trace one. The states in an ensemble need not be orthogonal or distinct. For any [measurement in quantum mechanics](../../../quantum-measurement.md) effect $E$, averaging the [Born rule](../../../quantum-mechanics.md#born-rule) over the preparation label gives

$$
P(E)=\sum_i p_i\langle\psi_i|E|\psi_i\rangle=\operatorname{Tr}(E\rho).
$$

Thus the density operator summarizes all measurements performed on the prepared system alone. For an ensemble of mixed states $\rho_i$, the same reasoning gives $\rho=\sum_i p_i\rho_i$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**Yes: distinct density operators have a projective measurement with different outcome probabilities.** Let $\rho,\sigma$ be the two [density operators](../../../quantum-theory.md#density-matrix) and let $D=\rho-\sigma$. It is a nonzero [Hermitian operator](../../../hilbert-space.md#hermitian-operator) with trace zero. Its nonzero eigenvalues cannot all have the same sign, since their sum is zero. Let $P_+$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto its positive-eigenvalue subspace. Then the two-outcome [projective measurement](../../../quantum-measurement.md#projective-measurement) $\{P_+,I-P_+\}$ satisfies

$$
P_\rho(+)-P_\sigma(+)=\operatorname{Tr}[P_+(\rho-\sigma)]
=\sum_{\lambda_j(D)>0}\lambda_j(D)>0.
$$

The outcome therefore carries statistical information about which [quantum ensemble](../../../quantum-theory.md#quantum-state-ensemble) was used.

For example, with equal prior probabilities, guess $\rho$ after $+$ and $\sigma$ after the other outcome. The success probability is

$$
P_{\rm succ}=\frac12\operatorname{Tr}(P_+\rho)+\frac12\operatorname{Tr}[(I-P_+)\sigma]
=\frac12+\frac12\operatorname{Tr}(P_+D).
$$

Since the positive and negative eigenvalue sums of $D$ have equal absolute value, $\operatorname{Tr}(P_+D)=\|D\|_1/2$. Consequently

$$
\boxed{P_{\rm succ}=\frac12+\frac14\|\rho-\sigma\|_1>\frac12.}
$$

This is the equal-prior measurement in the [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem), expressed using the [trace distance](../../../quantum-theory.md#trace-distance). The conclusion is some information, not necessarily perfect one-shot discrimination: nonorthogonal density operators generally cannot be distinguished with certainty.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**No measurement on the supplied system alone distinguishes ensembles with the same density operator.** A completely general [measurement in quantum mechanics](../../../quantum-measurement.md) has [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) effects $E_r\geq0$ with $\sum_r E_r=I$. The outcome probability for a [quantum ensemble](../../../quantum-theory.md#quantum-state-ensemble) is

$$
P(r)=\sum_i p_i\langle\psi_i|E_r|\psi_i\rangle
=\operatorname{Tr}(E_r\rho).
$$

If both ensembles have the same $\rho$, every outcome probability is identical. This proves the claim for all [positive operator-valued measures](../../../quantum-measurement.md#positive-operator-valued-measure), and includes [projective measurements](../../../quantum-measurement.md#projective-measurement) as a special case. An [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) in a fixed independent state does not help: the input density operators remain identical after tensoring with that ancilla, and the same argument applies to any joint measurement.

The premise concerns access only to the prepared state. An accessible preparation label or a correlated [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) is additional information outside that premise and can distinguish global preparations. Without such side information, different ensemble decompositions do not define distinguishable states.

## 3

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $s=\sin^2\alpha$ and $t=\sin^2\beta$. Then $0<s<t<1/2$, and the ordered squared [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) of the source and target are $(1-s,s)$ and $(1-t,t)$.

[Nielsen's pure-state conversion theorem](../../../bell-state.md#nielsen-s-pure-state-conversion-theorem) states that a deterministic exact conversion between bipartite pure states by [LOCC](../../../bell-state.md#local-operations-and-classical-communication) exists precisely when the source's vector of squared [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) is majorized by the target's vector, with zero padding if needed. In the convention $x\prec y$, [majorization](../../../vector-space.md#majorization) requires $\sum_{j=1}^k x_j^\downarrow\leq\sum_{j=1}^k y_j^\downarrow$ for every $k$, and equality of total sums. Here the first inequality would require $1-s\leq1-t$, but $s<t$ gives the reverse strict inequality. Thus **exact conversion with certainty is impossible**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

An upper bound follows directly from the [Schmidt-tail entanglement monotone](../../../bell-state.md#schmidt-tail-entanglement-monotone)

$$
E_2(\chi)=1-\lambda_{\max}(\rho_A^\chi),
$$

where $\rho_A^\chi$ is the [reduced density matrix](../../../bell-state.md#reduced-density-matrix) of a bipartite pure state. On these two-qubit states, this is the smaller squared [Schmidt coefficient](../../../von-neumann-entropy.md#schmidt-coefficient), so $E_2(\psi)=s$ and $E_2(\phi)=t$.

Here is the average-monotonicity argument needed for all [LOCC](../../../bell-state.md#local-operations-and-classical-communication) strategies. The largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is convex: for any unit vector $v$, $\langle v|\sum_r p_r\rho_r|v\rangle\leq\sum_r p_r\lambda_{\max}(\rho_r)$, and maximizing the left side gives the claim. Hence $1-\lambda_{\max}$ is concave. If Alice makes a local measurement, Bob's conditional reductions average to his original reduction. Concavity therefore gives $\sum_r p_rE_2(\chi_r)\leq E_2(\chi)$. If Bob measures, use Alice's reductions instead. The two reductions of a pure state have the same nonzero eigenvalues by the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition). Refining all measurement outcomes into individual [Kraus operators](../../../quantum-information-theory.md#kraus-operator) keeps conditional states pure; iterating the inequality covers adaptive rounds of classical communication. The same bound persists for limits of such protocols.

If success produces the target with probability $p$, its contribution to the final average is $pt$. Failure branches have nonnegative $E_2$. Thus

$$
pt\leq s,\qquad
\boxed{p_{\max}\leq\frac{s}{t}=\frac{\sin^2\alpha}{\sin^2\beta}.}
$$

This is a bound on arbitrary local protocols, not merely on a particular filtering measurement.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Alice makes a two-outcome local [measurement in quantum mechanics](../../../quantum-measurement.md) with [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
K_{\rm s}=\begin{pmatrix}\tan\alpha/\tan\beta&0\\0&1\end{pmatrix},\qquad
K_{\rm f}=\begin{pmatrix}\sqrt{1-\tan^2\alpha/\tan^2\beta}&0\\0&0\end{pmatrix}.
$$

Since $0<\tan\alpha/\tan\beta<1$, these are valid and satisfy $K_{\rm s}^\dagger K_{\rm s}+K_{\rm f}^\dagger K_{\rm f}=I$. Alice sends Bob the success or failure outcome. The successful unnormalized branch is

$$
\begin{aligned}
(K_{\rm s}\otimes I)|\psi\rangle
&=\frac{\sin\alpha\cos\beta}{\sin\beta}|00\rangle+\sin\alpha|11\rangle\\
&=\frac{\sin\alpha}{\sin\beta}|\phi\rangle.
\end{aligned}
$$

Therefore the normalized success state is exactly the target and

$$
\boxed{p_{\rm succ}=\frac{\sin^2\alpha}{\sin^2\beta}=\frac{s}{t}=p_{\max}.}
$$

Bob needs no quantum correction in this known Schmidt basis. The failure branch is proportional to $|00\rangle$, a [product state](../../../bell-state.md#product-state), and has probability $1-s/t$. The successful branch saturates the previous bound: $p_{\rm succ}E_2(\phi)=E_2(\psi)$ and failure contributes zero. This establishes [optimal stochastic conversion of a two-qubit pure state](../../../bell-state.md#optimal-stochastic-conversion-of-a-two-qubit-pure-state).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use the usual asymptotic convention: the output approaches the desired $m(n)$-copy pure target in [trace distance](../../../quantum-theory.md#trace-distance), and any recorded failure probability tends to zero. Define the [binary entropy](../../../information-theory.md#binary-entropy)

$$
h_2(x)=-x\log_2x-(1-x)\log_2(1-x).
$$

The [entanglement entropies](../../../von-neumann-entropy.md#entanglement-entropy) per source and target are $E_\psi=h_2(s)$ and $E_\phi=h_2(t)$. The [asymptotic pure-state entanglement conversion rate](../../../bell-state.md#asymptotic-pure-state-entanglement-conversion-rate) is

$$
\boxed{R_{\max}=\frac{h_2(\sin^2\alpha)}{h_2(\sin^2\beta)}.}
$$

Both achievability and the upper bound matter here.

For [entanglement concentration](../../../bell-state.md#entanglement-concentration), expand $n$ sources in their correlated computational basis. Every pair of strings of [Hamming weight](../../../coding-theory.md#hamming-weight) $k$ has the same amplitude $(1-s)^{(n-k)/2}s^{k/2}$. Alice measures only this weight, without resolving the individual string. Bob's string has the same weight automatically. Conditional on $k$, the normalized state is maximally entangled on $D_k=\binom nk$ correlated strings. Its outcome probability is $\binom nk s^k(1-s)^{n-k}$, a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution). By the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers), $k/n\to s$ in probability; [Stirling's formula](../../../real-analysis.md#stirling-formula) then gives $n^{-1}\log_2D_k\to h_2(s)$. A uniform Schmidt vector on $D_k$ entries is majorized by a uniform vector on $2^{\lfloor\log_2D_k\rfloor}$ entries padded with zeros. Thus [Nielsen's pure-state conversion theorem](../../../bell-state.md#nielsen-s-pure-state-conversion-theorem) converts the conditional state into that many [Bell pairs](../../../bell-state.md#bell-pair) exactly. For any fixed $\delta>0$, one obtains at least $n(E_\psi-\delta)$ Bell pairs with probability tending to one.

For [entanglement dilution](../../../bell-state.md#entanglement-dilution), consider the Schmidt strings of $m$ targets with probabilities $q_x$. The [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace) retains strings satisfying

$$
2^{-m(E_\phi+\delta)}\leq q_x\leq2^{-m(E_\phi-\delta)}.
$$

The retained probability $Q_m$ tends to one by the weak law applied to the independent variables $-\log_2q_{x_j}$. The number of retained strings is at most $2^{m(E_\phi+\delta)}$, because their probabilities sum to at most one. Normalize the target after truncation to those strings. Its squared overlap with the full target is $Q_m\to1$. A uniform Schmidt vector of dimension $2^L$, with $L=\lceil m(E_\phi+\delta)\rceil$, is majorized by the truncated target's Schmidt vector padded with zeros: the sum of its largest $k$ entries is at least $k/2^L$. Hence $L$ Bell pairs prepare the truncated target exactly by [LOCC](../../../bell-state.md#local-operations-and-classical-communication). Its trace distance from the true target is $\sqrt{1-Q_m}\to0$. Combining concentration and dilution achieves any rate $R<E_\psi/E_\phi$. Choosing margins tending sufficiently slowly to zero attains the ratio as a limiting rate.

For the converse, [average monotonicity of pure-state entanglement entropy](../../../von-neumann-entropy.md#average-monotonicity-of-pure-state-entanglement-entropy) follows from [Concavity of Von Neumann entropy](../../../von-neumann-entropy.md#concavity-of-von-neumann-entropy): a measurement by one party leaves the other party's reduction unchanged on average, so its average conditional entropy cannot increase. Refine local measurement records, including local discarded systems, to obtain pure output branches $\{p_r,|\chi_r\rangle\}$ on the $m$ output qubits of each party. Iterating the concavity argument gives

$$
\sum_r p_r E(\chi_r)\leq nE_\psi.
$$

Let $|\Phi_m\rangle=|\phi\rangle^{\otimes m}$ and let the squared-overlap error of the average output $\rho_{\rm out}$ be $\varepsilon=1-\langle\Phi_m|\rho_{\rm out}|\Phi_m\rangle\to0$. Define $d_r=\sqrt{1-|\langle\Phi_m|\chi_r\rangle|^2}$, the pure-state [trace distance](../../../quantum-theory.md#trace-distance). Concavity of the square root gives $\sum_rp_rd_r\leq\sqrt\varepsilon$. Partial trace cannot increase trace distance, so the reduced states are also within $d_r$. The [continuity bound for quantum conditional entropy](../../../von-neumann-entropy.md#continuity-bound-for-quantum-conditional-entropy), with trivial conditioning and local dimension $2^m$, implies

$$
|E(\chi_r)-mE_\phi|\leq2m d_r+g(d_r),\qquad
g(d)=(1+d)h_2\!\left(\frac d{1+d}\right)\leq2.
$$

Consequently

$$
nE_\psi\geq mE_\phi-2m\sqrt\varepsilon-2,
$$

which excludes a limiting rate exceeding $E_\psi/E_\phi$.

The vanishing-error convention is essential. If exact deterministic conversion were required for every finite block, [majorization](../../../vector-space.md#majorization) would also require the largest squared Schmidt coefficient to satisfy $(1-s)^n\leq(1-t)^m$, hence

$$
\frac mn\leq\frac{-\log(1-s)}{-\log(1-t)}.
$$

This can be strictly smaller than the entropy ratio: at $s=0.1,t=0.2$, the two bounds are approximately $0.4722$ and $0.6496$. Thus the boxed rate answers the standard asymptotic task, rather than imposing unmentioned exact zero-error conditions on every finite block.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Applying the optimal single-copy filter independently gives a random number $M_n$ of exact successful targets with [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution)

$$
M_n\sim\operatorname{Bin}(n,s/t),\qquad
\mathbb E M_n=n\frac{s}{t}.
$$

The [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) gives $M_n/n\to s/t$ in probability. In contrast, collective [entanglement concentration](../../../bell-state.md#entanglement-concentration) and [entanglement dilution](../../../bell-state.md#entanglement-dilution) yield asymptotically $n h_2(s)/h_2(t)$ targets with vanishing output error. The improvement is strict, not just nonnegative. Differentiating [binary entropy](../../../information-theory.md#binary-entropy) gives

$$
\frac{d}{dx}\left(\frac{h_2(x)}x\right)
=\frac{\log_2(1-x)}{x^2}<0\qquad(0<x<1).
$$

Since $s<t$, it follows that

$$
\boxed{\frac{h_2(s)}{h_2(t)}>\frac{s}{t},\qquad
m(n)\sim n\frac{h_2(s)}{h_2(t)}>\mathbb E M_n.}
$$

This is [collective advantage over independent two-qubit filtering](../../../bell-state.md#collective-advantage-over-independent-two-qubit-filtering). Independent filtering discards the entanglement in product-state failure branches; the collective reversible asymptotic procedure avoids that extensive loss. The separately filtered targets are exact conditional on success, whereas the collective statement uses the vanishing-error convention from the previous part. Here the counted outputs are target states $|\phi\rangle$; that is also the notation in the original printed question.

## 4

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Diagonalize the [density operator](../../../quantum-theory.md#density-matrix) in the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) basis $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. Its eigenvalues are $2/3,1/3$, so

$$
\rho_A=\frac23|+\rangle\langle+|+\frac13|-\rangle\langle-|.
$$

Choose orthonormal records on a second qubit to construct the first [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator):

$$
\boxed{|\Omega_1\rangle=\sqrt{\frac23}|+\rangle_A|0\rangle_B+\sqrt{\frac13}|-\rangle_A|1\rangle_B.}
$$

It is normalized. In its outer product the cross terms have partial trace zero because $\langle0|1\rangle_B=0$, while the diagonal terms give precisely $\rho_A$.

A different purification follows from [unitary freedom of purification](../../../quantum-theory.md#unitary-freedom-of-purification). Apply the [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to $B$:

$$
\boxed{|\Omega_2\rangle=(I\otimes H)|\Omega_1\rangle
=\sqrt{\frac23}|+\rangle_A|+\rangle_B+\sqrt{\frac13}|-\rangle_A|-\rangle_B.}
$$

The same partial-trace calculation uses $\langle+|-\rangle_B=0$ and gives $\rho_A$. The two global states are distinct, not related by a global phase, although their reduced density operators agree. Explicitly the second is

$$
|\Omega_2\rangle=a(|00\rangle+|11\rangle)+b(|01\rangle+|10\rangle),\qquad
a=\frac{\sqrt2+1}{2\sqrt3},\quad b=\frac{\sqrt2-1}{2\sqrt3}.
$$

Its reduction has diagonal entries $a^2+b^2=1/2$ and off-diagonal entries $2ab=1/6$, checking all the required matrix entries.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Use the first copy to determine computational-basis parity and the second to determine phase parity. On the first pair, Alice and Bob each measure the [Pauli operator](../../../quantum-circuit.md#pauli-operator) $Z$ and communicate their signs $z_A,z_B$. On the second, each measures $X$ in the $|+\rangle,|-\rangle$ basis and communicates the signs $x_A,x_B$.

Every [Bell state](../../../bell-state.md) is an eigenstate of both $Z\otimes Z$ and $X\otimes X$. Direct application to its two basis terms gives the table

$$
\begin{array}{c|cc}
\text{state}&z_Az_B&x_Ax_B\\\hline
\Phi^+&+1&+1\\
\Phi^-&+1&-1\\
\Psi^+&-1&+1\\
\Psi^-&-1&-1
\end{array}
$$

For example, $Z\otimes Z$ acts positively on $|00\rangle,|11\rangle$ and negatively on $|01\rangle,|10\rangle$; $X\otimes X$ exchanges the two terms in each pair, detecting their relative sign. Thus individual outcomes are random, but the products in the table are certain. The [Bell parity and phase observables](../../../quantum-theory.md#bell-parity-and-phase-observables) label the state uniquely.

**The two communicated parities identify all four states with probability one.** Each measurement is local and all remaining operations are classical, so the protocol is [LOCC discrimination of four Bell states using two copies](../../../quantum-theory.md#locc-discrimination-of-four-bell-states-using-two-copies). Alice can simply send her two signs to Bob, who combines them with his own. Measuring $Z$ on the first copy destroys its phase information, but the second identical copy still supplies it; this is why the two-copy assumption enables this protocol.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Charlie measures his qubit in the $X$ basis, $|\pm\rangle=(|0\rangle\pm|1\rangle)/\sqrt2$. Rewriting the [GHZ state](../../../quantum-theory.md#greenberger-horne-zeilinger-state) in that basis gives

$$
|\mathrm{GHZ}\rangle_{ABC}
=\frac1{\sqrt2}\left(|\Phi^+\rangle_{AB}|+\rangle_C+|\Phi^-\rangle_{AB}|-\rangle_C\right).
$$

Each outcome occurs with probability $1/2$. Charlie records $c=0$ for $+$ and $c=1$ for $-$ and sends that bit to Bob. Alice and Bob's conditional [Bell state](../../../bell-state.md) is $(I\otimes Z^c)|\Phi^+\rangle$. Bob applies $XZ^c$, with $Z^c$ applied first. Then

$$
(I\otimes XZ^c)(I\otimes Z^c)|\Phi^+\rangle
=(I\otimes X)|\Phi^+\rangle
=\boxed{|\Psi^+\rangle_{AB}=\frac{|01\rangle+|10\rangle}{\sqrt2}.}
$$

Thus every measurement branch gives the requested state after a known local correction: success is deterministic. All quantum operations act on only one party, and the only nonlocal resource used during the protocol is classical communication. This is [localizing a Bell pair from a GHZ state](../../../quantum-theory.md#localizing-a-bell-pair-from-a-ghz-state) by [LOCC](../../../bell-state.md#local-operations-and-classical-communication).

Ignoring Charlie's outcome instead gives Alice and Bob the average state $\tfrac12(|\Phi^+\rangle\langle\Phi^+|+|\Phi^-\rangle\langle\Phi^-|)=\tfrac12(|00\rangle\langle00|+|11\rangle\langle11|)$, which is separable. The classical record supplies the correction needed to use the conditional entanglement; no communication-free preparation of a known entangled state is being claimed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
