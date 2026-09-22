<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The flavor content is $K^0=d\bar s$ and $\bar K^0=s\bar d$. A charged-current [box diagram](../../../../../box-diagram.md) changes [strangeness](../../../../../strangeness.md) by two units. The two internal [quark](../../../../../quark.md) lines can contain any up-type flavors $u_i,u_j\in\{u,c,t\}$, connected by two charged $W$ propagators. One allowed topology is shown below; its crossed counterpart also contributes to the full mixing amplitude.

<a id="4/image-charged-weak-box-diagram-converting-a-neutral-kaon-into-its-antikaon"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-52-kaon-box.png)

**[Figure 1](#4/image-charged-weak-box-diagram-converting-a-neutral-kaon-into-its-antikaon). Charged weak box diagram converting a neutral kaon into its antikaon**.

Each charged-current vertex contains the appropriate [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) element. The flavor sum has combinations $\lambda_i\lambda_j$, with $\lambda_i=V_{is}^*V_{id}$, multiplying [mass](../../../../../mass.md)-dependent loop functions. [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md) unitarity gives $\sum_i\lambda_i=0$, illustrating the GIM cancellation of flavor-independent loop terms. The diagram is at order $g^4$ and second order in the [weak interaction](../../../../../weak-interaction.md).

Let $\Theta$ be the antiunitary [CPT](../../../../../cpt-symmetry.md) operator. It interchanges the neutral-[kaon](../../../../../kaon.md) flavor states up to phases. For a Hermitian [Hamiltonian](../../../../../hamiltonian.md) invariant under [CPT](../../../../../cpt-symmetry.md),

$$
\langle\Theta K^0|H'|\Theta K^0\rangle
=\langle K^0|\Theta^{-1}H'\Theta|K^0\rangle^*
=\langle K^0|H'|K^0\rangle,
$$

since the diagonal expectation is real. Therefore **[CPT](../../../../../cpt-symmetry.md) gives $R_{11}=R_{22}$.** More generally an effective decay [Hamiltonian](../../../../../hamiltonian.md) has $R=M-i\Gamma/2$, where both $M$ and $\Gamma$ are Hermitian. [CPT](../../../../../cpt-symmetry.md) gives $M_{11}=M_{22}$ and $\Gamma_{11}=\Gamma_{22}$, hence the same equality of the complex diagonal entries. It does not require $R_{12}=R_{21}$; that is a [CP](../../../../../cp-symmetry.md) condition. Nor is $R_{21}=R_{12}^*$ true for the full decay matrix in general.

Choose the [CP](../../../../../cp-symmetry.md) convention $CP|K^0\rangle=-|\bar K^0\rangle$ and $CP|\bar K^0\rangle=-|K^0\rangle$. Then [CP](../../../../../cp-symmetry.md) acts as $-\sigma_x$ on the flavor basis. Invariance of $H'$ means $R=\sigma_xR\sigma_x$, and therefore

$$
\boxed{\text{CP invariance: }R_{12}=R_{21}.}
$$

With a different flavor-state phase convention this relation carries the corresponding phase factors; equality is the relation in the convention adopted here. For a Hermitian [mass matrix](../../../../../mass-matrix.md) it makes the off-diagonal element real.

For the requested production-time [mass eigenstates](../../../../../mass-eigenstate.md), discard the absorptive part. From now on $R$ denotes the Hermitian part $(R_{\rm original}+R_{\rm original}^\dagger)/2$, so its entries have the form

$$
R=\begin{pmatrix}r_0&z\\z^*&r_0\end{pmatrix},\qquad r_0\in\mathbb R,\quad z\ne0.
$$

If the original matrix already was Hermitian no replacement is needed. The [neutral-kaon mass matrix diagonalization](../../../../../neutral-kaon-mass-matrix-diagonalization.md) gives [eigenvalues](../../../../../eigenvalue.md) $r_0\pm|z|$, since $(r_0-\lambda)^2-|z|^2=0$. Write $z=r e^{i\varphi}$, $r=|z|>0$. Use the [kaon mixing square-root branch convention](../../../../../kaon-mixing-square-root-branch-convention.md)

$$
a=\sqrt{R_{12}}=\sqrt r\,e^{i\varphi/2},\qquad
b=\sqrt{R_{21}}=\sqrt r\,e^{-i\varphi/2},\qquad ab=r,
$$

continuously from the [CP](../../../../../cp-symmetry.md)-conserving convention in which $z>0$. Independent unrelated root signs would interchange the [eigenvalue](../../../../../eigenvalue.md) labels. Direct multiplication gives $R(a,-b)^T=(r_0-r)(a,-b)^T$ and $R(a,b)^T=(r_0+r)(a,b)^T$. Assigning the larger [mass](../../../../../mass.md) to $K_L^0$ gives

$$
\boxed{|K_S^0\rangle=\frac{a|K^0\rangle-b|\bar K^0\rangle}{\sqrt{2r}},\qquad
|K_L^0\rangle=\frac{a|K^0\rangle+b|\bar K^0\rangle}{\sqrt{2r}},}
$$

with [mass](../../../../../mass.md) shifts $r_0-r$ and $r_0+r$ respectively. A common strong-interaction [mass](../../../../../mass.md) may simply be added to both. Their norms are one and their inner product is zero. A Hermitian [mass](../../../../../mass.md)-only calculation determines the lighter and heavier combinations; it does not determine their different lifetimes.

In the [CP](../../../../../cp-symmetry.md)-conserving limit, the chosen lighter and heavier combinations are

$$
\boxed{|K_1^0\rangle=\frac{|K^0\rangle-|\bar K^0\rangle}{\sqrt2},\qquad
|K_2^0\rangle=\frac{|K^0\rangle+|\bar K^0\rangle}{\sqrt2}.}
$$

They are [CP eigenstates](../../../../../cp-eigenstate.md) with [eigenvalues](../../../../../eigenvalue.md) $+1$ and $-1$ in the convention above. The sign of the real off-diagonal entry and the flavor-state convention are chosen together so that the stated $K_1^0=K_S^0$ limit is the lower-[mass](../../../../../mass.md) state.

Changing to this [CP](../../../../../cp-symmetry.md) basis gives

$$
\begin{aligned}
a|K^0\rangle-b|\bar K^0\rangle
&=\frac{a+b}{\sqrt2}|K_1^0\rangle+\frac{a-b}{\sqrt2}|K_2^0\rangle,\\
a|K^0\rangle+b|\bar K^0\rangle
&=\frac{a+b}{\sqrt2}|K_2^0\rangle+\frac{a-b}{\sqrt2}|K_1^0\rangle.
\end{aligned}
$$

Consequently, provided $a+b\ne0$, define

$$
\boxed{\epsilon=\frac{a-b}{a+b}
=\frac{\sqrt{R_{12}}-\sqrt{R_{21}}}{\sqrt{R_{12}}+\sqrt{R_{21}}}.}
$$

Absorbing the common phase of $a+b$ into the definitions of the [mass eigenstates](../../../../../mass-eigenstate.md) and normalizing now yields

$$
\boxed{|K_S^0\rangle=\frac{|K_1^0\rangle+\epsilon|K_2^0\rangle}{\sqrt{1+|\epsilon|^2}},\qquad
|K_L^0\rangle=\frac{|K_2^0\rangle+\epsilon|K_1^0\rangle}{\sqrt{1+|\epsilon|^2}}.}
$$

For this Hermitian approximation, $\epsilon=i\tan(\varphi/2)$ is purely imaginary, so $\langle K_S^0|K_L^0\rangle=(\epsilon+\epsilon^*)/(1+|\epsilon|^2)=0$. The phase convention matters for the [kaon CP mixing parameter](../../../../../kaon-cp-mixing-parameter.md). Physical [kaon](../../../../../kaon.md) decay eigenstates instead diagonalize the generally non-[Hermitian matrix](../../../../../hermitian-operator.md) $M-i\Gamma/2$, for which the mixing parameter can have a real part and the eigenstates need not be [orthogonal](../../../../../orthogonal-vectors.md). The formula here is the requested [mass](../../../../../mass.md)-only result, not a calculation of that full decay dynamics.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
