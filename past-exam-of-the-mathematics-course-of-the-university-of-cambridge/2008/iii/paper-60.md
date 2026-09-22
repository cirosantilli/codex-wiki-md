# Paper 60

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper60.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper60.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use base-two logarithms throughout, so classical rates are measured in bits and quantum compression rates in qubits. A [memoryless classical information source](../../../information-theory.md#memoryless-classical-information-source) is a sequence $U_1,U_2,\ldots$ of [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) on a finite alphabet $\mathcal U$, with fixed [probability mass function](../../../probability-theory.md#probability-mass-function) $p$. A length-$n$ word has probability $p(u^n)=\prod_{j=1}^np(u_j)$, and the one-symbol [Shannon entropy](../../../information-theory.md#information-entropy) is $H(U)=-\sum_up(u)\log_2p(u)$, with $0\log_20=0$.

For $\varepsilon>0$, the [typical set](../../../information-theory.md#typical-set) is

$$
T_\varepsilon^{(n)}=\left\{u^n:p(u^n)>0,\quad
\left|-\frac1n\log_2p(u^n)-H(U)\right|\leq\varepsilon\right\}.
$$

This is weak typicality: it constrains the normalized self-information, not each empirical symbol count separately.

The [typical sequence theorem](../../../information-theory.md#typical-sequence-theorem) gives the following three facts for fixed $\varepsilon>0$. The [probability](../../../probability-theory.md#probability) $P(U^n\in T_\varepsilon^{(n)})$ tends to one; each word in the set has probability between $2^{-n(H(U)+\varepsilon)}$ and $2^{-n(H(U)-\varepsilon)}$; and, once the set has probability at least $1-\delta$,

$$
(1-\delta)2^{n(H(U)-\varepsilon)}\leq |T_\varepsilon^{(n)}|
\leq2^{n(H(U)+\varepsilon)}.
$$

The concentration assertion follows from the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) applied to the iid information variables $-\log_2p(U_j)$, whose finite-alphabet mean is $H(U)$. The probability bounds are the definition of typicality exponentiated. Summing the lower bound over the typical words and using total probability at most one proves the cardinality upper bound; summing the upper bound and using total typical probability at least $1-\delta$ proves the lower bound.

Fix $R>H(U)$ and choose $0<\varepsilon<R-H(U)$. Enumerate all words in $T_\varepsilon^{(n)}$ and assign a distinct fixed-length binary index to each. Reserve one more index as a failure symbol for every atypical input. For all sufficiently large $n$,

$$
|T_\varepsilon^{(n)}|+1\leq2^{\lceil nR\rceil},
$$

so these indices can be transmitted using $\lceil nR\rceil$ bits. The decoder inverts the typical-word enumeration; on the failure index it returns any fixed word. This describes both the compressor and decompressor, and its block error probability obeys

$$
\boxed{P(\widehat U^n\ne U^n)\leq P(U^n\notin T_\varepsilon^{(n)})\longrightarrow0.}
$$

Its rate tends to $R$ bits per symbol. Thus every $R>H(U)$ permits reliable fixed-rate compression, with no claim that atypical words are reconstructed correctly.

For the [memoryless quantum information source](../../../quantum-information-theory.md#memoryless-quantum-information-source), the average one-use [density matrix](../../../quantum-theory.md#density-matrix) is

$$
\rho=\frac12|0\rangle\langle0|+\frac12|+\rangle\langle+|
=\begin{pmatrix}3/4&1/4\\1/4&1/4\end{pmatrix}.
$$

Its trace is one and determinant $1/8$, so its two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are

$$
\lambda_\pm=\frac12\left(1\pm\frac1{\sqrt2}\right).
$$

The source-coding limit in [Schumacher compression](../../../quantum-information-theory.md#schumacher-compression) is the [Von Neumann entropy](../../../von-neumann-entropy.md) of this average state: every larger qubit rate allows asymptotically faithful recovery of the emitted states, and a smaller rate cannot do so. Applying that limit gives

$$
\boxed{R_{\mathrm{opt}}=S(\rho)
=h_2\!\left(\frac{1+1/\sqrt2}{2}\right)\approx0.600876\ \text{qubits per signal},}
$$

where $h_2(t)=-t\log_2t-(1-t)\log_2(1-t)$ is the [binary entropy](../../../information-theory.md#binary-entropy). The [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace) of $\rho^{\otimes n}$ has dimension about $2^{nS(\rho)}$ and carries asymptotically all source weight, which explains the compression rate. The entropy of the classical emission label is one bit; it is not the quantum rate because the two emitted [pure states](../../../quantum-theory.md#pure-state) are nonorthogonal.

## 2

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The physical space of $n$ [qubits](../../../quantum-mechanics.md#qubit) is $\mathcal H_n=(\mathbb C^2)^{\otimes n}$. An error operator is a [linear operator](../../../vector-space.md#linear-operator) on this space, for example one [Kraus operator](../../../quantum-information-theory.md#kraus-operator) of a noise [quantum channel](../../../quantum-information-theory.md#quantum-channel). The usual channel description assumes initially uncorrelated system and environment, with the environment subsequently ignored; more general initial correlations need not define a channel on arbitrary system inputs. Finite dimension and the tensor decomposition into identifiable qubits allow an exact [Pauli expansion of a quantum error](../../../quantum-circuit.md#pauli-expansion-of-a-quantum-error). No independence between errors on different qubits is assumed by this expansion.

The $4^n$ [tensor products](../../../linear-algebra.md#tensor-product) of $I,X,Y,Z$ form an orthogonal basis of the operator space under the [Hilbert-Schmidt inner product](../../../compact-operator.md#hilbert-schmidt-inner-product). Equivalently, absorbing phases into coefficients, every error has an expansion

$$
E=\sum_{a,b\in\mathbb F_2^n}c_{a,b}X^aZ^b,
\qquad X^a=\bigotimes_{j=1}^nX^{a_j},\quad Z^b=\bigotimes_{j=1}^nZ^{b_j}.
$$

For a [computational basis](../../../quantum-theory.md#computational-basis) vector $|x\rangle$ labelled by $x\in\mathbb F_2^n$, this gives

$$
\boxed{E|x\rangle=\sum_{a,b}c_{a,b}(-1)^{b\cdot x}|x+a\rangle,}
$$

where addition and the dot product in the exponent are modulo two. Thus $X$ changes a bit, $Z$ changes its phase, and $Y$ performs both up to a scalar phase. A general error is a coherent linear combination of such actions; it need not be a classical random choice of [Pauli operators](../../../quantum-circuit.md#pauli-operator). A restriction to at most $t$ faulty qubits is an additional locality assumption, expressed by the span of [Pauli operators](../../../quantum-circuit.md#pauli-operator) of weight at most $t$.

The [weight of a Pauli operator](../../../quantum-circuit.md#weight-of-a-pauli-operator) is the number of tensor factors different from $I$, ignoring global phase. Let $P$ be the [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) onto a $2^k$-dimensional code $\mathcal X$. [Quantum error detection](../../../quantum-error-correction.md#quantum-error-detection) means

$$
PEP=c_EP.
$$

Indeed, a [projective measurement](../../../quantum-measurement.md#projective-measurement) of $P$ flags departure from the code, while its code-space outcome acts as the scalar $c_E$ on every encoded state and hence does not change logical information. Harmless scalar actions are included in this criterion. The [quantum code distance](../../../quantum-error-correction.md#distance-of-a-quantum-error-correcting-code) is

$$
d=\min\{\operatorname{wt}(E):E\text{ is Pauli and }PEP\text{ is not scalar on }\mathcal X\}.
$$

Thus every [Pauli operator](../../../quantum-circuit.md#pauli-operator) of weight at most $d-1$ is detectable. The condition is linear in $E$, so it holds for any error in their span. This proves detection of arbitrary errors affecting at most $d-1$ qubits, including coherent errors.

For correction, put $t=\lfloor(d-1)/2\rfloor$ and take all phase-free [Pauli operators](../../../quantum-circuit.md#pauli-operator) $E_a$ of weight at most $t$. Their pairwise products satisfy

$$
\operatorname{wt}(E_a^\dagger E_b)\leq2t\leq d-1,
\qquad PE_a^\dagger E_bP=C_{ab}P.
$$

These are the [Knill--Laflamme conditions](../../../quantum-error-correction.md#knill-laflamme-condition). Here is their recovery construction, rather than merely using the criterion's name. For any normalized code state $|\psi\rangle$, the matrix $C$ is a [Gram matrix](../../../linear-algebra.md#gram-matrix), since $C_{ab}=\langle\psi|E_a^\dagger E_b|\psi\rangle$, and is therefore positive semidefinite. Choose linear combinations $F_j$ of the errors diagonalizing this matrix, so that

$$
PF_j^\dagger F_lP=c_j\delta_{jl}P,\qquad c_j\geq0.
$$

For $c_j>0$, the operators $V_j=F_jP/\sqrt{c_j}$ are isometries from the code into mutually orthogonal error-image subspaces: $V_j^\dagger V_l=\delta_{jl}P$. Measure the projectors $Q_j=V_jV_j^\dagger$ and, on outcome $j$, apply $V_j^\dagger$. Complete this recovery arbitrarily on the remaining orthogonal subspace to make a trace-preserving [quantum channel](../../../quantum-information-theory.md#quantum-channel).

For an error $E=\sum_j\beta_jF_j$ and any encoded [density operator](../../../quantum-theory.md#density-matrix) $\rho$, the recovered contribution is

$$
\sum_j V_j^\dagger E\rho E^\dagger V_j
=\left(\sum_j|\beta_j|^2c_j\right)\rho.
$$

Terms with $c_j=0$ annihilate the code. For a physical noise channel whose [Kraus operators](../../../quantum-information-theory.md#kraus-operator) belong to this span, summing the displayed scalar over those operators gives one by trace preservation. The resulting recovered state is exactly $\rho$. This proves the [constructive recovery from the Knill-Laflamme condition](../../../quantum-error-correction.md#constructive-recovery-from-the-knill-laflamme-condition) and the requested guarantee

$$
\boxed{[[n,k,d]]\text{ detects }d-1\text{ qubit errors and corrects }\left\lfloor\frac{d-1}{2}\right\rfloor.}
$$

This argument allows degenerate codes; distinct physical errors may have identical actions on the code.

For the [Shor code](../../../quantum-error-correction.md#shor-code), define $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. Its two normalized basis codewords are

$$
\boxed{|0_L\rangle=|G_+\rangle^{\otimes3},\qquad |1_L\rangle=|G_-\rangle^{\otimes3}.}
$$

Six [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) are $Z_1Z_2,Z_2Z_3,Z_4Z_5,Z_5Z_6,Z_7Z_8,Z_8Z_9$; the two phase checks are

$$
g_7=X_1X_2X_3X_4X_5X_6,\qquad
g_8=X_4X_5X_6X_7X_8X_9.
$$

All eight have [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $+1$ on both basis codewords. A phase error $Z_4$ commutes with the six $Z$ checks and anticommutes with both $g_7$ and $g_8$. Their [projective measurements](../../../quantum-measurement.md#projective-measurement) therefore return

$$
\boxed{(+,+,+,+,+,+,-,-).}
$$

The two negative phase checks identify the middle three-qubit block. Apply the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) $Z_4$ to restore the state, since $Z_4^2=I$. This procedure acts identically on every logical superposition, and the checks reveal no logical amplitudes. The syndrome cannot distinguish $Z_4$ from $Z_5$ or $Z_6$, but all three have the same action on the code: their pairwise products lie in the [stabilizer group](../../../quantum-circuit.md#stabilizer-group). Correcting with any one of them is sufficient. Thus the degeneracy in the syndrome is harmless.

## 3

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For [probability distributions](../../../probability-theory.md#probability-distribution) $p$ and $q$ on a finite alphabet, their classical [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) in bits is

$$
D(p\|q)=\sum_{x:p(x)>0}p(x)\log_2\frac{p(x)}{q(x)}.
$$

A zero-$p$ term contributes zero, including when $q(x)=0$; a term with $p(x)>0$ and $q(x)=0$ makes the result $+\infty$. In that infinite case nonnegativity is immediate. Otherwise $q(x)>0$ on the support $J_p$ of $p$. For every $u>0$, $\ln u\leq u-1$: the function $u-1-\ln u$ has derivative $1-1/u$ and its minimum zero at $u=1$. Apply this with $u=q(x)/p(x)$ to obtain

$$
\begin{aligned}
D(p\|q)&=-\frac1{\ln2}\sum_{x\in J_p}p(x)\ln\frac{q(x)}{p(x)}\\
&\geq\frac1{\ln2}\sum_{x\in J_p}[p(x)-q(x)]\\
&=\frac{1-\sum_{x\in J_p}q(x)}{\ln2}\geq0.
\end{aligned}
$$

The last inequality uses normalization of $q$. Thus $\boxed{D(p\|q)\geq0}$. Equality requires $q(x)=p(x)$ wherever $p(x)>0$ and no $q$-mass outside that support, hence occurs precisely when $p=q$.

For [density matrices](../../../quantum-theory.md#density-matrix), use

$$
S(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)
$$

when the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) $\rho$ is contained in that of $\sigma$, and set it to $+\infty$ otherwise. The [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) states that for any [quantum channel](../../../quantum-information-theory.md#quantum-channel) $\Phi$,

$$
\boxed{S(\Phi(\rho)\|\Phi(\sigma))\leq S(\rho\|\sigma).}
$$

Thus the relative entropy of the two output states cannot exceed that of the inputs.

For the states with a classical flag, omit indices of weight zero. On a positive-weight block, the [matrix logarithms](../../../vector-space.md#matrix-logarithm) obey

$$
\log_2(p_i\rho_i)=(\log_2p_i)I+\log_2\rho_i,
\qquad
\log_2(p_i\sigma_i)=(\log_2p_i)I+\log_2\sigma_i
$$

on the relevant supports. The logarithms of $p_i$ cancel. Taking the trace block by block therefore gives the [relative entropy of classically flagged states](../../../von-neumann-entropy.md#relative-entropy-of-classically-flagged-states):

$$
\boxed{S\!\left(\sum_ip_i|i\rangle\langle i|\otimes\rho_i\ \middle\|\
\sum_ip_i|i\rangle\langle i|\otimes\sigma_i\right)
=\sum_{i:p_i>0}p_iS(\rho_i\|\sigma_i).}
$$

If support inclusion fails in a positive-weight block, both sides are infinite. A zero-weight block makes no contribution, even if its unweighted relative entropy is infinite.

Tracing out the flag is a [quantum channel](../../../quantum-information-theory.md#quantum-channel) with operators $A_i=\langle i|\otimes I$, since $\sum_iA_i^\dagger A_i=I$. It sends the two flagged states to $\sum_ip_i\rho_i$ and $\sum_ip_i\sigma_i$. Applying the [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) to this [partial trace](../../../quantum-theory.md#partial-trace) proves [joint convexity of quantum relative entropy](../../../quantum-information-theory.md#joint-convexity-of-quantum-relative-entropy):

$$
\boxed{S\!\left(\sum_ip_i\rho_i\ \middle\|\ \sum_ip_i\sigma_i\right)
\leq\sum_{i:p_i>0}p_iS(\rho_i\|\sigma_i).}
$$

For a bipartite state, set $\rho_A=\operatorname{Tr}_B\rho_{AB}$ and $\rho_B=\operatorname{Tr}_A\rho_{AB}$. Its [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) is

$$
S(A:B)=S(\rho_A)+S(\rho_B)-S(\rho_{AB}),
$$

where $S(\tau)=-\operatorname{Tr}\tau\log_2\tau$ is the [Von Neumann entropy](../../../von-neumann-entropy.md). The support of $\rho_{AB}$ lies in $\operatorname{supp}\rho_A\otimes\operatorname{supp}\rho_B$. To justify this when marginals are singular, let $Q_A$ project onto $\ker\rho_A$. Then $\operatorname{Tr}[(Q_A\otimes I)\rho_{AB}]=\operatorname{Tr}(Q_A\rho_A)=0$; positivity implies $(Q_A\otimes I)\rho_{AB}=0$. Applying the same argument on $B$ proves the claimed support inclusion.

On that support, product eigenvectors show

$$
\log_2(\rho_A\otimes\rho_B)=\log_2\rho_A\otimes I+I\otimes\log_2\rho_B.
$$

The definition of the [partial trace](../../../quantum-theory.md#partial-trace) therefore gives

$$
\begin{aligned}
S(\rho_{AB}\|\rho_A\otimes\rho_B)
&=\operatorname{Tr}\rho_{AB}\log_2\rho_{AB}
-\operatorname{Tr}\rho_A\log_2\rho_A
-\operatorname{Tr}\rho_B\log_2\rho_B\\
&=S(\rho_A)+S(\rho_B)-S(\rho_{AB}).
\end{aligned}
$$

Consequently $\boxed{S(A:B)=S(\rho_{AB}\|\rho_A\otimes\rho_B)}$.

For completeness, [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) also follows from the classical proof above. Diagonalize $\rho$ in a basis $|j\rangle$, with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $r_j$, and put $q_j=\langle j|\sigma|j\rangle$. These are two classical [probability distributions](../../../probability-theory.md#probability-distribution). Scalar concavity of the logarithm applied to the spectral weights of $\sigma$ gives $\langle j|\log_2\sigma|j\rangle\leq\log_2q_j$ whenever $r_j>0$ and support inclusion holds. Hence

$$
S(\rho\|\sigma)\geq\sum_{j:r_j>0}r_j\log_2\frac{r_j}{q_j}=D(r\|q)\geq0.
$$

The support-failure case is again infinite. Applying this to the product of the marginals proves $\boxed{S(A:B)\geq0}$ without requiring an additional entropy inequality.

## 4

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The $n$-qubit [Pauli group](../../../quantum-circuit.md#pauli-group) is

$$
G_n=\{i^rP_1\otimes\cdots\otimes P_n:r\in\{0,1,2,3\},\ P_j\in\{I,X,Y,Z\}\}.
$$

A [stabilizer group](../../../quantum-circuit.md#stabilizer-group) $S$ is an abelian subgroup of $G_n$ excluding $-I$. Its associated [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) is the common positive [eigenspace](../../../linear-operator-theory.md#eigenspace)

$$
\boxed{\mathcal X_S=\{|\psi\rangle:s|\psi\rangle=|\psi\rangle\text{ for every }s\in S\}.}
$$

The exclusion of $-I$ is necessary for a nonzero code, since no nonzero vector has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $+1$ under $-I$.

Every $s\in S$ is a signed Hermitian [tensor product](../../../linear-algebra.md#tensor-product) of [Pauli matrices](../../../algebra.md#pauli-matrices). An imaginary-phase Pauli element would have $s^2=-I$, contradicting closure of $S$ and exclusion of $-I$; hence $s^2=I$ and $s^\dagger=s$. If $s\ne I$, it cannot be a nontrivial scalar Pauli element, and at least one of its local factors is $X,Y$ or $Z$. Each of these has trace zero. Using $\operatorname{Tr}(A\otimes B)=\operatorname{Tr}(A)\operatorname{Tr}(B)$ gives $\operatorname{Tr}s=0$.

The [spectral theorem](../../../hilbert-space.md#spectral-theorem) for Hermitian operators and $s^2=I$ show that all [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $+1$ or $-1$. If their multiplicities are $m_+$ and $m_-$, then

$$
m_++m_-=2^n,\qquad m_+-m_-=\operatorname{Tr}s=0.
$$

Thus the [balanced spectrum of a nonidentity stabilizer](../../../quantum-circuit.md#balanced-spectrum-of-a-nonidentity-stabilizer) is

$$
\boxed{m_+=m_-=2^{n-1}.}
$$

This concerns a nonidentity stabilizer acting on the entire physical space; on the code every stabilizer acts with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $+1$.

Because all elements commute and square to $I$, $S$ is a [vector space](../../../vector-space.md) over $\mathbb F_2$ under multiplication. Its independent [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) $g_1,\ldots,g_r$ satisfy that no nonempty product is $I$; all $2^r$ products are distinct. The [stabilizer-projector formula](../../../quantum-circuit.md#stabilizer-projector-formula) is

$$
P_S=\frac1{|S|}\sum_{s\in S}s=\prod_{j=1}^r\frac{I+g_j}{2}.
$$

To verify it, group multiplication gives $P_S^2=P_S$, Hermiticity gives $P_S^\dagger=P_S$, and $sP_S=P_S$ for every $s\in S$. Conversely every code vector is fixed by this average, so its range is exactly $\mathcal X_S$. All nonidentity stabilizers have trace zero by the preceding proof. Therefore

$$
\dim\mathcal X_S=\operatorname{Tr}P_S=\frac{2^n}{|S|}=2^{n-r}.
$$

For a code of dimension $2^k$, the number of independent generators is consequently $\boxed{r=n-k}$. One can list additional redundant generators, but an independent generating set has exactly this size.

For a correctable Pauli error $E_\alpha$, define the syndrome bit $s_j(\alpha)$ to be zero when $E_\alpha$ commutes with $g_j$ and one when it anticommutes. On an encoded state,

$$
g_jE_\alpha|\psi\rangle=(-1)^{s_j(\alpha)}E_\alpha|\psi\rangle.
$$

Measure the commuting [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator); their [eigenvalues](../../../linear-operator-theory.md#eigenvalue) reveal the [error syndrome](../../../quantum-error-correction.md#error-syndrome) without revealing logical amplitudes. In a [nondegenerate quantum code](../../../quantum-error-correction.md#nondegenerate-quantum-error-correcting-code), the distinct specified correctable errors have orthogonal images of the code and distinct syndromes. A syndrome therefore identifies the error representative, and applying the inverse [Pauli operator](../../../quantum-circuit.md#pauli-operator) $E_\alpha^\dagger$ restores the encoded state.

If an actual error operator is a coherent linear combination of the specified errors, its state is a sum of these orthogonal syndrome components. Syndrome measurement selects one component, followed by the same inverse operation. The [linearity of coherent quantum error correction](../../../quantum-error-correction.md#linearity-of-coherent-quantum-error-correction) ensures the logical state is recovered in every outcome. The same procedure handles noise [Kraus operators](../../../quantum-information-theory.md#kraus-operator) in that error span; it does not require a probabilistic Pauli-noise assumption.

A Pauli error commuting with every stabilizer has the all-zero syndrome and preserves the code space. If it is a stabilizer up to global phase, this silent action is harmless. If it lies in the [centralizer of a stabilizer group](../../../quantum-error-correction.md#centralizer-of-a-stabilizer-group) but is not a stabilizer up to phase, it acts as a nontrivial logical operator, and syndrome measurements cannot detect it. More generally, a non-scalar component $P_SEP_S$ of an error is an undetectable logical action. This distinguishes harmful undetected errors from scalar actions that satisfy [quantum error detection](../../../quantum-error-correction.md#quantum-error-detection) algebraically.

The three-qubit [bit-flip repetition code](../../../quantum-error-correction.md#bit-flip-repetition-code) has basis $|000\rangle,|111\rangle$ and generators

$$
\boxed{g_1=Z_1Z_2,\qquad g_2=Z_2Z_3.}
$$

A single phase flip $Z_1$ commutes with both and has zero syndrome, but

$$
Z_1(\alpha|000\rangle+\beta|111\rangle)
=\alpha|000\rangle-\beta|111\rangle.
$$

It is a nontrivial logical phase operation. In particular, $P_SZ_1P_S$ is not scalar, so the error set $\{I,Z_1\}$ violates the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) and cannot be corrected. Thus **the code corrects single bit flips but not single phase flips**; its distance against arbitrary quantum errors is one.

## 5

↑ **Parent:** [Paper 60](paper-60.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The printed normalization has its factors reversed. For the displayed map $\Phi(X)=\sum_kA_kXA_k^\dagger$, the condition $\sum_kA_kA_k^\dagger=I$ says $\Phi(I)=I$, which is unitality. Trace preservation instead requires

$$
\boxed{\sum_kA_k^\dagger A_k=I.}
$$

These are distinct [trace-preserving and unital Kraus conditions](../../../quantum-information-theory.md#trace-preserving-and-unital-kraus-conditions). To disprove the printed equivalence, take $0<\gamma<1$ and

$$
B_0=\begin{pmatrix}1&0\\0&\sqrt{1-\gamma}\end{pmatrix},\qquad
B_1=\sqrt\gamma|1\rangle\langle0|.
$$

They obey $\sum_jB_jB_j^\dagger=I$, but

$$
\sum_jB_j^\dagger B_j=\operatorname{diag}(1+\gamma,1-\gamma),
\qquad
\operatorname{Tr}\!\left[\sum_jB_j|0\rangle\langle0|B_j^\dagger\right]=1+\gamma.
$$

Thus their [completely positive map](../../../quantum-information-theory.md#completely-positive-map) is not trace preserving. They are the adjoints of the operators of an [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel). That channel is trace preserving but sends $I$ to $\operatorname{diag}(1+\gamma,1-\gamma)$, so it cannot satisfy the printed normalization in any [Kraus representation](../../../quantum-information-theory.md#kraus-representation) either. The corrected characterization is proved next.

Work in finite-dimensional input and output [Hilbert spaces](../../../hilbert-space.md), with a linear map $\Phi$ on operators. Suppose first that $\Phi(X)=\sum_kA_kXA_k^\dagger$ and $\sum_kA_k^\dagger A_k=I$. For every auxiliary dimension $m$ and every positive operator $W$ on the extended space,

$$
(\operatorname{id}_m\otimes\Phi)(W)
=\sum_k(I_m\otimes A_k)W(I_m\otimes A_k)^\dagger\geq0.
$$

Each summand is positive because conjugation preserves positivity. This is exactly the definition of a [completely positive map](../../../quantum-information-theory.md#completely-positive-map). Cyclicity of the trace gives

$$
\operatorname{Tr}\Phi(X)=\operatorname{Tr}\!\left[X\sum_kA_k^\dagger A_k\right]=\operatorname{Tr}X,
$$

so the map is also trace preserving.

Conversely, suppose $\Phi$ is completely positive and trace preserving, and let $|i\rangle$ be an orthonormal input basis. Use the unnormalized entangled vector $|\Omega\rangle=\sum_i|i\rangle\otimes|i\rangle$, with the reference factor first. Complete positivity makes the corresponding unnormalized [Choi matrix](../../../quantum-information-theory.md#choi-matrix) positive:

$$
J_\Phi=(\operatorname{id}\otimes\Phi)(|\Omega\rangle\langle\Omega|)
=\sum_{i,j}|i\rangle\langle j|\otimes\Phi(|i\rangle\langle j|)\geq0.
$$

Its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) can be written $J_\Phi=\sum_k|v_k\rangle\langle v_k|$, absorbing the nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) into the vectors. Define [linear operators](../../../vector-space.md#linear-operator) $A_k$ uniquely by

$$
|v_k\rangle=\sum_i|i\rangle\otimes A_k|i\rangle.
$$

Expanding the outer products and comparing their $(i,j)$ reference blocks yields

$$
\Phi(|i\rangle\langle j|)=\sum_kA_k|i\rangle\langle j|A_k^\dagger.
$$

The matrix units span all operators, so linearity proves the [Kraus representation](../../../quantum-information-theory.md#kraus-representation) $\Phi(X)=\sum_kA_kXA_k^\dagger$ for every $X$. Finally, trace preservation gives

$$
\operatorname{Tr}\!\left[X\left(\sum_kA_k^\dagger A_k-I\right)\right]=0
$$

for all $X$. Taking matrix units as test operators shows that the matrix in parentheses is zero. This proves both directions of the corrected CPT characterization, including the normalization rather than assuming it.

For an input [quantum state ensemble](../../../quantum-theory.md#quantum-state-ensemble) $\{p_x,\rho_x\}$, write $\sigma_x=\Phi(\rho_x)$ and $\bar\sigma=\sum_xp_x\sigma_x$. Its output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) is

$$
\chi(\{p_x,\sigma_x\})=S(\bar\sigma)-\sum_xp_xS(\sigma_x).
$$

The [Holevo capacity](../../../quantum-information-theory.md#holevo-capacity) is the optimized one-use quantity

$$
\boxed{\chi^*(\Phi)=\sup_{\{p_x,\rho_x\}}
\left[S\!\left(\sum_xp_x\Phi(\rho_x)\right)-\sum_xp_xS(\Phi(\rho_x))\right],}
$$

where the supremum ranges over finite input ensembles and $S$ is the [Von Neumann entropy](../../../von-neumann-entropy.md) in bits.

For $n$ uses of a [memoryless quantum channel](../../../quantum-information-theory.md#memoryless-quantum-channel), the map is $\Phi^{\otimes n}$. An $n$-use code consists of a finite message set $\mathcal M_n$ of size $M_n$, an encoding state $\rho_m^{(n)}$ on the $n$ inputs for each message, and a decoding [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) $\{D_m^{(n)}:m\in\mathcal M_n\}$ on the output space, with $D_m^{(n)}\geq0$ and $\sum_mD_m^{(n)}=I$. The encoding states may be entangled across uses. The measurement outcome is the receiver's decoded message, with conditional probability

$$
P(\widehat m=l\mid m)=\operatorname{Tr}\!\left[D_l^{(n)}\Phi^{\otimes n}(\rho_m^{(n)})\right].
$$

For uniformly distributed messages the average error and rate are

$$
\boxed{P_e^{(n)}=1-\frac1{M_n}\sum_m\operatorname{Tr}\!\left[D_m^{(n)}\Phi^{\otimes n}(\rho_m^{(n)})\right],\qquad
R_n=\frac1n\log_2M_n.}
$$

A rate $R$ is achievable if there is a sequence of such codes with $P_e^{(n)}\to0$ and $\liminf_nR_n\geq R$. The unassisted [classical capacity of a quantum channel](../../../quantum-information-theory.md#classical-capacity-of-a-quantum-channel) is the supremum of achievable rates; the sender and receiver do not share prior entanglement.

The operational content of the [Holevo-Schumacher-Westmoreland theorem](../../../quantum-information-theory.md#holevo-schumacher-westmoreland-theorem) is that $\chi^*(\Phi)$ is the capacity for product-state input encodings with collective output measurements. Allowing arbitrary entangled block inputs gives the regularized formula

$$
\boxed{C(\Phi)=\lim_{n\to\infty}\frac1n\chi^*(\Phi^{\otimes n})
=\sup_{n\geq1}\frac1n\chi^*(\Phi^{\otimes n}).}
$$

The limit equals the supremum because [superadditivity of Holevo capacity](../../../quantum-information-theory.md#superadditivity-of-holevo-capacity) follows by taking product ensembles for two blocks and using additivity of the [Von Neumann entropy](../../../von-neumann-entropy.md) on product states. The coding theorem makes every rate below the one-block [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) achievable through many independently encoded blocks, with collective decoding.

The converse can be seen explicitly from the [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) and [Fano's inequality](../../../information-theory.md#fano-s-inequality). For a uniform transmitted message $M$ and decoded message $\widehat M$,

$$
(1-P_e^{(n)})\log_2M_n-h_2(P_e^{(n)})
\leq I(M:\widehat M)
\leq\chi\!\left(\left\{\frac1{M_n},\Phi^{\otimes n}(\rho_m^{(n)})\right\}\right)
\leq\chi^*(\Phi^{\otimes n}).
$$

The first inequality is obtained by subtracting the Fano bound on $H(M\mid\widehat M)$ from $H(M)=\log_2M_n$. Dividing by $n$ and letting the average error vanish bounds every achievable rate by the regularized expression. The block-coding achievability just described supplies the reverse bound.

Under the assumed [additivity of Holevo capacity](../../../quantum-information-theory.md#additivity-of-holevo-capacity) across tensor powers, $\chi^*(\Phi^{\otimes n})=n\chi^*(\Phi)$ for every $n$. Thus

$$
\boxed{C(\Phi)=\chi^*(\Phi)=C_{\mathrm{product}}(\Phi).}
$$

**The stated conditional assertion is true:** under this additivity assumption, entangled input states cannot increase the asymptotic unassisted classical rate beyond the rate already achievable with product inputs. The decoder may still use collective measurements across channel outputs.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
