# Paper 65

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_65.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_65.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
    - [1](#4/i/1)
      - [Solution](#4/i/1/solution)
    - [2](#4/i/2)
      - [Solution](#4/i/2/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)

## 1

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Set $X=\rho-\sigma$. The [trace distance](../../../quantum-theory.md#trace-distance) is $D(\rho,\sigma)=\tfrac12\|X\|_1$, where $\|X\|_1=\operatorname{Tr}\sqrt{X^\dagger X}$. Since $X$ is a [Hermitian operator](../../../hilbert-space.md#hermitian-operator), its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) is $X=\sum_jx_j|j\rangle\langle j|$. Define its [positive part of a Hermitian operator](../../../hilbert-space.md#positive-part-of-a-hermitian-operator) and [negative part of a Hermitian operator](../../../hilbert-space.md#negative-part-of-a-hermitian-operator) by

$$
Q=\sum_{x_j>0}x_j|j\rangle\langle j|,\qquad
R=\sum_{x_j<0}(-x_j)|j\rangle\langle j|.
$$

They are [positive semidefinite operators](../../../hilbert-space.md#positive-operator), satisfy $X=Q-R$ and $QR=0$, and obey $|X|=Q+R$. Therefore

$$
\boxed{D(\rho,\sigma)=\frac12(\operatorname{Tr}Q+\operatorname{Tr}R).}
$$

The states have equal trace, so $\operatorname{Tr}X=0$ and $\operatorname{Tr}Q=\operatorname{Tr}R=D(\rho,\sigma)$. This is the [spectral-parts formula for trace distance](../../../quantum-theory.md#spectral-parts-formula-for-trace-distance).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For every [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) $P$, positivity gives

$$
\operatorname{Tr}(PX)=\operatorname{Tr}(PQ)-\operatorname{Tr}(PR)
\leq\operatorname{Tr}(PQ)\leq\operatorname{Tr}Q.
$$

These inequalities do not require $P$ to commute with $Q$ or $R$: for example, $\operatorname{Tr}(PR)=\operatorname{Tr}(R^{1/2}PR^{1/2})\geq0$, and apply the same observation to $I-P$ and $Q$.

Let $P_+$ project onto the positive spectral subspace of $X$. Then $P_+Q=Q$ and $P_+R=0$, so $\operatorname{Tr}(P_+X)=\operatorname{Tr}Q=D(\rho,\sigma)$. Hence the [variational characterization of trace distance](../../../quantum-theory.md#variational-characterization-of-trace-distance) over projectors is

$$
\boxed{D(\rho,\sigma)=\max_{P=P^\dagger=P^2}\operatorname{Tr}[P(\rho-\sigma)].}
$$

One may include or exclude the zero eigenspace without changing the optimum.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The allowed operators are exactly the [positive contractions](../../../hilbert-space.md#positive-contraction) $0\leq T\leq I$, or binary measurement effects. As in (ii),

$$
\operatorname{Tr}(TX)=\operatorname{Tr}(TQ)-\operatorname{Tr}(TR)
\leq\operatorname{Tr}Q,
$$

because $\operatorname{Tr}(TR)\geq0$ and $\operatorname{Tr}[(I-T)Q]\geq0$. The positive-spectral [orthogonal projector](../../../hilbert-space.md#orthogonal-projection) $P_+$ is among these effects and attains the bound. Thus

$$
\boxed{D(\rho,\sigma)=\max_{0\leq T\leq I}\operatorname{Tr}[T(\rho-\sigma)].}
$$

Allowing general binary effects instead of projectors does not improve the optimal [trace distance](../../../quantum-theory.md#trace-distance) test.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Use the unsquared convention for [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states):

$$
F(\tau,\omega)=\operatorname{Tr}\sqrt{\sqrt\tau\,\omega\sqrt\tau}.
$$

Choose a [purification of a density operator](../../../quantum-theory.md#purification-of-a-density-operator) $|\Psi\rangle_{RA}$ of $\rho$, and put $\tau_{RA}=(\operatorname{id}_R\otimes\Lambda)(|\Psi\rangle\langle\Psi|)$. By definition,

$$
F_e(\rho,\Lambda)=\langle\Psi|\tau_{RA}|\Psi\rangle
=F(|\Psi\rangle\langle\Psi|,\tau_{RA})^2.
$$

The [monotonicity of quantum fidelity under partial trace](../../../quantum-information-theory.md#monotonicity-of-quantum-fidelity-under-partial-trace) follows from [Uhlmann's theorem](../../../quantum-theory.md#uhlmann-s-theorem): maximizing purifications of two joint states are also candidate purifications of their marginals, with the discarded subsystem included in the purifying system. The optimization for the marginals therefore cannot give a smaller overlap. Here those marginals are $\rho$ and $\Lambda(\rho)$. Consequently

$$
\boxed{F_e(\rho,\Lambda)\leq F(\rho,\Lambda(\rho))^2.}
$$

This [entanglement fidelity bound by state fidelity](../../../quantum-information-theory.md#entanglement-fidelity-bound-by-state-fidelity) distinguishes preserving a reference entanglement from merely reproducing the input marginal.

## 2

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The $+1$ measurement effect of the [Pauli operator](../../../quantum-circuit.md#pauli-operator) $\sigma_x$ is $P_+=(I+\sigma_x)/2$. The [Born rule](../../../quantum-mechanics.md#born-rule) and the [Bloch vector](../../../quantum-theory.md#bloch-vector) representation give

$$
\Pr(+1)=\operatorname{Tr}(\rho P_+)=\frac{1+s_x}{2}
=\boxed{\frac34}.
$$

The other two [Bloch vector](../../../quantum-theory.md#bloch-vector) components do not enter this [projective measurement](../../../quantum-measurement.md#projective-measurement) probability.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

In the [computational basis](../../../quantum-theory.md#computational-basis), write

$$
\rho=\frac12\begin{pmatrix}1+s_z&s_x-is_y\\s_x+is_y&1-s_z\end{pmatrix}.
$$

The [Kraus representation](../../../quantum-information-theory.md#kraus-representation) of the [amplitude damping channel](../../../quantum-information-theory.md#amplitude-damping-channel) gives

$$
\Lambda(\rho)=\begin{pmatrix}
\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\
\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}
\end{pmatrix}.
$$

Reading off its [Bloch vector](../../../quantum-theory.md#bloch-vector) gives the [Bloch-vector map of amplitude damping](../../../quantum-information-theory.md#bloch-vector-map-of-amplitude-damping):

$$
\boxed{(s_x,s_y,s_z)\longmapsto
\left(\sqrt{1-p}\,s_x,\sqrt{1-p}\,s_y,p+(1-p)s_z\right).}
$$

Here $0\leq p\leq1$. The shift in $s_z$ shows that this [quantum channel](../../../quantum-information-theory.md#quantum-channel) is not unital unless $p=0$; its fixed ground state lies at the north pole, rather than the center of the [Bloch sphere](../../../quantum-theory.md#bloch-sphere).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Iterating the [Bloch-vector map of amplitude damping](../../../quantum-information-theory.md#bloch-vector-map-of-amplitude-damping) gives

$$
s_x^{(n)}=(1-p)^{n/2}s_x,\qquad
s_y^{(n)}=(1-p)^{n/2}s_y,\qquad
s_z^{(n)}=1-(1-p)^n(1-s_z).
$$

Therefore

$$
\boxed{\lim_{n\to\infty}\mathbf s^{(n)}=(0,0,1)\quad\text{for }0<p\leq1.}
$$

The [repeated amplitude damping limit](../../../quantum-information-theory.md#repeated-amplitude-damping-limit) describes irreversible relaxation of the excited state $|1\rangle$ into the ground state $|0\rangle$, with energy transferred to the environment and no compensating thermal excitation. At $p=1$, the ground state is reached in one action. At the endpoint $p=0$, the [quantum channel](../../../quantum-information-theory.md#quantum-channel) is the identity and the initial [Bloch vector](../../../quantum-theory.md#bloch-vector) remains unchanged; the ground-state conclusion requires nonzero damping.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

For [Kraus operators](../../../quantum-information-theory.md#kraus-operator) $A_j$, the [Kraus formula for entanglement fidelity](../../../quantum-information-theory.md#kraus-formula-for-entanglement-fidelity) is

$$
F_e(\rho,\Lambda)=\sum_j|\operatorname{Tr}(\rho A_j)|^2.
$$

Indeed each Kraus contribution to the purified-state overlap is $|\langle\Psi|(I\otimes A_j)|\Psi\rangle|^2$, and the expectation in a purification is $\operatorname{Tr}(\rho A_j)$. In this case,

$$
\operatorname{Tr}(\rho A_1)=\frac{1+s_z+\sqrt{1-p}(1-s_z)}2,\qquad
\operatorname{Tr}(\rho A_2)=\frac{\sqrt p}{2}(s_x+is_y).
$$

The [entanglement fidelity of amplitude damping](../../../quantum-information-theory.md#entanglement-fidelity-of-amplitude-damping) is thus

$$
\boxed{F_e(\rho,\Lambda)=\frac14\left[1+s_z+\sqrt{1-p}(1-s_z)\right]^2
+\frac p4(s_x^2+s_y^2).}
$$

For $p=0$, this is one. For a ground-state input it is one for every $p$, whereas for an excited-state input it is $1-p$. These checks agree with the physical relaxation mechanism.

## 3

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use base-two logarithms throughout, so information and entropy are in bits. The [relative entropy](../../../probability-and-statistics.md#kullback-leibler-divergence) of classical probability distributions is

$$
D(p\|q)=\sum_{x:p(x)>0}p(x)\log_2\frac{p(x)}{q(x)}.
$$

Set $0\log_2(0/q)=0$; if $p(x)>0$ and $q(x)=0$, define the value to be $+\infty$. In the finite case, $\ln u\leq u-1$ gives

$$
\begin{aligned}
(\ln2)D(p\|q)
&=-\sum_{x\in\operatorname{supp}p}p(x)\ln\frac{q(x)}{p(x)}\\
&\geq\sum_{x\in\operatorname{supp}p}[p(x)-q(x)]
=1-q(\operatorname{supp}p)\geq0.
\end{aligned}
$$

Hence **$D(p\|q)\geq0$**, with equality exactly when $p=q$: equality in the logarithm inequality requires $q(x)=p(x)$ on the support, and equality in the last step leaves no mass outside it.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy) is $S(\rho\|\sigma)=\operatorname{Tr}\rho(\log_2\rho-\log_2\sigma)$ when the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) $\rho$ is contained in that of $\sigma$, and $+\infty$ otherwise. Write spectral decompositions $\rho=\sum_i r_i|i\rangle\langle i|$ and $\sigma=\sum_j t_j|u_j\rangle\langle u_j|$, and set $q_i=\langle i|\sigma|i\rangle$.

The weights $w_{ij}=|\langle i|u_j\rangle|^2$ sum to one. Concavity of the scalar logarithm gives the [diagonal logarithm concavity bound](../../../vector-space.md#diagonal-logarithm-concavity-bound)

$$
\langle i|\log_2\sigma|i\rangle
=\sum_jw_{ij}\log_2t_j
\leq\log_2\left(\sum_jw_{ij}t_j\right)=\log_2q_i.
$$

For $r_i>0$, support inclusion removes overlaps with zero eigenvalues of $\sigma$; alternatively take a positive regularization and pass to the limit. The two diagonal vectors $r$ and $q$ are probability distributions. Therefore

$$
\boxed{S(\rho\|\sigma)\geq\sum_i r_i\log_2\frac{r_i}{q_i}
=D(r\|q)\geq0.}
$$

This proves [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) without assuming the states commute. Equality in the strict logarithmic concavity condition makes each occupied $|i\rangle$ an eigenvector of $\sigma$; classical equality gives $q_i=r_i$ and no weight outside the support, hence equality occurs exactly for $\rho=\sigma$.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

A deterministic quantum operation here is a [CPTP map](../../../quantum-information-theory.md#quantum-channel). By [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation), there is an [isometry](../../../riemannian-geometry.md#isometry) $V:B\to B'E$ with $\Lambda(\tau)=\operatorname{Tr}_E(V\tau V^\dagger)$. Let $\omega_{AB'E}=(I\otimes V)\rho_{AB}(I\otimes V^\dagger)$. An [isometry](../../../riemannian-geometry.md#isometry) preserves all nonzero eigenvalues, so

$$
I(A:B'E)_\omega=I(A:B)_\rho.
$$

The [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) is $I(A:B)=S(A)+S(B)-S(AB)$. The difference after discarding the environment is

$$
\begin{aligned}
I(A:B'E)_\omega-I(A:B')_\omega
&=S(AB')+S(B'E)-S(B')-S(AB'E)\\
&=I(A:E\mid B')_\omega\geq0,
\end{aligned}
$$

where the last inequality is [Strong subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#strong-subadditivity-of-quantum-entropy), in the form $S(AB')+S(B'E)\geq S(B')+S(AB'E)$. Thus [data processing for quantum mutual information](../../../von-neumann-entropy.md#data-processing-for-quantum-mutual-information) gives

$$
\boxed{I(A':B')\leq I(A:B).}
$$

Subsystem $A$ is unchanged; its prime simply labels the output. Keeping the environment would preserve the mutual information, while tracing it out cannot increase it.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Put $u=\varepsilon/2$. The state is well defined for $0\leq\varepsilon\leq2$, with eigenvalues $1-u,u$. The first state is pure and has zero [Von Neumann entropy](../../../von-neumann-entropy.md), so the exact difference is

$$
\boxed{|S(\rho)-S(\sigma)|=h_2(\varepsilon/2),\qquad
h_2(u)=-u\log_2u-(1-u)\log_2(1-u).}
$$

This is the [entropy of a binary diagonal qubit mixture](../../../von-neumann-entropy.md#entropy-of-a-binary-diagonal-qubit-mixture). Its [trace distance](../../../quantum-theory.md#trace-distance) from the [pure state](../../../quantum-theory.md#pure-state) is $u$, not $\varepsilon$. An explicit elementary upper bound follows from $-(1-u)\ln(1-u)\leq u$:

$$
\boxed{|S(\rho)-S(\sigma)|\leq
\min\left\{1,\frac{\varepsilon}{2}\log_2\frac{2e}{\varepsilon}\right\}
\quad(0<\varepsilon\leq2).}
$$

At zero the limit is zero. For small $\varepsilon$, the sharp exact answer behaves as $(\varepsilon/2)\log_2(2/\varepsilon)+\varepsilon/(2\ln2)+O(\varepsilon^2)$, displaying the logarithmic continuity of entropy near a [pure state](../../../quantum-theory.md#pure-state).

## 4

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For a finite-dimensional memoryless [quantum channel](../../../quantum-information-theory.md#quantum-channel) $\Lambda$, the [Holevo-Schumacher-Westmoreland theorem](../../../quantum-information-theory.md#holevo-schumacher-westmoreland-theorem) identifies its [product-state classical capacity](../../../quantum-information-theory.md#holevo-capacity) with the optimized output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity):

$$
\boxed{C_{\rm prod}(\Lambda)=\chi^*(\Lambda)
=\max_{\{p_x,\rho_x\}}
\left[S\left(\sum_xp_x\Lambda(\rho_x)\right)-\sum_xp_xS(\Lambda(\rho_x))\right].}
$$

With product codewords and a collective measurement on the outputs, every rate below this value is achievable with vanishing error; no larger rate can be reliable under that product-input restriction. For a fixed classical-quantum output alphabet the corresponding optimized entropy difference gives its classical coding capacity. If entangled inputs across channel uses are also allowed, the general unassisted capacity is the regularized value $C(\Lambda)=\lim_{n\to\infty}n^{-1}\chi^*(\Lambda^{\otimes n})$. The requested calculation below concerns the single-use optimized product-input expression, so no unproved additivity assumption is needed.

<h4 id="4/i/1">1</h4>

↑ **Parent:** [I](#4/i)

<h5 id="4/i/1/solution">Solution</h5>

↑ **Parent:** [1](#4/i/1)

Conjugation by a [Pauli operator](../../../quantum-circuit.md#pauli-operator) preserves its matching [Bloch vector](../../../quantum-theory.md#bloch-vector) component and reverses the other two. Summing all three conjugations therefore sends $\mathbf s$ to $-\mathbf s$. The specified [quantum depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel) has retention factor

$$
\eta=p-\frac{1-p}{3}=\frac{4p-1}{3},\qquad
\mathbf s\longmapsto\eta\mathbf s.
$$

This [Pauli-mixture parametrization of qubit depolarization](../../../quantum-information-theory.md#pauli-mixture-parametrization-of-qubit-depolarization) differs from a convention in which $p$ itself is the retention factor. For $0\leq p\leq1$, $-1/3\leq\eta\leq1$. A pure input gives output eigenvalues $(1\pm|\eta|)/2$, and hence entropy $h_2((1+\eta)/2)$ by symmetry of [binary entropy](../../../information-theory.md#binary-entropy). Mixed inputs have a smaller output radius and at least this much entropy. Every average output has entropy at most one. Thus

$$
\chi(\mathcal E_{\rm out})\leq1-h_2\left(\frac{1+\eta}{2}\right).
$$

Two equiprobable orthogonal pure inputs have antipodal output [Bloch vectors](../../../quantum-theory.md#bloch-vector), maximally mixed average output, and this same minimal individual output entropy. They attain the bound. Applying the coding theorem gives

$$
\boxed{C_{\rm prod}(\Lambda)=1-h_2\left(\frac{2p+1}{3}\right)
\quad\text{bits per channel use}.}
$$

At $p=1$ it is one; at $p=1/4$ it is zero; at $p=0$ it is $1-h_2(1/3)\simeq0.0817$. Negative retention reverses the labels of the two signals but does not eliminate their distinguishability.

<h4 id="4/i/2">2</h4>

↑ **Parent:** [I](#4/i)

<h5 id="4/i/2/solution">Solution</h5>

↑ **Parent:** [2](#4/i/2)

Encode the ensemble label in an orthogonal classical register:

$$
\omega_{XB}=\sum_xp_x|x\rangle\langle x|\otimes\rho_x.
$$

The [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state) has $S(XB)=H(p)+\sum_xp_xS(\rho_x)$, $S(X)=H(p)$ and $S(B)=S(\bar\rho)$, where $\bar\rho=\sum_xp_x\rho_x$. Hence

$$
I(X:B)_\omega=S(\bar\rho)-\sum_xp_xS(\rho_x)=\chi(\mathcal E).
$$

Applying $\operatorname{id}_X\otimes\Lambda$ changes the conditional states to the output ensemble. The same identity gives $I(X:B')=\chi(\mathcal E')$. [Data processing for quantum mutual information](../../../von-neumann-entropy.md#data-processing-for-quantum-mutual-information), proved in Question 3, therefore yields the [Holevo quantity under a quantum channel](../../../quantum-information-theory.md#holevo-quantity-under-a-quantum-channel):

$$
\boxed{\chi(\mathcal E')\leq\chi(\mathcal E).}
$$

This concerns the information available in the whole ensemble, not the change in the entropy of each individual state.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Diagonalize the source average $\pi=\sum_j\lambda_j|j\rangle\langle j|$, using its positive eigenvalues. For fixed $\delta>0$, let $\Pi_{n,\delta}$ project onto product eigenvectors whose eigenvalues obey

$$
2^{-n(S(\pi)+\delta)}\leq\lambda_{j_1}\cdots\lambda_{j_n}
\leq2^{-n(S(\pi)-\delta)}.
$$

The [typical subspace theorem](../../../quantum-information-theory.md#typical-subspace-theorem) states that, for every $\epsilon>0$ and all sufficiently large $n$,

$$
\operatorname{Tr}(\pi^{\otimes n}\Pi_{n,\delta})\geq1-\epsilon,
$$



$$
2^{-n(S(\pi)+\delta)}\Pi_{n,\delta}
\leq\Pi_{n,\delta}\pi^{\otimes n}\Pi_{n,\delta}
\leq2^{-n(S(\pi)-\delta)}\Pi_{n,\delta},
$$



$$
(1-\epsilon)2^{n(S(\pi)-\delta)}
\leq\dim\mathcal T_{n,\delta}\leq2^{n(S(\pi)+\delta)}.
$$

The probability statement is the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) applied to $-\log_2\lambda_j$; the dimension bounds follow by summing the typical eigenvalue bounds. This explains why the [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace) retains almost all probability using about $nS(\pi)$ qubits.

For $R>S(\pi)$ choose $0<\delta<R-S(\pi)$. Measure $\{\Pi_{n,\delta},I-\Pi_{n,\delta}\}$. On success, encode the projected state isometrically into a space of dimension $\dim\mathcal T_{n,\delta}$; on failure, output a separate fixed flag. Decode the successful sector by the inverse [isometry](../../../riemannian-geometry.md#isometry), and map the flag to a fixed state $|\varphi_0\rangle$. The compressed dimension is at most $2^{n(S(\pi)+\delta)}+1$, hence fits within rate $R$ for all sufficiently large $n$. Both maps are trace-preserving [quantum channels](../../../quantum-information-theory.md#quantum-channel), not merely successful postselected operations.

Writing $\Pi=\Pi_{n,\delta}$, the composite channel is

$$
\mathcal N_n(\tau)=\Pi\tau\Pi+
\operatorname{Tr}[(I-\Pi)\tau]|\varphi_0\rangle\langle\varphi_0|.
$$

For a pure source signal $|\Psi_k\rangle$, set $a_k=\langle\Psi_k|\Pi|\Psi_k\rangle$. Its squared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) after the composite channel is at least $a_k^2$. Since the source is memoryless, its average state on $n$ uses is $\pi^{\otimes n}$. Convexity of the square gives

$$
\sum_kp_k^{(n)}\langle\Psi_k|\mathcal N_n(|\Psi_k\rangle\langle\Psi_k|)|\Psi_k\rangle
\geq\sum_kp_k^{(n)}a_k^2
\geq\left[\operatorname{Tr}(\pi^{\otimes n}\Pi)\right]^2
\geq(1-\epsilon)^2.
$$

The [Kraus formula for entanglement fidelity](../../../quantum-information-theory.md#kraus-formula-for-entanglement-fidelity) gives the same lower bound for $F_e(\pi^{\otimes n},\mathcal N_n)$, because one [Kraus operator](../../../quantum-information-theory.md#kraus-operator) is $\Pi$ and the other terms are nonnegative. Taking $\epsilon\to0$ proves **reliable compression at every $R>S(\pi)$**, in both average pure-signal fidelity and the stronger entanglement-fidelity sense. This is [typical-subspace compression with a failure flag](../../../quantum-information-theory.md#typical-subspace-compression-with-a-failure-flag).

## 5

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The [Bell basis](../../../quantum-theory.md#bell-basis) consists of

$$
|\Phi^\pm\rangle=\frac{|00\rangle\pm|11\rangle}{\sqrt2},\qquad
|\Psi^\pm\rangle=\frac{|01\rangle\pm|10\rangle}{\sqrt2}.
$$

Let $Z=\sigma_z$, $X=\sigma_x$. The [Pauli operators](../../../quantum-circuit.md#pauli-operator) $Z\otimes Z$ and $X\otimes X$ commute: each of the two local anticommutations contributes a minus sign, so they cancel. Their eigenvalue table is

$$
\begin{array}{c|cc|cc}
\text{state}&Z\otimes Z&X\otimes X&\text{parity bit}&\text{phase bit}\\\hline
\Phi^+&+1&+1&0&0\\
\Phi^-&+1&-1&0&1\\
\Psi^+&-1&+1&1&0\\
\Psi^-&-1&-1&1&1
\end{array}
$$

To make the bit values literally zero or one rather than signed eigenvalues, the commuting [Bell parity and phase observables](../../../quantum-theory.md#bell-parity-and-phase-observables) are

$$
\boxed{B_{\rm parity}=\frac{I-Z\otimes Z}{2},\qquad
B_{\rm phase}=\frac{I-X\otimes X}{2}.}
$$

They distinguish all four states jointly. The parity bit records whether the computational bits agree; the phase bit records the relative sign.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Apply a [Hadamard gate](../../../quantum-theory.md#hadamard-gate) to qubit $A$, followed by a [controlled-NOT gate](../../../quantum-theory.md#controlled-not-gate) with $A$ controlling $B$. The resulting [Bell-basis conversion circuit](../../../quantum-theory.md#bell-basis-conversion-circuit) is $U=\operatorname{CNOT}(H\otimes I)$ and gives

$$
U|ij\rangle=\frac{|0j\rangle+(-1)^i|1,j\oplus1\rangle}{\sqrt2}.
$$

Thus $00,01,10,11$ map respectively to $\Phi^+,\Psi^+,\Phi^-,\Psi^-$. The first input bit becomes the phase bit and the second becomes the parity bit.

Both gates are self-inverse, but inversion of their product reverses the order:

$$
\boxed{U^{-1}=U^\dagger=(H\otimes I)\operatorname{CNOT}.}
$$

So **the same two gates convert the [Bell basis](../../../quantum-theory.md#bell-basis) back to the [computational basis](../../../quantum-theory.md#computational-basis) when applied in reverse order**: first the controlled-NOT, then the Hadamard. Using the forward order twice does not generally work, since these gates do not commute. For example, $U|\Phi^+\rangle=(|00\rangle+|01\rangle-|10\rangle+|11\rangle)/2$, which is not a computational-basis state.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Write a bipartite [pure state](../../../quantum-theory.md#pure-state) in fixed product bases as $|\psi\rangle=\sum_{ij}M_{ij}|i\rangle|j\rangle$. The [Schmidt decomposition theorem](../../../von-neumann-entropy.md#schmidt-decomposition), equivalently the [singular value decomposition](../../../linear-algebra.md#singular-value-decomposition) of $M$, says that its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) equals $\operatorname{rank}M$. A branch of local operations is a product operator $A\otimes B$, so its coefficient matrix is

$$
M'=AMB^{\mathsf T}.
$$

The elementary rank inequality $\operatorname{rank}(AMB^{\mathsf T})\leq\operatorname{rank}M$ proves [Schmidt-rank contraction under product operators](../../../von-neumann-entropy.md#schmidt-rank-contraction-under-product-operators). Normalizing a nonzero branch does not change matrix rank.

For an adaptive [LOCC](../../../bell-state.md#local-operations-and-classical-communication) protocol, a complete classical transcript selects one local [Kraus operator](../../../quantum-information-theory.md#kraus-operator) at each stage. Multiplying the local operators along that transcript still gives one product $A_t\otimes B_t$. Consequently

$$
\boxed{\operatorname{Schmidt\ rank}(\psi_t)\leq
\operatorname{Schmidt\ rank}(\psi)\quad\text{in every nonzero branch}.}
$$

Classical communication changes which product operator is chosen, not this rank bound. If the overall output is a [pure state](../../../quantum-theory.md#pure-state), every nonzero branch must be proportional to that same vector, so its [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) also cannot increase. If the outcome is discarded and the output is mixed, pure-state [Schmidt rank](../../../von-neumann-entropy.md#schmidt-rank) is not defined; the induced decomposition instead shows that its [Schmidt number](../../../von-neumann-entropy.md#schmidt-number) is at most the original rank. This includes probabilistic filtering as well as deterministic pure-state conversion.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

The final printed direction is reversed under the [majorization](../../../vector-space.md#majorization) convention stated in the same part. A completely depolarizing [unital quantum channel](../../../quantum-information-theory.md#unital-quantum-channel) sends a pure qubit state to $I/2$, giving spectra $r=(1,0)$ and $s=(1/2,1/2)$. The proposed $r\prec s$ fails already at the first partial sum, since $1>1/2$. The valid conclusion is

$$
\boxed{s\prec r.}
$$

Here is its general proof. Choose eigenbases $\rho=\sum_i r_i|u_i\rangle\langle u_i|$ and $\sigma=\sum_j s_j|v_j\rangle\langle v_j|$, and define the [eigenvalue mixing matrix of a unital quantum channel](../../../quantum-information-theory.md#eigenvalue-mixing-matrix-of-a-unital-quantum-channel)

$$
A_{ji}=\langle v_j|\Lambda(|u_i\rangle\langle u_i|)|v_j\rangle.
$$

Its entries are nonnegative by positivity. Trace preservation gives $\sum_jA_{ji}=1$ for every column. Unitality gives $\sum_iA_{ji}=\langle v_j|\Lambda(I)|v_j\rangle=1$ for every row. Thus $A$ is a [doubly stochastic matrix](../../../vector-space.md#doubly-stochastic-matrix), and linearity gives

$$
s_j=\sum_iA_{ji}r_i,\qquad s=Ar.
$$

The supplied doubly stochastic characterization of [majorization](../../../vector-space.md#majorization) then yields $s\prec r$, completing the intended corrected result. This proves [spectral majorization under a unital quantum channel](../../../quantum-information-theory.md#spectral-majorization-under-a-unital-quantum-channel). A [unital quantum channel](../../../quantum-information-theory.md#unital-quantum-channel) can make a spectrum more uniform; it cannot generally make the output spectrum majorize the input. The counterexample resolves the false printed assertion rather than treating the reversed inequality as a convention change.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
