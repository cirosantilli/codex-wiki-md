# Paper 35

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper35.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper35.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Pauli group](../../../quantum-circuit.md#pauli-group) includes scalar phases $\mathcal Z=\{\pm I,\pm iI\}$. For a nonzero [stabilizer code](../../../quantum-error-correction.md#stabilizer-code), its Abelian subgroup must satisfy $-I\notin S$. Otherwise a common positive [eigenvector](../../../linear-operator-theory.md#eigenvector) would satisfy $-|\psi\rangle=|\psi\rangle$ and vanish; for example $S=\{I,-I\}$ is Abelian but yields no nonzero [stabilizer code](../../../quantum-error-correction.md#stabilizer-code). We impose this standard admissibility condition.

Every element of such a [stabilizer group](../../../quantum-circuit.md#stabilizer-group) is Hermitian and squares to $I$: an imaginary-phase Pauli with square $-I$ is excluded. The associated [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) and its [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) are

$$
\mathcal C_S=\{|\psi\rangle:s|\psi\rangle=|\psi\rangle\text{ for every }s\in S\},\qquad
P=\frac1{|S|}\sum_{s\in S}s.
$$

The group multiplication proves $P^2=P$, Hermiticity gives $P^\dagger=P$, and its range is exactly the common positive eigenspace. If $S$ has $r$ independent generators, $|S|=2^r$. Every nonidentity element has trace zero, while $\operatorname{tr}I=2^n$, so

$$
\boxed{\dim\mathcal C_S=\operatorname{tr}P=2^{n-r}.}
$$

Thus it encodes $k=n-r$ [logical qubits](../../../quantum-error-correction.md#logical-qubit).

For the [symplectic representation of a stabilizer code](../../../quantum-error-correction.md#symplectic-representation-of-a-stabilizer-code), label $i^tX^aZ^b$ by $(a,b)\in\mathbb F_2^{2n}$, ignoring scalar phase. Products add labels, and

$$
(X^aZ^b)(X^{a'}Z^{b'})=(-1)^{a\cdot b'+b\cdot a'}(X^{a'}Z^{b'})(X^aZ^b).
$$

This is the nondegenerate alternating form $\omega((a,b),(a',b'))=a\cdot b'+b\cdot a'$ on the [binary symplectic space of Pauli labels](../../../quantum-circuit.md#binary-symplectic-space-of-pauli-labels). The image $L$ of $S$ is an r-dimensional [isotropic subspace of a binary symplectic space](../../../quantum-circuit.md#isotropic-subspace-of-a-binary-symplectic-space), since the generators commute and no nontrivial scalar lies in $S$. Consequently $L\subseteq L^\perp$ and $r\le n$. A binary generator [matrix](../../../vector-space.md#matrix) $(A\mid B)$ satisfies $AB^T+BA^T=0$. Conversely an isotropic subspace can be lifted by choosing commuting Hermitian generators with independent labels; their products cannot equal $-I$, and the [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) formula supplies the [stabilizer code](../../../quantum-error-correction.md#stabilizer-code). The labels of the [centralizer of a stabilizer group](../../../quantum-error-correction.md#centralizer-of-a-stabilizer-group) are $L^\perp$, with nontrivial logical actions represented by $L^\perp\setminus L$.

For an example, the three-[qubit](../../../quantum-mechanics.md#qubit) [bit-flip repetition code](../../../quantum-error-correction.md#bit-flip-repetition-code) has $S=\langle Z_1Z_2,Z_2Z_3\rangle$ and $\mathcal C_S=\operatorname{span}\{|000\rangle,|111\rangle\}$. Its two binary rows have zero X part and Z parts $110,011$. The errors $I,X_1,X_2,X_3$ have respective [error syndromes](../../../quantum-error-correction.md#error-syndrome) $00,10,11,01$, so all single bit flips can be corrected. This is not a [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) correcting every single-[qubit](../../../quantum-mechanics.md#qubit) error: $Z_1$ acts as a nontrivial logical phase error.

Let $C(S)$ denote the Pauli centralizer. The exact [Pauli error criterion for a stabilizer code](../../../quantum-error-correction.md#pauli-error-criterion-for-a-stabilizer-code) is

$$
\boxed{\text{For all }E_a,E_b\in\mathbb E,\quad E_a^\dagger E_b\in\mathcal ZS\ \text{or}\ E_a^\dagger E_b\notin C(S).}
$$

Equivalently, no difference of error labels lies in $L^\perp\setminus L$. The scalar phases in $\mathcal ZS$ are essential: an error product $-I$ is harmless even though it is not in $S$.

We prove the criterion. For $T=E_a^\dagger E_b$ outside $C(S)$, some $s\in S$ anticommutes with $T$. Since $sP=Ps=P$, we have $PTP=PsTsP=-PTP$, hence $PTP=0$. If $T=\lambda s\in\mathcal ZS$, then $PTP=\lambda P$. If $T\in C(S)\setminus\mathcal ZS$, it restricts to a [unitary operator](../../../vector-space.md#unitary-operator) on the [stabilizer code](../../../quantum-error-correction.md#stabilizer-code), but

$$
\operatorname{tr}(PT)=|S|^{-1}\sum_{s\in S}\operatorname{tr}(sT)=0:
$$

no $sT$ is scalar. A scalar restriction would have scalar coefficient zero by this trace equation, contradicting unitarity. Thus this third case is not scalar.

To justify why scalar compressions are exactly what correction requires, suppose one recovery corrects every $E_a$. Dilate that recovery to an isometry $W$ including its auxiliary system. Correct recovery of every pure [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) state gives $WE_a|\psi\rangle=|\psi\rangle\otimes|\eta_a\rangle$. The auxiliary state is independent of $\psi$: linearity on basis states and their superpositions forces their auxiliary vectors to coincide. Preservation of inner products then gives

$$
\langle\phi|E_a^\dagger E_b|\psi\rangle
=\langle\phi|\psi\rangle\langle\eta_a|\eta_b\rangle,
$$

which is the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) $PE_a^\dagger E_bP=c_{ab}P$. The three cases above prove necessity of the boxed criterion.

For sufficiency, put errors in the same class when $E_a^\dagger E_b\in\mathcal ZS$. They act identically on the [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) up to scalar phase, so give the same error-image subspace. Under the criterion, different classes give mutually orthogonal subspaces $E_a\mathcal C_S$, because their cross-compressions vanish. Measure which of these subspaces is occupied and apply the inverse of a representative error. This returns every [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) state unchanged; extend the recovery on the orthogonal complement by preparing any fixed [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) state. Linearity also corrects any valid noise channel whose [Kraus operators](../../../quantum-information-theory.md#kraus-operator) are linear combinations of the specified errors: within each syndrome all amplitudes multiply the same logical state, and trace preservation normalizes the recovered state. This proves sufficiency, including degenerate error classes.

## 2

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a classical [error-correcting code](../../../coding-theory.md#error-correcting-code) of length $n$, alphabet size $q$, minimum [Hamming distance](../../../coding-theory.md#hamming-distance) $d$ and $M$ codewords, the [Singleton bound](../../../coding-theory.md#singleton-bound) is

$$
M\le q^{n-d+1}.
$$

For a linear $[n,k,d]_q$ code this is **$n-k\ge d-1$**. Deleting any $d-1$ coordinates is injective on the codewords, since two words agreeing on the remaining coordinates would differ in fewer than $d$ positions; this also explains the classical bound.

For an n-[qubit](../../../quantum-mechanics.md#qubit) [quantum code](../../../quantum-error-correction.md#quantum-error-correcting-code) carrying $k>0$ [logical qubits](../../../quantum-error-correction.md#logical-qubit) and having [quantum code distance](../../../quantum-error-correction.md#distance-of-a-quantum-error-correcting-code) $d$, the [quantum Singleton bound](../../../quantum-error-correction.md#quantum-singleton-bound) is

$$
\boxed{n-k\ge2(d-1).}
$$

More generally replace $k$ by $\log_2K$ for code dimension $K>1$. The proof applies to degenerate codes too.

Let $r=d-1$. Purify the maximally mixed encoded input by a reference $R$ of dimension $K$:

$$
|\Omega\rangle=K^{-1/2}\sum_{j=1}^K|j\rangle_R|j_L\rangle,\qquad S(R)=\log_2K=:k.
$$

Distance $d$ makes erasure of any subset of at most $r$ [qubits](../../../quantum-mechanics.md#qubit) correctable. The allowed [quantum erasure correction](../../../quantum-error-correction.md#quantum-erasure-correction) condition says that a correctable erased set $A$ is decoupled from $R$:

$$
\rho_{RA}=\rho_R\otimes\rho_A,\qquad S(RA)=k+S(A).
$$

This is the [matrix](../../../vector-space.md#matrix)-element correction condition in another form: all operators on $A$ have constant diagonal [matrix](../../../vector-space.md#matrix) elements and zero off-diagonal [matrix](../../../vector-space.md#matrix) elements in the logical basis, so tracing the other physical [qubits](../../../quantum-mechanics.md#qubit) in $|\Omega\rangle\langle\Omega|$ yields the displayed product.

First justify the sizes needed for the partition. If $2r>n$, partition all physical [qubits](../../../quantum-mechanics.md#qubit) into $A,B$, both of size at most $r$. Both sets are correctable. Purity of $RAB$ and the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) give

$$
k+S(A)=S(RA)=S(B),\qquad k+S(B)=S(RB)=S(A).
$$

Adding forces $k=0$, a contradiction. Thus $2r\le n$, without assuming the bound we aim to prove.

Choose disjoint sets $A,B$ of size $r$, and let $C$ contain the remaining $n-2r$ [qubits](../../../quantum-mechanics.md#qubit). The joint state $RABC$ is pure, so decoupling and [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) give

$$
k+S(A)=S(RA)=S(BC)\le S(B)+S(C),
$$



$$
k+S(B)=S(RB)=S(AC)\le S(A)+S(C).
$$

Adding and cancelling gives $k\le S(C)$. The [Von Neumann entropy](../../../von-neumann-entropy.md) of $D$-dimensional states is at most $\log_2D$: for positive [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $p_i$, concavity of the [logarithm](../../../calculus.md#logarithm) gives $\sum_i p_i\log_2(1/p_i)\le\log_2\sum_i p_i/p_i\le\log_2D$. Here $D=2^{n-2r}$, so $k\le n-2r$, proving the quantum bound. The code is assumed to encode information ($K>1$); a one-dimensional code requires a separate distance convention, since simply re-preparing a known state makes its erasure-correction condition vacuous.

## 3

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [channel capacity](../../../information-theory.md#channel-capacity) is the supremum of reliable communication rates: a rate $R$ bits per use is achievable if block encoders and decoders using $n$ channel uses can transmit $M_n$ messages with error [probability](../../../probability-theory.md#probability) tending to zero and $\liminf n^{-1}\log_2M_n\ge R$.

A [discrete memoryless channel](../../../coding-theory.md#discrete-memoryless-channel) has fixed transition [probabilities](../../../probability-theory.md#probability) $W(y|x)$ on finite input and output alphabets, and

$$
W(y_1,\ldots,y_n|x_1,\ldots,x_n)=\prod_{j=1}^nW(y_j|x_j).
$$

Its single-letter capacity formula is

$$
\boxed{C=\max_{P_X}I(X;Y)=\max_{P_X}\bigl(H(Y)-H(Y|X)\bigr),}
$$

with [logarithms](../../../calculus.md#logarithm) to base two. The [Shannon second coding theorem](../../../coding-theory.md#noisy-channel-coding-theorem) identifies this maximum with the operational reliable rate.

For the [binary erasure channel](../../../coding-theory.md#binary-erasure-channel), use output symbols $0,1,e$, where $e$ is a recognizable erasure flag. Given input $x$, the output is $x$ with [probability](../../../probability-theory.md#probability) $1-p$ and $e$ with [probability](../../../probability-theory.md#probability) $p$. If $\Pr(X=1)=a$, the output [probabilities](../../../probability-theory.md#probability) are $(1-p)(1-a),(1-p)a,p$. Thus, writing $h_2$ for [binary entropy](../../../information-theory.md#binary-entropy),

$$
H(Y)=h_2(p)+(1-p)h_2(a),\qquad H(Y|X)=h_2(p),
$$

and $I(X;Y)=(1-p)h_2(a)$. Its maximum is attained by the uniform input $a=1/2$, giving

$$
\boxed{C=1-p\text{ bits per channel use},\qquad0\le p\le1.}
$$

In particular the noiseless and complete-erasure endpoints have capacities one and zero. The erasure flag reveals which positions were lost; it does not reveal the erased input values.

## 4

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a [density matrix](../../../quantum-theory.md#density-matrix) $\rho$ on a finite-dimensional [Hilbert space](../../../hilbert-space.md), its [Von Neumann entropy](../../../von-neumann-entropy.md) in bits is

$$
\boxed{S(\rho)=-\operatorname{tr}(\rho\log_2\rho)=-\sum_j\lambda_j\log_2\lambda_j,}
$$

where $\lambda_j$ are its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and $0\log_20=0$. It is the [Shannon entropy](../../../information-theory.md#information-entropy) of the spectrum, is zero for a [pure state](../../../quantum-theory.md#pure-state), and is invariant under unitary conjugation.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

**The concavity inequality is true, but its printed equality condition is false.** At $b=1$ equality always holds, even for distinct states; for example take $\rho_1=|0\rangle\langle0|$ and $\rho_2=|1\rangle\langle1|$. The correct statement on $0\le b\le1$ is

$$
\boxed{\text{Equality holds iff }b\in\{0,1\}\text{ or }\rho_1=\rho_2.}
$$

For $0<b<1$, entropy is therefore strictly concave.

We give the [matrix](../../../vector-space.md#matrix) inequality needed for the proof. Define the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) $D(\tau\|\sigma)=\operatorname{tr}\tau(\log_2\tau-\log_2\sigma)$ if the support of $\tau$ is contained in that of $\sigma$, and $+\infty$ otherwise. Diagonalize the two states with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $r_i,s_j$, and put $q_{ij}=|\langle i|j\rangle|^2$. Each row and column of $q$ sums to one. The elementary scalar inequality

$$
u\ln(u/v)\ge u-v
$$

follows from $x\ln x-x+1\ge0$, with equality exactly at $x=1$; use limits at zero. Consequently

$$
D(\tau\|\sigma)=\frac1{\ln2}\sum_{ij}q_{ij}r_i\ln(r_i/s_j)
\ge\frac1{\ln2}\sum_{ij}q_{ij}(r_i-s_j)=0.
$$

Equality forces $r_i=s_j$ whenever $q_{ij}>0$. Hence every [eigenvector](../../../linear-operator-theory.md#eigenvector) $|i\rangle$ of $\tau$ is also a $\sigma$-[eigenvector](../../../linear-operator-theory.md#eigenvector) with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $r_i$, so $\tau=\sigma$. Conversely identical states give zero relative entropy. This proves [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) and its equality condition, including states with zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) under the support convention.

Now set $\rho=b\rho_1+(1-b)\rho_2$. For $0<b<1$ its support contains both component supports. Direct expansion gives

$$
S(\rho)-bS(\rho_1)-(1-b)S(\rho_2)
=bD(\rho_1\|\rho)+(1-b)D(\rho_2\|\rho)\ge0.
$$

Since both coefficients are positive, equality holds exactly when both component states equal $\rho$, equivalently $\rho_1=\rho_2$. At either endpoint the mixture has only one component and equality is automatic. This proves the corrected [strict concavity of Von Neumann entropy](../../../von-neumann-entropy.md#strict-concavity-of-von-neumann-entropy).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

**False.** Take the [Bell state](../../../bell-state.md)

$$
|\Phi^+\rangle=\frac{|00\rangle+|11\rangle}{\sqrt2},\qquad\rho=|\Phi^+\rangle\langle\Phi^+|.
$$

The joint state is pure, so $S(\rho)=0$. Taking either [partial trace](../../../quantum-theory.md#partial-trace) kills the off-diagonal terms and gives $\rho_1=\rho_2=I_2/2$, whose two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $1/2$. Thus $S(\rho_1)=S(\rho_2)=1$, contradicting the proposed inequality $1\le0$. [Quantum entanglement](../../../bell-state.md#entangled-state) allows a pure joint state to have mixed subsystem states.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

**True: quantum entropy is subadditive.** Write $\sigma=\rho_1\otimes\rho_2$. Positivity ensures the support of $\rho$ lies in that of $\sigma$. Indeed, if $|v\rangle\in\ker\rho_1$, then $\sum_j\langle v,j|\rho|v,j\rangle=0$; all summands are nonnegative, so $\rho^{1/2}|v,j\rangle=0$ for every $j$. Thus $\rho$ annihilates $\ker\rho_1\otimes\mathcal K_2$, and similarly the kernel from the other factor.

On the resulting support, $\log_2(\rho_1\otimes\rho_2)=\log_2\rho_1\otimes I+I\otimes\log_2\rho_2$. Using the defining property of the [partial trace](../../../quantum-theory.md#partial-trace) and [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) proved in part (i),

$$
0\le D(\rho\|\rho_1\otimes\rho_2)
=-S(\rho)-\operatorname{tr}\rho_1\log_2\rho_1-\operatorname{tr}\rho_2\log_2\rho_2
=S(\rho_1)+S(\rho_2)-S(\rho).
$$

Hence

$$
\boxed{S(\rho)\le S(\rho_1)+S(\rho_2).}
$$

Equality holds exactly for the [product state](../../../bell-state.md#product-state) $\rho=\rho_1\otimes\rho_2$. This proves [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) directly.

## 5

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a [memoryless quantum channel](../../../quantum-information-theory.md#memoryless-quantum-channel) $\mathcal N$, successive uses are described by $\mathcal N^{\otimes n}$. Its [entanglement-assisted classical capacity](../../../quantum-information-theory.md#entanglement-assisted-classical-capacity) is the supremum of classical bits per use achievable with error tending to zero when sender and receiver may use unlimited preshared [quantum entanglement](../../../bell-state.md#entangled-state), independent of the message. Only the channel is used to transmit the message.

For input state $\rho_A$, choose a [purification](../../../quantum-theory.md#purification-of-a-density-operator) $|\psi_\rho\rangle_{RA}$ and set $\omega_{RB}=(\operatorname{id}_R\otimes\mathcal N)(|\psi_\rho\rangle\langle\psi_\rho|)$. The capacity formula is

$$
\boxed{C_E(\mathcal N)=\max_{\rho_A}I(R;B)_\omega
=\max_{\rho_A}\bigl[S(\rho_A)+S(\mathcal N(\rho_A))-S(\omega_{RB})\bigr].}
$$

[Purifications](../../../quantum-theory.md#purification-of-a-density-operator) differ only by an isometry on the reference, so this expression depends only on the input [density matrix](../../../quantum-theory.md#density-matrix). The quantity optimized is [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information).

The binary [quantum erasure channel](../../../quantum-information-theory.md#quantum-erasure-channel) sends a [qubit](../../../quantum-mechanics.md#qubit) to a [qubit](../../../quantum-mechanics.md#qubit) subspace plus an orthogonal erasure flag:

$$
\mathcal E_p(\rho)=(1-p)\rho\oplus p|e\rangle\langle e|,\qquad0\le p\le1.
$$

On the nonerased branch it transmits the entire state, including its coherences. Put $s=S(\rho)$. The [entropy of an orthogonal quantum mixture](../../../von-neumann-entropy.md#entropy-of-an-orthogonal-quantum-mixture) gives

$$
S(\mathcal E_p(\rho))=h_2(p)+(1-p)s.
$$

The reference-output state has two orthogonal branches:

$$
\omega_{RB}=(1-p)|\psi_\rho\rangle\langle\psi_\rho|\ \oplus\ p\rho_R\otimes|e\rangle\langle e|.
$$

The first branch is pure; the second has entropy $S(\rho_R)=s$. Thus $S(\omega_{RB})=h_2(p)+ps$ and

$$
I(R;B)_\omega=s+h_2(p)+(1-p)s-h_2(p)-ps=2(1-p)s.
$$

A [qubit](../../../quantum-mechanics.md#qubit) has entropy at most one bit, with equality at $\rho=I_2/2$. We conclude

$$
\boxed{C_E(\mathcal E_p)=2(1-p)\text{ bits per channel use}.}
$$

The endpoint capacities are two and zero. As an operational check, [superdense coding](../../../bell-state.md#superdense-coding) encodes four classical messages in one member of a shared Bell pair. A successful channel use lets the receiver identify the message; an erased [qubit](../../../quantum-mechanics.md#qubit) yields the flag. This induces a four-symbol classical erasure channel of capacity $(1-p)\log_24=2(1-p)$, agreeing with the entropy calculation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
