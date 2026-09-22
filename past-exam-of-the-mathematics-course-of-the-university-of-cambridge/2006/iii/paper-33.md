# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper33.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
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
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
    - [1](#5/a/1)
      - [Solution](#5/a/1/solution)
    - [2](#5/a/2)
      - [Solution](#5/a/2/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Bloch vector](../../../quantum-theory.md#bloch-vector) representation of a [qubit](../../../quantum-mechanics.md#qubit) [density matrix](../../../quantum-theory.md#density-matrix) is $\rho=\frac12(I+r_xX+r_yY+r_zZ)$, where $r_j=\operatorname{Tr}(\rho\sigma_j)$ and $|\boldsymbol r|\le1$. Pure states have $|\boldsymbol r|=1$, while the origin represents the [maximally mixed state](../../../quantum-theory.md#maximally-mixed-state) $I/2$, not a [pure state](../../../quantum-theory.md#pure-state).

For the two preparations, direct evaluation of the [Pauli matrices](../../../algebra.md#pauli-matrices) gives

$$
\boxed{\boldsymbol r_1=(0,0,1),\qquad\boldsymbol r_2=(-\sqrt3/2,0,-1/2).}
$$

Their dot product is $-1/2$, so their [Bloch vectors](../../../quantum-theory.md#bloch-vector) meet at angle $\boxed{2\pi/3}$, or $120$ degrees. This is the angle between Bloch vectors; the angle determined by the modulus of the Hilbert-space overlap is different.

Completeness of the [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) requires $E_3=I-E_1-E_2$. In the [computational basis](../../../quantum-theory.md#computational-basis), subtraction gives

$$
E_3=\begin{pmatrix}\frac12&-\frac{\sqrt3}{6}\\-\frac{\sqrt3}{6}&\frac16\end{pmatrix}=\frac23|\phi_3\rangle\langle\phi_3|,\qquad\boxed{|\phi_3\rangle=\frac{\sqrt3}{2}|0\rangle-\frac12|1\rangle.}
$$

An overall phase of $\phi_3$ is immaterial. The matrix has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $2/3$ and zero, so it is positive; together with $E_1,E_2$ it is a valid [trine qubit POVM](../../../quantum-measurement.md#trine-qubit-povm).

The [Born rule](../../../quantum-mechanics.md#born-rule) gives $\Pr(j\mid\rho_i)=\operatorname{Tr}(E_j\rho_i)=\frac23|\langle\phi_j|\psi_i\rangle|^2$. The conditional probabilities are

$$
\begin{array}{c|ccc}&j=1&j=2&j=3\\\hline\rho_1&0&1/2&1/2\\\rho_2&1/2&0&1/2\end{array}.
$$

Outcome one identifies $\rho_2$, since $\phi_1$ is orthogonal to $\psi_1$; outcome two identifies $\rho_1$, since $\phi_2$ is orthogonal to $\psi_2$. Outcome three is inconclusive. If Alice's prior probability for $\rho_1$ is $q$, the unconditional outcome probabilities are $(1-q)/2$, $q/2$, and $1/2$ respectively. Because outcome three has the same likelihood for both preparations, it leaves the prior odds unchanged. **Bob's conclusive identification succeeds with probability one half and is never wrong; he does not identify the state on the inconclusive trials.** This is [unambiguous quantum state discrimination](../../../quantum-theory.md#unambiguous-quantum-state-discrimination).

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [linear map](../../../vector-space.md#linear-map) $\Phi$ is a [completely positive map](../../../quantum-information-theory.md#completely-positive-map) if $\operatorname{id}_R\otimes\Phi$ sends every [positive operator](../../../hilbert-space.md#positive-operator) to a [positive operator](../../../hilbert-space.md#positive-operator) for every finite-dimensional auxiliary system $R$. Positivity of $\Phi$ alone tests only inputs without an auxiliary system and is weaker.

For the [Kraus representation](../../../quantum-information-theory.md#kraus-representation), let $\Omega\ge0$ be any operator on the auxiliary system and the input system. Then

$$
(\operatorname{id}_R\otimes\Phi)(\Omega)=\sum_k(I_R\otimes A_k)\Omega(I_R\otimes A_k^\dagger).
$$

For any vector $v$, its expectation is $\sum_k\langle(I_R\otimes A_k^\dagger)v,\Omega(I_R\otimes A_k^\dagger)v\rangle\ge0$. Every amplification is therefore positive, proving **the Kraus-form map is completely positive**. No normalization condition on the $A_k$ is needed for this positivity proof. To make it a deterministic [quantum channel](../../../quantum-information-theory.md#quantum-channel), one additionally requires $\sum_kA_k^\dagger A_k=I$; a physical outcome branch instead obeys $\sum_kA_k^\dagger A_k\le I$.

Transposition is positive on one system: for any positive $\rho$ and any $v$, $v^\dagger\rho^Tv$ is the complex conjugate of $\bar v^\dagger\rho\bar v$, hence is real and nonnegative. It fails complete positivity already for a [qubit](../../../quantum-mechanics.md#qubit). Apply partial transposition to the second subsystem of the [Bell state](../../../bell-state.md) $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$. The resulting operator is

$$
(\operatorname{id}\otimes T)(|\Phi^+\rangle\langle\Phi^+|)=\frac12\bigl(|00\rangle\langle00|+|01\rangle\langle10|+|10\rangle\langle01|+|11\rangle\langle11|\bigr).
$$

On the antisymmetric vector $(|01\rangle-|10\rangle)/\sqrt2$, its eigenvalue is $-1/2$. Thus the [partial transpose](../../../quantum-information-theory.md#partial-transpose) is not positive on this entangled input, and

$$
\boxed{T\text{ is positive but not completely positive in dimension at least two}.}
$$

The same witness embeds into any larger input dimension; in the exceptional one-dimensional case transposition is simply the identity.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Choose $|0\rangle$ as the ground state and $|1\rangle$ as the excited state. The relevant [quantum channel](../../../quantum-information-theory.md#quantum-channel) is the [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel). Its [Kraus operators](../../../quantum-information-theory.md#kraus-operator) are

$$
\boxed{K_0=\begin{pmatrix}1&0\\0&\sqrt{1-p}\end{pmatrix},\qquad K_1=\begin{pmatrix}0&\sqrt p\\0&0\end{pmatrix}=\sqrt p\,|0\rangle\langle1|.}
$$

They satisfy $K_0^\dagger K_0+K_1^\dagger K_1=I$. The $K_0$ branch corresponds to no emitted photon: the ground-state amplitude is unchanged and the excited-state amplitude is attenuated. The $K_1$ branch corresponds to photon emission and transition to the ground state. These are unnormalized branch states; the squared norm or [matrix trace](../../../linear-algebra.md#matrix-trace) of each branch gives its probability.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Model the environment's vacuum and one-photon states by $|0_E\rangle,|1_E\rangle$. A [unitary dilation of amplitude damping](../../../quantum-information-theory.md#unitary-dilation-of-amplitude-damping) acts on the initially vacant environment as

$$
U|0,0_E\rangle=|0,0_E\rangle,\qquad U|1,0_E\rangle=\sqrt{1-p}|1,0_E\rangle+\sqrt p|0,1_E\rangle.
$$

These images are orthonormal. One unitary completion takes $U|0,1_E\rangle=-\sqrt p|1,0_E\rangle+\sqrt{1-p}|0,1_E\rangle$ and fixes $|1,1_E\rangle$. Taking environment matrix elements $\langle k_E|U|0_E\rangle$ gives $K_0,K_1$.

Evolve $\rho\otimes|0_E\rangle\langle0_E|$ by $U$ and take the [partial trace](../../../quantum-theory.md#partial-trace) over the environment. Orthogonality of the two environment records removes the cross-branch terms, giving $\mathcal A_p(\rho)=K_0\rho K_0^\dagger+K_1\rho K_1^\dagger$. Entrywise,

$$
\boxed{\mathcal A_p(\rho)=\begin{pmatrix}\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}\end{pmatrix}.}
$$

Excited population is transferred to the ground state, while coherence is reduced by the square root of the survival probability.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Successive uses of the same [quantum channel](../../../quantum-information-theory.md#quantum-channel) mean coupling to a fresh vacuum environment each time, or resetting the environment between uses. They do not mean repeatedly applying the dilation unitary to one unreinitialized two-state environment. Direct composition gives

$$
\mathcal A_p^2(\rho)=\begin{pmatrix}\rho_{00}+(2p-p^2)\rho_{11}&(1-p)\rho_{01}\\(1-p)\rho_{10}&(1-p)^2\rho_{11}\end{pmatrix}.
$$

Inductively, with $q_n=1-(1-p)^n$,

$$
\boxed{\mathcal A_p^n(\rho)=\begin{pmatrix}\rho_{00}+q_n\rho_{11}&(1-p)^{n/2}\rho_{01}\\(1-p)^{n/2}\rho_{10}&(1-p)^n\rho_{11}\end{pmatrix}.}
$$

For $0<p\le1$, this tends to the pure ground state $|0\rangle\langle0|$, whose [Von Neumann entropy](../../../von-neumann-entropy.md) is zero. For $p=0$, the channel is the identity: the state remains $\rho$ and its [Von Neumann entropy](../../../von-neumann-entropy.md) remains $S(\rho)$. Thus the [repeated amplitude damping limit](../../../quantum-information-theory.md#repeated-amplitude-damping-limit) must include this no-decay exception.

A zero-[Von Neumann entropy](../../../von-neumann-entropy.md) output means there is no uncertainty about the final atomic state. It does not mean that the receiver has gained information about the initial preparation: all initial states have the same limiting output, so their distinguishability has been erased from the atom. Under the global unitary evolution, information is carried into the environment. Without observing an emission record, this is a nonselective dissipative process, not an inference about which input was sent. Indeed, starting from the excited [pure state](../../../quantum-theory.md#pure-state), one intermediate output has [Von Neumann entropy](../../../von-neumann-entropy.md) equal to the [binary entropy](../../../information-theory.md#binary-entropy) of $p$, which is positive for $0<p<1$; the atom's [Von Neumann entropy](../../../von-neumann-entropy.md) need not decrease monotonically during the approach to the final ground state.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

A [unital quantum channel](../../../quantum-information-theory.md#unital-quantum-channel) preserves the identity operator: $\Phi(I)=I$. In equal input and output dimensions, it therefore preserves the [maximally mixed state](../../../quantum-theory.md#maximally-mixed-state). For [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel),

$$
\mathcal A_p(I)=K_0K_0^\dagger+K_1K_1^\dagger=\begin{pmatrix}1+p&0\\0&1-p\end{pmatrix}=I+pZ.
$$

Hence **the channel is not unital for $p>0$; it is unital only in the identity case $p=0$**. Trace preservation involves the opposite products $K_i^\dagger K_i$ and does not imply unitality.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $e_j$ be the bit string with one in position $j$ and zero elsewhere, and use the standard convention $Y=iXZ$. On the [computational basis](../../../quantum-theory.md#computational-basis), the single-site [Pauli operators](../../../quantum-circuit.md#pauli-operator) act as

$$
\boxed{X_j|x\rangle=|x\mathbin{\oplus}e_j\rangle,\quad Z_j|x\rangle=(-1)^{x_j}|x\rangle,\quad Y_j|x\rangle=i(-1)^{x_j}|x\mathbin{\oplus}e_j\rangle.}
$$

The identity leaves the basis state unchanged. A tensor-product [Pauli operator](../../../quantum-circuit.md#pauli-operator) applies these actions at each occupied site; operators at different sites commute. Their linear span is the full operator algebra, so correcting their span handles coherent combinations as well as random Pauli errors.

Let $P$ project onto the code $\mathcal C$, with orthonormal logical basis $|i_L\rangle$. A set $\mathcal E=\{E_a\}$ is correctable exactly when the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) holds:

$$
\boxed{PE_a^\dagger E_bP=C_{ab}P,\quad\text{equivalently }\langle i_L|E_a^\dagger E_b|j_L\rangle=C_{ab}\delta_{ij},}
$$

for a matrix $C$ independent of the logical indices. A set $\mathcal D$ is detectable when

$$
\boxed{PDP=c_DP\quad\text{for every }D\in\mathcal D.}
$$

These conditions extend by linearity to the corresponding operator spans. Detection allows an error to act as a harmless scalar on the code; it need not assign a distinct syndrome to such an error.

For distinct Pauli representatives modulo phase, a [nondegenerate quantum error-correcting code](../../../quantum-error-correction.md#nondegenerate-quantum-error-correcting-code) has orthogonal error-image subspaces, giving $C_{ab}=\delta_{ab}$ because each Pauli is unitary. In the usual nondegenerate, or pure, detection convention, every nonidentity detectable Pauli has $PDP=0$, while $PIP=P$. More generally a nonsingular error-overlap matrix can be diagonalized and the resulting error operators rescaled to obtain orthogonal syndrome spaces; a singular overlap matrix expresses degeneracy of the specified independent error family.

For an $[[n,k,d]]$ code, the [quantum code distance](../../../quantum-error-correction.md#distance-of-a-quantum-error-correcting-code) is the smallest [Pauli weight](../../../quantum-circuit.md#weight-of-a-pauli-operator) for which scalar compression fails. Hence every Pauli of weight at most $d-1$ is detectable. If $E_a,E_b$ each have weight at most $t$, their product $E_a^\dagger E_b$ has weight at most $2t$. When $2t<d$, its compression is scalar, so the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition) proves simultaneous correction of all such errors. Therefore

$$
\boxed{\text{detectable weight: }d-1,\qquad\text{correctable unknown-location weight: }\left\lfloor\frac{d-1}{2}\right\rfloor.}
$$

The integer part is understood when the printed half-distance is not an integer. Arbitrary operators on such subsets are covered by their Pauli expansion.

For errors confined to a known set of $m$ positions, every pairwise product is still supported on that same set and has weight at most $m$, rather than $2m$. Thus $m<d$ supplies [quantum erasure correction](../../../quantum-error-correction.md#quantum-erasure-correction), with maximum guaranteed number

$$
\boxed{m=d-1.}
$$

This guarantee cannot hold for every set of $d$ positions: a minimum-weight undetectable Pauli has support in such a set, and the pair consisting of it and the identity violates the [Knill--Laflamme condition](../../../quantum-error-correction.md#knill-laflamme-condition). Particular larger location sets can sometimes be correctable; $d-1$ is the maximum uniform guarantee over all possible known sets.

For the [Shor code](../../../quantum-error-correction.md#shor-code), write $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. The logical codewords are $|G_+\rangle^{\otimes3}$ and $|G_-\rangle^{\otimes3}$. A [phase flip](../../../quantum-theory.md#pauli-z-gate) $Z_j$ in one block interchanges $G_+$ and $G_-$ in that block, independently of its position within the block. Let $B_1=X_1X_2X_3$, $B_2=X_4X_5X_6$, $B_3=X_7X_8X_9$. Measure the two commuting [stabilizer generators](../../../quantum-circuit.md#stabilizer-generator) $S_1=B_1B_2$ and $S_2=B_2B_3$. Both are $+1$ on the entire logical code space. The [Shor-code phase-flip syndrome](../../../quantum-error-correction.md#shor-code-phase-flip-syndrome) is

$$
\begin{array}{c|cc|c}\text{affected block}&S_1&S_2&\text{correction}\\\hline\text{none}&+1&+1&I\\1&-1&+1&Z_1\\2&-1&-1&Z_4\\3&+1&-1&Z_7\end{array}.
$$

These parity measurements reveal the erroneous block without revealing the logical amplitudes, so they preserve arbitrary superpositions of the two codewords. Applying the listed representative phase flip restores the state.

For any two physical positions $i,j$ in the same block, $Z_iZ_j$ acts as $+1$ on both $|000\rangle$ and $|111\rangle$, and hence on the code. Therefore $Z_iP=Z_jP$ and $PZ_i^\dagger Z_jP=P$ even when $i\ne j$. Their error spaces coincide, and the error-overlap matrix has a nonzero off-diagonal entry. **The correction is degenerate because different within-block phase errors have exactly the same action on every logical state.**

## 5

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Use base-two logarithms, so the [Von Neumann entropy](../../../von-neumann-entropy.md) is $S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)$, with $0\log0=0$. The [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) is $I(A:B)=S(A)+S(B)-S(AB)$; this is the quantity denoted by $S(\rho_A:\rho_B)$ in the question, using the given joint state.

[Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy) states that for every tripartite [density operator](../../../quantum-theory.md#density-matrix),

$$
\boxed{S(AB)+S(BC)\ge S(B)+S(ABC).}
$$

Equivalently the conditional [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) $I(A:C\mid B)$ is nonnegative. We apply this property to the original state or to a dilation of the relevant [quantum channel](../../../quantum-information-theory.md#quantum-channel).

<h4 id="5/a/1">1</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/1/solution">Solution</h5>

↑ **Parent:** [1](#5/a/1)

Expand the difference between the two [quantum mutual informations](../../../von-neumann-entropy.md#quantum-mutual-information):

$$
I(A:BC)-I(A:B)=S(BC)-S(ABC)-S(B)+S(AB).
$$

This is precisely the nonnegative expression in [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy). Thus

$$
\boxed{I(A:B)\le I(A:BC).}
$$

The reduced state on $AB$ is obtained by the [partial trace](../../../quantum-theory.md#partial-trace) over $C$, so this proves that discarding a system cannot increase its [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) with the retained reference.

<h4 id="5/a/2">2</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/2/solution">Solution</h5>

↑ **Parent:** [2](#5/a/2)

Here a quantum operation is interpreted as a deterministic [quantum channel](../../../quantum-information-theory.md#quantum-channel), so it is completely positive and [matrix trace](../../../linear-algebra.md#matrix-trace) preserving. Write its [Kraus representation](../../../quantum-information-theory.md#kraus-representation) with $\sum_kA_k^\dagger A_k=I$ and define the [isometry](../../../riemannian-geometry.md#isometry) in its [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation)

$$
V|\psi\rangle=\sum_kA_k|\psi\rangle\otimes|k\rangle_E.
$$

Then $V^\dagger V=I$ and $\Phi(\rho)=\operatorname{Tr}_E(V\rho V^\dagger)$. Acting on $B$ gives $\sigma_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger)$. An [isometry](../../../riemannian-geometry.md#isometry) preserves the nonzero [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of a [density operator](../../../quantum-theory.md#density-matrix). Hence $S(AB'E)=S(AB)$, $S(B'E)=S(B)$, and $S(A)$ is unchanged. It follows that $I(A:B'E)_\sigma=I(A:B)_\rho$.

Now discard $E$ and apply part 1. This proves [data processing for quantum mutual information](../../../von-neumann-entropy.md#data-processing-for-quantum-mutual-information):

$$
\boxed{I(A:B')\le I(A:B'E)=I(A:B).}
$$

The [matrix trace](../../../linear-algebra.md#matrix-trace)-preserving convention matters. [Postselection can increase conditional quantum mutual information](../../../von-neumann-entropy.md#postselection-can-increase-conditional-quantum-mutual-information): take a uniform classical bit $A$, copy it to $B$ with probability $\varepsilon$, and otherwise put $B$ in an erasure state independent of $A$. Initially $I(A:B)=\varepsilon$ bits. Projecting onto the nonerased sector and conditioning on success gives a perfectly correlated bit pair with [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) one. That success branch is [matrix trace](../../../linear-algebra.md#matrix-trace) decreasing, and its renormalized action is not a deterministic channel. Retaining the full outcome flag and averaging all branches restores the ordinary channel inequality.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $A$ be a register with [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $\{|x\rangle\}$ for Alice's classical symbol, $Q$ the transmitted system, and $B$ a register initially in a fixed blank state. The initial [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state) is

$$
\boxed{\rho_{AQB}=\sum_xp(x)|x\rangle\langle x|_A\otimes\rho_x\otimes|0\rangle\langle0|_B.}
$$

A [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) fixes probabilities but not a unique conditional state of $Q$. Choose the [Lüders rule](../../../quantum-measurement.md#luders-rule) instrument $M_y=\sqrt{E_y}$, which satisfies $\sum_yM_y^\dagger M_y=I$. Record outcome $y$ in orthogonal states of $B'$ and retain the corresponding quantum output $Q'$. The final nonselective state is

$$
\boxed{\rho_{A'Q'B'}=\sum_{x,y}p(x)|x\rangle\langle x|_{A'}\otimes M_y\rho_xM_y^\dagger\otimes|y\rangle\langle y|_{B'}.}
$$

The positive operators in this sum are unnormalized: their traces already include the outcome probabilities. If $\operatorname{Tr}(E_y\rho_x)>0$, the normalized conditional state of $Q'$ is $M_y\rho_xM_y^\dagger/\operatorname{Tr}(E_y\rho_x)$.

More generally, an instrument may use operators $M_{y\mu}$ with $\sum_\mu M_{y\mu}^\dagger M_{y\mu}=E_y$, replacing $M_y\rho_xM_y^\dagger$ by $\sum_\mu M_{y\mu}\rho_xM_{y\mu}^\dagger$. All subsequent classical information bounds are unchanged. This explicitly accounts for the fact that a [POVM does not determine the post-measurement state](../../../quantum-measurement.md#povm-does-not-determine-the-post-measurement-state) of a retained quantum system.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

The initially blank register $B$ is pure and independent, so adding it changes neither relevant [Von Neumann entropy](../../../von-neumann-entropy.md) difference: $I(A:QB)=I(A:Q)$. Bob's measurement and recording procedure, with all outcomes retained, is a [matrix trace](../../../linear-algebra.md#matrix-trace)-preserving [quantum channel](../../../quantum-information-theory.md#quantum-channel) from $QB$ to $Q'B'$. Part (a) therefore gives $I(A':Q'B')\le I(A:QB)$. Discarding $Q'$ gives $I(A':B')\le I(A':Q'B')$. Combining the two inequalities proves

$$
\boxed{I(A':B')\le I(A:Q).}
$$

Alice's register is not changed by Bob's local operation; the primes label its place in the final joint state rather than a change in its classical symbol.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

Trace out $Q'$ in the final state. With $q(x,y)=p(x)\operatorname{Tr}(E_y\rho_x)$, the remaining state is diagonal in the product classical basis:

$$
\rho_{A'B'}=\sum_{x,y}q(x,y)|x\rangle\langle x|\otimes|y\rangle\langle y|.
$$

The [Von Neumann entropy](../../../von-neumann-entropy.md) of a classical diagonal [density operator](../../../quantum-theory.md#density-matrix) equals the [Shannon entropy](../../../information-theory.md#information-entropy) of its diagonal probabilities, by its spectrum. Therefore $I(A':B')=H(X)+H(Y)-H(X,Y)=I(X:Y)$, the [mutual information](../../../information-theory.md#mutual-information) between source symbol and measurement outcome.

For the input, put $\bar\rho=\sum_xp(x)\rho_x$. The marginal on $Q$ is $\bar\rho$, the marginal on $A$ has [Von Neumann entropy](../../../von-neumann-entropy.md) $H(X)$, and the [entropy of a classical-quantum state](../../../quantum-information-theory.md#entropy-of-a-classical-quantum-state) is

$$
S(AQ)=H(X)+\sum_xp(x)S(\rho_x).
$$

To justify the last formula, diagonalize each $\rho_x$ with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\lambda_{xj}$. The joint block-diagonal state has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $p(x)\lambda_{xj}$; expanding $-\sum_{x,j}p(x)\lambda_{xj}\log_2[p(x)\lambda_{xj}]$ yields exactly the displayed [Von Neumann entropy](../../../von-neumann-entropy.md). Thus $I(A:Q)=S(\bar\rho)-\sum_xp(x)S(\rho_x)$, the [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) of the ensemble. Part (ii) becomes the [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem)

$$
\boxed{I(X:Y)\le\chi=S\!\left(\sum_xp(x)\rho_x\right)-\sum_xp(x)S(\rho_x).}
$$

It holds for every POVM, and hence also for the accessible information obtained by maximizing the [mutual information](../../../information-theory.md#mutual-information) over all measurements. The only extra [Von Neumann entropy](../../../von-neumann-entropy.md) identities used were the classical-diagonal and classical–quantum block-spectrum formulas, both justified above; the information inequality itself followed from the requested strong-subadditivity argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
