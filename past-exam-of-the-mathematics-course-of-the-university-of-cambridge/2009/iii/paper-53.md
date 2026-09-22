# Paper 53

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper53.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper53.pdf)

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
  - [A](#4/a)
    - [1](#4/a/1)
      - [Solution](#4/a/1/solution)
    - [2](#4/a/2)
      - [Solution](#4/a/2/solution)
    - [3](#4/a/3)
      - [Solution](#4/a/3/solution)
    - [4](#4/a/4)
      - [Solution](#4/a/4/solution)
    - [5](#4/a/5)
      - [Solution](#4/a/5/solution)
  - [B](#4/b)
    - [Protocol 1](#4/b/protocol-1)
      - [Solution](#4/b/protocol-1/solution)
    - [Protocol 2](#4/b/protocol-2)
      - [Solution](#4/b/protocol-2/solution)
    - [Protocol 3](#4/b/protocol-3)
      - [Solution](#4/b/protocol-3/solution)

## 1

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Take the vectors in the [quantum state ensemble](../../../quantum-theory.md#quantum-state-ensemble) to be normalized, with $p_i\geq0$ and $\sum_i p_i=1$. The corresponding [density matrix](../../../quantum-theory.md#density-matrix) is

$$
\boxed{\rho=\sum_i p_i|\psi_i\rangle\langle\psi_i|.}
$$

Each rank-one projector is a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator), so $\rho^\dagger=\rho$. For every $|v\rangle$ in the [Hilbert space](../../../hilbert-space.md),

$$
\langle v|\rho|v\rangle=\sum_i p_i|\langle\psi_i|v\rangle|^2\geq0,
$$

proving that $\rho$ is [positive semidefinite](../../../linear-algebra.md#positive-semidefinite-matrix). The [trace](../../../linear-algebra.md#matrix-trace) is $\operatorname{Tr}\rho=\sum_i p_i\langle\psi_i|\psi_i\rangle=1$.

Conversely, diagonalize a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) $\rho$ in an [orthonormal eigenbasis](../../../linear-operator-theory.md#orthonormal-eigenbasis), writing $\rho=\sum_j\lambda_j|e_j\rangle\langle e_j|$. Its [positive semidefiniteness](../../../linear-algebra.md#positive-semidefinite-matrix) implies $\lambda_j=\langle e_j|\rho|e_j\rangle\geq0$, and its unit [trace](../../../linear-algebra.md#matrix-trace) gives $\sum_j\lambda_j=1$. Thus $\{\lambda_j,|e_j\rangle\}$ is a [quantum state ensemble](../../../quantum-theory.md#quantum-state-ensemble) with precisely this [density matrix](../../../quantum-theory.md#density-matrix). Terms with zero [eigenvalue](../../../linear-operator-theory.md#eigenvalue) may be omitted. This argument includes rank-one [pure states](../../../quantum-theory.md#pure-state); an ensemble representation need not describe a genuinely [mixed state](../../../quantum-theory.md#mixed-state).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The stated condition is the definition of an [extreme point](../../../mathematical-optimization.md#extreme-point) in the convex set of [density matrices](../../../quantum-theory.md#density-matrix). Suppose first that $\rho=|\psi\rangle\langle\psi|$ with $\|\psi\|=1$, and consider any [convex combination](../../../mathematical-optimization.md#convex-combination) $\rho=\sum_i a_i\rho_i$ with all $a_i>0$. For every $|w\rangle$ [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to $|\psi\rangle$,

$$
0=\langle w|\rho|w\rangle=\sum_i a_i\langle w|\rho_i|w\rangle.
$$

Every term is nonnegative, so $\langle w|\rho_i|w\rangle=0$ for each $i$. To see that this implies $\rho_iw=0$, expand $\rho_i=\sum_j\mu_j|u_j\rangle\langle u_j|$, $\mu_j\geq0$. The equality $\sum_j\mu_j|\langle u_j|w\rangle|^2=0$ implies $\mu_j\langle u_j|w\rangle=0$ for every $j$, which kills $\rho_iw$. Thus each [density matrix](../../../quantum-theory.md#density-matrix) $\rho_i$ vanishes on $\psi^\perp$. By self-adjointness its range lies in the line $\mathbb C\psi$, so $\rho_i=c_i|\psi\rangle\langle\psi|$. Its unit [trace](../../../linear-algebra.md#matrix-trace) forces $c_i=1$, establishing the required purity.

Conversely, suppose $\rho$ is not rank one. In its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition), at least two [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are positive. Select a normalized eigenvector $|e_1\rangle$ with positive [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\lambda_1$; then $0<\lambda_1<1$. Define

$$
\sigma=\frac{\rho-\lambda_1|e_1\rangle\langle e_1|}{1-\lambda_1}.
$$

The remaining [eigenvalues](../../../linear-operator-theory.md#eigenvalue) show that $\sigma$ is a [density matrix](../../../quantum-theory.md#density-matrix). The decomposition $\rho=\lambda_1|e_1\rangle\langle e_1|+(1-\lambda_1)\sigma$ is a [convex combination](../../../mathematical-optimization.md#convex-combination) of two different [density matrices](../../../quantum-theory.md#density-matrix), neither equal to $\rho$. This violates the given purity condition. Hence the [extreme points of the density-operator state space](../../../quantum-theory.md#extreme-points-of-the-density-operator-state-space) obey

$$
\boxed{\rho\text{ is pure}\iff\rho=|\psi\rangle\langle\psi|\text{ for a normalized }|\psi\rangle.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $R=|\psi\rangle\langle\psi|$ and choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $\{|e_\mu\rangle\}$ of $\mathcal H_2$. The [reduced density matrix](../../../bell-state.md#reduced-density-matrix) on $S_1$ is the [partial trace](../../../quantum-theory.md#partial-trace)

$$
\boxed{\rho_1=\operatorname{Tr}_2R=\sum_\mu(I_1\otimes\langle e_\mu|)R(I_1\otimes|e_\mu\rangle).}
$$

Here $I_1$ is the identity on $\mathcal H_1$, and the bras and kets in the sum contract only the second tensor factor. Equivalently, if $|\psi\rangle=\sum_{a,\mu}c_{a\mu}|f_a\rangle\otimes|e_\mu\rangle$, then $(\rho_1)_{ab}=\sum_\mu c_{a\mu}c_{b\mu}^*$. The definition is independent of the chosen basis: it is characterized by $\operatorname{Tr}(M\rho_1)=\operatorname{Tr}[(M\otimes I_2)R]$ for every operator $M$ on $\mathcal H_1$.

The [generalized measurement postulate](../../../quantum-measurement.md#generalized-measurement-postulate) takes $A_i$ to be operators on $\mathcal H_2$ satisfying $\sum_iA_i^\dagger A_i=I_2$. The [Born rule](../../../quantum-mechanics.md#born-rule) and the conditional state update give

$$
\boxed{p_i=\langle\psi|I_1\otimes A_i^\dagger A_i|\psi\rangle,\qquad |\psi_i\rangle=\frac{(I_1\otimes A_i)|\psi\rangle}{\sqrt{p_i}}\quad(p_i>0).}
$$

If the outcome is not supplied to $S_1$, the appropriate post-measurement [density matrix](../../../quantum-theory.md#density-matrix) is $R'=\sum_i(I_1\otimes A_i)R(I_1\otimes A_i^\dagger)$. For any local operator $M$, cyclicity of the full [trace](../../../linear-algebra.md#matrix-trace) gives

$$
\begin{aligned}
\operatorname{Tr}[(M\otimes I_2)R']
&=\sum_i\operatorname{Tr}[(M\otimes A_i^\dagger A_i)R]\\
&=\operatorname{Tr}[(M\otimes I_2)R].
\end{aligned}
$$

Since this holds for every $M$, $\boxed{\operatorname{Tr}_2R'=\rho_1}$. This is the [no-communication theorem](../../../bell-state.md#no-communication-theorem).

The invariance concerns the nonselective [measurement in quantum mechanics](../../../quantum-measurement.md). A conditional [reduced density matrix](../../../bell-state.md#reduced-density-matrix) $\rho_{1|i}=\operatorname{Tr}_2|\psi_i\rangle\langle\psi_i|$ can change, although $\sum_i p_i\rho_{1|i}=\rho_1$. For example, measuring one half of a [Bell pair](../../../bell-state.md#bell-pair) in the [computational basis](../../../quantum-theory.md#computational-basis) changes the other half conditionally to $|0\rangle$ or $|1\rangle$; before learning the outcome, its [density matrix](../../../quantum-theory.md#density-matrix) remains $I/2$. Thus distant [measurement in quantum measurements](../../../quantum-measurement.md) cannot transmit a controllable signal without classical communication. This [quantum no-signalling](../../../quantum-theory.md#quantum-no-signalling) is compatible with [special relativity](../../../special-relativity.md), even though some [entangled](../../../bell-state.md#entangled-state) states have correlations incompatible with a [local hidden-variable theory](../../../quantum-theory.md#local-hidden-variable-theory).

## 2

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [EPR criterion of reality](../../../quantum-theory.md#epr-criterion-of-reality) says that if a physical quantity can be predicted with certainty without disturbing the system, then it represents an element of physical reality. For separated particles, the EPR locality assumption regards choices of measurements on the other particles as nondisturbing. The perfect correlations below therefore imply predetermined local values for both $X=\sigma_x$ and $Y=\sigma_y$, independent of which distant measurements are chosen.

Put $|0\rangle=|\uparrow\rangle$ and $|1\rangle=|\downarrow\rangle$. The [Pauli matrices](../../../algebra.md#pauli-matrices) satisfy

$$
X|0\rangle=|1\rangle,\quad X|1\rangle=|0\rangle,\quad Y|0\rangle=i|1\rangle,\quad Y|1\rangle=-i|0\rangle.
$$

For three particles, each operator with one $X$ and two $Y$ takes $|000\rangle$ to $-|111\rangle$ and $|111\rangle$ to $-|000\rangle$, whereas $X\otimes X\otimes X$ interchanges the two strings without a minus sign. Thus the [GHZ state](../../../quantum-theory.md#greenberger-horne-zeilinger-state) in the question has the certain outcomes

$$
\boxed{XYY=YXY=YYX=+1,\qquad XXX=-1.}
$$

Each local $X$ or $Y$ value can be predicted from measurements at the other two sites in one of these contexts. If the [EPR criterion of reality](../../../quantum-theory.md#epr-criterion-of-reality) and locality assign values $x_j,y_j\in\{\pm1\}$, the first three equalities require

$$
x_1y_2y_3=1,\qquad y_1x_2y_3=1,\qquad y_1y_2x_3=1.
$$

Multiplying these ordinary numbers and using $y_j^2=1$ yields $x_1x_2x_3=1$, contradicting the certain quantum outcome $-1$. This derives the [GHZ theorem](../../../quantum-theory.md#ghz-theorem) explicitly; the multiplication is of hypothetical local values, not of mutually incompatible local observables.

For general $N$, let $O_j=X_j\bigotimes_{k\ne j}Y_k$, with the tensor factors ordered by their site labels, and let $X_N=X^{\otimes N}$. Directly,

$$
O_j|0\rangle^{\otimes N}=i^{N-1}|1\rangle^{\otimes N},\qquad O_j|1\rangle^{\otimes N}=(-i)^{N-1}|0\rangle^{\otimes N}.
$$

For the difference of the two strings to be an [eigenstate](../../../quantum-mechanics.md#eigenstate), these phases must agree, which happens exactly when $N-1$ is even. For odd $N$ the common phase is $(-1)^{(N-1)/2}$, and interchanging the strings negates their difference. Consequently

$$
\boxed{N\text{ odd}:\quad O_j|\psi\rangle_N=(-1)^{(N+1)/2}|\psi\rangle_N\ \text{for every }j,\qquad X_N|\psi\rangle_N=-|\psi\rangle_N.}
$$

For even $N$, $X_N$ still has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $-1$, but every $O_j$ takes the difference state to a phase times the sum state, which is [orthogonal](../../../linear-algebra.md#orthogonal-vectors) to it. Thus it is not an [eigenstate](../../../quantum-mechanics.md#eigenstate) of any $O_j$; those operators each have outcomes $\pm1$ with equal [probabilities](../../../probability-theory.md#probability). Among the stated $N\geq4$, simultaneous eigenstates therefore occur precisely at $N=5,7,9,\ldots$.

For odd $N$, certainty of each $O_j$ again permits remote prediction of both local $X$ and $Y$. Writing $\lambda_N=(-1)^{(N+1)/2}$, the [local hidden-variable theory](../../../quantum-theory.md#local-hidden-variable-theory) would require $x_j\prod_{k\ne j}y_k=\lambda_N$ for all $j$. Their product is

$$
\left(\prod_jx_j\right)\prod_k y_k^{N-1}=\lambda_N^N,
$$

hence $\prod_jx_j=\lambda_N$, since $N-1$ is even and $N$ is odd. Quantum theory requires the same product to be $-1$. The contradiction occurs when $\lambda_N=+1$, giving the infinite family

$$
\boxed{N\equiv3\pmod4;\quad N\geq4\text{ gives }N=7,11,15,\ldots.}
$$

For $N\equiv1\pmod4$, these particular certain product constraints are consistent; for example $x_j=-1$, $y_j=+1$ satisfies them. This distinguishes the [GHZ contradiction for N congruent to 3 modulo 4](../../../quantum-theory.md#ghz-contradiction-for-n-congruent-to-3-modulo-4) from the larger set of odd $N$ for which simultaneous eigenstates exist.

## 3

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $a=|\alpha|^2$, $b=|\beta|^2=1-a$, so $1/2<a<1$ and $0<b<1/2$. Regrouping the four copies by party gives

$$
|\Psi\rangle=\sum_{x\in\{0,1\}^4}\alpha^{z(x)}\beta^{4-z(x)}|x\rangle_A|x\rangle_B,
$$

where $z(x)$ counts zeroes. Alice must measure only this count, preserving coherence inside each degenerate [eigenspace](../../../linear-operator-theory.md#eigenspace), rather than measuring her four bits separately. Her [projective measurement](../../../quantum-measurement.md#projective-measurement) has projectors $\Pi_k=\sum_{z(x)=k}|x\rangle\langle x|$, and the [Born rule](../../../quantum-mechanics.md#born-rule) gives

$$
\boxed{p_k=\binom4k a^k b^{4-k},\qquad k=0,1,2,3,4.}
$$

Alice sends $k$ to Bob. Up to the common phase of $\alpha^k\beta^{4-k}$, their conditional [pure state](../../../quantum-theory.md#pure-state) is

$$
|T_k\rangle=\frac1{\sqrt{d_k}}\sum_{z(x)=k}|x\rangle_A|x\rangle_B,\qquad d_k=\binom4k.
$$

This is [Schmidt projection entanglement concentration](../../../bell-state.md#schmidt-projection-entanglement-concentration): its equal [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient) give a [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) of [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) $d_k$.

For $k=0$ or $4$, $d_k=1$, and the branch is a [product state](../../../bell-state.md#product-state). No [Bell pair](../../../bell-state.md#bell-pair) can be extracted using [local operations and classical communication](../../../bell-state.md#local-operations-and-classical-communication). The respective [probabilities](../../../probability-theory.md#probability) are $b^4$ and $a^4$.

For $k=1$ or $3$, $d_k=4$. List the four surviving strings in lexicographic order as $x_0,x_1,x_2,x_3$. For $k=1$ this list is $0111,1011,1101,1110$; for $k=3$ it is $0001,0010,0100,1000$. Each party applies a [local unitary operation](../../../bell-state.md#local-unitary-operation) extending the basis relabelling

$$
|x_j\rangle\longmapsto |j_1j_0\rangle\otimes|00\rangle,\qquad j=2j_1+j_0.
$$

Such a unitary exists because these are four distinct [orthonormal](../../../linear-algebra.md#orthonormal-set) basis vectors mapped to four distinct basis vectors; extend the mapping to a permutation of all sixteen. Discarding the two fixed local ancillary bits leaves

$$
\frac12\sum_{j_1,j_0=0}^1|j_1j_0\rangle_A|j_1j_0\rangle_B
=|\Phi^+\rangle_{A_1B_1}\otimes|\Phi^+\rangle_{A_0B_0}.
$$

Thus these branches give exactly two [Bell pairs](../../../bell-state.md#bell-pair), with [probabilities](../../../probability-theory.md#probability) $4ab^3$ and $4a^3b$, and no further [measurement in quantum mechanics](../../../quantum-measurement.md) is needed.

For $k=2$, the six strings in lexicographic order are $x_0=0011$, $x_1=0101$, $x_2=0110$, $x_3=1001$, $x_4=1010$, $x_5=1100$. A suitable local [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) gives two [Bell pairs](../../../bell-state.md#bell-pair) with certainty, rather than losing some of these branches to a simple subspace projection. Partition these labels into the three pairs $T_0=\{0,1\}$, $T_1=\{2,3\}$, $T_2=\{4,5\}$. Alice uses the [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
K_r=\frac1{\sqrt2}\sum_{j\notin T_r}|x_j\rangle\langle x_j|,\qquad r=0,1,2.
$$

On the six-dimensional support, each label is retained by two operators, so $\sum_{r=0}^2K_r^\dagger K_r=\Pi_2$. Add $K_\perp=I-\Pi_2$ to define a complete [measurement in quantum mechanics](../../../quantum-measurement.md) on Alice's four qubits; that extra outcome has [probability](../../../probability-theory.md#probability) zero on this branch. Each nonzero outcome has conditional [probability](../../../probability-theory.md#probability) $(1/2)(4/6)=1/3$, and gives the normalized state

$$
\frac12\sum_{j\notin T_r}|x_j\rangle_A|x_j\rangle_B.
$$

Alice sends $r$ to Bob. Both parties relabel the four surviving strings in increasing order to $|00\rangle,|01\rangle,|10\rangle,|11\rangle$ on two output qubits, with two fixed ancillary bits, just as above. Every $r$ therefore gives two [Bell pairs](../../../bell-state.md#bell-pair). The joint [probability](../../../probability-theory.md#probability) of $(k,r)=(2,r)$ is $p_2/3=2a^2b^2$ for each $r$.

For an explicit local implementation of this [POVM](../../../quantum-measurement.md#positive-operator-valued-measure), Alice can append an ancilla in a fixed state and apply an isometry on the six-dimensional support,

$$
|x_j\rangle\longmapsto |x_j\rangle\otimes\frac1{\sqrt2}\sum_{r:\,j\notin T_r}|r\rangle.
$$

It preserves inner products, extends to a unitary on system and ancilla, and measuring the ancilla realizes precisely the operators $K_r$. No nonlocal operation has been used. This is a [deterministic reduction of maximally entangled Schmidt rank](../../../bell-state.md#deterministic-reduction-of-maximally-entangled-schmidt-rank) from six to four.

The complete output distribution for this strategy is consequently

$$
\boxed{\Pr(2\text{ Bell pairs})=1-a^4-b^4,\qquad \Pr(0\text{ Bell pairs})=a^4+b^4.}
$$

The mean yield is $2(1-a^4-b^4)$ pairs per four-copy block. These are the maximum possible pair counts after the stipulated count measurement: any nonzero branch has [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) at most six, whereas three independent [Bell pairs](../../../bell-state.md#bell-pair) require [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) eight. In any refined [LOCC](../../../bell-state.md#local-operations-and-classical-communication) branch the coefficient matrix is multiplied by local matrices on the left and right, which cannot increase its [rank](../../../linear-algebra.md#rank-one-quadratic-form).

## 4

↑ **Parent:** [Paper 53](paper-53.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The relevant security model gives Eve the purifying system and access to the public transcript. A useful preliminary fact is that [purity decouples a subsystem from its purification](../../../quantum-theory.md#purity-decouples-a-subsystem-from-its-purification). If the Alice–Bob marginal is $|u\rangle\langle u|$ and $|\Omega\rangle_{ABE}$ is a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator), then for every $v\perp u$,

$$
\|(\langle v|_{AB}\otimes I_E)|\Omega\rangle\|^2=\langle v|\rho_{AB}|v\rangle=0.
$$

Hence $|\Omega\rangle_{ABE}=|u\rangle_{AB}|e\rangle_E$: Eve is uncorrelated with their joint [pure state](../../../quantum-theory.md#pure-state). A [Bell pair](../../../bell-state.md#bell-pair) then supplies a uniform shared secret bit when both parties measure in the [computational basis](../../../quantum-theory.md#computational-basis). Pure [product states](../../../bell-state.md#product-state) have no shared random correlations, while a [mixed state](../../../quantum-theory.md#mixed-state) must be assessed with its purifying information included. The classifications below use the usual [quantum key distribution](../../../computer-science.md#quantum-key-distribution) setting with an authenticated public classical channel; no full security proof is required.

<h3 id="4/a">A</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/1">1</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/1/solution">Solution</h5>

↑ **Parent:** [1](#4/a/1)

**A secure key can be produced, at one ideal secret bit per copy.** The shared [Bell state](../../../bell-state.md) is pure, so the preceding factorization shows that Eve's purifying system is independent of it. Measuring both qubits in the [computational basis](../../../quantum-theory.md#computational-basis) gives matching outcomes $00$ or $11$, each with [probability](../../../probability-theory.md#probability) $1/2$. Neither party announces these key outcomes. Eve's state is the same for both possibilities, so each copy supplies a shared uniform private bit.

<h4 id="4/a/2">2</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/2/solution">Solution</h5>

↑ **Parent:** [2](#4/a/2)

**The normalized ray produces a secure key; the literal printed vector is not normalized.** The squared norm of the coefficients in the PDF is $8/9+1/81=73/81$. Thus the physical [pure state](../../../quantum-theory.md#pure-state) on that ray has normalized coefficients $6\sqrt2/\sqrt{73}$ and $1/\sqrt{73}$. This is a genuine [entangled state](../../../bell-state.md#entangled-state) with two nonzero [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient), and Eve is independent of it by [purity decouples a subsystem from its purification](../../../quantum-theory.md#purity-decouples-a-subsystem-from-its-purification).

For an explicit way to obtain uniform key bits, Alice applies a two-outcome local [measurement in quantum mechanics](../../../quantum-measurement.md) with [Kraus operators](../../../quantum-information-theory.md#kraus-operator)

$$
K_s=\begin{pmatrix}1/(6\sqrt2)&0\\0&1\end{pmatrix},\qquad K_f=\begin{pmatrix}\sqrt{71/72}&0\\0&0\end{pmatrix}.
$$

Their squared products sum to the identity. The successful unnormalized state is $(|00\rangle+|11\rangle)/\sqrt{73}$, so

$$
\boxed{p_s=2/73,\qquad p_f=71/73.}
$$

Alice announces only success or failure. Success leaves an exact [Bell pair](../../../bell-state.md#bell-pair), yielding one uniform secret bit; failure leaves $|00\rangle$ and is discarded. With many copies the successful fraction is positive. Alternatively, direct [computational basis](../../../quantum-theory.md#computational-basis) measurements give a shared biased bit with probabilities $72/73$ and $1/73$, from which [privacy amplification](../../../computer-science.md#privacy-amplification) can extract uniform secret bits. The coefficient $1/9$ has not been silently replaced by $1/3$.

<h4 id="4/a/3">3</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/3/solution">Solution</h5>

↑ **Parent:** [3](#4/a/3)

**No secure key can be produced from this state alone.** Factoring the printed amplitudes gives the normalized [product state](../../../bell-state.md#product-state)

$$
\left(\frac{\sqrt2}{3}|0\rangle_A+\frac{\sqrt7}{3}|1\rangle_A\right)\otimes|+\rangle_B.
$$

Eve is uncorrelated with the joint [pure state](../../../quantum-theory.md#pure-state), but Alice and Bob also have no correlations with each other: local outcome probabilities factor. They may generate independent private random bits locally, but [local operations and classical communication](../../../bell-state.md#local-operations-and-classical-communication) cannot make those bits shared and secret using only public messages. A [product state](../../../bell-state.md#product-state) supplies no shared secret resource.

<h4 id="4/a/4">4</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/4/solution">Solution</h5>

↑ **Parent:** [4](#4/a/4)

**No secure key can be produced.** The off-diagonal terms in the two [Bell state](../../../bell-state.md) projectors cancel, giving the [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state)

$$
\rho_{AB}=\tfrac12|00\rangle\langle00|+\tfrac12|11\rangle\langle11|.
$$

A possible [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) is $(|00\rangle_{AB}|0\rangle_E+|11\rangle_{AB}|1\rangle_E)/\sqrt2$. Eve measures her register in the [computational basis](../../../quantum-theory.md#computational-basis) and learns whether Alice and Bob have $00$ or $11$. Their apparently shared random bit is therefore completely known to Eve. Conditioned on her record the Alice–Bob state is a known [product state](../../../bell-state.md#product-state); public discussion and local private randomness cannot create a shared secret unknown to that record. The state has no distillable secret key in the stated purification model.

<h4 id="4/a/5">5</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/5/solution">Solution</h5>

↑ **Parent:** [5](#4/a/5)

**A secure key can be produced, at one ideal secret bit per copy.** Denote Alice's additional flag qubit by $F$. Alice can measure $F$ in the [computational basis](../../../quantum-theory.md#computational-basis) and, when its outcome is $1$, apply the [Pauli Z gate](../../../quantum-theory.md#pauli-z-gate) to her half of the shared pair. The two flag outcomes each have [probability](../../../probability-theory.md#probability) $1/2$, and $Z_A|\Phi^-\rangle=|\Phi^+\rangle$; either branch therefore supplies the same pure [Bell pair](../../../bell-state.md#bell-pair).

Equivalently, Alice applies the local controlled unitary

$$
U=I_{AB}\otimes|0\rangle\langle0|_F+(Z_A\otimes I_B)\otimes|1\rangle\langle1|_F.
$$

This [local flag correction of a Bell-state phase mixture](../../../bell-state.md#local-flag-correction-of-a-bell-state-phase-mixture) changes the full [density matrix](../../../quantum-theory.md#density-matrix) into

$$
\boxed{|\Phi^+\rangle\langle\Phi^+|_{AB}\otimes I_F/2.}
$$

The corrected pair is pure, so every purification factors between $AB$ and $FE$. Eve may know the flag without knowing the key bit obtained from $AB$. Alice need not disclose the flag, but even disclosing it does not compromise the corrected pure [Bell pair](../../../bell-state.md#bell-pair). Tracing out the flag before correction would give the nonprivate mixture in the preceding case; retaining Alice's local side information is essential.

<h3 id="4/b">B</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/protocol-1">Protocol 1</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/protocol-1/solution">Solution</h5>

↑ **Parent:** [Protocol 1](#4/b/protocol-1)

**Insecure as a proposed test-and-purify protocol: the basis string and check positions are announced before receipt.** Eve can intercept and store the travelling qubits until the announcement. For each data position with basis bit $b_j$, she measures the stored qubit in the basis $\{H^{b_j}|0\rangle,H^{b_j}|1\rangle\}$. If the outcome is $z_j$, the Alice–Bob pair becomes

$$
|z_j\rangle_A\otimes H^{b_j}|z_j\rangle_B,
$$

and Eve knows $z_j$. She forwards that qubit, and forwards every publicly identified check qubit untouched. After Bob's [Hadamard gate](../../../quantum-theory.md#hadamard-gate) decoding, every data pair is the known [product state](../../../bell-state.md#product-state) $|z_jz_j\rangle$, while the unmodified check pairs remain perfect. Thus the check [bit error rate](../../../quantum-theory.md#bit-error-rate) is zero even though Eve knows all raw data bits. This is [premature basis announcement in quantum key distribution](../../../computer-science.md#premature-basis-announcement-in-quantum-key-distribution).

The retained data are a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) with a classical label held by Eve; [LOCC](../../../bell-state.md#local-operations-and-classical-communication) cannot turn them into private [Bell pairs](../../../bell-state.md#bell-pair). Consequently the listed check does not justify the claimed success of the subsequent [entanglement purification](../../../bell-state.md#entanglement-distillation). A sound purification procedure that independently detects the missing entanglement must fail or abort on this attack. If Step 9 were instead read as an independently guaranteed production of private, nearly perfect [Bell pairs](../../../bell-state.md#bell-pair), their subsequent key would of course be private; the flaw is that this protocol's test cannot establish that guarantee. Naming an EPP does not repair the information leak or the invalid sampling test.

<h4 id="4/b/protocol-2">Protocol 2</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/protocol-2/solution">Solution</h5>

↑ **Parent:** [Protocol 2](#4/b/protocol-2)

**Impossible to implement as written: Bob is never given the basis string.** Step 7 requires him to know which incoming qubits were acted on by a [Hadamard gate](../../../quantum-theory.md#hadamard-gate), but the announcement contains only the check positions. Since $H^{-1}=H$, knowing that a transformation is its own inverse does not identify which qubits need it.

Bob cannot recover the missing information from the qubits alone. For each encoded [Bell pair](../../../bell-state.md#bell-pair), his [reduced density matrix](../../../bell-state.md#reduced-density-matrix) is

$$
\operatorname{Tr}_A[(I\otimes H^b)|\Phi^+\rangle\langle\Phi^+|(I\otimes H^b)]=I/2
$$

for either $b=0$ or $b=1$. His entire received register has the same [density matrix](../../../quantum-theory.md#density-matrix) $I/2^{2n}$ for every string $b$, so every local [measurement in quantum mechanics](../../../quantum-measurement.md) has statistics independent of $b$. Nor can one fixed unitary undo both possibilities: preserving $|\Phi^+\rangle$ requires that unitary to be proportional to $I$, whereas decoding $(I\otimes H)|\Phi^+\rangle$ requires it to be proportional to $H$. Supplying the missing basis announcement after receipt would repair the protocol and make it the third one, but that communication is absent from the printed sequence.

<h4 id="4/b/protocol-3">Protocol 3</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/protocol-3/solution">Solution</h5>

↑ **Parent:** [Protocol 3](#4/b/protocol-3)

**Secure in the intended ideal setting, with a sound entanglement-purification procedure.** Bob confirms receipt before Alice reveals either the random basis string or the randomly chosen check positions. Eve must therefore release the travelling qubits before knowing which basis to use and which positions to protect from disturbance. Bob can then decode because $H^2=I$.

The random check sample tests the same ensemble of encoded transmissions as the retained data. Random [computational basis](../../../quantum-theory.md#computational-basis) and [Hadamard basis](../../../quantum-theory.md#hadamard-basis) encodings make the test sensitive to complementary disturbances; Eve cannot use the targeted zero-error attack available in Protocol 1. For example, measuring every intercepted qubit in one fixed one of these two bases uses the wrong basis half the time, and then disagrees with Alice half the time, producing a [bit error rate](../../../quantum-theory.md#bit-error-rate) of $1/4$. A sound [entanglement purification](../../../bell-state.md#entanglement-distillation) protocol uses the tested error bounds, corrects both relevant types of error, and aborts if the noise is too high; secrecy is not claimed for every possible attack without an abort option.

When the protocol succeeds in producing nearly perfect [Bell pairs](../../../bell-state.md#bell-pair), [purity decouples a subsystem from its purification](../../../quantum-theory.md#purity-decouples-a-subsystem-from-its-purification) explains why they are nearly independent of Eve, and matching [computational basis](../../../quantum-theory.md#computational-basis) measurements produce an approximately uniform shared secret key. The disclosed check outcomes are discarded rather than included in that key. This is the standard entanglement-based [quantum key distribution](../../../computer-science.md#quantum-key-distribution) ordering: receipt first, basis and sample disclosure second, testing and purification next, and private measurements last.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
