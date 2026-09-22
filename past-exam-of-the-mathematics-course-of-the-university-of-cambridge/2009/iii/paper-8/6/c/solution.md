<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the round unit sphere with its complex orientation and unique [spin structure](../../../../../../spin-structure.md). Its chiral [spinor bundles](../../../../../../spinor-bundle.md) are $S^+=\mathcal O(-1)$ and $S^-=\Lambda^{0,1}\otimes\mathcal O(-1)$, the latter a smooth line bundle of degree $+1$. The [Dirac operator](../../../../../../dirac-operator.md) is

$$
D=c\circ\nabla^S=\begin{pmatrix}0&D^-\\D^+&0\end{pmatrix},\qquad
D^+=\sqrt2\,\overline\partial_{\mathcal O(-1)},\quad D^-=(D^+)^*.
$$

Here [Clifford multiplication](../../../../../../clifford-multiplication.md) has $c(v)^2=-|v|^2$, and $D$ acts self-adjointly on the L2 spinors with first-order Sobolev domain. The geometric spin connection is invariant under the lifted $SU(2)$ action, hence $D$ is equivariant.

We justify the spectral properties needed for its phase. The [Peter-Weyl theorem](../../../../../../peter-weyl-theorem.md) and [Frobenius reciprocity for compact groups](../../../../../../frobenius-reciprocity-for-compact-groups.md) give the decomposition of sections of an isotropy-weight-$q$ line bundle: $E_n$ occurs once exactly when $n\geq|q|$ and $n\equiv q\pmod2$, because its torus weights are $n,n-2,\ldots,-n$. The spinor isotropy weights are $+1,-1$, so each chirality contains $E_1,E_3,E_5,\ldots$, each once. The horizontal connection Laplacian is the total Casimir minus the vertical generator square, $\nabla^*\nabla=C-1/4$ on these weight-one bundles. Expanding the Dirac square in a normal orthonormal frame gives the diagonal connection-Laplacian terms and the off-diagonal curvature contraction. The Clifford relations contract spin curvature to $\operatorname{Scal}/4$, the [Lichnerowicz formula for a twisted Dirac operator](../../../../../../lichnerowicz-formula-for-a-twisted-dirac-operator.md) with no twisting bundle. Since the scalar curvature here is two,

$$
D^2=\nabla^*\nabla+\tfrac12=C+\tfrac14,
\qquad D^2|_{E_n}=\frac{(n+1)^2}{4}I.
$$

Thus there is no kernel, the [eigenvalues](../../../../../../eigenvalue.md) of $D$ are $\pm1,\pm2,\ldots$ with finite multiplicities, and the resolvent is compact by spectral truncation. These round-sphere spectral facts agree with the explicit calculation in [Abrikosov's paper](https://arxiv.org/abs/hep-th/0212134).

Define the [chiral phase of the round-sphere Dirac operator](../../../../../../chiral-phase-of-the-round-sphere-dirac-operator.md)

$$
\boxed{V=D^+(D^-D^+)^{-1/2}:H_+\longrightarrow H_-,\qquad H_\pm=L^2(S^\pm).}
$$

It is unitary because both chiral kernels vanish; equivariance follows from that of $D$. The full phase is $F=D|D|^{-1}=\begin{pmatrix}0&V^*\\V&0\end{pmatrix}$.

For a smooth scalar $f$, the Leibniz rule gives $[D,M_f]=c(df)$, a bounded bundle endomorphism. The spectral integral for the sign operator gives, in the strong topology,

$$
F=\frac2\pi\int_0^\infty D(D^2+t^2)^{-1}\,dt.
$$

Write $R_\pm=(D\mp it)^{-1}$. Since $2D(D^2+t^2)^{-1}=R_++R_-$ and $[R_\pm,M_f]=-R_\pm[D,M_f]R_\pm$, the commutator integral is norm convergent: its integrands are compact and bounded by $\|[D,M_f]\|/(1+t^2)$. A norm limit of their integrals is compact. Thus $[F,M_f]$ is compact, and its off-diagonal blocks say $VM_f^+-M_f^-V$ is compact. Uniform approximation of continuous $f$ by smooth functions extends this to all $f\in C(S^2)$, using the bound $2\|f-g\|_\infty$ for the change of commutator.

**The chiral phase is an equivariant unitary which intertwines the two multiplication representations modulo compacts.** This specifies the grading implicit in the subsequent index question; treating the full self-adjoint phase as an endomorphism would yield a different, zero, compressed index.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
