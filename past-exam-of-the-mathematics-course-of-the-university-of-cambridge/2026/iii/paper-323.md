# Paper 323

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20323.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20323.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
    - [iv](#4/c/iv)
      - [Solution](#4/c/iv/solution)
    - [v](#4/c/v)
      - [Solution](#4/c/v/solution)

## 1

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

A [quantum channel](../../../quantum-information-theory.md#quantum-channel) $T:\mathcal B(\mathcal H)\to\mathcal B(\mathcal K)$ is a linear, completely positive, trace-preserving map. Complete positivity means $T\otimes\operatorname{id}_n$ is positive for every ancillary dimension $n$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [Kraus representation](../../../quantum-information-theory.md#kraus-representation) is

$$
\boxed{T(\rho)=\sum_jK_j\rho K_j^\dagger},
\qquad
\boxed{\sum_jK_j^\dagger K_j=I}.
$$

The second identity is precisely trace preservation. Different Kraus families related by an isometry represent the same channel.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Since $|\phi\rangle\langle\phi|\geq0$ and a channel is completely positive,

$$
\boxed{C=(T\otimes\operatorname{id})(|\phi\rangle\langle\phi|)\geq0}.
$$

Writing

$$
C=\frac1d\sum_{j,k}T(|j\rangle\langle k|)
\otimes|j\rangle\langle k|
$$

and tracing over the output system gives

$$
\operatorname{Tr}_1C
=\frac1d\sum_{j,k}\operatorname{Tr}T(|j\rangle\langle k|)
|j\rangle\langle k|
=\frac1d\sum_j|j\rangle\langle j|.
$$

Thus

$$
\boxed{\operatorname{Tr}_1C=I_d/d},
$$

where the factor $1/d$ follows from the normalized maximally entangled state.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

For $T(\rho)=\sum_kp_kU_k\rho U_k^\dagger$,

$$
C_T=\sum_kp_k
(U_k\otimes I)|\phi\rangle\langle\phi|
(U_k^\dagger\otimes I).
$$

Each $(U_k\otimes I)|\phi\rangle$ is a [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state), so the [Choi matrix](../../../quantum-information-theory.md#choi-matrix) is a convex combination of maximally entangled pure states.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Every [random unitary channel](../../../quantum-information-theory.md#random-unitary-channel) satisfies

$$
T(I)=\sum_kp_kU_kIU_k^\dagger
=\left(\sum_kp_k\right)I=I.
$$

It is therefore a [unital quantum channel](../../../quantum-information-theory.md#unital-quantum-channel).

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

The normalized [Choi matrix](../../../quantum-information-theory.md#choi-matrix) of the trace-to-identity map is $I\otimes I/d$, while that of transposition is the flip operator $F/d$. Hence the [Werner–Holevo channel](../../../quantum-information-theory.md#werner-holevo-channel) has

$$
C_T=\frac{I-F}{d(d-1)}
=\frac{2}{d(d-1)}P_-,
$$

the normalized projector onto the antisymmetric subspace.

If the channel were random unitary, part (i) would express $C_T$ as a mixture of maximally entangled vectors. Every vector in such a mixture must lie in the support of $C_T$, hence in the antisymmetric subspace. Under vectorization, an antisymmetric vector corresponds to a skew-symmetric matrix $A$, while maximal entanglement requires $AA^\dagger$ to be proportional to $I$. In odd dimension, $\det A=\det(-A^T)=-\det A$, so $\det A=0$; such an $A$ cannot be proportional to a unitary. Thus for odd $d\geq3$, and in particular $d=3$, this unital channel is not random unitary, disproving the converse. The odd-dimensional qualification matters because antisymmetric maximally entangled vectors can exist in even dimension.

## 2

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A bipartite density operator is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) when

$$
\rho_{AB}=\sum_jp_j\rho_j^A\otimes\rho_j^B
$$

for probabilities $p_j$ and local states. If no such convex decomposition exists, it is an [entangled state](../../../bell-state.md#entangled-state).

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) says separability implies $\rho_{AB}^{T_B}\geq0$. A nonpositive partial transpose therefore proves entanglement. Positive partial transpose is also sufficient for separability in dimensions $2\otimes2$ and $2\otimes3$, but not in general higher dimensions.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

After permuting the computational basis, $\rho$ is the direct sum of

$$
\begin{pmatrix}a&x\\x^*&d\end{pmatrix},
\qquad
\begin{pmatrix}b&y\\y^*&c\end{pmatrix}.
$$

The stated diagonal and trace conditions already give Hermiticity and trace one. Each $2\times2$ block is positive semidefinite exactly when its determinant is nonnegative. Thus $\rho$ is a density matrix precisely when

$$
\boxed{|x|^2\leq ad,\qquad |y|^2\leq bc}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Partial transposition interchanges the positions occupied by $x$ and $y$. Positivity of $\rho^{T_B}$ therefore requires

$$
|y|^2\leq ad,
\qquad
|x|^2\leq bc.
$$

Because the system is $2\otimes2$, the [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) is necessary and sufficient. Combining these inequalities with validity of the original state gives

$$
\boxed{|x|^2\leq\min(ad,bc),\qquad
|y|^2\leq\min(ad,bc)}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

For a bipartite input,

$$
(T\otimes\operatorname{id})(\rho_{AB})
=\sum_k\sigma_k^A\otimes
\operatorname{Tr}_A[(M_k\otimes I)\rho_{AB}].
$$

Each second factor is positive and has trace equal to the probability of measurement outcome $k$. Dividing nonzero factors by their traces therefore writes the output as a convex combination of product states. Hence every measure-and-prepare channel is an [entanglement-breaking channel](../../../quantum-information-theory.md#entanglement-breaking-channel).

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

If $T$ is entanglement breaking, applying it to one half of $|\phi\rangle\langle\phi|$ immediately shows that its [Choi matrix](../../../quantum-information-theory.md#choi-matrix) is separable.

Conversely suppose

$$
C_T=\sum_kq_k\sigma_k\otimes\tau_k
$$

is separable. The Choi reconstruction formula for the normalized convention is

$$
T(\rho)=d\,\operatorname{Tr}_2[C_T(I\otimes\rho^T)]
=\sum_k\operatorname{Tr}(M_k\rho)\sigma_k,
\qquad
M_k=dq_k\tau_k^T.
$$

The trace-preserving condition $\operatorname{Tr}_1C_T=I/d$ implies $\sum_kM_k=I$, so $\{M_k\}$ is a POVM. Part (i) now proves that $T$ is entanglement breaking. Thus

$$
\boxed{T\text{ is entanglement breaking}
\iff C_T\text{ is separable}}.
$$

## 3

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

In [quantum binary hypothesis testing](../../../quantum-information-theory.md#quantum-binary-hypothesis-testing), hypothesis zero supplies $\rho_0$ with prior $p$ and hypothesis one supplies $\rho_1$ with prior $1-p$. A two-outcome POVM $\{Q,I-Q\}$ decides zero on outcome $Q$. The conditional errors are

$$
\alpha=\operatorname{Tr}[(I-Q)\rho_0],
\qquad
\beta=\operatorname{Tr}[Q\rho_1].
$$

Symmetric testing minimizes the prior-weighted average error $p\alpha+(1-p)\beta$, equivalently maximizing the average success probability.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Let $\Delta=p\rho_0-(1-p)\rho_1$. The success probability of $Q$ is

$$
P_{\rm succ}(Q)
=p\operatorname{Tr}(Q\rho_0)
+(1-p)\operatorname{Tr}[(I-Q)\rho_1]
=1-p+\operatorname{Tr}(Q\Delta).
$$

Write the spectral decomposition $\Delta=\Delta_+-\Delta_-$. For every effect $0\leq Q\leq I$,

$$
\operatorname{Tr}(Q\Delta)
\leq\operatorname{Tr}\Delta_+,
$$

with equality when $Q$ projects onto the positive spectral subspace, with arbitrary action on the kernel. Since $\operatorname{Tr}\Delta=2p-1$ and $\|\Delta\|_1=\operatorname{Tr}\Delta_++\operatorname{Tr}\Delta_-$, the [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem) follows:

$$
\boxed{P_{\rm succ}^*
=\frac12(1+\|\Delta\|_1)},
\qquad
\boxed{P_{\rm err}^*
=\frac12(1-\|\Delta\|_1)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Put $c=\cos(\theta/2)$, $s=\sin(\theta/2)$, and $\zeta=e^{2\pi i/3}$. Averaging the three states cancels the off-diagonal phases:

$$
\bar\rho=\frac13\sum_{k=0}^2|\psi_k\rangle\langle\psi_k|
=\begin{pmatrix}c^2&0\\0&s^2\end{pmatrix}.
$$

For $c,s>0$, the [pretty good measurement](../../../quantum-information-theory.md#pretty-good-measurement) is

$$
\boxed{M_k=\frac13
\begin{pmatrix}
1&\zeta^{-k}\\
\zeta^k&1
\end{pmatrix}}
$$

because $\bar\rho^{-1/2}|\psi_k\rangle=|0\rangle+\zeta^k|1\rangle$. The matrices are positive and $\sum_kM_k=I$. At the endpoint values of $\theta$, the same formula is understood on the support of $\bar\rho$ and may be completed arbitrarily on its kernel.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

The Holevo optimality conditions say a POVM is optimal when

$$
\Gamma=\sum_kp_k\rho_kM_k
$$

is Hermitian and $\Gamma-p_k\rho_k\geq0$ for every $k$. Here

$$
\Gamma=\frac{c+s}{3}
\begin{pmatrix}c&0\\0&s\end{pmatrix}
$$

and

$$
\Gamma-\frac13\rho_k
=\frac{cs}{3}
\begin{pmatrix}
1&-\zeta^{-k}\\
-\zeta^k&1
\end{pmatrix}\geq0,
$$

whose eigenvalues are $0$ and $2cs/3$. The [pretty good measurement](../../../quantum-information-theory.md#pretty-good-measurement) is therefore optimal. Its success probability is

$$
\boxed{P_{\rm succ}=\frac13(c+s)^2
=\frac13(1+\sin\theta)}.
$$

## 4

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a [density operator](../../../quantum-theory.md#density-matrix) $\rho$ on a finite-dimensional [Hilbert space](../../../hilbert-space.md), the [Von Neumann entropy](../../../von-neumann-entropy.md) is

$$
\boxed{S(\rho)=-\operatorname{Tr}(\rho\log\rho)},
$$

with $0\log0=0$. Its [concavity](../../../von-neumann-entropy.md#concavity-of-von-neumann-entropy) says that, for $0\leq p\leq1$,

$$
\boxed{S(p\rho_1+(1-p)\rho_2)
\geq pS(\rho_1)+(1-p)S(\rho_2)}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $\rho=p\rho_1+(1-p)\rho_2$. The [operator inequality](../../../hilbert-space.md#lowner-order) $\rho\geq p\rho_1$ and the [operator monotonicity of logarithm](../../../calculus.md#operator-monotonicity-of-logarithm) give, on the support of $\rho_1$,

$$
\log\rho\geq\log(p\rho_1)
=(\log p)I+\log\rho_1.
$$

Consequently,

$$
-p\operatorname{Tr}(\rho_1\log\rho)
\leq pS(\rho_1)-p\log p.
$$

The corresponding inequality from $\rho\geq(1-p)\rho_2$ yields

$$
-(1-p)\operatorname{Tr}(\rho_2\log\rho)
\leq(1-p)S(\rho_2)-(1-p)\log(1-p).
$$

Adding these inequalities and using $S(\rho)=-\operatorname{Tr}(\rho\log\rho)$ proves the [entropy bound for a binary mixture](../../../von-neumann-entropy.md#entropy-bound-for-a-binary-mixture):

$$
\boxed{S(\rho)\leq pS(\rho_1)+(1-p)S(\rho_2)+H(p)}.
$$

Singular states follow by adding a positive multiple of the identity and taking a [limit](../../../calculus.md#limit-of-a-function); the endpoint cases use $0\log0=0$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

If $\varepsilon=0$, then $\rho_{AB}=\sigma_{AB}$ and the desired continuity bound is immediate, so assume $\varepsilon>0$. Apply the [positive-negative decomposition of a Hermitian operator](../../../hilbert-space.md#positive-negative-decomposition-of-a-hermitian-operator) to

$$
X=\rho_{AB}-\sigma_{AB}=X_+-X_-.
$$

Because $\operatorname{Tr}X=0$ and $\lVert X\rVert_1=2\varepsilon$, one has

$$
\operatorname{Tr}X_+=\operatorname{Tr}X_-=\varepsilon.
$$

Thus $\Delta_{AB}=X_+/\varepsilon$ is positive with trace one, hence is a [density operator](../../../quantum-theory.md#density-matrix). Define

$$
\omega_{AB}=\frac{\sigma_{AB}+\varepsilon\Delta_{AB}}{1+\varepsilon}
=\frac{\sigma_{AB}+X_+}{1+\varepsilon}
=\frac{\rho_{AB}+X_-}{1+\varepsilon}.
$$

It is a [convex combination](../../../mathematical-optimization.md#convex-combination) of states. The equation $\varepsilon\Delta'_{AB}=(1+\varepsilon)\omega_{AB}-\rho_{AB}$ gives

$$
\Delta'_{AB}=X_-/\varepsilon,
$$

which is likewise positive and has trace one.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

The two forms of $\omega_{AB}$ found in part (i) give

$$
(1+\varepsilon)\omega_{AB}-\rho_{AB}=X_-\geq0,
\qquad
(1+\varepsilon)\omega_{AB}-\sigma_{AB}=X_+\geq0.
$$

Therefore, in the [Löwner order](../../../hilbert-space.md#lowner-order),

$$
\boxed{\rho_{AB}\leq(1+\varepsilon)\omega_{AB}},
\qquad
\boxed{\sigma_{AB}\leq(1+\varepsilon)\omega_{AB}}.
$$

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Set $q=(1+\varepsilon)^{-1}$, so $1-q=\varepsilon/(1+\varepsilon)$ and $\omega=q\rho+(1-q)\Delta'$. For every state $\xi_B$, the [entropy bound for a binary mixture](../../../von-neumann-entropy.md#entropy-bound-for-a-binary-mixture) gives

$$
\begin{aligned}
D(\omega_{AB}\|I_A\otimes\xi_B)
&=-S(\omega_{AB})-\operatorname{Tr}(\omega_B\log\xi_B)\\
&\geq qD(\rho_{AB}\|I_A\otimes\xi_B)
 +(1-q)D(\Delta'_{AB}\|I_A\otimes\xi_B)-H(q).
\end{aligned}
$$

Taking the minimum over $\xi_B$ and using the [variational characterization of quantum conditional entropy](../../../von-neumann-entropy.md#variational-characterization-of-quantum-conditional-entropy) on each term gives

$$
-H(A|B)_\omega
\geq-qH(A|B)_\rho-(1-q)H(A|B)_{\Delta'}-H(q).
$$

Since [binary entropy](../../../information-theory.md#binary-entropy) satisfies $H(q)=H(1-q)$, this is

$$
\boxed{H(A|B)_\omega\leq
\frac{H(A|B)_\rho+\varepsilon H(A|B)_{\Delta'}}{1+\varepsilon}
+H\!\left(\frac{\varepsilon}{1+\varepsilon}\right)}.
$$

<h4 id="4/c/iv">iv</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/c/iv)

The other convex decomposition is $\omega=q\sigma+(1-q)\Delta$. Applying the [concavity of quantum conditional entropy](../../../von-neumann-entropy.md#concavity-of-quantum-conditional-entropy), which follows from the [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy), yields

$$
\boxed{H(A|B)_\omega\geq
\frac{H(A|B)_\sigma+\varepsilon H(A|B)_\Delta}{1+\varepsilon}}.
$$

<h4 id="4/c/v">v</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/v/solution">Solution</h5>

↑ **Parent:** [V](#4/c/v)

Combining parts (iii) and (iv), then multiplying by $1+\varepsilon$, gives

$$
H(A|B)_\sigma-H(A|B)_\rho
\leq\varepsilon\bigl(H(A|B)_{\Delta'}-H(A|B)_\Delta\bigr)
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right).
$$

The [dimension bound for quantum conditional entropy](../../../von-neumann-entropy.md#dimension-bound-for-quantum-conditional-entropy) is

$$
-\log d_A\leq H(A|B)_\tau\leq\log d_A.
$$

Indeed, [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) gives $H(A|B)_\tau\leq S(\tau_A)\leq\log d_A$, while the [Araki–Lieb inequality](../../../von-neumann-entropy.md#araki-lieb-inequality) gives $H(A|B)_\tau\geq-S(\tau_A)\geq-\log d_A$. Hence

$$
H(A|B)_\sigma-H(A|B)_\rho
\leq2\varepsilon\log d_A
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right).
$$

Interchanging $\rho$ and $\sigma$ proves the [continuity bound for quantum conditional entropy](../../../von-neumann-entropy.md#continuity-bound-for-quantum-conditional-entropy):

$$
\boxed{|H(A|B)_\rho-H(A|B)_\sigma|
\leq2\varepsilon\log d_A
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right)}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
