# Paper 323

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_323.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_323.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [1](#1/b/i/1)
        - [Solution](#1/b/i/1/solution)
      - [2](#1/b/i/2)
        - [Solution](#1/b/i/2/solution)
      - [3](#1/b/i/3)
        - [Solution](#1/b/i/3/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [1](#2/a/ii/1)
        - [Solution](#2/a/ii/1/solution)
      - [2](#2/a/ii/2)
        - [Solution](#2/a/ii/2/solution)
      - [3](#2/a/ii/3)
        - [Solution](#2/a/ii/3/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [1](#3/a/ii/1)
        - [Solution](#3/a/ii/1/solution)
      - [2](#3/a/ii/2)
        - [Solution](#3/a/ii/2/solution)
      - [3](#3/a/ii/3)
        - [Solution](#3/a/ii/3/solution)
        - [b](#3/a/ii/3/b)
          - [i](#3/a/ii/3/b/i)
            - [Solution](#3/a/ii/3/b/i/solution)
          - [ii](#3/a/ii/3/b/ii)
            - [Solution](#3/a/ii/3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
    - [iv](#4/a/iv)
      - [Solution](#4/a/iv/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) states that every finite-dimensional bipartite pure state has

$$
\boxed{|\phi\rangle_{AB}
=\sum_{j=1}^r s_j|a_j\rangle_A|b_j\rangle_B},
$$

where $s_j>0$, $\sum_js_j^2=1$, and the two displayed families are orthonormal. The integer $r$ is the [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank).

To prove it, choose product bases and write

$$
|\phi\rangle=\sum_{m,n}C_{mn}|m\rangle_A|n\rangle_B.
$$

Apply the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) $C=USV^\dagger$. Absorbing the columns of $U$ and the complex conjugates of the columns of $V$ into new orthonormal bases gives the stated sum, with the nonzero singular values as the [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient). Equivalently, $s_j^2$ are the common nonzero eigenvalues of the two [reduced density matrices](../../../bell-state.md#reduced-density-matrix), so $r=\operatorname{rank}\rho_A=\operatorname{rank}\rho_B$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For a purification $|\Psi_\rho\rangle_{RA}$ of $\rho$, the [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity) is

$$
F_e(\rho,\Lambda)=
\langle\Psi_\rho|
(\operatorname{id}_R\otimes\Lambda)
(|\Psi_\rho\rangle\langle\Psi_\rho|)
|\Psi_\rho\rangle.
$$

Using a [Kraus representation](../../../quantum-information-theory.md#kraus-representation) $\Lambda(X)=\sum_kA_kXA_k^\dagger$ gives

$$
F_e(\rho,\Lambda)
=\sum_k\left|
\langle\Psi_\rho|I\otimes A_k|\Psi_\rho\rangle
\right|^2.
$$

In a [Schmidt decomposition](../../../von-neumann-entropy.md#schmidt-decomposition) of the purification,

$$
\langle\Psi_\rho|I\otimes A_k|\Psi_\rho\rangle
=\sum_j\lambda_j\langle j|A_k|j\rangle
=\operatorname{Tr}(A_k\rho).
$$

Therefore

$$
\boxed{F_e(\rho,\Lambda)
=\sum_k|\operatorname{Tr}(A_k\rho)|^2}.
$$

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

Embed the input qubit as the span of $|0\rangle,|1\rangle$ in the three-dimensional output. Because the input is pure, its only purification has a trivial reference and [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity) reduces to its survival probability:

$$
\begin{aligned}
F_e(|+\rangle\langle+|,\mathcal E_{1/2})
&=\langle+|\mathcal E_{1/2}(|+\rangle\langle+|)|+\rangle\\
&=\frac12+\frac12|\langle+|e\rangle|^2.
\end{aligned}
$$

Since $|e\rangle$ is orthogonal to the embedded qubit subspace,

$$
\boxed{F_e=\frac12}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/1">1</h5>

↑ **Parent:** [I](#1/b/i)

<h6 id="1/b/i/1/solution">Solution</h6>

↑ **Parent:** [1](#1/b/i/1)

The state is a convex combination of product density operators and is therefore a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). Every product density operator has a decomposition into product pure states, so

$$
\boxed{\operatorname{SN}(\rho)=1}.
$$

<h5 id="1/b/i/2">2</h5>

↑ **Parent:** [I](#1/b/i)

<h6 id="1/b/i/2/solution">Solution</h6>

↑ **Parent:** [2](#1/b/i/2)

The Bell state $|\Phi^+\rangle=(|00\rangle+|11\rangle)/\sqrt2$ has two nonzero [Schmidt coefficients](../../../von-neumann-entropy.md#schmidt-coefficient). Since the density operator is pure, every ensemble decomposition uses vectors in the same one-dimensional support, and hence

$$
\boxed{\operatorname{SN}(|\Phi^+\rangle\langle\Phi^+|)=2}.
$$

<h5 id="1/b/i/3">3</h5>

↑ **Parent:** [I](#1/b/i)

<h6 id="1/b/i/3/solution">Solution</h6>

↑ **Parent:** [3](#1/b/i/3)

The four [Bell states](../../../bell-state.md) form an orthonormal basis, so their uniform mixture is

$$
\rho=\frac{I_4}{4}
=\frac{I_2}{2}\otimes\frac{I_2}{2}.
$$

It is a product state and therefore

$$
\boxed{\operatorname{SN}(\rho)=1}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The linear extension of the stated [k-reduction map](../../../quantum-information-theory.md#k-reduction-map) is

$$
\Lambda_k(X)=k\operatorname{Tr}(X)I-X.
$$

It suffices to consider a pure state $|v\rangle$ of [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) $r\leq k$, because positivity is preserved by sums. Write

$$
|v\rangle=\sum_{j=1}^r\sqrt{\lambda_j}|j\rangle|j\rangle,
\qquad
\rho_A=\sum_{j=1}^r\lambda_j|j\rangle\langle j|.
$$

Then

$$
(\operatorname{id}\otimes\Lambda_k)(|v\rangle\langle v|)
=k\rho_A\otimes I-|v\rangle\langle v|.
$$

For every $|x\rangle=\sum_{ij}x_{ij}|ij\rangle$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
|\langle v|x\rangle|^2
=\left|\sum_{j=1}^r\sqrt{\lambda_j}x_{jj}\right|^2
\leq r\sum_{j=1}^r\lambda_j|x_{jj}|^2
\leq k\langle x|\rho_A\otimes I|x\rangle.
$$

Thus the operator is a [positive semidefinite operator](../../../hilbert-space.md#positive-operator). Applying this to every vector in a Schmidt-number-$k$ ensemble proves

$$
\boxed{\operatorname{SN}(\sigma)\leq k
\ \Longrightarrow\
(\operatorname{id}_n\otimes\Lambda_k)(\sigma)\geq0}.
$$

<h2 id="2">2</h2>

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Take [Schmidt decompositions](../../../von-neumann-entropy.md#schmidt-decomposition) of the two purifications across $A:R$. Their squared Schmidt coefficients and their $A$-side eigenspaces are fixed by the same reduced state $\rho_A$. The reference-side Schmidt vectors are two orthonormal families, so a unitary $U_R$ maps one family to the other, including arbitrary choices inside degenerate subspaces. Hence the [unitary freedom of purification](../../../quantum-theory.md#unitary-freedom-of-purification) gives

$$
\boxed{|\Psi\rangle_{AR}
=(I_A\otimes U_R)|\Phi\rangle_{AR}}.
$$

If the reference supports have different dimensions, the corresponding statement uses an isometry.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/1">1</h5>

↑ **Parent:** [Ii](#2/a/ii)

<h6 id="2/a/ii/1/solution">Solution</h6>

↑ **Parent:** [1](#2/a/ii/1)

For

$$
|\Psi\rangle_{AR}
=\sum_i\sqrt{\lambda_i}|a_i\rangle_A|b_i\rangle_R,
$$

orthonormality of the $|b_i\rangle$ gives

$$
\operatorname{Tr}_R|\Psi\rangle\langle\Psi|
=\sum_i\lambda_i|a_i\rangle\langle a_i|
=\rho_A.
$$

Normalization follows from $\sum_i\lambda_i=1$, so this is a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator).

<h5 id="2/a/ii/2">2</h5>

↑ **Parent:** [Ii](#2/a/ii)

<h6 id="2/a/ii/2/solution">Solution</h6>

↑ **Parent:** [2](#2/a/ii/2)

With $|\Omega\rangle_{RA}=n^{-1/2}\sum_i|i\rangle_R|i\rangle_A$,

$$
|\Psi\rangle_{RA}
=\sqrt n(I_R\otimes\sqrt{\rho_A})|\Omega\rangle
=\sum_{i,j}(\sqrt{\rho_A})_{ji}|i\rangle_R|j\rangle_A.
$$

The [partial trace](../../../quantum-theory.md#partial-trace) over $R$ is

$$
\operatorname{Tr}_R|\Psi\rangle\langle\Psi|
=\sqrt{\rho_A}\sqrt{\rho_A}^{\,\dagger}
=\rho_A.
$$

Its norm is $\operatorname{Tr}\rho_A=1$. The [positive square root of an operator](../../../hilbert-space.md#positive-square-root-of-an-operator) $\sqrt{\rho_A}$ is unique, proving the claim.

<h5 id="2/a/ii/3">3</h5>

↑ **Parent:** [Ii](#2/a/ii)

<h6 id="2/a/ii/3/solution">Solution</h6>

↑ **Parent:** [3](#2/a/ii/3)

The states $\rho_A^i=|a_i\rangle\langle a_i|$ are pure, so a purification is

$$
\boxed{
|\Psi\rangle
=\sum_{i=1}^n\sum_{\substack{j=1\\j\ne i}}^n
\sqrt{p_{ij}}\,
|i\rangle_{X_1}|j\rangle_{X_2}
|a_i\rangle_{A_1}|a_j\rangle_{A_2}
|ij\rangle_R}.
$$

Tracing out the orthonormal reference labels removes all cross terms and recovers the stated classical-quantum mixture. Its rank is the number of nonzero $p_{ij}$, so that is the minimum reference dimension for a particular state. The smallest dimension that can purify every state of the stated form is

$$
\boxed{\dim H_R=n(n-1)}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Construct ensemble purifications

$$
|\Phi_1\rangle=\sum_j\sqrt{p_j}|\phi_j\rangle|j\rangle,
\qquad
|\Phi_2\rangle=\sum_k\sqrt{q_k}|\psi_k\rangle|k\rangle.
$$

They have the same reduced state exactly when $\rho_1=\rho_2$. By the [unitary freedom of purification](../../../quantum-theory.md#unitary-freedom-of-purification), this holds exactly when $|\Phi_2\rangle=(I\otimes U)|\Phi_1\rangle$ for a unitary $U$. Comparing reference-basis coefficients gives the [Hughston–Jozsa–Wootters theorem](../../../quantum-theory.md#hughston-jozsa-wootters-theorem) relation

$$
\boxed{\sqrt{q_k}|\psi_k\rangle
=\sum_jU_{kj}\sqrt{p_j}|\phi_j\rangle}.
$$

Conversely, substituting this relation and using $U^\dagger U=I$ immediately gives $\rho_2=\rho_1$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

**Yes.** [Uhlmann's theorem](../../../quantum-theory.md#uhlmann-s-theorem) says that, for the fixed purification $|\Psi^\rho\rangle_{AR}$,

$$
F(\rho_A,\sigma_A)
=\max_{|\Phi^\sigma\rangle}
|\langle\Psi^\rho|\Phi^\sigma\rangle|.
$$

Choose a maximizing purification of $\sigma_A$ on the same reference space. In the unsquared fidelity convention,

$$
\boxed{F(|\Psi^\rho\rangle,|\Phi^\sigma\rangle)
=F(\rho_A,\sigma_A)\geq1-\epsilon}.
$$

<h2 id="3">3</h2>

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The finite-dimensional [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) theorem states that every [quantum channel](../../../quantum-information-theory.md#quantum-channel) $\Lambda:\mathcal B(H_A)\to\mathcal B(H_B)$ has an environment $H_E$ and an [isometry](../../../riemannian-geometry.md#isometry) $V:H_A\to H_B\otimes H_E$ such that

$$
\boxed{\Lambda(\rho)=\operatorname{Tr}_E(V\rho V^\dagger)}.
$$

Conversely, every map of this form is completely positive and trace preserving. From [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $A_j$, one may take $V=\sum_jA_j\otimes|j\rangle_E$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/1">1</h5>

↑ **Parent:** [Ii](#3/a/ii)

<h6 id="3/a/ii/1/solution">Solution</h6>

↑ **Parent:** [1](#3/a/ii/1)

Conjugation by $\sigma_z$ maps $(r_x,r_y,r_z)$ to $(-r_x,-r_y,r_z)$. The [phase-flip channel](../../../quantum-information-theory.md#phase-flip-channel) therefore acts on the [Bloch vector](../../../quantum-theory.md#bloch-vector) as

$$
\boxed{(r_x,r_y,r_z)\longmapsto
((1-2p)r_x,(1-2p)r_y,r_z)}.
$$

<h5 id="3/a/ii/2">2</h5>

↑ **Parent:** [Ii](#3/a/ii)

<h6 id="3/a/ii/2/solution">Solution</h6>

↑ **Parent:** [2](#3/a/ii/2)

In the [computational basis](../../../quantum-theory.md#computational-basis),

$$
|\psi\rangle\langle\psi|
=\begin{pmatrix}
|\alpha|^2&\alpha\beta^*\\
\alpha^*\beta&|\beta|^2
\end{pmatrix}.
$$

At $p=1/2$, the two opposite off-diagonal contributions cancel, giving

$$
\boxed{\widetilde\rho
=\Lambda_{1/2}(\rho)
=\begin{pmatrix}|\alpha|^2&0\\0&|\beta|^2\end{pmatrix}}.
$$

<h5 id="3/a/ii/3">3</h5>

↑ **Parent:** [Ii](#3/a/ii)

<h6 id="3/a/ii/3/solution">Solution</h6>

↑ **Parent:** [3](#3/a/ii/3)

A computational-basis [projective measurement](../../../quantum-measurement.md#projective-measurement) has projections $P_0=|0\rangle\langle0|$ and $P_1=|1\rangle\langle1|$. Discarding its result produces the [nonselective projective measurement](../../../quantum-measurement.md#nonselective-projective-measurement)

$$
\sigma=P_0\rho P_0+P_1\rho P_1
=\begin{pmatrix}|\alpha|^2&0\\0&|\beta|^2\end{pmatrix}.
$$

Thus

$$
\boxed{\sigma=\Lambda_{1/2}(\rho)}.
$$

Complete phase randomization and unread computational-basis measurement implement the same [dephasing](../../../quantum-information-theory.md#dephasing-channel) on this qubit.

<h6 id="3/a/ii/3/b">b</h6>

↑ **Parent:** [3](#3/a/ii/3)

<h6 id="3/a/ii/3/b/i">i</h6>

↑ **Parent:** [B](#3/a/ii/3/b)

<h6 id="3/a/ii/3/b/i/solution">Solution</h6>

↑ **Parent:** [I](#3/a/ii/3/b/i)

The four index pairs give

$$
\sigma_z^0\sigma_x^0=I,\quad
\sigma_z^0\sigma_x^1=\sigma_x,\quad
\sigma_z^1\sigma_x^0=\sigma_z,\quad
\sigma_z\sigma_x=i\sigma_y.
$$

The last global phase cancels under conjugation. Hence the [Pauli channel](../../../quantum-information-theory.md#pauli-channel) probabilities are

$$
\boxed{p_0=p_{00},\qquad
p_x=p_{01},\qquad
p_y=p_{11},\qquad
p_z=p_{10}}.
$$

<h6 id="3/a/ii/3/b/ii">ii</h6>

↑ **Parent:** [B](#3/a/ii/3/b)

<h6 id="3/a/ii/3/b/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#3/a/ii/3/b/ii)

Conjugation by one [Pauli matrix](../../../algebra.md#pauli-matrices) preserves its parallel Bloch component and reverses the other two. Therefore

$$
\boxed{\begin{aligned}
r_x'&=(p_0+p_x-p_y-p_z)r_x
=[1-2(p_y+p_z)]r_x,\\
r_y'&=(p_0-p_x+p_y-p_z)r_y
=[1-2(p_x+p_z)]r_y,\\
r_z'&=(p_0-p_x-p_y+p_z)r_z
=[1-2(p_x+p_y)]r_z.
\end{aligned}}
$$

## 4

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The [trace distance](../../../quantum-theory.md#trace-distance) and [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states), in the unsquared convention, are

$$
\boxed{D(\rho,\sigma)=\frac12\|\rho-\sigma\|_1},
\qquad
\boxed{F(\rho,\sigma)
=\operatorname{Tr}\sqrt{\sqrt\rho\,\sigma\sqrt\rho}}.
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Let $\Delta=\rho-\sigma=\Delta_+-\Delta_-$ be the [positive-negative decomposition of a Hermitian operator](../../../hilbert-space.md#positive-negative-decomposition-of-a-hermitian-operator). Since $\operatorname{Tr}\Delta=0$,

$$
\operatorname{Tr}\Delta_+
=\operatorname{Tr}\Delta_-
=\frac12\|\Delta\|_1.
$$

For $0\leq P\leq I$,

$$
\operatorname{Tr}(P\Delta)
\leq\operatorname{Tr}(P\Delta_+)
\leq\operatorname{Tr}\Delta_+.
$$

Equality is attained by the projector onto the positive eigenspace of $\Delta$. This proves the [variational characterization of trace distance](../../../quantum-theory.md#variational-characterization-of-trace-distance)

$$
\boxed{D(\rho,\sigma)
=\max_{0\leq P\leq I}\operatorname{Tr}[P(\rho-\sigma)]}.
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

Distinct [Bell states](../../../bell-state.md) are orthogonal. For orthogonal pure states, the trace distance is one and the fidelity is the absolute overlap, zero. Hence

$$
\boxed{D(|\Phi^+\rangle,|\Psi^-\rangle)=1},
\qquad
\boxed{F(|\Psi^+\rangle,|\Phi^-\rangle)=0}.
$$

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

The difference $\tau=\rho_1-\rho_2$ determines

$$
\boxed{D(\rho_1,\rho_2)=\frac12\|\tau\|_1},
$$

so it suffices for trace distance.

It does not determine fidelity. For $0<t<1$, both pairs

$$
\rho_1=\begin{pmatrix}(1+t)/2&0\\0&(1-t)/2\end{pmatrix},
\quad
\rho_2=\begin{pmatrix}(1-t)/2&0\\0&(1+t)/2\end{pmatrix}
$$

and

$$
\rho_1'=\begin{pmatrix}t&0\\0&1-t\end{pmatrix},
\quad
\rho_2'=\begin{pmatrix}0&0\\0&1\end{pmatrix}
$$

have the same difference $\operatorname{diag}(t,-t)$. Their fidelities are respectively $\sqrt{1-t^2}$ and $\sqrt{1-t}$, which are generally unequal.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For the binary [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) $\{E,I-E\}$ and equal priors,

$$
p_{\rm succ}
=\frac12\operatorname{Tr}(E\rho_1)
+\frac12\operatorname{Tr}[(I-E)\rho_2]
=\frac12\left[1+\operatorname{Tr}E(\rho_1-\rho_2)\right].
$$

Maximizing with the [variational characterization of trace distance](../../../quantum-theory.md#variational-characterization-of-trace-distance) gives the equal-prior [Holevo–Helstrom theorem](../../../quantum-information-theory.md#holevo-helstrom-theorem)

$$
\boxed{p_{\rm succ}^{\max}
=\frac12[1+D(\rho_1,\rho_2)]}.
$$

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For priors $p_1,p_2$,

$$
p_{\rm succ}
=p_2+\operatorname{Tr}[E(p_1\rho_1-p_2\rho_2)].
$$

If $\Delta=p_1\rho_1-p_2\rho_2$, the maximum is $p_2+\operatorname{Tr}\Delta_+$. Since

$$
\operatorname{Tr}\Delta_+
=\frac12(\|\Delta\|_1+\operatorname{Tr}\Delta)
=\frac12(\|\Delta\|_1+p_1-p_2),
$$

one obtains

$$
\boxed{p_{\rm succ}^{\max}
=\frac12\left(1+\|p_1\rho_1-p_2\rho_2\|_1\right)}.
$$

## 5

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

The [generalized measurement postulate](../../../quantum-measurement.md#generalized-measurement-postulate) specifies operators $\{M_i\}$ satisfying

$$
\sum_iM_i^\dagger M_i=I.
$$

On state $\rho$, outcome $i$ has probability

$$
\boxed{p_i=\operatorname{Tr}(M_i^\dagger M_i\rho)},
$$

and, when $p_i>0$, conditional state

$$
\boxed{\rho_i=\frac{M_i\rho M_i^\dagger}{p_i}}.
$$

The effects $E_i=M_i^\dagger M_i$ form a [positive operator-valued measure](../../../quantum-measurement.md#positive-operator-valued-measure).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Introduce a [quantum ancilla](../../../quantum-information-theory.md#quantum-ancilla) with basis $|i\rangle$ and define

$$
V|\psi\rangle=\sum_iM_i|\psi\rangle\otimes|i\rangle.
$$

The completeness relation gives $V^\dagger V=I$, so $V$ is an [isometry](../../../riemannian-geometry.md#isometry) and extends to a [unitary operator](../../../vector-space.md#unitary-operator) on a sufficiently large system-plus-ancilla space. Prepare the ancilla in a fixed state, apply that unitary, and perform the projective measurement $\{I\otimes|i\rangle\langle i|\}$. Outcome $i$ has probability $\|M_i|\psi\rangle\|^2$ and leaves the system in the normalized state $M_i|\psi\rangle$. By linearity the same holds for mixed states, implementing the generalized measurement.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let

$$
|\theta^\perp\rangle=\sin\theta|0\rangle-\cos\theta|1\rangle,
\qquad
c=\frac1{1+\cos\theta}.
$$

The three effects

$$
\boxed{E_1=c|\theta^\perp\rangle\langle\theta^\perp|},
\qquad
\boxed{E_2=c|1\rangle\langle1|},
\qquad
\boxed{E_?=I-E_1-E_2}
$$

form a [POVM](../../../quantum-measurement.md#positive-operator-valued-measure), because the largest eigenvalue of the sum of the two rank-one projectors is $1+\cos\theta$. Outcome 1 never occurs on $|\theta\rangle$, while outcome 2 never occurs on $|0\rangle$. Thus conclusive outcomes are never wrong; $E_?$ records failure. This is [unambiguous quantum state discrimination](../../../quantum-theory.md#unambiguous-quantum-state-discrimination).

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Arrange the amplitudes of $|\phi_1\rangle$ as the matrix

$$
C_1=\begin{pmatrix}a&b\\c&d\end{pmatrix}.
$$

The second state has $C_2=C_1X$, where $X$ swaps the $A_2$ basis states. If Bob receives $A_1$, his two [reduced density matrices](../../../bell-state.md#reduced-density-matrix) are

$$
\rho_{A_1}^{(1)}=C_1C_1^\dagger,
\qquad
\rho_{A_1}^{(2)}=C_2C_2^\dagger
=C_1XX^\dagger C_1^\dagger,
$$

and are identical. No measurement on $A_1$ contains any information about the shared state.

If Bob instead receives $A_2$,

$$
\rho_{A_2}^{(1)}
=\begin{pmatrix}
a^2+c^2&ab+cd\\
ab+cd&b^2+d^2
\end{pmatrix},
\qquad
\rho_{A_2}^{(2)}=X\rho_{A_2}^{(1)}X.
$$

They differ because $a^2+c^2<b^2+d^2$. Bob can therefore distinguish them with better-than-random success. For equal priors,

$$
\boxed{D(\rho_{A_2}^{(1)},\rho_{A_2}^{(2)})
=b^2+d^2-a^2-c^2},
$$

so the optimal success probability is $\frac12(1+D)$. It is generally below one, so a single copy does not permit certain identification.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Discarding the outcome of the complete projective measurement gives

$$
\boxed{\sigma=\sum_iP_i\rho P_i}.
$$

For $m$ projectors, let $\omega=e^{2\pi i/m}$ and $U=\sum_j\omega^jP_j$. Then the pinching identity is

$$
\sigma=\frac1m\sum_{k=0}^{m-1}U^k\rho U^{-k}.
$$

The [Concavity of Von Neumann entropy](../../../von-neumann-entropy.md#concavity-of-von-neumann-entropy) and its invariance under [unitary operators](../../../vector-space.md#unitary-operator) imply

$$
\boxed{S(\sigma)\geq\frac1m\sum_kS(U^k\rho U^{-k})
=S(\rho)}.
$$

Equality holds exactly when every conjugate in the average is the same, equivalently

$$
\boxed{[\rho,P_i]=0\quad\hbox{for every }i}.
$$

**Thus equality holds when the input already has no coherence between distinct measurement subspaces.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
