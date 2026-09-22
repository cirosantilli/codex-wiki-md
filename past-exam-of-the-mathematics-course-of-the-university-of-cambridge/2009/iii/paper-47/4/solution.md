<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An experimentally observed example of [CP violation](../../../../../cp-violation.md) is the long-lived neutral [kaon](../../../../../kaon.md) decay $K_L\to\pi^+\pi^-$. The two-pion spin-zero final state is CP even, whereas $K_L$ would be the CP-odd neutral-kaon state in the CP-conserving limit. Its two-pion decay reveals CP violation. The historical experimental account is [https://cern-courier.web.cern.ch/a/cp-violations-early-days/](https://cern-courier.web.cern.ch/a/cp-violations-early-days/) .

For the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md), diagonalize the up- and down-quark mass matrices independently by biunitary transformations. Write

$$
u'_L=L_u u_L,\qquad d'_L=L_d d_L,\qquad
u'_R=R_u u_R,\qquad d'_R=R_d d_R,
$$

with $L_u^\dagger M'_uR_u$ and $L_d^\dagger M'_dR_d$ positive diagonal matrices. Only the left transformations enter the [weak charged current](../../../../../charged-current.md), because its [chiral projector](../../../../../chiral-projector.md) removes the right-handed fields. Substitution gives

$$
\boxed{V=L_u^\dagger L_d,\qquad
\mathcal L_{qW}=-\frac g{2\sqrt2}\sum_{ij}
\overline u_i\gamma^\mu(1-\gamma_5)V_{ij}d_jW^+_\mu+\mathrm{h.c.}}
$$

The matrix is unitary but need not be diagonal: the two left mass diagonalizations generally differ.

Using the field transformations in the subparts and reordering the anticommuting [Dirac fields](../../../../../dirac-field.md), the charged bilinear transforms as

$$
\overline u_i\gamma^\mu(1-\gamma_5)d_j
\longmapsto-\Pi^\mu{}_{\nu}\overline d_j\gamma^\nu(1-\gamma_5)u_i(x_P),
$$

where the fields on the right are both evaluated at $x_P$. The [W boson](../../../../../w-boson.md) contributes its second minus sign and Lorentz parity factor, so the product maps into its Hermitian-conjugate product. Crucially [CP symmetry](../../../../../cp-symmetry.md) acts unitarily: it does not separately complex-conjugate the numerical coefficient $V_{ij}$. Thus the transformed interaction is

$$
\mathcal L_{qW}^{CP}(x)=-\frac g{2\sqrt2}\sum_{ij}
\left[V_{ij}\,\overline d_j\gamma^\mu(1-\gamma_5)u_iW^-_\mu
+V_{ij}^*\,\overline u_i\gamma^\mu(1-\gamma_5)d_jW^+_\mu\right](x_P).
$$

Comparing with the original interaction requires $V_{ij}=V_{ij}^*$ in this canonical CP convention. The physical condition is [quark rephasing and CP conservation](../../../../../quark-rephasing-and-cp-conservation.md):

$$
\boxed{\text{CP conservation requires that }V\text{ can be made real by allowed quark phase choices.}}
$$

A merely complex-looking matrix in an arbitrary mass-eigenstate phase convention is not itself proof of [CP violation](../../../../../cp-violation.md).

For [CKM parameter counting](../../../../../ckm-parameter-counting.md), a unitary $N\times N$ matrix has $N^2$ real parameters: $N(N-1)/2$ mixing angles and $N(N+1)/2$ phases. Rephasing the $N$ up and $N$ down mass eigenfields removes $2N-1$ phases, since their common phase cancels out of $V$. For generic nondegenerate masses this leaves

$$
\boxed{N_{\mathrm{CP\ phases}}=\frac{(N-1)(N-2)}2.}
$$

There is one physical phase for three families and none for one or two. Degenerate masses would permit additional transformations, so the generic count need not apply unchanged.

For the QCD part of the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md), define the Hermitian colour matrix $\mathcal A_\mu=A_\mu^aT^a$ and choose

$$
\boxed{D_\mu u=(\partial_\mu+ig_s\mathcal A_\mu)u.}
$$

This sign convention agrees with the field-strength definition $\mathcal F_{\mu\nu}=-i[D_\mu,D_\nu]/g_s$ in the source. The kinetic term contains $-g_s\overline u\gamma^\mu\mathcal A_\mu u$. A vector bilinear under CP changes sign, gains the Lorentz parity matrix, and transposes its colour matrix upon exchanging quark and antiquark. Invariance of this interaction therefore requires the [CP transformation of a non-Abelian gauge connection](../../../../../cp-transformation-of-a-non-abelian-gauge-connection.md):

$$
\boxed{\mathcal A_\mu(x)\longmapsto
-\Pi_\mu{}^\nu\mathcal A_\nu(x_P)^T.}
$$

Both the time/spatial distinction and the colour transpose are essential; individual colour components need not all share one charge-conjugation sign.

The same [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) gives

$$
\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu
+ig_s[\mathcal A_\mu,\mathcal A_\nu].
$$

Apply the transformation above and the chain rule $\partial_\mu f(x_P)=\Pi_\mu{}^\alpha(\partial_\alpha f)(x_P)$. The transpose reverses commutator order, $[X^T,Y^T]=-[X,Y]^T$, so the nonlinear term transforms with the same overall minus sign as the derivatives. This proves the [CP transformation of non-Abelian field strength](../../../../../cp-transformation-of-non-abelian-field-strength.md):

$$
\boxed{\mathcal F_{\mu\nu}(x)\longmapsto
-\Pi_\mu{}^\alpha\Pi_\nu{}^\beta\mathcal F_{\alpha\beta}(x_P)^T.}
$$

Finally $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$ rewrites the theta density as $2\theta\epsilon^{\mu\nu\rho\sigma}\operatorname{tr}(\mathcal F_{\mu\nu}\mathcal F_{\rho\sigma})$. The two minus signs cancel, and transposition followed by cyclicity leaves the colour trace unchanged. But the four parity matrices acting on the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) contribute $\det\Pi=-1$. Hence

$$
\boxed{\mathcal L_\theta(x)\longmapsto-\mathcal L_\theta(x_P).}
$$

The density is C even and P odd, therefore CP odd. **A generic fixed nonzero theta coefficient violates [CP symmetry](../../../../../cp-symmetry.md).** This is the source of the [Strong CP problem](../../../../../strong-cp-problem.md), separate from the charged-current phase in the [CKM matrix](../../../../../cabibbo-kobayashi-maskawa-matrix.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
