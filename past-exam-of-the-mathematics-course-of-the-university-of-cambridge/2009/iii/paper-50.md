# Paper 50

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper50.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper50.pdf)

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
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)

## 1

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $P$ be the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the code, and let $\{E_a\}$ be the specified error operators, including their [linear span](../../../vector-space.md#linear-span). The necessary and sufficient [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) is

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P\quad\text{for every }a,b,}
$$

where the scalar [matrix](../../../vector-space.md#matrix) $C$ is independent of the encoded state. In an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $\{|j_L\rangle\}$ of the code this means

$$
\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij}.
$$

There must be one recovery [quantum channel](../../../quantum-information-theory.md#quantum-channel) which corrects every allowed error channel, rather than a different recovery chosen using the unknown logical input.

The scalar condition means that any information carried away by the errors depends on their labels but not on the encoded amplitudes. To see how recovery works, diagonalize the [positive semidefinite matrix](../../../linear-algebra.md#positive-semidefinite-matrix) $C$ and take corresponding linear combinations $F_\ell$ of the errors. Then $PF_\ell^\dagger F_mP=\lambda_\ell\delta_{\ell m}P$. For each positive $\lambda_\ell$, the map $F_\ell P/\sqrt{\lambda_\ell}$ is an [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) into an error-image subspace, and these subspaces are mutually orthogonal. Measuring their label and reversing the associated [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) recovers the logical state without measuring its amplitudes. Zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) correspond to errors that annihilate the code. This also explains why the condition corrects arbitrary coherent combinations of the listed errors.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $A$ be the known set of affected [qubits](../../../quantum-mechanics.md#qubit), with $|A|\leq d-1$. Expand arbitrary operators on $A$ in [tensor products](../../../linear-algebra.md#tensor-product) of $I,X,Y,Z$. These [Pauli operators](../../../quantum-circuit.md#pauli-operator) span the complete error space on $A$.

By the [distance of a quantum error-correcting code](../../../quantum-error-correction.md#distance-of-a-quantum-error-correcting-code), every [Pauli operator](../../../quantum-circuit.md#pauli-operator) $F$ of weight below $d$ has scalar compression $PFP=c_FP$. For two errors $E_a,E_b$ on the same known set $A$, their product $E_a^\dagger E_b$ is also supported entirely on $A$. Its weight is therefore at most $|A|$, rather than twice $|A|$. Expansion in the Pauli basis consequently gives

$$
PE_a^\dagger E_bP=C_{ab}P.
$$

The [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) applies to the full operator space on $A$, so it gives a recovery for any error channel acting on that subsystem. **Every set of at most $d-1$ known error locations is correctable.** This is [quantum erasure correction](../../../quantum-error-correction.md#quantum-erasure-correction); the ability to use the locations is what improves the guarantee over unknown-location errors.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use base-two logarithms, so [Von Neumann entropy](../../../von-neumann-entropy.md) is measured in bits. Take an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the code and purify its maximally mixed logical state as

$$
|\Omega\rangle_{RQ}=2^{-k/2}\sum_{j=1}^{2^k}|j\rangle_R|j_L\rangle_Q.
$$

Only a $2^k$-dimensional reference support is needed; it can be embedded in the larger reference [Hilbert space](../../../hilbert-space.md) in the hint. Its [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is maximally mixed on that support, so $S(R)=k$.

For any correctable erased subsystem $A$, the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) gives $P(O_A\otimes I)P=c(O_A)P$ for every operator $O_A$. Taking its [matrix](../../../vector-space.md#matrix) elements in the logical basis shows that $\operatorname{Tr}_{Q\setminus A}|i_L\rangle\langle j_L|=0$ for $i\ne j$, and that the diagonal reductions are all the same state $\rho_A$. Thus

$$
\rho_{RA}=\rho_R\otimes\rho_A.
$$

In particular, the reference is decoupled from every set of at most $m=d-1$ erased [qubits](../../../quantum-mechanics.md#qubit).

For an information-carrying code $k>0$, first justify that two disjoint sets of size $m$ fit. If $2m\geq n$, partition all the physical [qubits](../../../quantum-mechanics.md#qubit) into sets $A,B$ each of size at most $m$. Both are correctable. Additivity of [Von Neumann entropy](../../../von-neumann-entropy.md) for a [product state](../../../bell-state.md#product-state), and equality of complementary entropies for the [pure state](../../../quantum-theory.md#pure-state) on $RAB$, give

$$
S(R)+S(A)=S(B),\qquad S(R)+S(B)=S(A).
$$

Adding yields $2S(R)=0$, contradicting $S(R)=k>0$. Hence $2m<n$.

Now choose disjoint $A,B$ of size $m$, and let $C$ contain the remaining $n-2m$ [qubits](../../../quantum-mechanics.md#qubit). The state on $RABC$ is pure. Product-state entropy additivity, equality of complementary entropies, and [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) give

$$
S(R)+S(A)=S(RA)=S(BC)\leq S(B)+S(C),
$$

and

$$
S(R)+S(B)=S(RB)=S(AC)\leq S(A)+S(C).
$$

Adding and cancelling proves $S(R)\leq S(C)$. Finally use the [maximum entropy of a quantum state](../../../von-neumann-entropy.md#maximum-entropy-of-a-quantum-state) bound $S(C)\leq\log_2\dim\mathcal H_C=n-2m$. Therefore the [quantum Singleton bound](../../../quantum-error-correction.md#quantum-singleton-bound) is

$$
\boxed{k\leq n-2(d-1),\qquad n-k\geq2(d-1).}
$$

This proof uses [quantum erasure correction](../../../quantum-error-correction.md#quantum-erasure-correction), not nondegeneracy, so it applies to degenerate codes as well. A code encoding no logical information requires a separate distance convention; the argument above concerns the usual $k>0$ coding problem.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Interpret $t$ as the largest guaranteed radius for correcting all unknown-location [Pauli operators](../../../quantum-circuit.md#pauli-operator) of weight at most $t$ together. Products of two such errors have weight at most $2t$, so the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) holds when $2t<d$. Conversely, let $F$ be a minimum-weight [Pauli operator](../../../quantum-circuit.md#pauli-operator) with nonscalar compression $PFP$. If $d\leq2t$, split its support into two sets of size at most $t$ and write $F=E_a^\dagger E_b$, up to an irrelevant phase. These two admissible errors violate the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition). Thus the [correctable Pauli error radius](../../../quantum-error-correction.md#correctable-pauli-error-radius) is

$$
\boxed{t=\left\lfloor\frac{d-1}{2}\right\rfloor,\qquad d\in\{2t+1,2t+2\}.}
$$

In particular, $d=2t+1$ requires the additional assumption that $d$ is odd. Distance is not uniquely determined by $t$ alone. Nor does the weight of a particular correctable error characterize this radius: particular higher-weight errors can also be correctable.

For a concrete even-distance example, the [stabilizer code](../../../quantum-error-correction.md#stabilizer-code) generated by $X^{\otimes4}$ and $Z^{\otimes4}$ has parameters $[[4,2,2]]$. Every single-qubit nonidentity [Pauli operator](../../../quantum-circuit.md#pauli-operator) anticommutes with a generator, so it has zero compression. But $Z_1Z_2$ commutes with both generators and acts nonscalarly on the code: it is unitary there and its code [trace](../../../linear-algebra.md#matrix-trace) is zero. Hence the distance is two and its guaranteed radius is zero. This shows why an unconditional odd-distance formula would be incorrect.

Ignoring overall phases, an error of weight $j$ has $\binom nj$ choices of support and three choices, $X,Y,Z$, at each affected [qubit](../../../quantum-mechanics.md#qubit). The identity is the weight-zero term, so

$$
\boxed{N(t)=\sum_{j=0}^t3^j\binom nj.}
$$

For a [nondegenerate quantum code](../../../quantum-error-correction.md#nondegenerate-quantum-error-correcting-code), distinct correctable Pauli errors have orthogonal error-image subspaces. Each has dimension $2^k$, since a [Pauli operator](../../../quantum-circuit.md#pauli-operator) is unitary. All $N(t)$ subspaces lie in the physical [Hilbert space](../../../hilbert-space.md) of dimension $2^n$. Counting dimensions proves the [quantum Hamming bound](../../../quantum-error-correction.md#quantum-hamming-bound)

$$
N(t)2^k\leq2^n,
\qquad
\boxed{N(t)\leq2^{n-k}.}
$$

Degeneracy would allow distinct errors to share an error-image subspace, so this particular counting argument would then fail.

## 2

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $D=\dim\mathcal H_A$ and introduce an isomorphic reference system $R$. Choose a basis $\{|j\rangle\}_{j=1}^D$ and the [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state)

$$
|\Omega\rangle_{RA}=\frac1{\sqrt D}\sum_{j=1}^D|j\rangle_R|j\rangle_A.
$$

Complete positivity makes

$$
\omega_{RA}=(\operatorname{id}_R\otimes\Phi)(|\Omega\rangle\langle\Omega|)
$$

a positive [density operator](../../../quantum-theory.md#density-matrix). This is the normalized [Choi matrix](../../../quantum-information-theory.md#choi-matrix), with the reference placed first. Its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) can be written

$$
\omega_{RA}=\sum_{\ell=1}^{r}\lambda_\ell|v_\ell\rangle\langle v_\ell|,
\qquad \lambda_\ell>0.
$$

The number $r$ is at most $D^2$.

Here an [index state](../../../quantum-theory.md#index-state) is a chosen basis vector $|j\rangle_R$ in the reference. The corresponding [relative state](../../../quantum-theory.md#relative-state-of-a-bipartite-vector) of $|v_\ell\rangle$ is the generally unnormalized vector

$$
|\eta_{\ell j}\rangle_A=(\langle j|_R\otimes I_A)|v_\ell\rangle_{RA}.
$$

Thus $|v_\ell\rangle=\sum_j|j\rangle_R|\eta_{\ell j}\rangle_A$. Define a [linear map](../../../vector-space.md#linear-map) $A_\ell$ by its columns:

$$
A_\ell|j\rangle=\sqrt{D\lambda_\ell}\,|\eta_{\ell j}\rangle.
$$

Then $(I_R\otimes A_\ell)|\Omega\rangle=\sqrt{\lambda_\ell}|v_\ell\rangle$, so

$$
\omega_{RA}=\sum_\ell(I_R\otimes A_\ell)|\Omega\rangle\langle\Omega|(I_R\otimes A_\ell^\dagger).
$$

Expand both sides in reference [matrix units](../../../vector-space.md#matrix-unit). The block with reference indices $i,j$ on the left is $D^{-1}\Phi(|i\rangle\langle j|)$; on the right it is $D^{-1}\sum_\ell A_\ell|i\rangle\langle j|A_\ell^\dagger$. Since [matrix units](../../../vector-space.md#matrix-unit) span all operators and $\Phi$ is linear,

$$
\boxed{\Phi(\rho)=\sum_\ell A_\ell\rho A_\ell^\dagger.}
$$

This constructs the [Kraus representation](../../../quantum-information-theory.md#kraus-representation) explicitly from the relative states, rather than assuming it.

Finally, [trace](../../../linear-algebra.md#matrix-trace) preservation implies for every [density operator](../../../quantum-theory.md#density-matrix) $\rho$ that

$$
\operatorname{Tr}\rho=\operatorname{Tr}\Phi(\rho)
=\operatorname{Tr}\left[\rho\sum_\ell A_\ell^\dagger A_\ell\right].
$$

Taking every rank-one [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) as $\rho$ forces the [Hermitian operator](../../../hilbert-space.md#hermitian-operator) in brackets to have the same quadratic form as the identity. Therefore

$$
\boxed{\sum_\ell A_\ell^\dagger A_\ell=I.}
$$

The argument is finite-dimensional, as appropriate to the quantum-information setting; a channel with a different output dimension has the same construction with rectangular [Kraus operators](../../../quantum-information-theory.md#kraus-operator).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Fix a basis for the [transposition map](../../../vector-space.md#transpose) $T$. If $M\geq0$, write $M=BB^\dagger$. Then

$$
T(M)=M^T=\overline B B^T=\overline B(\overline B)^\dagger\geq0.
$$

Thus transposition is a [positive linear map](../../../quantum-information-theory.md#positive-linear-map) and also preserves the [trace](../../../linear-algebra.md#matrix-trace).

For dimension $D\geq2$, apply it to one subsystem of the [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) from part (a):

$$
(\operatorname{id}\otimes T)(|\Omega\rangle\langle\Omega|)
=\frac1D\sum_{i,j}|i\rangle\langle j|\otimes|j\rangle\langle i|
=\frac FD,
$$

where $F$ is the [swap operator](../../../quantum-information-theory.md#swap-operator), $F(|u\rangle\otimes|v\rangle)=|v\rangle\otimes|u\rangle$. It satisfies $F^\dagger=F$ and $F^2=I$, so its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $+1$ on symmetric vectors and $-1$ on antisymmetric vectors. In particular,

$$
|\eta\rangle=\frac{|1\rangle|2\rangle-|2\rangle|1\rangle}{\sqrt2},
\qquad
\langle\eta|\frac FD|\eta\rangle=-\frac1D<0.
$$

A positive input has therefore acquired a negative expectation value after adjoining an identity channel. **Transposition is positive but not completely positive in dimension at least two.** The one-dimensional case is the identity map and is completely positive; the dimension qualification is necessary.

## 3

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write $\overline\rho=\sum_i p_i\rho_i$. The [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) is

$$
\boxed{\chi(\mathcal E)=S(\overline\rho)-\sum_i p_iS(\rho_i),}
$$

where $S$ is [Von Neumann entropy](../../../von-neumann-entropy.md), with a consistent logarithm base. Attach an orthogonal classical label register $X$ to form the [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state)

$$
\omega_{XB}=\sum_i p_i|i\rangle\langle i|_X\otimes\rho_i.
$$

The [entropy of an orthogonal quantum mixture](../../../von-neumann-entropy.md#entropy-of-an-orthogonal-quantum-mixture) gives

$$
S(X)=H(p),\quad S(XB)=H(p)+\sum_i p_iS(\rho_i),\quad S(B)=S(\overline\rho).
$$

Here $H(p)$ is the [Shannon entropy](../../../information-theory.md#information-entropy) of the classical label. Hence $I(X:B)=\chi(\mathcal E)$, where $I$ denotes [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information).

Let $\Phi:B\to C$ be the proposed [quantum channel](../../../quantum-information-theory.md#quantum-channel). Using its [Kraus representation](../../../quantum-information-theory.md#kraus-representation), define an [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) $V=\sum_\ell A_\ell\otimes|\ell\rangle_E$, since $V^\dagger V=I$. This is a [Stinespring representation](../../../quantum-information-theory.md#stinespring-representation-of-a-completely-positive-map). Apply it to $B$, obtaining a state $\eta_{XCE}$; tracing out $E$ applies $\Phi$ to every ensemble member. An [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) preserves nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) and therefore [Von Neumann entropy](../../../von-neumann-entropy.md), so

$$
I(X:CE)_\eta=I(X:B)_\omega=\chi(\mathcal E),
\qquad
I(X:C)_\eta=\chi(\{p_i,\Phi(\rho_i)\}).
$$

Their difference is

$$
I(X:CE)-I(X:C)=S(XC)+S(CE)-S(C)-S(XCE).
$$

The [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy) states that this expression is nonnegative for every tripartite state. Consequently

$$
\boxed{\chi(\{p_i,\Phi(\rho_i)\})\leq\chi(\mathcal E).}
$$

Thus the [Holevo quantity under a quantum channel](../../../quantum-information-theory.md#holevo-quantity-under-a-quantum-channel) decreases because discarding the dilation environment cannot improve correlations with the classical label. The probabilities remain unchanged throughout.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Using base-two logarithms, define the [quantum conditional entropy](../../../von-neumann-entropy.md#quantum-conditional-entropy) by

$$
\boxed{S(A\mid B)=S(\rho_{AB})-S(\rho_B).}
$$

The [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy), $S(AB)\leq S(A)+S(B)$, immediately gives $S(A\mid B)\leq S(A)$.

For the lower bound, purify $\rho_{AB}$ by an auxiliary system $C$. Complementary subsystems of a [pure state](../../../quantum-theory.md#pure-state) have the same nonzero reduced-state [eigenvalues](../../../linear-operator-theory.md#eigenvalue), by the [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition). Hence $S(BC)=S(A)$ and $S(C)=S(AB)$. Applying [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) to $BC$ gives

$$
S(A)=S(BC)\leq S(B)+S(C)=S(B)+S(AB).
$$

Rearranging yields $S(A\mid B)\geq-S(A)$. This is the relevant side of the [Araki–Lieb inequality](../../../von-neumann-entropy.md#araki-lieb-inequality), here derived using purification.

Finally the [maximum entropy of a quantum state](../../../von-neumann-entropy.md#maximum-entropy-of-a-quantum-state) gives $S(A)\leq\log_2\dim\mathcal H_A$. For example, this follows directly from

$$
D\left(\rho_A\middle\|\frac{I_A}{\dim\mathcal H_A}\right)
=\log_2\dim\mathcal H_A-S(A)\geq0
$$

by [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy). Combining the two bounds proves

$$
\boxed{|S(A\mid B)|\leq\log_2\dim\mathcal H_A.}
$$

Both signs can be attained: a maximally mixed $A$ independent of $B$ has the positive extreme, while a [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) with a sufficiently large $B$ has the negative extreme.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\mathcal P$ be the [pinching map](../../../quantum-measurement.md#pinching-map) determined by the projectors, and put $\sigma=\mathcal P(\rho)$. This is a [nonselective projective measurement](../../../quantum-measurement.md#nonselective-projective-measurement); its projectors are its [Kraus operators](../../../quantum-information-theory.md#kraus-operator). We will prove the exact [relative entropy of a pinched state](../../../von-neumann-entropy.md#relative-entropy-of-a-pinched-state) identity.

First the support of $\rho$ is contained in that of $\sigma$. Indeed, if $v$ lies in the kernel of $\sigma$, positivity gives

$$
0=\langle v|\sigma|v\rangle=\sum_i\langle P_iv|\rho|P_iv\rangle
=\sum_i\|\rho^{1/2}P_iv\|^2.
$$

Every summand is zero. Since $\sum_iP_i=I$, also $\rho^{1/2}v=0$, and thus $v$ is in the kernel of $\rho$. Therefore the logarithm of $\sigma$ may be used on its support without an infinite relative-entropy term.

The operator $\sigma$ is block diagonal, so each $P_i$ commutes with $\log\sigma$ on that support. Cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) gives

$$
\operatorname{Tr}(\sigma\log\sigma)
=\sum_i\operatorname{Tr}(P_i\rho P_i\log\sigma)
=\operatorname{Tr}\left(\rho\sum_iP_i\log\sigma P_i\right)
=\operatorname{Tr}(\rho\log\sigma).
$$

Expand the [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy):

$$
D(\rho\|\sigma)=\operatorname{Tr}(\rho\log\rho)-\operatorname{Tr}(\rho\log\sigma)
=S(\sigma)-S(\rho).
$$

Its nonnegativity now proves the [entropy increase under nonselective projective measurement](../../../von-neumann-entropy.md#entropy-increase-under-nonselective-projective-measurement):

$$
\boxed{S(\sigma)\geq S(\rho).}
$$

The equality case in [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) says equality holds exactly when $\rho=\sigma$. Equivalently,

$$
\boxed{P_i\rho P_j=0\text{ for }i\ne j,\quad\text{or, equivalently, }[\rho,P_i]=0\text{ for every }i.}
$$

Thus equality means the state already has no coherence between distinct measurement blocks. It need not be diagonal inside a block of rank greater than one.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Take the rank-one [orthogonal projections](../../../hilbert-space.md#orthogonal-projection) $P_i=|\phi_i\rangle\langle\phi_i|$. Their [pinching map](../../../quantum-measurement.md#pinching-map) gives

$$
\mathcal P(\rho)=\sum_iP_i\rho P_i
=\sum_i\langle\phi_i|\rho|\phi_i\rangle\,|\phi_i\rangle\langle\phi_i|=\rho_d.
$$

This has exactly the specified diagonal entries and no off-diagonal entries. Applying the [entropy increase under nonselective projective measurement](../../../von-neumann-entropy.md#entropy-increase-under-nonselective-projective-measurement) proved in part (c) therefore gives

$$
\boxed{S(\rho)\leq S(\rho_d).}
$$

Writing $q_i=\langle\phi_i|\rho|\phi_i\rangle$, the output [Von Neumann entropy](../../../von-neumann-entropy.md) is the [Shannon entropy](../../../information-theory.md#information-entropy) $S(\rho_d)=-\sum_iq_i\log q_i$. Equality holds precisely when $\rho$ was already diagonal in this basis.

## 4

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

**Yes: use [superdense coding](../../../bell-state.md#superdense-coding), with a shared [Bell state](../../../bell-state.md).** Let the sender and receiver initially hold the first and second [qubits](../../../quantum-mechanics.md#qubit) of $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. To encode bits $(a,b)$, the sender applies $Z^aX^b$ to her [qubit](../../../quantum-mechanics.md#qubit). These [Pauli operators](../../../quantum-circuit.md#pauli-operator) produce four orthogonal states:

$$
\begin{array}{c|c}
(a,b)&(Z^aX^b\otimes I)|\Phi^+\rangle\\
(0,0)&(|00\rangle+|11\rangle)/\sqrt2\\
(1,0)&(|00\rangle-|11\rangle)/\sqrt2\\
(0,1)&(|01\rangle+|10\rangle)/\sqrt2\\
(1,1)&(|01\rangle-|10\rangle)/\sqrt2
\end{array}
$$

She sends this [qubit](../../../quantum-mechanics.md#qubit) through the noiseless [quantum channel](../../../quantum-information-theory.md#quantum-channel). The receiver then possesses both [qubits](../../../quantum-mechanics.md#qubit). He applies a [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) from the received [qubit](../../../quantum-mechanics.md#qubit) to his original [qubit](../../../quantum-mechanics.md#qubit), followed by a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) on the received [qubit](../../../quantum-mechanics.md#qubit). This maps the four states in the table to $|ab\rangle$. A measurement in the [computational basis](../../../quantum-theory.md#computational-basis) therefore recovers the two bits with certainty. No classical message is sent.

The resource assumption deserves care: one-qubit [superdense coding](../../../bell-state.md#superdense-coding) needs a [Bell pair](../../../bell-state.md#bell-pair) already shared before encoding. If none is initially available, the sender can prepare a [Bell pair](../../../bell-state.md#bell-pair) locally and send one half through the same noiseless [quantum channel](../../../quantum-information-theory.md#quantum-channel) in advance. The protocol then uses two transmitted [qubits](../../../quantum-mechanics.md#qubit) in total, including distribution of the entanglement, still with no classical communication. Alternatively, sending two [computational basis](../../../quantum-theory.md#computational-basis) [qubits](../../../quantum-mechanics.md#qubit) directly also communicates two bits. **With a pre-shared [Bell pair](../../../bell-state.md#bell-pair), one transmitted [qubit](../../../quantum-mechanics.md#qubit) suffices; without it, the entanglement-distribution cost must be counted.** An unassisted single transmitted [qubit](../../../quantum-mechanics.md#qubit) cannot perfectly encode four classical messages: its [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) is at most $\log_2 2=1$ bit.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

**Yes, the conversion can be deterministic using [local operations and classical communication](../../../bell-state.md#local-operations-and-classical-communication).** Put $s=\sin\theta$ and $c=\cos\theta$. The initial state's squared [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are $(1/2,1/2)$, while the target's decreasingly ordered squared [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) are $(c^2,s^2)$. Since $0<\theta<\pi/4$, one has $1/2<c^2$ and both pairs sum to one. Thus

$$
(1/2,1/2)\prec(c^2,s^2).
$$

The direction of this [majorization](../../../vector-space.md#majorization) is the allowed one in [Nielsen's pure-state conversion theorem](../../../bell-state.md#nielsen-s-pure-state-conversion-theorem): maximal entanglement can be reduced by deterministic [LOCC](../../../bell-state.md#local-operations-and-classical-communication).

Here is an explicit protocol, so no conversion theorem need be assumed. The sender first applies a [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) to remove the initial Bell-state minus sign. Starting from $|\Phi^+\rangle$, she performs a two-outcome local measurement with [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
M_0=\begin{pmatrix}s&0\\0&c\end{pmatrix},
\qquad
M_1=\begin{pmatrix}c&0\\0&s\end{pmatrix}.
$$

They define a valid measurement because $M_0^\dagger M_0+M_1^\dagger M_1=I$. The two unnormalized states after measurement are

$$
(M_0\otimes I)|\Phi^+\rangle=\frac{s|00\rangle+c|11\rangle}{\sqrt2},
\qquad
(M_1\otimes I)|\Phi^+\rangle=\frac{c|00\rangle+s|11\rangle}{\sqrt2}.
$$

Each outcome has probability $1/2$. For outcome zero, the normalized state is already $s|00\rangle+c|11\rangle$. For outcome one, both parties apply [Pauli X gates](../../../quantum-theory.md#pauli-x-gate), obtaining the same state. The sender communicates only which outcome occurred. Finally the receiver applies a [Pauli X gate](../../../quantum-theory.md#pauli-x-gate), giving $s|01\rangle+c|10\rangle$ in either branch. This is [deterministic two-qubit entanglement dilution](../../../bell-state.md#deterministic-two-qubit-entanglement-dilution), with total success probability one; it does not rely on postselection.

## 5

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Label the atomic ground state $|0\rangle$ and excited state $|1\rangle$, with $0\leq p\leq1$. The process is the [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel), with [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
\boxed{A_0=|0\rangle\langle0|+\sqrt{1-p}\,|1\rangle\langle1|
=\begin{pmatrix}1&0\\0&\sqrt{1-p}\end{pmatrix},
\qquad
A_1=\sqrt p\,|0\rangle\langle1|
=\begin{pmatrix}0&\sqrt p\\0&0\end{pmatrix}.}
$$

They satisfy $A_0^\dagger A_0+A_1^\dagger A_1=I$, so the resulting [Kraus representation](../../../quantum-information-theory.md#kraus-representation) is [trace](../../../linear-algebra.md#matrix-trace) preserving.

The operator $A_1$ represents emission: it maps the excited state to $\sqrt p$ times the ground state and annihilates the ground state. Its probability for an initially excited atom is $p$. The operator $A_0$ represents no emission: it leaves the ground state unchanged and retains the excited amplitude with factor $\sqrt{1-p}$. This branch is not generally the identity operation; the absence of a photon itself changes the conditional relative amplitudes. For an arbitrary atomic [density operator](../../../quantum-theory.md#density-matrix), the emission probability is $\operatorname{Tr}(A_1\rho A_1^\dagger)=p\rho_{11}$ and the no-emission probability is $1-p\rho_{11}$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

A [unital quantum channel](../../../quantum-information-theory.md#unital-quantum-channel) preserves the identity operator: $\Phi(I)=I$. For equal input and output dimensions, this is equivalent to preserving the maximally mixed [density operator](../../../quantum-theory.md#density-matrix).

For the [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel),

$$
\Phi(I)=A_0A_0^\dagger+A_1A_1^\dagger
=\begin{pmatrix}1+p&0\\0&1-p\end{pmatrix}.
$$

Thus **the channel is not unital for $p>0$; it is unital only at $p=0$, when it is the identity channel.** In particular, it biases the [maximally mixed state](../../../quantum-theory.md#maximally-mixed-state) toward the atomic ground state. The trace-preservation condition involves $\sum_jA_j^\dagger A_j$, whereas unitality involves the opposite products $\sum_jA_jA_j^\dagger$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Take an environment initially in its vacuum state $|0\rangle_E$, with $|1\rangle_E$ recording an emitted photon. In atom-environment order, put $q=\sqrt{1-p}$ and $u=\sqrt p$. A [unitary dilation of amplitude damping](../../../quantum-information-theory.md#unitary-dilation-of-amplitude-damping) is defined by

$$
\begin{aligned}
U|00\rangle&=|00\rangle,& U|10\rangle&=q|10\rangle+u|01\rangle,\\
U|01\rangle&=q|01\rangle-u|10\rangle,& U|11\rangle&=|11\rangle.
\end{aligned}
$$

The middle two images are orthonormal, and they are orthogonal to the two fixed images. Thus this completion really is a [unitary operator](../../../vector-space.md#unitary-operator). For the occupied initial environmental subspace, it leaves a ground-state atom unchanged and splits an excited-state atom into no-emission and emission alternatives with probabilities $1-p$ and $p$.

Tracing out the environment after this unitary evolution gives

$$
\Phi(\rho)=\operatorname{Tr}_E\bigl[U(\rho\otimes|0\rangle\langle0|_E)U^\dagger\bigr].
$$

The environment [matrix](../../../vector-space.md#matrix) elements are $\langle0|_EU|0\rangle_E=A_0$ and $\langle1|_EU|0\rangle_E=A_1$, recovering the [Kraus operators](../../../quantum-information-theory.md#kraus-operator) in part (a). More explicitly, the basis operators transform as

$$
\begin{aligned}
|0\rangle\langle0|&\longmapsto|0\rangle\langle0|,\\
|1\rangle\langle1|&\longmapsto(1-p)|1\rangle\langle1|+p|0\rangle\langle0|,\\
|0\rangle\langle1|&\longmapsto\sqrt{1-p}|0\rangle\langle1|,\\
|1\rangle\langle0|&\longmapsto\sqrt{1-p}|1\rangle\langle0|.
\end{aligned}
$$

Applying linearity to the atomic [density operator](../../../quantum-theory.md#density-matrix) therefore yields

$$
\boxed{\Phi(\rho)=\begin{pmatrix}
\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\
\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}
\end{pmatrix}.}
$$

The lost excited population goes to the ground state, the [trace](../../../linear-algebra.md#matrix-trace) stays one, and coherences decrease by $\sqrt{1-p}$. Discarding the distinguishable environmental photon record is precisely what turns the joint unitary evolution into a noisy atomic [quantum channel](../../../quantum-information-theory.md#quantum-channel).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Let the [quantum channel](../../../quantum-information-theory.md#quantum-channel) send $B$ to $B'$. From its [Kraus representation](../../../quantum-information-theory.md#kraus-representation), choose a [Stinespring representation](../../../quantum-information-theory.md#stinespring-representation-of-a-completely-positive-map) $V:B\to B'E$ and form

$$
\sigma_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger).
$$

The channel output is $\sigma_{AB'}=\operatorname{Tr}_E\sigma_{AB'E}$. Isometric invariance of [Von Neumann entropy](../../../von-neumann-entropy.md) gives

$$
S(B'E)_\sigma=S(B)_\rho,\quad S(AB'E)_\sigma=S(AB)_\rho,\quad S(A)_\sigma=S(A)_\rho.
$$

Therefore the [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) satisfies $I(A:B)_\rho=I(A:B'E)_\sigma$. Expanding its loss after discarding the environment gives

$$
\begin{aligned}
I(A:B)_\rho-I(A:B')_\sigma
&=I(A:B'E)_\sigma-I(A:B')_\sigma\\
&=S(AB')_\sigma+S(B'E)_\sigma-S(B')_\sigma-S(AB'E)_\sigma.
\end{aligned}
$$

The final expression is the [quantum conditional mutual information](../../../von-neumann-entropy.md#quantum-conditional-mutual-information) $I(A:E\mid B')$. The [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy) states exactly that it is nonnegative. Hence

$$
\boxed{I(A:B')\leq I(A:B).}
$$

This proves [data processing for quantum mutual information](../../../von-neumann-entropy.md#data-processing-for-quantum-mutual-information) for any mixed input and any local [quantum channel](../../../quantum-information-theory.md#quantum-channel), not just the atomic channel in earlier parts. The correlations lost are exactly the conditional correlations with the discarded environment.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
