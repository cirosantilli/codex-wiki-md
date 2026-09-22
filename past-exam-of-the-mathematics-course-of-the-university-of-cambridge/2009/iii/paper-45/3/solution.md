<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use units $c=\hbar=1$ and the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. Composing two affine [Poincaré group](../../../../../poincare-group.md) transformations, with the rightmost applied first, gives

$$
\boxed{(\Lambda,a)(\Sigma,b)=(\Lambda\Sigma,a+\Lambda b),\qquad
(\Lambda,a)^{-1}=(\Lambda^{-1},-\Lambda^{-1}a).}
$$

The translations form a normal subgroup, so this is the [semidirect product](../../../../../semidirect-product.md) of the [Lorentz group](../../../../../lorentz-group.md) with $\mathbb R^{1,3}$. The transformations $(\operatorname{diag}(1,R),0)$, $R\in SO(3)$, fix time and the spatial origin. Their products and inverses correspond to $RR'$ and $R^{-1}$, hence they form a subgroup isomorphic to [SO(3)](../../../../../so-3-group.md).

A rotationless [Lorentz boost](../../../../../lorentz-boost.md) changes the velocity of a frame without adding a spatial rotation. For $|\mathbf v|<1$ a convenient active convention is

$$
B(\mathbf v)=
\begin{pmatrix}
\gamma&\gamma\mathbf v^T\\
\gamma\mathbf v&I+(\gamma-1)\widehat{\mathbf v}\widehat{\mathbf v}^{,T}
\end{pmatrix},\qquad
\gamma=(1-|\mathbf v|^2)^{-1/2},
$$

with $B(0)=I$. It satisfies $B^TgB=g$, $\det B=1$, and $B(m,\mathbf0)=(m\gamma,m\gamma\mathbf v)$. Collinear boosts form a one-parameter subgroup with additive rapidity, but general boosts do not. For nonzero boosts along $x$ and $y$, $(B_xB_y)_{02}=\gamma_x\gamma_yv_y$ while $(B_xB_y)_{20}=\gamma_yv_y$: their product is not symmetric, whereas every rotationless boost above is symmetric. The product contains a [Wigner rotation](../../../../../wigner-rotation.md). Infinitesimally, the [Poincare algebra](../../../../../poincare-algebra.md) gives $[K_i,K_j]=-i\epsilon_{ijk}J_k$ for Hermitian generators, so the boost generators do not close amongst themselves.

There is a group-versus-cover qualification in the spin range: an honest [unitary representation](../../../../../unitary-representation.md) of the proper orthochronous [Poincaré group](../../../../../poincare-group.md) permits integer spin only. Half-integer spin requires its double cover $SL(2,\mathbb C)\ltimes\mathbb R^{1,3}$, or a [projective unitary representation](../../../../../projective-unitary-representation.md) of the ordinary group. The construction below gives the requested range on that double cover and descends for integer spin.

Fix $m>0$ and the rest momentum $k=(m,\mathbf0)$. Its [little group](../../../../../little-group.md) consists of rotations: if a proper orthochronous Lorentz transformation fixes $k$, its time column is $(1,\mathbf0)$, the metric condition forces the corresponding time row, and the remaining block belongs to [SO(3)](../../../../../so-3-group.md). On the [Lorentz spinor double cover](../../../../../lorentz-spinor-double-cover.md), this little group is [SU(2)](../../../../../su-2-group.md). Choose its irreducible spin-$s$ representation, with rest-frame states $|k,s,\sigma\rangle$, $\sigma=-s,-s+1,\ldots,s$, and matrices $D^{(s)}$, the [Wigner D-matrices](../../../../../wigner-d-matrix.md).

For each $p$ on the forward [mass shell](../../../../../mass-shell.md), $p^2=m^2$, $p^0>0$, choose the standard rotationless [Lorentz boost](../../../../../lorentz-boost.md) $L(p)=B(\mathbf p/p^0)$ and define

$$
|p,s,\sigma\rangle=U[L(p),0]|k,s,\sigma\rangle.
$$

The labels are canonical spin projections, defined by this choice of boosts. For any proper orthochronous $\Lambda$, factor

$$
\Lambda L(p)=L(\Lambda p)W(\Lambda,p),\qquad
W(\Lambda,p)=L(\Lambda p)^{-1}\Lambda L(p).
$$

The last factor fixes $k$ and hence is a [Wigner rotation](../../../../../wigner-rotation.md). On the double cover, use its lift to [SU(2)](../../../../../su-2-group.md). Taking the translation convention $U[I,a]|p,s,\sigma\rangle=e^{ip\cdot a}|p,s,\sigma\rangle$ yields the [massive induced representation of the Poincare double cover](../../../../../massive-induced-representation-of-the-poincare-double-cover.md):

$$
\boxed{U[\Lambda,a]|p,s,\sigma\rangle
=e^{i(\Lambda p)\cdot a}\sum_{\tau=-s}^s
D^{(s)}_{\tau\sigma}\bigl(W(\Lambda,p)\bigr)|\Lambda p,s,\tau\rangle.}
$$

The argument of the translation phase is $\Lambda p$, since $U[\Lambda,a]=U[I,a]U[\Lambda,0]$. The [Wigner rotation](../../../../../wigner-rotation.md) identity

$$
W(\Lambda_2\Lambda_1,p)=W(\Lambda_2,\Lambda_1p)W(\Lambda_1,p)
$$

proves the Lorentz part of the representation law; the phases multiply according to the affine product already derived.

Normalize the generalized momentum states by $\langle p,s,\sigma|q,s,\tau\rangle=2p^0(2\pi)^3\delta^3(\mathbf p-\mathbf q)\delta_{\sigma\tau}$. The invariant [mass shell](../../../../../mass-shell.md) measure $d^3p/(2p^0)$ and unitarity of $D^{(s)}$ make the induced representation unitary on $L^2(d^3p/(2p^0))\otimes\mathbb C^{2s+1}$. This covariant normalization accounts for the absence of an energy square-root factor in the displayed transformation law. To see irreducibility, translations force an operator in the commutant to act within momentum fibres; the little-group action and [Schur lemma](../../../../../schur-s-lemma.md) make its action scalar on each irreducible spin fibre. Lorentz transitivity on the forward mass shell makes this scalar constant. The commutant is therefore scalar, so the unitary representation is irreducible. Conversely, the simultaneous translation spectrum and its little-group representation give the massive positive-energy sector of [Wigner's classification](../../../../../wigner-s-classification.md).

Thus every $m>0$ and $s\in\{0,\tfrac12,1,\ldots\}$ gives such an irreducible representation on the double cover. Its central element over a $2\pi$ spatial rotation acts as $(-1)^{2s}$. Since this rotation is the identity in the ordinary [Poincaré group](../../../../../poincare-group.md),

$$
\boxed{\text{all integer and half-integer }s\text{ occur on the double cover};\quad
\text{descent to the ordinary group requires }s\in\mathbb Z_{\geq0}.}
$$

For the [parity operator](../../../../../parity-operator.md), put $\Pi=\operatorname{diag}(1,-1,-1,-1)$ and $\bar p=\Pi p=(p^0,-\mathbf p)$. The extension obeys $P U[\Lambda,a]P^{-1}=U[\Pi\Lambda\Pi,\Pi a]$. At rest, $P$ commutes with the rotations; [Schur lemma](../../../../../schur-s-lemma.md) therefore gives $P|k,s,\sigma\rangle=\eta_P|k,s,\sigma\rangle$ with a common phase $|\eta_P|=1$. Since $\Pi L(p)\Pi=L(\bar p)$, the [parity action on canonical massive spin states](../../../../../parity-action-on-canonical-massive-spin-states.md) is

$$
\boxed{P|p,s,\sigma\rangle=\eta_P|p^0,-\mathbf p,s,\sigma\rangle.}
$$

For the usual reflection convention $P^2=I$, $\eta_P=\pm1$ is the [intrinsic parity](../../../../../intrinsic-parity.md). Canonical spin is an axial quantity and its label $\sigma$ is unchanged; a [helicity](../../../../../helicity.md) label instead changes sign because momentum is reversed. Either intrinsic parity extends a given massive spin representation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
