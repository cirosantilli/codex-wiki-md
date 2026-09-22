# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper33.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $P$ be the [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) onto the [quantum code](../../../quantum-error-correction.md#quantum-error-correcting-code) $\mathcal X$, and choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $|i_L\rangle$ for it. The necessary and sufficient [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) is that one [matrix](../../../vector-space.md#matrix) $C$, independent of the logical labels, satisfies

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P\quad\text{for all }E_a,E_b\in\mathcal E.}
$$

Equivalently, $\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij}$. This makes the information in the error label independent of the encoded [quantum state](../../../quantum-mechanics.md#quantum-state). It applies to the whole linear span of the errors, and hence to every noise [quantum channel](../../../quantum-information-theory.md#quantum-channel) with [Kraus operators](../../../quantum-information-theory.md#kraus-operator) in that span.

Here is a proof of both directions. For [necessity of the Knill-Laflamme condition](../../../quantum-error-correction.md#necessity-of-the-knill-laflamme-condition), let $R_\mu$ be [Kraus operators](../../../quantum-information-theory.md#kraus-operator) of a common recovery, so $\sum_\mu R_\mu^\dagger R_\mu=I$. Since recovery after $E_a$ must return the pure input state, every vector $R_\mu E_a|\psi\rangle$ is parallel to $|\psi\rangle$. A [linear operator](../../../vector-space.md#linear-operator) on the code which sends every vector to a multiple of itself is scalar: apply it to two basis vectors and their sum to force the two multipliers to agree. Therefore $R_\mu E_aP=c_{\mu a}P$ with no dependence on $|\psi\rangle$. It follows that

$$
PE_a^\dagger E_bP=\sum_\mu PE_a^\dagger R_\mu^\dagger R_\mu E_bP
=\sum_\mu c_{\mu a}^*c_{\mu b}P.
$$

This proves necessity without assuming in advance that the physical errors have orthogonal syndromes.

For sufficiency, $C$ is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix): for any normalized code state and coefficients $v_a$, $v^\dagger Cv=\|\sum_a v_aE_a|\psi\rangle\|^2\geq0$. Diagonalize $C$ by a unitary change of the error basis to get operators $F_j$ with $PF_j^\dagger F_lP=c_j\delta_{jl}P$. If $c_j>0$, $V_j=F_jP/\sqrt{c_j}$ is a [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces) from the code to an error-image subspace, and distinct such images are orthogonal. If $c_j=0$, then $F_jP=0$. A [projective measurement](../../../quantum-measurement.md#projective-measurement) of these image subspaces followed by $V_j^\dagger$ recovers every logical state. Complete the recovery on the unused orthogonal complement in any trace-preserving manner. For a coherent error $\sum_jv_jF_j$, the measurement branch $j$ contains $v_j\sqrt{c_j}|\psi\rangle$; the branch probability is independent of the logical state, and discarding the syndrome leaves the original state. This is [constructive recovery from the Knill-Laflamme condition](../../../quantum-error-correction.md#constructive-recovery-from-the-knill-laflamme-condition).

For the usual family of distinct unitary [Pauli errors](../../../quantum-circuit.md#pauli-operator) modulo scalar phase, [nondegenerate quantum code](../../../quantum-error-correction.md#nondegenerate-quantum-error-correcting-code) correction means that different physical errors have orthogonal image subspaces. The precise condition is

$$
\boxed{C_{ab}=\delta_{ab},\qquad
\langle i_L|E_a^\dagger E_b|j_L\rangle=\delta_{ab}\delta_{ij}.}
$$

For nonunitary errors, replace the unit diagonal by positive norm factors. In an arbitrary error basis the Gram matrix need not initially be diagonal; its positive-eigenvalue modes give the independent syndrome spaces just constructed. A kernel of $C$ exhibits a linear combination of errors acting as zero on the code. In particular two distinct physical errors with the same action on the code cannot be distinguished and give degenerate correction, as in part (c).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Here the number of errors means the number of affected physical [qubits](../../../quantum-mechanics.md#qubit): assume that all errors supported on at most $t$ qubits are jointly correctable. It does not mean the cardinality of an arbitrary selected error list. Let $F$ be any [Pauli operator](../../../quantum-circuit.md#pauli-operator) of weight at most $2t$. Split its support into disjoint sets $A,B$, each of size at most $t$, and write $F=F_AF_B$. Each Pauli factor is Hermitian, so take $E_a=F_A$, $E_b=F_B$ to get $F=E_a^\dagger E_b$, up to an irrelevant scalar phase if different Pauli representatives are used. The [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) gives

$$
PFP=PE_a^\dagger E_bP=C_{ab}P.
$$

This is precisely [quantum error detection](../../../quantum-error-correction.md#quantum-error-detection): a [projective measurement](../../../quantum-measurement.md#projective-measurement) with outcomes $P,I-P$ either detects departure from the code or leaves the accepted logical state unchanged up to a scalar. Some errors can be harmless scalars on the code, particularly for degenerate correction; detection is not required to flag such an error with certainty.

Any [linear operator](../../../vector-space.md#linear-operator) supported on at most $2t$ qubits is a linear combination of [Pauli operators](../../../quantum-circuit.md#pauli-operator) on those qubits, so its code compression is scalar by [linearity](../../../vector-space.md#linearity). Thus

$$
\boxed{\text{correction of all errors of weight at most }t\ \Longrightarrow\ \text{detection of all errors of weight at most }2t.}
$$

This is [correction implies detection at twice the weight](../../../quantum-error-correction.md#correction-implies-detection-at-twice-the-weight). The premise about all locations and all error types is essential: merely correcting one selected operator gives no universal statement about every operator of twice its weight.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use the normalized three-qubit states $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. The [Shor code](../../../quantum-error-correction.md#shor-code) has logical basis

$$
\boxed{|0_L\rangle=|G_+\rangle^{\otimes3},\qquad
|1_L\rangle=|G_-\rangle^{\otimes3}.}
$$

It encodes $\alpha|0\rangle+\beta|1\rangle$ as $\alpha|0_L\rangle+\beta|1_L\rangle$, preserving the unknown amplitudes by a [linear isometry](../../../hilbert-space.md#linear-isometry-of-hilbert-spaces). It concatenates a three-block [phase-flip repetition code](../../../quantum-error-correction.md#phase-flip-repetition-code) with the three-qubit [bit-flip repetition code](../../../quantum-error-correction.md#bit-flip-repetition-code) inside each block. Six [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator), $Z_1Z_2,Z_2Z_3,Z_4Z_5,Z_5Z_6,Z_7Z_8,Z_8Z_9$, test bit errors inside the blocks. The other two [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) are

$$
A=X_1X_2X_3X_4X_5X_6,\qquad
B=X_4X_5X_6X_7X_8X_9.
$$

All eight commute and have eigenvalue $+1$ on both logical basis states. They define the $[[9,1,3]]$ [stabilizer code](../../../quantum-error-correction.md#stabilizer-code). The inner checks identify single bit flips, and the outer checks identify a block phase flip; combined they also correct a [Pauli Y gate](../../../quantum-theory.md#pauli-y-gate) error, since $Y=iXZ$.

For the requested [phase flip](../../../quantum-theory.md#pauli-z-gate), a $Z$ on any one qubit interchanges $|G_+\rangle$ and $|G_-\rangle$ in its block. It commutes with the six $Z$-pair checks. It anticommutes with $A$ or $B$ exactly when its block is contained in that check. The [Shor-code phase-flip syndrome](../../../quantum-error-correction.md#shor-code-phase-flip-syndrome) is therefore

$$
\begin{array}{c|c|c}
\text{error block}&(A,B)\text{ outcomes}&\text{recovery}\\\hline
\text{none}&(+1,+1)&I\\
1&(-1,+1)&Z_1\\
2&(-1,-1)&Z_4\\
3&(+1,-1)&Z_7
\end{array}
$$

A [projective measurement](../../../quantum-measurement.md#projective-measurement) of the two commuting checks yields the displayed [error syndrome](../../../quantum-error-correction.md#error-syndrome) without learning $\alpha$ or $\beta$: both logical components have the same check eigenvalues after the error. Applying the indicated [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) restores every encoded [quantum state](../../../quantum-mechanics.md#quantum-state).

The correction is genuinely degenerate. For $i,j$ in the same block, $Z_iZ_j$ fixes both $|000\rangle$ and $|111\rangle$, so $Z_iZ_jP=P$ and consequently $Z_iP=Z_jP$. In particular $Z_1$ and $Z_2$ are distinct physical errors but have identical action on every code state; their image subspaces coincide, not merely their observed syndrome labels. In the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) for $I,Z_1,\ldots,Z_9$, the error [Gram matrix](../../../linear-algebra.md#gram-matrix) has $C_{00}=1$, $C_{0i}=C_{i0}=0$, and

$$
C_{ij}=\begin{cases}1,&i,j\text{ in the same block},\\0,&i,j\text{ in different blocks}.
\end{cases}
$$

The zero overlaps between different blocks follow because a phase flip changes a different pattern of orthogonal $G_+,G_-$ factors; cross-logical overlaps also vanish. Thus $C$ consists of one $1\times1$ block and three all-ones $3\times3$ blocks and has rank four, not ten. This both proves correctability of the entire single-phase-error span and exhibits its degeneracy. A coherent sum of phase errors in one block has the same logical action with its coefficients summed, so inability to locate the individual qubit loses no logical information. **The two block checks suffice to correct every single phase flip, even though the within-block errors are indistinguishable.**

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For an $n$-qubit [quantum code](../../../quantum-error-correction.md#quantum-error-correcting-code) with projector $P$, the [quantum code distance](../../../quantum-error-correction.md#distance-of-a-quantum-error-correcting-code) is

$$
\boxed{d=\min\{\operatorname{wt}(F):F\text{ is a Pauli operator and }PFP\notin\mathbb CP\}.}
$$

Here the weight counts nonidentity tensor factors. Thus every error supported on fewer than $d$ qubits is detectable, by the [Pauli expansion of a quantum error](../../../quantum-circuit.md#pauli-expansion-of-a-quantum-error). A scalar action on the code, including a nonidentity [stabilizer](../../../group-theory.md#stabilizer-subgroup), is harmless and does not reduce this distance. For a [stabilizer code](../../../quantum-error-correction.md#stabilizer-code), the equivalent definition minimizes weight among [Pauli operators](../../../quantum-circuit.md#pauli-operator) which commute with every [stabilizer generator](../../../quantum-circuit.md#stabilizer-generator) but act nontrivially on the logical information. The [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) then guarantees correction of all errors of weight at most $t=\lfloor(d-1)/2\rfloor$, since each pairwise product has weight at most $2t<d$.

Suppose the code encodes $k$ logical [qubits](../../../quantum-mechanics.md#qubit) and is nondegenerate for all errors through weight $t$. There are

$$
N_t=\sum_{j=0}^t3^j\binom nj
$$

distinct [Pauli errors](../../../quantum-circuit.md#pauli-operator) modulo phase: choose the $j$ affected positions and choose $X,Y$ or $Z$ at each. Each error is unitary, so its image of the code has dimension $2^k$. Nondegeneracy makes these images mutually orthogonal, equivalently the combined vectors $E_a|i_L\rangle$ are orthonormal. They all lie in the physical [Hilbert space](../../../hilbert-space.md) of dimension $2^n$. Counting dimensions proves the [quantum Hamming bound](../../../quantum-error-correction.md#quantum-hamming-bound)

$$
\boxed{2^k\sum_{j=0}^t3^j\binom nj\leq2^n.}
$$

This dimension argument requires nondegeneracy. For a degenerate code, different errors can share an image, as in the [Shor code](../../../quantum-error-correction.md#shor-code), and this counting proof cannot be applied unchanged.

For a binary classical code of $M$ words, the [Hamming bound](../../../coding-theory.md#hamming-bound) is $M\sum_{j=0}^t\binom nj\leq2^n$: disjoint [Hamming balls](../../../coding-theory.md#hamming-ball) around the words must fit into all binary strings. The quantum factor $3^j$ is needed because at each erroneous [qubit](../../../quantum-mechanics.md#qubit) there are three linearly independent nonidentity [Pauli operators](../../../quantum-circuit.md#pauli-operator), not just a classical bit flip. A [phase flip](../../../quantum-theory.md#pauli-z-gate) is invisible to a computational-basis classical record but changes a quantum superposition. A $Y$ error combines bit and phase effects, and the identity with $X,Y,Z$ spans every one-qubit operator. Quantum correction must protect amplitudes and coherences, and consequently count whole orthogonal logical subspaces rather than just classical words.

For parameters $[[5,1,3]]$, $t=1$, and

$$
2^1\left(1+3\binom51\right)=2\cdot16=32=2^5.
$$

Thus a nondegenerate such code saturates the bound: the sixteen two-dimensional error images exhaust the physical space. **It is a perfect quantum error-correcting code for single-qubit errors.** It also has the smallest possible length for nondegenerate single-error protection of one logical qubit: for $1\leq n\leq4$, the required inequality $1+3n\leq2^{n-1}$ fails.

Here is an explicit realization and its [five-qubit stabilizer syndrome table](../../../quantum-error-correction.md#five-qubit-stabilizer-syndrome-table). Write tensor products without multiplication symbols and use

$$
g_1=XZZXI,\qquad g_2=IXZZX,\qquad g_3=XIXZZ,\qquad g_4=ZXIXZ.
$$

Each pair has an even number of anticommuting single-site factors, so the four [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) commute. Their binary Pauli labels are independent: no nonempty product has identity label. For example, the $X$-support at site three fixes the exponent of $g_3$ in such a product to zero, site five then fixes that of $g_2$, site one fixes that of $g_1$, and site two fixes that of $g_4$. Thus their group has sixteen elements and excludes $-I$. The common $+1$ eigenspace has projector $P=\prod_{a=1}^4(I+g_a)/16$ and dimension $\operatorname{Tr}P=32/16=2$, since all nonidentity Pauli strings have zero trace.

Record a syndrome bit as one when an error anticommutes with the corresponding generator, in order $g_1,g_2,g_3,g_4$. Direct local commutation gives

$$
\begin{array}{c|c|c|c}
\text{site}&X&Y&Z\\\hline
1&0001&1011&1010\\
2&1000&1101&0101\\
3&1100&1110&0010\\
4&0110&1111&1001\\
5&0011&0111&0100
\end{array}
$$

These are all fifteen nonzero four-bit [error syndromes](../../../quantum-error-correction.md#error-syndrome); the identity has $0000$. Distinct errors in this list have a product with nonzero syndrome, so it anticommutes with some $g_a$. Inserting $g_aP=P$ on both sides gives $PE_b^\dagger E_cP=-PE_b^\dagger E_cP=0$. The diagonal product is the identity. Hence the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) is exactly $C_{bc}=\delta_{bc}$, proving nondegenerate correction. Measure the four commuting checks, apply the unique indicated [Pauli error](../../../quantum-circuit.md#pauli-operator) again, and every logical state is recovered. The [Pauli expansion of a quantum error](../../../quantum-circuit.md#pauli-expansion-of-a-quantum-error) extends this recovery to an arbitrary one-qubit noise channel, not just the fifteen discrete errors.

The table also proves that every Pauli operator of weight one or two has nonzero syndrome: a weight-two operator is the product of distinct single-site errors, whose syndromes differ. Therefore the distance is at least three. The operators $\overline X=X^{\otimes5}$ and $\overline Z=Z^{\otimes5}$ commute with all four generators and anticommute with each other. They are nontrivial logical [Pauli operators](../../../quantum-circuit.md#pauli-operator). Multiplication of $\overline X$ by $g_1$ gives $-IYYIX$, a weight-three operator with the same logical action; it cannot be scalar on the code because it anticommutes with the invertible logical operator $\overline Z$. This proves $d=3$ exactly.

The code consequently detects every two-qubit error and corrects two known-location erasures by the [quantum erasure correction](../../../quantum-error-correction.md#quantum-erasure-correction) criterion, but it cannot correct all two-qubit errors of unknown location. A nontrivial weight-three logical operator can be split into a weight-one and a weight-two error, whose pairwise product violates the correction condition. It also saturates the [quantum Singleton bound](../../../quantum-error-correction.md#quantum-singleton-bound), since $n-k=4=2(d-1)$. These properties distinguish single-error perfectness from unrestricted protection against larger errors.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use logarithms to base two, so all entropies are in bits. For a discrete [probability distribution](../../../probability-theory.md#probability-distribution) $p$ and a [density operator](../../../quantum-theory.md#density-matrix) $\rho$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_j$, the [Shannon entropy](../../../information-theory.md#information-entropy) and [Von Neumann entropy](../../../von-neumann-entropy.md) are respectively

$$
\boxed{H(p)=-\sum_xp_x\log_2p_x,\qquad
S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)=-\sum_j\lambda_j\log_2\lambda_j.}
$$

Use $0\log0=0$. The second definition is basis-independent by the [spectral theorem](../../../hilbert-space.md#spectral-theorem); for a density operator diagonal with probabilities $p_x$, it agrees with the first.

The classical [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence), or [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence), of $p$ from $q$ is

$$
\boxed{D(p\Vert q)=\sum_{x:p_x>0}p_x\log_2\frac{p_x}{q_x}.}
$$

It is $+\infty$ if some $p_x>0$ has $q_x=0$. The [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) is

$$
\boxed{D(\rho\Vert\sigma)=\operatorname{Tr}\bigl[\rho(\log_2\rho-\log_2\sigma)\bigr]}
$$

when the support of $\rho$ is contained in that of $\sigma$, and is $+\infty$ otherwise. Matrix logarithms are taken on the corresponding positive supports. In a common eigenbasis this reduces to classical relative entropy; both divergences are nonnegative and are generally asymmetric.

To prove [Fano's inequality](../../../information-theory.md#fano-s-inequality), let the finite alphabet size be $m\geq2$ and let $E$ indicate an incorrect guess. Since $E$ is determined by $(X,Y)$, the [chain rule for conditional entropy](../../../information-theory.md#chain-rule-for-conditional-entropy) first gives

$$
H(E,X\mid Y)=H(X\mid Y)+H(E\mid X,Y)=H(X\mid Y).
$$

Expanding in the opposite order gives

$$
H(E,X\mid Y)=H(E\mid Y)+H(X\mid E,Y).
$$

[Conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy), so $H(E\mid Y)\leq H(E)=h_2(p_e)$, the [binary entropy function](../../../combinatorics.md#binary-entropy-function). When $E=0$, knowledge of $Y$ determines $X=f(Y)$ and the conditional entropy is zero. When $E=1$, $X$ can lie in at most the $m-1$ alphabet values other than $f(Y)$. Entropy on $m-1$ values is at most $\log_2(m-1)$: its deficit from that number is the nonnegative [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) from the uniform distribution. Averaging the two cases therefore gives

$$
H(X\mid E,Y)\leq p_e\log_2(m-1).
$$

Combining the two expansions proves

$$
\boxed{H(X\mid Y)\leq h_2(p_e)+p_e\log_2(m-1).}
$$

This proof of [Fano's inequality via an error indicator](../../../information-theory.md#fano-s-inequality-via-an-error-indicator) works for any alphabet-valued guessing rule, not just an optimal one. If $m=1$, there is no guessing uncertainty and the claim is simply $H(X\mid Y)=0$; that case is treated separately rather than writing $\log0$.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [measurement in quantum mechanics](../../../quantum-measurement.md) with outcomes $m$ is specified, in the single-operator-per-outcome description, by [linear operators](../../../vector-space.md#linear-operator) $M_m$ satisfying $\sum_mM_m^\dagger M_m=I$. Its effects $F_m=M_m^\dagger M_m$ form a [positive operator-valued measure](../../../quantum-measurement.md#positive-operator-valued-measure). The two measurement postulates are the [Born rule](../../../quantum-mechanics.md#born-rule) for outcomes and the conditional state update:

$$
\boxed{p_m=\langle\psi|M_m^\dagger M_m|\psi\rangle,\qquad
|\psi\rangle\longmapsto\frac{M_m|\psi\rangle}{\sqrt{p_m}}\quad(p_m>0).}
$$

For a [density operator](../../../quantum-theory.md#density-matrix) the corresponding formulas are $p_m=\operatorname{Tr}(M_m\rho M_m^\dagger)$ and $\rho_m=M_m\rho M_m^\dagger/p_m$. More general [quantum instruments](../../../quantum-measurement.md#quantum-instrument) have multiple operators for each outcome and sum these terms. For a [projective measurement](../../../quantum-measurement.md#projective-measurement) of an [observable](../../../quantum-mechanics.md#observable) $A=\sum_m a_mP_m$, take $M_m=P_m$; the outcome value is $a_m$ and the postmeasurement state lies in its eigenspace. A POVM alone specifies probabilities, whereas the measurement operators or instrument also specify the backaction.

For [quantum teleportation](../../../bell-state.md#quantum-teleportation), Alice and Bob initially share the [Bell pair](../../../bell-state.md#bell-pair) $|\Phi^+\rangle_{AB}=(|00\rangle+|11\rangle)/\sqrt2$. Alice also holds the input $|\psi\rangle_C=\alpha|0\rangle+\beta|1\rangle$, with $|\alpha|^2+|\beta|^2=1$. The shared entanglement is a resource; the two transmitted [classical bits](../../../information-theory.md#bit) alone could not transfer an arbitrary unknown quantum state.

Alice applies a [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) with $C$ as control and $A$ as target, then a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to $C$. Starting from $|\psi\rangle_C|\Phi^+\rangle_{AB}$, direct expansion gives

$$
\frac12\left(
|00\rangle_{CA}|\psi\rangle_B+
|01\rangle_{CA}X|\psi\rangle_B+
|10\rangle_{CA}Z|\psi\rangle_B+
|11\rangle_{CA}XZ|\psi\rangle_B
\right).
$$

For example, the four receiver vectors are $\alpha|0\rangle+\beta|1\rangle$, $\beta|0\rangle+\alpha|1\rangle$, $\alpha|0\rangle-\beta|1\rangle$, and $-\beta|0\rangle+\alpha|1\rangle$. Thus the gate calculation fixes the ordering of the Pauli corrections, including the last branch's sign.

Alice measures $C,A$ in the [computational basis](../../../quantum-theory.md#computational-basis), obtaining $(a,b)$. The [Born rule](../../../quantum-mechanics.md#born-rule) gives each outcome probability $1/4$, independent of the input amplitudes. Bob's normalized conditional state is $X^bZ^a|\psi\rangle$. Alice sends the two outcome bits. Bob applies the inverse, $Z^aX^b$, and hence

$$
\boxed{Z^aX^bX^bZ^a|\psi\rangle=|\psi\rangle.}
$$

The same circuit is a [Bell-basis measurement](../../../bell-state.md#bell-basis-measurement) on Alice's two qubits, expressed using ordinary gates followed by computational-basis measurements. It restores the state without Alice or Bob knowing $\alpha,\beta$.

By [linearity](../../../vector-space.md#linearity), the calculation also holds when the input is entangled with a reference: each outcome has branch map $|\psi\rangle\mapsto X^bZ^a|\psi\rangle/2$, and after correction every branch is one-half of the identity map. Summing the four corrected density operators gives exactly the original input density operator, with all reference correlations preserved. This is [teleportation as an identity channel on a reference](../../../bell-state.md#teleportation-as-an-identity-channel-on-a-reference). Without the two classical bits Bob must average the four uncorrected states, giving $\tfrac14\sum_{a,b}X^bZ^a\rho Z^aX^b=I/2$, so the process cannot signal before the message arrives. The Bell pair is consumed and Alice retains no copy of the unknown state, in accordance with the [no-cloning theorem](../../../quantum-theory.md#no-cloning-theorem).

## 5

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $U$ be a [unitary operator](../../../vector-space.md#unitary-operator) and suppose initially that the target is an [eigenstate](../../../quantum-mechanics.md#eigenstate) $|u\rangle$ with $U|u\rangle=e^{2\pi i\phi}|u\rangle$, $0\leq\phi<1$. Use $t$ control [qubits](../../../quantum-mechanics.md#qubit), so $L=2^t$. [Hadamard gates](../../../quantum-theory.md#hadamard-gate) prepare the uniform superposition $L^{-1/2}\sum_{a=0}^{L-1}|a\rangle$. For each binary control position $j$, apply the [controlled unitary gate](../../../quantum-theory.md#controlled-unitary-gate) $U^{2^j}$. The resulting state is

$$
\frac1{\sqrt L}\sum_{a=0}^{L-1}e^{2\pi ia\phi}|a\rangle|u\rangle.
$$

Apply the inverse [quantum Fourier transform](../../../quantum-theory.md#quantum-fourier-transform), with convention $\operatorname{QFT}_L|j\rangle=L^{-1/2}\sum_a e^{2\pi iaj/L}|a\rangle$, and measure the control. The exact amplitude and [probability](../../../probability-theory.md#probability) are

$$
A_j=\frac1L\sum_{a=0}^{L-1}e^{2\pi ia(\phi-j/L)},\qquad p_j=|A_j|^2.
$$

For an exactly representable phase $\phi=j_0/L$, [orthogonality of roots of unity](../../../algebra.md#orthogonality-of-roots-of-unity) makes the outcome $j_0$ certain. Otherwise the [finite geometric series](../../../real-analysis.md#finite-geometric-series) gives

$$
p_j=\frac{\sin^2(\pi L(\phi-j/L))}{L^2\sin^2(\pi(\phi-j/L))}.
$$

The estimate is $j/L$, with phases interpreted modulo one.

To prove an error bound, choose a nearest label $j_0$ to $L\phi$ on the circular grid and put $d=L\phi-j_0$ in the interval $[-1/2,1/2]$. For $d\ne0$, concavity of sine on $[0,\pi/2]$ gives $|\sin\pi d|\geq2|d|$, while $L|\sin(\pi d/L)|\leq\pi|d|$. Therefore the [nearest-integer success bound for quantum phase estimation](../../../quantum-theory.md#nearest-integer-success-bound-for-quantum-phase-estimation) is

$$
\boxed{\Pr\left(\left\|\frac JL-\phi\right\|_{\mathbb R/\mathbb Z}\leq\frac1{2L}\right)\geq\frac4{\pi^2}.}
$$

Here $\|x\|_{\mathbb R/\mathbb Z}=\min_{k\in\mathbb Z}|x-k|$. At an exact grid point the probability is one. If two nearest labels tie, either one separately has the displayed lower bound.

For high confidence one can prove a stronger [quantum phase estimation tail bound](../../../quantum-theory.md#quantum-phase-estimation-tail-bound). Let $d_j$ be the centered distance between $j$ and $L\phi$, chosen with $|d_j|\leq L/2$. The denominator estimate $|\sin(\pi d_j/L)|\geq2|d_j|/L$ implies $p_j\leq1/(4d_j^2)$ away from the exact-phase case. A label at circular integer distance $\ell$ from $j_0$ has $|d_j|\geq\ell-1/2$, and there are at most two labels at each such distance. For $m\geq2$, summing the tails gives

$$
\Pr\bigl(\operatorname{dist}(J,j_0)\geq m\bigr)
\leq\frac12\sum_{\ell=m}^\infty\frac1{(\ell-1/2)^2}
\leq\frac12\sum_{\ell=m}^\infty\frac1{\ell(\ell-1)}
=\frac1{2(m-1)}.
$$

On the complementary event the circular phase error is at most $(m-1/2)/L$. Thus, for $b$ desired bits of accuracy, take $t=b+u$ with $u\geq1$ and $m=2^u$ to obtain

$$
\boxed{\Pr\left(\left\|\frac JL-\phi\right\|_{\mathbb R/\mathbb Z}\geq2^{-b}\right)
\leq\frac1{2(2^u-1)}.}
$$

Taking $u=\lceil\log_2(1+1/(2\varepsilon))\rceil$ makes the right side at most $\varepsilon$. This adds only $O(\log(1/\varepsilon))$ control qubits. Efficient QFT is not by itself a guarantee of efficient controlled powers of an arbitrary $U$: implementing them by repeated oracle calls uses $L-1$ calls. The modular-arithmetic application has efficient powers, as follows.

Assume $n>1$ and $\gcd(x,n)=1$, and let $r$ be the [multiplicative order](../../../number-theory.md#multiplicative-order) of $x$ modulo $n$. Define the [unitary operator](../../../vector-space.md#unitary-operator) $U_x|y\rangle=|xy\bmod n\rangle$ on $0\leq y<n$, and extend it as the identity on unused computational-basis labels of the binary register. Coprimality makes multiplication a permutation, so this extension really is unitary. The orbit of $|1\rangle$ consists of the $r$ distinct states $|x^j\bmod n\rangle$. Its [modular multiplication eigenstates](../../../quantum-theory.md#modular-multiplication-eigenstates) are

$$
|u_s\rangle=\frac1{\sqrt r}\sum_{j=0}^{r-1}e^{-2\pi isj/r}|x^j\bmod n\rangle,
\qquad U_x|u_s\rangle=e^{2\pi is/r}|u_s\rangle,
\quad 0\leq s<r.
$$

The last relation follows by shifting the index $j$ cyclically; orthogonality follows from the finite Fourier sum. We do not need to know $r$ to prepare one of these eigenstates: the readily prepared target obeys

$$
|1\rangle=\frac1{\sqrt r}\sum_{s=0}^{r-1}|u_s\rangle.
$$

Running [quantum phase estimation](../../../quantum-theory.md#quantum-phase-estimation) on this state produces the mixture of the $r$ eigenphase distributions, each with weight $1/r$, because the target eigenstates are orthogonal. Thus it samples a uniformly random phase label $s$ and estimates $s/r$ with the bounds just proved. Equivalently the state before the inverse QFT is $L^{-1/2}\sum_a|a\rangle|x^a\bmod n\rangle$, which is obtained by [quantum modular exponentiation](../../../quantum-theory.md#quantum-modular-exponentiation) directly.

The controlled power $U_x^{2^j}$ multiplies by $x^{2^j}\bmod n$, whose constant is computed by [repeated squaring](../../../number-theory.md#exponentiation-by-squaring). Under the assumed efficient modular exponentiation, these controlled multiplications and the QFT use a number of gates polynomial in the register lengths. Taking $L>n^2$ requires only $O(\log n)$ phase qubits. The nearest-label event has probability at least $4/\pi^2$ and yields an estimate within $1/(2L)<1/(2r^2)$ of $s/r$. Since $r<n$, [continued-fraction recovery in quantum order finding](../../../quantum-theory.md#continued-fraction-recovery-in-quantum-order-finding) then identifies the reduced fraction $s/r$. The denominator is $r/\gcd(s,r)$, not necessarily $r$: when $s$ and $r$ are coprime it is the desired order, and when they are not it is only a divisor. One may test candidate denominators using modular exponentiation and repeat with fresh samples; denominators from successful samples can also be combined by a least common multiple. The probability of a nearest-label sample with $s$ coprime to $r$ is at least $(4/\pi^2)\varphi(r)/r$. These qualifications explain exactly what the phase estimate yields without falsely assuming that the unknown order or an eigenstate was available at the start.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
