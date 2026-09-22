# Paper 323

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_323.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_323.pdf)

All entropies and information rates below use base-two [logarithms](../../../calculus.md#logarithm). The [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) uses the unsquared convention.

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
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [a](#2/i/a)
      - [Solution](#2/i/a/solution)
    - [b](#2/i/b)
      - [Solution](#2/i/b/solution)
  - [ii](#2/ii)
    - [a](#2/ii/a)
      - [Solution](#2/ii/a/solution)
    - [b](#2/ii/b)
      - [Solution](#2/ii/b/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
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

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A bipartite [density operator](../../../quantum-theory.md#density-matrix) $\rho_{AB}$ has [positive partial transpose](../../../quantum-information-theory.md#positive-partial-transpose) when $\rho_{AB}^{T_B}\geq0$ in a product basis. Positivity is independent of the choice of local bases, although the matrix representing the [partial transpose](../../../quantum-information-theory.md#partial-transpose) changes.

If the state is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state), write $\rho_{AB}=\sum_jp_j\rho_j^A\otimes\rho_j^B$. Taking its [partial transpose](../../../quantum-information-theory.md#partial-transpose) gives

$$
\rho_{AB}^{T_B}=\sum_jp_j\rho_j^A\otimes(\rho_j^B)^T\geq0.
$$

Indeed, the [matrix transpose](../../../vector-space.md#transpose) preserves the nonnegative [eigenvalues](../../../linear-operator-theory.md#eigenvalue) of each local [density operator](../../../quantum-theory.md#density-matrix); a [tensor product](../../../linear-algebra.md#tensor-product) of [positive semidefinite operators](../../../hilbert-space.md#positive-operator) is positive, and so is their nonnegative sum. This proves the necessary direction of the [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use two precise finite-dimensional results. The [positive-map separability criterion](../../../quantum-information-theory.md#positive-map-separability-criterion) says that a state on $\mathbb C^2\otimes\mathbb C^3$ is separable exactly when $(\operatorname{id}_2\otimes\Phi)(\sigma)\geq0$ for every [positive linear map](../../../quantum-information-theory.md#positive-linear-map) $\Phi:M_3(\mathbb C)\to M_2(\mathbb C)$. The [Størmer-Woronowicz decomposability theorem](../../../quantum-information-theory.md#stormer-woronowicz-decomposability-theorem) says that every such map is a [decomposable positive map](../../../quantum-information-theory.md#decomposable-positive-map), so

$$
\Phi=\Phi_1+\Phi_2\circ T,
$$

with $\Phi_1,\Phi_2$ [completely positive maps](../../../quantum-information-theory.md#completely-positive-map) and $T$ the [matrix transpose](../../../vector-space.md#transpose) on $M_3$.

If $\sigma$ has [positive partial transpose](../../../quantum-information-theory.md#positive-partial-transpose), both $\sigma$ and $\sigma^{T_B}$ are positive. Hence

$$
(\operatorname{id}_2\otimes\Phi)(\sigma)
=(\operatorname{id}_2\otimes\Phi_1)(\sigma)
+(\operatorname{id}_2\otimes\Phi_2)(\sigma^{T_B})\geq0.
$$

The [positive-map separability criterion](../../../quantum-information-theory.md#positive-map-separability-criterion) now proves that $\sigma$ is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). The dimension-specific decomposability theorem is essential: the conclusion does not extend to arbitrary bipartite dimensions.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [partial transpose](../../../quantum-information-theory.md#partial-transpose) of the [spin singlet state](../../../bell-state.md#spin-singlet-state) projector is the [Hermitian operator](../../../hilbert-space.md#hermitian-operator)

$$
W=\frac12\left(|01\rangle\langle01|+|10\rangle\langle10|
-|00\rangle\langle11|-|11\rangle\langle00|\right)
=\frac I2-|\Phi^+\rangle\langle\Phi^+|.
$$

For every [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state) $\tau$, the [positive partial transpose criterion](../../../quantum-information-theory.md#positive-partial-transpose-criterion) and the [trace-adjoint identity for partial transpose](../../../quantum-information-theory.md#trace-adjoint-identity-for-partial-transpose) give

$$
\operatorname{Tr}(W\tau)
=\operatorname{Tr}(\Psi_-\tau^{T_B})
=\langle\Psi^-|\tau^{T_B}|\Psi^-\rangle\geq0.
$$

For the specified [Bell state](../../../bell-state.md), however,

$$
\boxed{\operatorname{Tr}\left(W|\Phi^+\rangle\langle\Phi^+|\right)=-\frac12}.
$$

Thus $W$ is an [entanglement witness](../../../quantum-information-theory.md#entanglement-witness) detecting $|\Phi^+\rangle$. In fact, it detects any state whose overlap with that [Bell state](../../../bell-state.md) exceeds $1/2$.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Use the normalized [Choi state](../../../quantum-information-theory.md#choi-state) $C_\Lambda=(\Lambda\otimes\operatorname{id})(|\Phi_d\rangle\langle\Phi_d|)$, with $|\Phi_d\rangle=d^{-1/2}\sum_i|ii\rangle$. If $\Lambda$ is an [entanglement-breaking channel](../../../quantum-information-theory.md#entanglement-breaking-channel), its action on this particular bipartite input makes $C_\Lambda$ a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state).

Conversely, suppose $C_\Lambda=\sum_ap_a\sigma_a\otimes\tau_a$, with local [density operators](../../../quantum-theory.md#density-matrix) $\sigma_a,\tau_a$. The [Choi reconstruction formula](../../../quantum-information-theory.md#choi-reconstruction-formula) gives

$$
\Lambda(X)=d\operatorname{Tr}_B\left[C_\Lambda(I\otimes X^T)\right]
=\sum_a\operatorname{Tr}(E_aX)\sigma_a,\qquad E_a=dp_a\tau_a^T\geq0.
$$

Because $\Lambda$ is trace preserving, $\operatorname{Tr}_A C_\Lambda=I/d$, so $\sum_aE_a=I$. Thus the $E_a$ form a [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) and the channel is a [measure-and-prepare channel](../../../quantum-information-theory.md#measure-and-prepare-channel).

For any bipartite input $\rho_{AR}$, define the positive, possibly unnormalized reference operators

$$
R_a=\operatorname{Tr}_A\left[(\sqrt{E_a}\otimes I)\rho_{AR}(\sqrt{E_a}\otimes I)\right].
$$

Its output is $\sum_a\sigma_a\otimes R_a$. Since $\sum_a\operatorname{Tr}R_a=1$, normalizing each nonzero $R_a$ expresses this as a [convex combination](../../../mathematical-optimization.md#convex-combination) of [product states](../../../bell-state.md#product-state). Hence every output is separable, proving the [separable Choi-state criterion for entanglement breaking](../../../quantum-information-theory.md#separable-choi-state-criterion-for-entanglement-breaking).

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

Apply the [measure-and-prepare channel](../../../quantum-information-theory.md#measure-and-prepare-channel) locally to an arbitrary bipartite [density operator](../../../quantum-theory.md#density-matrix) $\rho_{AR}$. The resulting state is

$$
(\Lambda\otimes\operatorname{id}_R)(\rho_{AR})=\sum_a\sigma_a\otimes R_a,
$$

where

$$
R_a=\operatorname{Tr}_A\left[(\sqrt{E_a}\otimes I)\rho_{AR}(\sqrt{E_a}\otimes I)\right]\geq0.
$$

To see that this is the correct output, the [partial trace](../../../quantum-theory.md#partial-trace) is cyclic for operators acting only on the traced subsystem, so the displayed expression equals $\operatorname{Tr}_A[(E_a\otimes I)\rho_{AR}]$. Put $q_a=\operatorname{Tr}R_a$. The [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) completeness relation implies $\sum_aq_a=1$, and terms with $q_a=0$ vanish. Therefore

$$
(\Lambda\otimes\operatorname{id}_R)(\rho_{AR})
=\sum_{a:q_a>0}q_a\sigma_a\otimes\frac{R_a}{q_a}
$$

is a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state). Thus the channel is an [entanglement-breaking channel](../../../quantum-information-theory.md#entanglement-breaking-channel), for every reference-system dimension.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Expanding the normalized [maximally entangled state](../../../quantum-theory.md#maximally-entangled-state) in the definition of the [Choi state](../../../quantum-information-theory.md#choi-state) gives

$$
C_{\widetilde\Lambda}
=\frac1d\sum_{k,\ell}\widetilde\Lambda(|k\rangle\langle\ell|)\otimes|k\rangle\langle\ell|
=\boxed{\sum_jp_j|a_j\rangle\langle a_j|\otimes|\overline{b_j}\rangle\langle\overline{b_j}|}.
$$

Here the bar denotes componentwise [complex conjugation](../../../complex-analysis.md#complex-conjugation) in the basis defining the [Choi state](../../../quantum-information-theory.md#choi-state). Every term is a positive [tensor-product operator](../../../linear-algebra.md#tensor-product-operator), and the whole operator has trace one because $\widetilde\Lambda$ is assumed to be a [quantum channel](../../../quantum-information-theory.md#quantum-channel). It is therefore a [separable quantum state](../../../quantum-information-theory.md#separable-quantum-state), proving entanglement breaking by the [separable Choi-state criterion for entanglement breaking](../../../quantum-information-theory.md#separable-choi-state-criterion-for-entanglement-breaking).

If the vectors are unit vectors, the displayed $p_j$ are already the product-state weights. If they are not normalized, absorb their squared norms into the weights and normalize the nonzero vectors. Trace preservation requires

$$
d\sum_jp_j\lVert a_j\rVert^2|b_j\rangle\langle b_j|=I;
$$

the probability-distribution condition alone would not guarantee this. Equivalently, the [Kraus operators](../../../quantum-information-theory.md#kraus-operator) are $K_j=\sqrt{dp_j}|a_j\rangle\langle b_j|$, exhibiting the [rank-one Kraus representation of an entanglement-breaking channel](../../../quantum-information-theory.md#rank-one-kraus-representation-of-an-entanglement-breaking-channel).

## 2

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/a">a</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/a/solution">Solution</h5>

↑ **Parent:** [A](#2/i/a)

Use base-two [logarithms](../../../calculus.md#logarithm). The [weakly typical sequence](../../../information-theory.md#weakly-typical-sequence) definition is

$$
\boxed{\left|-\frac1n\log_2p(x^n)-H(X)\right|\leq\varepsilon},\qquad
p(x^n)=\prod_{j=1}^np(x_j).
$$

Equivalently, $2^{-n(H(X)+\varepsilon)}\leq p(x^n)\leq2^{-n(H(X)-\varepsilon)}$. By the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) applied to the [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) $-\log_2p(X_j)$, the probability of this [typical set](../../../information-theory.md#typical-set) tends to one.

This captures the usual probability scale of a long sample, but it need not make every symbol frequency representative. For a fair binary source, every word has probability $2^{-n}$ and $H(X)=1$, so even the all-zero word is weakly typical. The [strongly typical sequence](../../../information-theory.md#strongly-typical-sequence) definition additionally controls empirical symbol frequencies and excludes this word for small tolerance. Thus weak typicality agrees with the high-probability-set intuition, while allowing individually unrepresentative members.

<h4 id="2/i/b">b</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/b/solution">Solution</h5>

↑ **Parent:** [B](#2/i/b)

Every member of the [typical set](../../../information-theory.md#typical-set) has probability at least $2^{-n(H(X)+\varepsilon)}$. Summing these probabilities gives

$$
1\geq\sum_{x^n\in T_\varepsilon^{(n)}}p(x^n)
\geq|T_\varepsilon^{(n)}|\,2^{-n(H(X)+\varepsilon)},
$$

so

$$
\boxed{|T_\varepsilon^{(n)}|\leq2^{n(H(X)+\varepsilon)}}.
$$

The upper bound itself holds at every block length. For sufficiently large $n$, the high-probability property also gives the companion lower bound

$$
1-\delta\leq\mathbb P(T_\varepsilon^{(n)})
\leq|T_\varepsilon^{(n)}|\,2^{-n(H(X)-\varepsilon)},
$$

hence $|T_\varepsilon^{(n)}|\geq(1-\delta)2^{n(H(X)-\varepsilon)}$. Together these are the [typical-set cardinality bounds](../../../information-theory.md#typical-set-cardinality-bounds) underlying [Shannon source coding theorem](../../../coding-theory.md#shannon-s-source-coding-theorem).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/a">a</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#2/ii/a)

Memorylessness means that the ensemble's average [density operator](../../../quantum-theory.md#density-matrix) is $\rho^{(n)}=\pi^{\otimes n}$. Its [spectral decomposition](../../../linear-operator-theory.md#spectral-decomposition) is

$$
\rho^{(n)}=\sum_{i^n}q_{i_1}\cdots q_{i_n}|\phi_{i^n}\rangle\langle\phi_{i^n}|,\qquad
|\phi_{i^n}\rangle=|\phi_{i_1}\rangle\otimes\cdots\otimes|\phi_{i_n}\rangle.
$$

The product eigenvalues give

$$
S(\rho^{(n)})
=-\sum_{i^n}\left(\prod_jq_{i_j}\right)\log_2\left(\prod_jq_{i_j}\right)
=nH(q)=nS(\pi).
$$

Zero eigenvalues contribute zero to the [Von Neumann entropy](../../../von-neumann-entropy.md) and are excluded from logarithmic typicality tests.

The [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace) is the span of eigenvectors whose eigenvalues satisfy

$$
\left|-\frac1n\log_2(q_{i_1}\cdots q_{i_n})-S(\pi)\right|\leq\varepsilon.
$$

Its orthogonal projection $P_\varepsilon^{(n)}$ selects precisely the classical [typical set](../../../information-theory.md#typical-set) for the eigenvalue distribution $q$. The [typical-set cardinality bounds](../../../information-theory.md#typical-set-cardinality-bounds) and the [weak law of large numbers](../../../convergence-of-random-variables.md#weak-law-of-large-numbers) therefore give

$$
\boxed{\dim\mathcal T_\varepsilon^{(n)}\leq2^{n(S(\pi)+\varepsilon)}},\qquad
\boxed{\operatorname{Tr}(\rho^{(n)}P_\varepsilon^{(n)})\geq1-\delta}
$$

for any fixed $\delta>0$ and all sufficiently large $n$.

<h4 id="2/ii/b">b</h4>

↑ **Parent:** [Ii](#2/ii)

<h5 id="2/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#2/ii/b)

A compression-decompression scheme consists of [quantum channels](../../../quantum-information-theory.md#quantum-channel) $\mathcal E_n:\mathcal D(\mathcal H^{\otimes n})\to\mathcal D(\mathcal K_n)$ and $\mathcal D_n:\mathcal D(\mathcal K_n)\to\mathcal D(\mathcal H^{\otimes n})$, where $\limsup_n n^{-1}\log_2\dim\mathcal K_n\leq R$. For the emitted pure-state ensemble, reliability means that the mean squared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) tends to one:

$$
\boxed{\sum_kp_k\langle\Psi_k^{(n)}|
(\mathcal D_n\circ\mathcal E_n)(|\Psi_k^{(n)}\rangle\langle\Psi_k^{(n)}|)
|\Psi_k^{(n)}\rangle\longrightarrow1}.
$$

The average is taken over the actual source distribution, rather than the worst possible input vector.

A standard stronger formulation of [reliable quantum source compression](../../../quantum-information-theory.md#reliable-quantum-source-compression) requires

$$
F_e(\pi^{\otimes n},\mathcal D_n\circ\mathcal E_n)\longrightarrow1,
$$

where [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity) tests preservation of a purification and its reference-system correlations. It implies the mean-fidelity condition for every pure-state ensemble of $\pi^{\otimes n}$. [Schumacher compression](../../../quantum-information-theory.md#schumacher-compression) achieves this at any rate $R>S(\pi)$: choose $0<\varepsilon<R-S(\pi)$, encode the [quantum typical subspace](../../../quantum-information-theory.md#quantum-typical-subspace), and map atypical outcomes to a fallback state. The composed channel has a Kraus term $P_\varepsilon^{(n)}$, so its [entanglement fidelity](../../../quantum-information-theory.md#entanglement-fidelity) is at least $[\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})]^2\to1$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Let $Z$ indicate whether the outcome differs from $x_1$. Then $\mathbb P(Z=1)=q$. The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) gives

$$
H(X)=H(Z)+qH(X\mid Z=1),
$$

since $X=x_1$ is determined when $Z=0$. The remaining conditional distribution has at most $m-1$ outcomes, so the [maximum entropy on a finite alphabet](../../../information-theory.md#maximum-entropy-on-a-finite-alphabet) is $\log_2(m-1)$. Therefore the [Shannon source coding theorem](../../../coding-theory.md#shannon-s-source-coding-theorem) limit obeys

$$
\boxed{H(X)\leq h_2(q)+q\log_2(m-1)}.
$$

Here $h_2$ is the [binary entropy function](../../../combinatorics.md#binary-entropy-function); equality holds when the rare outcomes are equiprobable. A convenient explicit small-$q$ bound is

$$
\boxed{H(X)\leq q\log_2\frac{e(m-1)}q},
$$

because $-(1-q)\log_2(1-q)\leq q\log_2e$. For a fixed alphabet, this upper bound tends to zero as $q\to0$.

## 3

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Assume no previously shared [entanglement](../../../bell-state.md#entangled-state). Alice's encoded ensemble $\{p_x,\rho_x\}$ lives in a [Hilbert space](../../../hilbert-space.md) of dimension $2^n$. Its [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) satisfies

$$
\chi_{\rm in}=S\left(\sum_xp_x\rho_x\right)-\sum_xp_xS(\rho_x)
\leq\log_2(2^n)=n,
$$

using nonnegativity of [Von Neumann entropy](../../../von-neumann-entropy.md) and the [maximum entropy of a quantum state](../../../von-neumann-entropy.md#maximum-entropy-of-a-quantum-state). The [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) implies $\chi_{\rm out}\leq\chi_{\rm in}$ for the transmission [quantum channel](../../../quantum-information-theory.md#quantum-channel). Finally, the [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) applied to Bob's [measurement in quantum mechanics](../../../quantum-measurement.md) gives

$$
\boxed{I(X:Y)\leq\chi_{\rm out}\leq n\text{ bits}}.
$$

This argument also works when the output system has larger dimension than the input. Prior shared [entanglement](../../../bell-state.md#entangled-state) changes the communication resource: [superdense coding](../../../bell-state.md#superdense-coding) can transmit two classical bits per sent qubit, so the absence of that resource is part of this bound's setting.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Assume a finite-dimensional memoryless [quantum channel](../../../quantum-information-theory.md#quantum-channel), no shared [entanglement](../../../bell-state.md#entangled-state), and a code of $M_n$ messages with $n^{-1}\log_2M_n\to R$. Use a uniform message $M$ to relate average and maximum error. Each permitted input is a [product state](../../../bell-state.md#product-state) $\rho_m^{(n)}=\bigotimes_{i=1}^n\rho_{m,i}$, giving output $\sigma_m^{(n)}=\bigotimes_i\Lambda(\rho_{m,i})$. The factors may depend on both the message and the channel use.

Let $\chi^*(\Lambda)$ denote the one-use [Holevo capacity](../../../quantum-information-theory.md#holevo-capacity) in the question. The [Subadditivity of Von Neumann entropy](../../../von-neumann-entropy.md#subadditivity-of-von-neumann-entropy) for the average output, and entropy additivity for each product output, imply

$$
\begin{aligned}
\chi_n
&=S\left(\frac1{M_n}\sum_m\sigma_m^{(n)}\right)
-\frac1{M_n}\sum_m\sum_iS(\Lambda(\rho_{m,i}))\\
&\leq\sum_i\left[S\left(\frac1{M_n}\sum_m\Lambda(\rho_{m,i})\right)
-\frac1{M_n}\sum_mS(\Lambda(\rho_{m,i}))\right]
\leq n\chi^*(\Lambda).
\end{aligned}
$$

This is the key step of the [product-input classical-capacity converse](../../../quantum-information-theory.md#product-input-classical-capacity-converse); it does not assume that the average output itself is a product.

Bob may measure all outputs jointly. The [Holevo bound](../../../quantum-information-theory.md#holevo-s-theorem) still gives $I(M:\widehat M)\leq\chi_n$. Let $P_e$ be his average message-error probability. [Fano's inequality](../../../information-theory.md#fano-s-inequality) gives

$$
\log_2M_n=I(M:\widehat M)+H(M\mid\widehat M)
\leq n\chi^*(\Lambda)+1+P_e\log_2M_n.
$$

Since the maximum error $P_{\max}$ is at least $P_e$,

$$
\boxed{\liminf_{n\to\infty}P_{\max}
\geq1-\frac{\chi^*(\Lambda)}R>0}
$$

when $R>\chi^*(\Lambda)$. Thus the maximum error cannot vanish asymptotically.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Put $p=\langle\psi|M_1^2|\psi\rangle\geq1-\varepsilon$. Since $M_1$ is a [positive contraction](../../../hilbert-space.md#positive-contraction), the successful [post-measurement state](../../../quantum-measurement.md#post-measurement-state) is the pure state represented by $|\psi'\rangle=M_1|\psi\rangle/\sqrt p$. Its squared [quantum fidelity](../../../quantum-information-theory.md#fidelity-of-quantum-states) with the input is

$$
F(\rho,\rho')^2=|\langle\psi|\psi'\rangle|^2
=\frac{\langle\psi|M_1|\psi\rangle^2}{p}.
$$

The [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem) and $0\leq M_1\leq I$ give $M_1^2\leq M_1$, so $\langle M_1\rangle\geq p$. Therefore the [pure-state gentle measurement bound](../../../quantum-information-theory.md#pure-state-gentle-measurement-bound) is

$$
\boxed{F(\rho,\rho')^2\geq p\geq1-\varepsilon}.
$$

The positive-operator assumption matters: an arbitrary unitary measurement operator can have success probability one while rotating the state to an orthogonal vector.

## 4

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $\Delta=\rho-\sigma=\Delta_+-\Delta_-$ be its [positive-negative decomposition](../../../hilbert-space.md#positive-negative-decomposition-of-a-hermitian-operator). Since $\operatorname{Tr}\Delta=0$, the positive and negative parts have equal trace, namely $D(\rho,\sigma)$. For every [positive contraction](../../../hilbert-space.md#positive-contraction) $M$,

$$
\operatorname{Tr}(M\Delta)
=\operatorname{Tr}(M\Delta_+)-\operatorname{Tr}(M\Delta_-)
\leq\operatorname{Tr}\Delta_+=D(\rho,\sigma).
$$

Here both products have nonnegative trace, and $M\leq I$ bounds the first term. Equality is attained by the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) $P_+$ onto the positive spectral subspace of $\Delta$, since $P_+\Delta_+=\Delta_+$ and $P_+\Delta_-=0$. Thus the [variational characterization of trace distance](../../../quantum-theory.md#variational-characterization-of-trace-distance) is

$$
\boxed{D(\rho,\sigma)=\max_{0\leq M\leq I}\operatorname{Tr}[M(\rho-\sigma)]}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Choose an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) $\{|j\rangle\}_{j=1}^d$ of the input space and define operators from the input to the $k$-dimensional outcome register by

$$
K_{a,j}=|a\rangle\langle j|\sqrt{E_a}.
$$

These give a [Kraus representation](../../../quantum-information-theory.md#kraus-representation):

$$
\sum_{a,j}K_{a,j}XK_{a,j}^\dagger
=\sum_a\operatorname{Tr}(E_aX)|a\rangle\langle a|=\Phi(X).
$$

The [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) completeness relation gives

$$
\sum_{a,j}K_{a,j}^\dagger K_{a,j}
=\sum_a\sqrt{E_a}\left(\sum_j|j\rangle\langle j|\right)\sqrt{E_a}
=\sum_aE_a=I.
$$

Therefore $\Phi$ is a [completely positive map](../../../quantum-information-theory.md#completely-positive-map) and is trace preserving: it is a [quantum channel](../../../quantum-information-theory.md#quantum-channel) representing a deterministic [measurement channel](../../../quantum-information-theory.md#measurement-channel).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $P_+$ be the maximizing projection in the [variational characterization of trace distance](../../../quantum-theory.md#variational-characterization-of-trace-distance). Use the binary [POVM](../../../quantum-measurement.md#positive-operator-valued-measure) $\{P_+,I-P_+\}$ and its [measurement channel](../../../quantum-information-theory.md#measurement-channel). The difference between its two output probability vectors is

$$
(p_1-q_1,p_2-q_2)
=\left(\operatorname{Tr}[P_+(\rho-\sigma)],\operatorname{Tr}[(I-P_+)(\rho-\sigma)]\right)
=(D,-D),
$$

where $D=D(\rho,\sigma)$ and the second equality uses $\operatorname{Tr}(\rho-\sigma)=0$. Since [trace distance](../../../quantum-theory.md#trace-distance) between diagonal [density operators](../../../quantum-theory.md#density-matrix) is half the [L1 norm](../../../functional-analysis.md#l1-norm) of their probability-vector difference,

$$
\boxed{D(\Phi(\rho),\Phi(\sigma))=\frac12(|D|+|-D|)=D(\rho,\sigma)}.
$$

Thus a binary [measurement in quantum mechanics](../../../quantum-measurement.md) can preserve the distinguishability of this particular pair exactly. This is the [trace-distance-preserving binary measurement](../../../quantum-theory.md#trace-distance-preserving-binary-measurement), which may depend on the two states.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Choose the [trace-distance-preserving binary measurement](../../../quantum-theory.md#trace-distance-preserving-binary-measurement) from the previous part. Let $p,q$ be its output probability distributions, so $\lVert p-q\rVert_1=2D(\rho,\sigma)$. The [data-processing inequality for quantum relative entropy](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy) gives

$$
D(\rho\|\sigma)\geq D(\Phi(\rho)\|\Phi(\sigma))=D(p\|q).
$$

For diagonal [density operators](../../../quantum-theory.md#density-matrix), the quantum expression is the classical [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence). Applying the supplied [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality) gives

$$
D(p\|q)\geq\frac1{2\ln2}\lVert p-q\rVert_1^2
=\frac2{\ln2}D(\rho,\sigma)^2.
$$

Consequently the [quantum Pinsker inequality](../../../von-neumann-entropy.md#quantum-pinsker-inequality) is

$$
\boxed{D(\rho\|\sigma)\geq\frac2{\ln2}D(\rho,\sigma)^2}.
$$

The $\ln2$ factor converts natural-logarithm relative entropy to bits. If the relative entropy is infinite because its support condition fails, the inequality holds automatically.

## 5

↑ **Parent:** [Paper 323](paper-323.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

First prove monotonicity for a [partial trace](../../../quantum-theory.md#partial-trace). Let $r=\dim\mathcal H_B$ and define the [Heisenberg-Weyl twirling channel](../../../quantum-information-theory.md#heisenberg-weyl-twirling-channel)

$$
\mathcal T_B(X)=\frac1{r^2}\sum_{k,m}(I_A\otimes W_{k,m})X(I_A\otimes W_{k,m})^\dagger
=(\operatorname{Tr}_BX)\otimes\frac{I_B}{r}.
$$

The supplied identity on individual operators extends to bipartite operators by expanding them in a [tensor-product basis](../../../linear-algebra.md#tensor-product-basis). The [joint convexity of quantum relative entropy](../../../quantum-information-theory.md#joint-convexity-of-quantum-relative-entropy) and its unitary invariance imply

$$
D\left(\rho_A\otimes\frac{I_B}r\middle\|\sigma_A\otimes\frac{I_B}r\right)
\leq\frac1{r^2}\sum_{k,m}D(U_{k,m}\rho_{AB}U_{k,m}^\dagger\|U_{k,m}\sigma_{AB}U_{k,m}^\dagger)
=D(\rho_{AB}\|\sigma_{AB}).
$$

The [additivity of quantum relative entropy](../../../von-neumann-entropy.md#additivity-of-quantum-relative-entropy) makes the left side $D(\rho_A\|\sigma_A)$, proving the partial-trace case.

For a general deterministic quantum operation, meaning a [quantum channel](../../../quantum-information-theory.md#quantum-channel), use a [Stinespring dilation](../../../quantum-information-theory.md#stinespring-dilation) $\Lambda(X)=\operatorname{Tr}_E(VXV^\dagger)$ with $V^\dagger V=I$. An [isometric embedding](../../../riemannian-geometry.md#isometric-embedding) preserves [quantum relative entropy](../../../von-neumann-entropy.md#quantum-relative-entropy), because restricting the output to the common image of $V$ preserves the eigenvalues and trace formula. Applying the partial-trace result gives

$$
\boxed{D(\Lambda(\rho)\|\Lambda(\sigma))
\leq D(V\rho V^\dagger\|V\sigma V^\dagger)=D(\rho\|\sigma)}.
$$

The other properties used are unitary invariance and invariance under adjoining an identical ancillary state; both follow directly from the relative-entropy trace formula. This is the [Lindblad-Uhlmann monotonicity theorem](../../../von-neumann-entropy.md#data-processing-inequality-for-quantum-relative-entropy). The proof applies to deterministic channels; normalized postselection is not such a linear channel.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Write a qubit [density operator](../../../quantum-theory.md#density-matrix) in [Bloch vector](../../../quantum-theory.md#bloch-vector) form, $\rho=(I+\mathbf r\mathbin\cdot\boldsymbol\sigma)/2$, with $|\mathbf r|\leq1$. The [quantum depolarizing channel](../../../quantum-information-theory.md#quantum-depolarizing-channel) maps $\mathbf r$ to $p\mathbf r$, so its output eigenvalues are $(1\pm p|\mathbf r|)/2$. The output [Von Neumann entropy](../../../von-neumann-entropy.md) is minimized on pure inputs, where it equals $h_2((1+p)/2)$.

For any input ensemble, its output [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity) is at most the maximum qubit entropy minus this minimum output entropy:

$$
\chi\leq1-h_2\left(\frac{1+p}2\right).
$$

Equality is attained by two equiprobable orthogonal pure inputs: their average output is $I/2$, while each output has the minimum entropy. Thus

$$
\boxed{\chi^*(\Lambda_{\rm dep})=1-h_2\left(\frac{1+p}2\right)}.
$$

This uses the question's retention parameter $p$; in the usual convex-mixture range, $0\leq p\leq1$. The expression also holds throughout the full completely positive qubit range $-1/3\leq p\leq1$, since $h_2((1+p)/2)=h_2((1+|p|)/2)$.

The supplied [additivity of Holevo capacity](../../../quantum-information-theory.md#additivity-of-holevo-capacity) gives $\chi^*(\Lambda_{\rm dep}^{\otimes n})=n\chi^*(\Lambda_{\rm dep})$. The [Holevo-Schumacher-Westmoreland theorem](../../../quantum-information-theory.md#holevo-schumacher-westmoreland-theorem) expresses the unassisted [classical capacity of a quantum channel](../../../quantum-information-theory.md#classical-capacity-of-a-quantum-channel) as the regularized [Holevo capacity](../../../quantum-information-theory.md#holevo-capacity), so

$$
\boxed{C(\Lambda_{\rm dep})=\chi^*(\Lambda_{\rm dep})}.
$$

Therefore entangled inputs across channel uses cannot increase this classical capacity.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Let $\overline\omega=\sum_jp_j\omega_j$. When the relative entropies are finite, expanding their trace definitions gives

$$
\begin{aligned}
\sum_jp_jD(\omega_j\|\rho)-\sum_jp_jD(\omega_j\|\overline\omega)
&=\sum_jp_j\operatorname{Tr}[\omega_j(\log_2\overline\omega-\log_2\rho)]\\
&=\operatorname{Tr}[\overline\omega(\log_2\overline\omega-\log_2\rho)]
=D(\overline\omega\|\rho).
\end{aligned}
$$

Thus [Donald's identity](../../../von-neumann-entropy.md#donald-s-identity) is

$$
\boxed{\sum_jp_jD(\omega_j\|\rho)
=\sum_jp_jD(\omega_j\|\overline\omega)+D(\overline\omega\|\rho)}.
$$

For every $p_j>0$, the [support of a positive operator](../../../hilbert-space.md#support-of-a-positive-operator) $\omega_j$ lies in that of $\overline\omega$, so the first sum on the right is finite in finite dimension. If the support of $\overline\omega$ is not contained in the support of $\rho$, at least one positive-weight $\omega_j$ also violates the support condition. Both sides of the identity are then $+\infty$. This extends the conclusion without subtracting infinite quantities.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

By [Donald's identity](../../../von-neumann-entropy.md#donald-s-identity), the objective equals

$$
\sum_jp_jD(\omega_j\|\rho)=\sum_jp_jD(\omega_j\|\overline\omega)+D(\overline\omega\|\rho).
$$

The [nonnegativity of quantum relative entropy](../../../von-neumann-entropy.md#nonnegativity-of-quantum-relative-entropy) makes the last term at least zero, with equality exactly when $\rho=\overline\omega$. Hence the unique minimizing [density operator](../../../quantum-theory.md#density-matrix) is the ensemble average and

$$
\min_\rho\sum_jp_jD(\omega_j\|\rho)
=\sum_jp_jD(\omega_j\|\overline\omega)
=S(\overline\omega)-\sum_jp_jS(\omega_j).
$$

For the [classical-quantum state](../../../quantum-information-theory.md#classical-quantum-state) $\sigma_{XB}$, its marginal on $X$ has entropy $H(p)$, its marginal on $B$ is $\overline\omega$, and its joint entropy is $H(p)+\sum_jp_jS(\omega_j)$. Substituting in the definition of [quantum mutual information](../../../von-neumann-entropy.md#quantum-mutual-information) gives

$$
\boxed{\min_\rho\sum_jp_jD(\omega_j\|\rho)
=\chi(\{p_j,\omega_j\})=I(X:B)_\sigma,\qquad\rho_{\min}=\overline\omega}.
$$

This is the [relative-entropy barycenter of a quantum ensemble](../../../von-neumann-entropy.md#relative-entropy-barycenter-of-a-quantum-ensemble): the average state minimizes mean distinguishability from the ensemble. Its minimal value is exactly the [Holevo quantity](../../../quantum-information-theory.md#holevo-quantity).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
