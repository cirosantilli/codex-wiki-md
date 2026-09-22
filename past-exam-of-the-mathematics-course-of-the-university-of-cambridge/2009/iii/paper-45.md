# Paper 45

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper45.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper45.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Adjoint double cover from SU(2) to SO(3)](../../../lie-theory.md#adjoint-double-cover-from-su-2-to-so-3) is obtained by writing a traceless Hermitian matrix as $X=x_i\sigma_i$, where the $\sigma_i$ are the [Pauli matrices](../../../algebra.md#pauli-matrices), and defining $AXA^\dagger=(R(A)x)_i\sigma_i$. Explicitly,

$$
R_{ij}(A)=\frac12\operatorname{tr}(\sigma_iA\sigma_jA^\dagger).
$$

Conjugation preserves $\tfrac12\operatorname{tr}X^2=|x|^2$, so $R(A)$ is orthogonal; connectedness of [SU(2)](../../../topological-group.md#su-2-group) gives $\det R(A)=1$. Composition of conjugations makes $R$ a [group homomorphism](../../../group-theory.md#group-homomorphism). A matrix in its kernel commutes with every [Pauli matrix](../../../algebra.md#pauli-matrices), so is scalar, and unit determinant then gives $A=\pm I$. Every spatial rotation occurs: $A=\exp(-i\theta\widehat n\cdot\sigma/2)$ induces the rotation through angle $\theta$ about $\widehat n$. Thus

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

Since [SU(2)](../../../topological-group.md#su-2-group) is the simply connected three-sphere, this is the universal double cover; the two [Lie algebras](../../../lie-algebra.md) are isomorphic, although the [groups](../../../group.md) are not.

Define the [conjugate fundamental spinor of SU(2)](../../../representation-theory.md#conjugate-fundamental-spinor-of-su-2) by $\bar\eta_\alpha=(\eta^\alpha)^*$. Regard $\bar\eta$ as a row, so unitarity gives

$$
\boxed{\bar\eta'_\alpha=\bar\eta_\beta(A^\dagger)^\beta{}_\alpha=\bar\eta_\beta(A^{-1})^\beta{}_\alpha.}
$$

Consequently $\bar\eta_\alpha\xi^\alpha$ is an invariant Hermitian pairing. The basic [invariant tensors](../../../representation-theory.md#invariant-tensor) are the [Kronecker delta](../../../linear-algebra.md#kronecker-delta) $\delta^\alpha{}_\beta$ and the alternating tensors $\epsilon_{\alpha\beta}$ and $\epsilon^{\alpha\beta}$. Choose $\epsilon_{12}=1$, $\epsilon^{12}=-1$, so that $\epsilon^{\alpha\gamma}\epsilon_{\gamma\beta}=\delta^\alpha{}_\beta$. The unit-determinant identity $A^T\epsilon A=\epsilon$ makes $[\eta,\xi]=\epsilon_{\alpha\beta}\eta^\alpha\xi^\beta$ invariant; its inverse gives the corresponding upper-index invariant. These contractions generate the tensor invariants of the defining representation. In particular $\widetilde\eta^\alpha=\epsilon^{\alpha\beta}\bar\eta_\beta$ transforms by $A$, showing that the conjugate representation is equivalent to the defining one. The antilinear map $\eta\mapsto\widetilde\eta$ squares to $-I$, so this is a [pseudoreal representation](../../../representation-theory.md#pseudoreal-representation), rather than a real structure.

For [Representation theory of SU2](../../../representation-theory.md#representation-theory-of-su-2), take $V_n=\operatorname{Sym}^n\mathbb C^2$, with $A$ acting on every index of a [symmetric tensor](../../../linear-algebra.md#symmetric-tensor). Its independent components are determined by the number $r$ of indices equal to $2$, so there are $n+1$ of them. Equivalently, the [homogeneous polynomial representation of SU2](../../../representation-theory.md#homogeneous-polynomial-representation-of-su2) has basis $z_1^{n-r}z_2^r$, $0\leq r\leq n$, with

$$
H=z_1\partial_{z_1}-z_2\partial_{z_2},\qquad E_+=z_1\partial_{z_2},\qquad E_-=z_2\partial_{z_1}.
$$

The basis weights are $n,n-2,\ldots,-n$, and the [raising operator](../../../semisimple-lie-algebra.md#raising-operator) and [lowering operator](../../../semisimple-lie-algebra.md#lowering-operator) connect consecutive basis vectors with nonzero coefficients until their endpoints. Any nonzero invariant subspace contains a weight vector, by applying polynomial spectral projections in $H$. Raising it reaches $z_1^n$, and lowering then obtains the entire basis. Thus $V_n$ is an [irreducible representation](../../../representation-theory.md#irreducible-representation), of [spin](../../../quantum-mechanics.md#spin) $j=n/2$. The [classification of finite-dimensional representations of SU2](../../../representation-theory.md#classification-of-finite-dimensional-representations-of-su2) gives every finite-dimensional complex irreducible representation in this way. The central element $-I$ acts on a rank-$n$ tensor as $(-1)^n$, so [descent of an SU(2) representation to SO(3)](../../../lie-theory.md#descent-of-an-su-2-representation-to-so-3) gives

$$
\boxed{\dim V_n=n+1,\qquad V_n\text{ descends to }SO(3)\iff n\text{ is even}.}
$$

For the [tensor contractions in the SU2 Clebsch-Gordan decomposition](../../../representation-theory.md#tensor-contractions-in-the-su2-clebsch-gordan-decomposition), contract $r$ indices of $S$ with $r$ indices of $T$ using $\epsilon$, and symmetrize all the remaining free indices:

$$
U_r^{\alpha_1\ldots\alpha_{m+n-2r}}=
\operatorname{Sym}_{\alpha_1,\ldots,\alpha_{m+n-2r}}
\left(\epsilon_{\beta_1\gamma_1}\cdots\epsilon_{\beta_r\gamma_r}
S^{\alpha_1\ldots\alpha_{m-r}\beta_1\ldots\beta_r}
T^{\alpha_{m-r+1}\ldots\alpha_{m+n-2r}\gamma_1\ldots\gamma_r}\right),
\qquad 0\leq r\leq\min(m,n).
$$

Each $U_r$ is an irreducible symmetric tensor in $V_{m+n-2r}$. To prove these are precisely the constituents, use two sets of formal variables $z,w$. The [highest-weight vectors](../../../semisimple-lie-algebra.md#highest-weight-vector)

$$
F_r=(z_1w_2-z_2w_1)^r z_1^{m-r}w_1^{n-r}
$$

are killed by the total [raising operator](../../../semisimple-lie-algebra.md#raising-operator) $z_1\partial_{z_2}+w_1\partial_{w_2}$ and have weights $m+n-2r$. The determinant factor is invariant; lowering the remaining factor gives an irreducible string of dimension $m+n-2r+1$. Distinct highest weights give inequivalent summands. The [unitary representation](../../../representation-theory.md#unitary-representation) on this tensor product makes invariant complements available, and the dimension check

$$
\sum_{r=0}^{\min(m,n)}(m+n-2r+1)=(m+1)(n+1)
$$

exhausts the space. Hence the contractions above are its irreducible projections, up to normalization, and the [Clebsch-Gordan decomposition for SU2](../../../representation-theory.md#clebsch-gordan-decomposition-for-su2) is

$$
\boxed{V_m\otimes V_n\cong\bigoplus_{r=0}^{\min(m,n)}V_{m+n-2r}.}
$$

For the [decomposition of three SU(2) spinors](../../../representation-theory.md#decomposition-of-three-su-2-spinors), write $Q^{\alpha\beta\gamma}=\eta_1^\alpha\eta_2^\beta\eta_3^\gamma$ and $S^{\alpha\beta\gamma}=Q^{(\alpha\beta\gamma)}$. The contractions

$$
\begin{aligned}
d_1^\alpha&=\epsilon_{\beta\gamma}Q^{\alpha\beta\gamma}=\eta_1^\alpha[\eta_2,\eta_3],\\
d_2^\alpha&=\epsilon_{\beta\gamma}Q^{\beta\alpha\gamma}=\eta_2^\alpha[\eta_1,\eta_3],\\
d_3^\alpha&=\epsilon_{\beta\gamma}Q^{\beta\gamma\alpha}=\eta_3^\alpha[\eta_1,\eta_2]
\end{aligned}
$$

transform as defining spinors. Alternation in three indices in dimension two vanishes, giving $d_1-d_2+d_3=0$; there are exactly two independent contractions. An explicit inverse, with the epsilon convention above, is

$$
Q^{\alpha\beta\gamma}=S^{\alpha\beta\gamma}
+\epsilon^{\alpha\beta}\frac{2d_1^\gamma-d_2^\gamma}{3}
-\epsilon^{\alpha\gamma}\frac{d_1^\beta+d_2^\beta}{3}.
$$

Symmetrizing this expression gives $S$, while its first two contractions give $d_1,d_2$, which verifies the decomposition. Thus

$$
\boxed{V_1^{\otimes3}=V_3\oplus V_1\oplus V_1,
\qquad \tfrac12\otimes\tfrac12\otimes\tfrac12=\tfrac32\oplus\tfrac12\oplus\tfrac12.}
$$

In the [quark model](../../../physics.md#quark-model), three spin-$1/2$ [quarks](../../../standard-model.md#quark) therefore have total quark [spin](../../../quantum-mechanics.md#spin) $S=3/2$ or $S=1/2$. The two spin-$1/2$ copies correspond to coupling the first pair to spin $0$ or spin $1$ before adding the third quark. For ground-state [baryons](../../../physics.md#baryon) with orbital angular momentum $L=0$, total $J=S$: the [nucleon](../../../physics.md#nucleon) has $J=1/2$ and the [Delta baryon](../../../physics.md#delta-baryon) has $J=3/2$. These two coupling copies alone do not assert two unrestricted physical baryon families. The antisymmetric [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet), the spatial wavefunction and [flavor symmetry](../../../standard-model.md#flavor-symmetry) must also satisfy the [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets); orbital excitations can give other total angular momenta.

## 2

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $R_a=\operatorname{ad}(T_a)$, where $\operatorname{ad}(X)Y=[X,Y]$. In the given basis, the [Adjoint representation of a Lie algebra](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is

$$
(R_a)^c{}_b=f^c{}_{ab}.
$$

The [Jacobi identity](../../../lie-algebra.md#jacobi-identity) gives $[\operatorname{ad}X,\operatorname{ad}Y]=\operatorname{ad}[X,Y]$, so $[R_a,R_b]=f^c{}_{ab}R_c$, as required for a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation). The [Killing form](../../../lie-algebra.md#killing-form) is the symmetric [Trace form of a Lie algebra representation](../../../lie-algebra.md#trace-form-of-a-lie-algebra-representation)

$$
\boxed{\kappa_{ab}=\operatorname{tr}(R_aR_b)=f^c{}_{ad}f^d{}_{bc}.}
$$

Cyclicity of the [trace](../../../linear-algebra.md#matrix-trace) proves its invariance directly:

$$
\begin{aligned}
\kappa([T_a,T_b],T_c)+\kappa(T_b,[T_a,T_c])
&=\operatorname{tr}\bigl([R_a,R_b]R_c+R_b[R_a,R_c]\bigr)\\
&=\operatorname{tr}(R_aR_bR_c-R_bR_cR_a)=0.
\end{aligned}
$$

In components this is precisely $\boxed{\kappa_{dc}f^d{}_{ab}+\kappa_{bd}f^d{}_{ac}=0}$, so the [Killing form](../../../lie-algebra.md#killing-form) is an [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra).

Choose the infinitesimal [gauge transformation](../../../electromagnetism.md#gauge-transformation) convention $\delta\phi=\omega\phi$, with $\omega(x)=\omega^a(x)t_a$, and write $A_\mu=A_\mu^at_a$. A [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) must satisfy $D'_\mu=UD_\mu U^{-1}$ for $U=1+\omega+O(\omega^2)$; hence

$$
A'_\mu=UA_\mu U^{-1}-(\partial_\mu U)U^{-1},\qquad
\boxed{\delta A_\mu=-\partial_\mu\omega+[\omega,A_\mu].}
$$

Equivalently $\delta A_\mu^a=-\partial_\mu\omega^a+f^a{}_{bc}\omega^bA_\mu^c$. Expanding $\delta(D_\mu\phi)$ makes the cancellation transparent:

$$
\begin{aligned}
\delta(D_\mu\phi)
&=(\partial_\mu\omega)\phi+\omega\partial_\mu\phi
+(-\partial_\mu\omega+[\omega,A_\mu])\phi+A_\mu\omega\phi\\
&=\omega(\partial_\mu\phi+A_\mu\phi).
\end{aligned}
$$

Thus $\boxed{\delta(D_\mu\phi)=\omega^at_aD_\mu\phi}$: it transforms in the same representation as $\phi$. In [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) notation, $\delta A_\mu=-D_\mu^{\mathrm{ad}}\omega$.

The commutator of two [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) defines the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength):

$$
[D_\mu,D_\nu]\phi=F_{\mu\nu}^at_a\phi,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu].
$$

Thus

$$
\boxed{F^a_{\mu\nu}=\partial_\mu A^a_\nu-\partial_\nu A^a_\mu+f^a{}_{bc}A^b_\mu A^c_\nu.}
$$

Conjugating the derivative commutator gives $F'_{\mu\nu}=UF_{\mu\nu}U^{-1}$, so the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) transforms homogeneously in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra):

$$
\boxed{\delta F_{\mu\nu}=[\omega,F_{\mu\nu}],\qquad
\delta F^a_{\mu\nu}=f^a{}_{bc}\omega^bF^c_{\mu\nu}.}
$$

Even if the matrices $t_a$ in a particular matter representation are not faithful, the displayed component formula defines the Lie-algebra-valued curvature independently of that representation.

Only $g_{(ab)}$ contributes to the [Yang-Mills theory](../../../relativistic-quantum-field.md#yang-mills-theory) Lagrangian, since $F^a_{\mu\nu}F^{b\mu\nu}$ is symmetric in $a,b$. Thus take $g_{ab}$ to be a constant real [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form). Its infinitesimal variation is

$$
\delta\mathcal L=-\frac14\omega^a\bigl(g_{dc}f^d{}_{ab}+g_{bd}f^d{}_{ac}\bigr)
F^b_{\mu\nu}F^{c\mu\nu}.
$$

Arbitrary local field strengths and gauge parameters give the necessary and sufficient [invariant gauge kinetic form](../../../relativistic-quantum-field.md#invariant-gauge-kinetic-form) condition

$$
\boxed{g_{dc}f^d{}_{ab}+g_{bd}f^d{}_{ac}=0,\qquad g_{ab}=g_{ba}.}
$$

An antisymmetric part is unconstrained but contributes nothing. A nondegenerate kinetic term additionally needs a [nondegenerate bilinear form](../../../linear-algebra.md#nondegenerate-bilinear-form); positive energy additionally needs a positive internal metric in the signature $(+---)$ convention. Neither extra condition follows solely from [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance). For a compact simple real [Lie algebra](../../../lie-algebra.md), $-\kappa$ is positive definite and is the standard choice up to a positive factor.

For the intended complex-simple setting, the [Killing form](../../../lie-algebra.md#killing-form) is nondegenerate. Consequently write any [invariant bilinear form on a Lie algebra](../../../lie-algebra.md#invariant-bilinear-form-on-a-lie-algebra) uniquely as $g(X,Y)=\kappa(SX,Y)$. Invariance of both forms implies

$$
\kappa\bigl((S\operatorname{ad}Z-\operatorname{ad}Z\,S)X,Y\bigr)=0
$$

for every $X,Y,Z$, so $S$ commutes with the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). A subspace invariant under all adjoint maps is an ideal, hence simplicity makes the adjoint representation irreducible. By [Schur lemma](../../../representation-theory.md#schur-s-lemma), $S=cI$, giving the [uniqueness of an invariant bilinear form on a simple Lie algebra](../../../lie-algebra.md#uniqueness-of-an-invariant-bilinear-form-on-a-simple-lie-algebra):

$$
\boxed{g_{ab}=c\kappa_{ab}.}
$$

The same conclusion holds for compact simple real algebras by complexification, with $c$ real; nondegeneracy excludes $c=0$, and positive energy selects $c<0$ in the stated convention.

There is a genuine [real-simple exception to uniqueness of the Killing form](../../../lie-algebra.md#real-simple-exception-to-uniqueness-of-the-killing-form) if “simple” is read as an arbitrary real simple algebra. Regard $\mathfrak{sl}_2(\mathbb C)$ as real. It is real simple: its complexification consists of two complex simple factors exchanged by conjugation, so a conjugation-stable ideal is zero or the whole algebra. Both $\operatorname{Re}\kappa_{\mathbb C}$ and $\operatorname{Im}\kappa_{\mathbb C}$ are real symmetric invariant forms, while $\kappa_{\mathbb R}=2\operatorname{Re}\kappa_{\mathbb C}$. With $H=\operatorname{diag}(1,-1)$, the [Killing form of the special linear Lie algebra](../../../lie-algebra.md#killing-form-of-the-special-linear-lie-algebra) gives $\kappa_{\mathbb C}(H,H)=8$ and $\kappa_{\mathbb C}(H,iH)=8i$. Therefore the imaginary part cannot be a real multiple of $\kappa_{\mathbb R}$. The uniqueness conclusion requires the customary complex-simple or compact-real interpretation.

## 3

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use units $c=\hbar=1$ and the [Minkowski metric](../../../special-relativity.md#minkowski-metric) $g=\operatorname{diag}(1,-1,-1,-1)$. Composing two affine [Poincaré group](../../../special-relativity.md#poincare-group) transformations, with the rightmost applied first, gives

$$
\boxed{(\Lambda,a)(\Sigma,b)=(\Lambda\Sigma,a+\Lambda b),\qquad
(\Lambda,a)^{-1}=(\Lambda^{-1},-\Lambda^{-1}a).}
$$

The translations form a normal subgroup, so this is the [semidirect product](../../../group-theory.md#semidirect-product) of the [Lorentz group](../../../special-relativity.md#lorentz-group) with $\mathbb R^{1,3}$. The transformations $(\operatorname{diag}(1,R),0)$, $R\in SO(3)$, fix time and the spatial origin. Their products and inverses correspond to $RR'$ and $R^{-1}$, hence they form a subgroup isomorphic to [SO(3)](../../../linear-algebra.md#so-3-group).

A rotationless [Lorentz boost](../../../special-relativity.md#lorentz-boost) changes the velocity of a frame without adding a spatial rotation. For $|\mathbf v|<1$ a convenient active convention is

$$
B(\mathbf v)=
\begin{pmatrix}
\gamma&\gamma\mathbf v^T\\
\gamma\mathbf v&I+(\gamma-1)\widehat{\mathbf v}\widehat{\mathbf v}^{,T}
\end{pmatrix},\qquad
\gamma=(1-|\mathbf v|^2)^{-1/2},
$$

with $B(0)=I$. It satisfies $B^TgB=g$, $\det B=1$, and $B(m,\mathbf0)=(m\gamma,m\gamma\mathbf v)$. Collinear boosts form a one-parameter subgroup with additive rapidity, but general boosts do not. For nonzero boosts along $x$ and $y$, $(B_xB_y)_{02}=\gamma_x\gamma_yv_y$ while $(B_xB_y)_{20}=\gamma_yv_y$: their product is not symmetric, whereas every rotationless boost above is symmetric. The product contains a [Wigner rotation](../../../special-relativity.md#wigner-rotation). Infinitesimally, the [Poincare algebra](../../../special-relativity.md#poincare-algebra) gives $[K_i,K_j]=-i\epsilon_{ijk}J_k$ for Hermitian generators, so the boost generators do not close amongst themselves.

There is a group-versus-cover qualification in the spin range: an honest [unitary representation](../../../representation-theory.md#unitary-representation) of the proper orthochronous [Poincaré group](../../../special-relativity.md#poincare-group) permits integer spin only. Half-integer spin requires its double cover $SL(2,\mathbb C)\ltimes\mathbb R^{1,3}$, or a [projective unitary representation](../../../quantum-mechanics.md#projective-unitary-representation) of the ordinary group. The construction below gives the requested range on that double cover and descends for integer spin.

Fix $m>0$ and the rest momentum $k=(m,\mathbf0)$. Its [little group](../../../special-relativity.md#little-group) consists of rotations: if a proper orthochronous Lorentz transformation fixes $k$, its time column is $(1,\mathbf0)$, the metric condition forces the corresponding time row, and the remaining block belongs to [SO(3)](../../../linear-algebra.md#so-3-group). On the [Lorentz spinor double cover](../../../special-relativity.md#lorentz-spinor-double-cover), this little group is [SU(2)](../../../topological-group.md#su-2-group). Choose its irreducible spin-$s$ representation, with rest-frame states $|k,s,\sigma\rangle$, $\sigma=-s,-s+1,\ldots,s$, and matrices $D^{(s)}$, the [Wigner D-matrices](../../../quantum-mechanics.md#wigner-d-matrix).

For each $p$ on the forward [mass shell](../../../special-relativity.md#mass-shell), $p^2=m^2$, $p^0>0$, choose the standard rotationless [Lorentz boost](../../../special-relativity.md#lorentz-boost) $L(p)=B(\mathbf p/p^0)$ and define

$$
|p,s,\sigma\rangle=U[L(p),0]|k,s,\sigma\rangle.
$$

The labels are canonical spin projections, defined by this choice of boosts. For any proper orthochronous $\Lambda$, factor

$$
\Lambda L(p)=L(\Lambda p)W(\Lambda,p),\qquad
W(\Lambda,p)=L(\Lambda p)^{-1}\Lambda L(p).
$$

The last factor fixes $k$ and hence is a [Wigner rotation](../../../special-relativity.md#wigner-rotation). On the double cover, use its lift to [SU(2)](../../../topological-group.md#su-2-group). Taking the translation convention $U[I,a]|p,s,\sigma\rangle=e^{ip\cdot a}|p,s,\sigma\rangle$ yields the [massive induced representation of the Poincare double cover](../../../special-relativity.md#massive-induced-representation-of-the-poincare-double-cover):

$$
\boxed{U[\Lambda,a]|p,s,\sigma\rangle
=e^{i(\Lambda p)\cdot a}\sum_{\tau=-s}^s
D^{(s)}_{\tau\sigma}\bigl(W(\Lambda,p)\bigr)|\Lambda p,s,\tau\rangle.}
$$

The argument of the translation phase is $\Lambda p$, since $U[\Lambda,a]=U[I,a]U[\Lambda,0]$. The [Wigner rotation](../../../special-relativity.md#wigner-rotation) identity

$$
W(\Lambda_2\Lambda_1,p)=W(\Lambda_2,\Lambda_1p)W(\Lambda_1,p)
$$

proves the Lorentz part of the representation law; the phases multiply according to the affine product already derived.

Normalize the generalized momentum states by $\langle p,s,\sigma|q,s,\tau\rangle=2p^0(2\pi)^3\delta^3(\mathbf p-\mathbf q)\delta_{\sigma\tau}$. The invariant [mass shell](../../../special-relativity.md#mass-shell) measure $d^3p/(2p^0)$ and unitarity of $D^{(s)}$ make the induced representation unitary on $L^2(d^3p/(2p^0))\otimes\mathbb C^{2s+1}$. This covariant normalization accounts for the absence of an energy square-root factor in the displayed transformation law. To see irreducibility, translations force an operator in the commutant to act within momentum fibres; the little-group action and [Schur lemma](../../../representation-theory.md#schur-s-lemma) make its action scalar on each irreducible spin fibre. Lorentz transitivity on the forward mass shell makes this scalar constant. The commutant is therefore scalar, so the unitary representation is irreducible. Conversely, the simultaneous translation spectrum and its little-group representation give the massive positive-energy sector of [Wigner's classification](../../../special-relativity.md#wigner-s-classification).

Thus every $m>0$ and $s\in\{0,\tfrac12,1,\ldots\}$ gives such an irreducible representation on the double cover. Its central element over a $2\pi$ spatial rotation acts as $(-1)^{2s}$. Since this rotation is the identity in the ordinary [Poincaré group](../../../special-relativity.md#poincare-group),

$$
\boxed{\text{all integer and half-integer }s\text{ occur on the double cover};\quad
\text{descent to the ordinary group requires }s\in\mathbb Z_{\geq0}.}
$$

For the [parity operator](../../../quantum-mechanics.md#parity-operator), put $\Pi=\operatorname{diag}(1,-1,-1,-1)$ and $\bar p=\Pi p=(p^0,-\mathbf p)$. The extension obeys $P U[\Lambda,a]P^{-1}=U[\Pi\Lambda\Pi,\Pi a]$. At rest, $P$ commutes with the rotations; [Schur lemma](../../../representation-theory.md#schur-s-lemma) therefore gives $P|k,s,\sigma\rangle=\eta_P|k,s,\sigma\rangle$ with a common phase $|\eta_P|=1$. Since $\Pi L(p)\Pi=L(\bar p)$, the [parity action on canonical massive spin states](../../../quantum-field-theory.md#parity-action-on-canonical-massive-spin-states) is

$$
\boxed{P|p,s,\sigma\rangle=\eta_P|p^0,-\mathbf p,s,\sigma\rangle.}
$$

For the usual reflection convention $P^2=I$, $\eta_P=\pm1$ is the [intrinsic parity](../../../quantum-field-theory.md#intrinsic-parity). Canonical spin is an axial quantity and its label $\sigma$ is unchanged; a [helicity](../../../special-relativity.md#helicity) label instead changes sign because momentum is reversed. Either intrinsic parity extends a given massive spin representation.

## 4

↑ **Parent:** [Paper 45](paper-45.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Start with a nonzero [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) $v_0=|n\rangle$ and set $v_r=E_-^rv_0$. The [sl2 highest-weight lowering formula](../../../semisimple-lie-algebra.md#sl2-highest-weight-lowering-formula) follows inductively from the [commutator](../../../lie-algebra.md#commutator) relations:

$$
Hv_r=(n-2r)v_r,\qquad E_+v_r=r(n-r+1)v_{r-1},\qquad E_-v_r=v_{r+1}.
$$

Indeed $[H,E_-]=-2E_-$ gives the weight formula, and $E_+E_-=E_-E_++H$ turns the coefficient $r(n-r+1)$ at step $r$ into $(r+1)(n-r)$ at step $r+1$. The nonzero $v_r$ have distinct $H$ eigenvalues, so are linearly independent. Finite dimensionality therefore forces a last nonzero vector $v_N$. Applying $E_+$ to $v_{N+1}=0$ gives $(N+1)(n-N)v_N=0$, hence $N=n$. This also proves that no earlier vector can vanish. Thus the cyclic [highest-weight representation](../../../semisimple-lie-algebra.md#highest-weight-representation) generated by $|n\rangle$ is

$$
\boxed{V_n=\operatorname{span}\{v_0,v_1,\ldots,v_n\},\qquad\dim V_n=n+1.}
$$

It is irreducible: spectral projections in $H$ select a weight vector from any nonzero invariant subspace, and its nonzero raising and lowering coefficients then generate the whole string. This gives the [classification of finite-dimensional sl2 representations](../../../semisimple-lie-algebra.md#classification-of-finite-dimensional-sl2-representations) used for each root direction below.

For the [SU(3) Lie algebra](../../../lie-algebra.md#su-3-lie-algebra), the repeated-index relation is the trace constraint $\sum_iT^i{}_i=0$. The displayed generators are a basis of its complexification, not nine independent generators or three individually vanishing diagonal elements. Realize them by [matrix units](../../../vector-space.md#matrix-unit) as $T^i{}_j=E_{ij}-\delta^i{}_jI/3$; the compact real algebra is obtained from anti-Hermitian combinations. Then

$$
H_1=\operatorname{diag}(1,-1,0),\qquad H_2=\operatorname{diag}(0,1,-1),
$$

and $E_{1+}=E_{12}$, $E_{1-}=E_{21}$, $E_{2+}=E_{23}$, $E_{2-}=E_{32}$. Substituting into the given commutators gives

$$
\begin{aligned}
[E_{1+},E_{1-}]&=T^1{}_1-T^2{}_2=H_1,&[H_1,E_{1\pm}]&=\pm2E_{1\pm},\\
[E_{2+},E_{2-}]&=T^2{}_2-T^3{}_3=H_2,&[H_2,E_{2\pm}]&=\pm2E_{2\pm}.
\end{aligned}
$$

Thus both root pairs obey the required [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra) relations. More generally, their [Cartan matrix](../../../semisimple-lie-algebra.md#cartan-matrix) is

$$
[H_i,E_{j\pm}]=\pm C_{ij}E_{j\pm},\qquad C=\begin{pmatrix}2&-1\\-1&2\end{pmatrix}.
$$

A [weight vector](../../../semisimple-lie-algebra.md#weight-vector) with eigenvalues $(h_1,h_2)$ moves by $(-2,1)$ under $E_{1-}$ and by $(1,-2)$ under $E_{2-}$. The third negative-root operator is $[E_{2-},E_{1-}]=E_{31}$ and moves it by $(-1,-1)$. In the required [weight diagram](../../../semisimple-lie-algebra.md#weight-diagram) coordinates

$$
x=h_1,\qquad y=\frac{h_1+2h_2}{\sqrt3},
$$

these moves are $(-2,0)$, $(1,-\sqrt3)$ and $(-1,-\sqrt3)$ respectively. Successive lowerings from a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector), with linear dependencies removed, construct the following bases.

For [Dynkin labels](../../../semisimple-lie-algebra.md#dynkin-label) $(1,0)$, use the defining action of [SU(3)](../../../topological-group.md#su-3-group) on $\mathbb C^3$. Its highest vector is $e_1$; lowering gives $e_2=E_{21}e_1$ and $e_3=E_{32}e_2$. There are no further independent vectors. The [weight diagram of the defining SU(3) representation](../../../semisimple-lie-algebra.md#weight-diagram-of-the-defining-su-3-representation), in the present rescaled coordinates, is

$$
\begin{array}{c|c|c}
\text{basis}&(h_1,h_2)&(x,y)\\\hline
e_1&(1,0)&(1,1/\sqrt3)\\
e_2&(-1,1)&(-1,1/\sqrt3)\\
e_3&(0,-1)&(0,-2/\sqrt3)
\end{array}
$$

and $\boxed{\dim R(1,0)=3}$. Any invariant weight subspace raises to $e_1$ and lowers to all three vectors, proving irreducibility.

For $(1,1)$, use the [adjoint representation of SU(3)](../../../lie-algebra.md#adjoint-representation-of-su-3) on traceless matrices, with $X$ acting by $Y\mapsto[X,Y]$. The highest vector is $E_{13}$: both $[E_{12},E_{13}]$ and $[E_{23},E_{13}]$ vanish, while $[H_i,E_{13}]=E_{13}$. Lowering gives $[E_{21},E_{13}]=E_{23}$ and $[E_{32},E_{13}]=-E_{12}$. Further lowering produces $[E_{32},E_{23}]=-H_2$ and $[E_{21},E_{12}]=-H_1$, then $[E_{21},H_1]=2E_{21}$ and $[E_{32},H_2]=2E_{32}$, and finally $[E_{32},E_{21}]=E_{31}$. Consequently the basis is the six off-diagonal matrix units together with $H_1,H_2$:

$$
\begin{array}{c|c|c}
\text{basis}&(h_1,h_2)&(x,y)\\\hline
E_{12}&(2,-1)&(2,0)\\
E_{21}&(-2,1)&(-2,0)\\
E_{23}&(-1,2)&(-1,\sqrt3)\\
E_{32}&(1,-2)&(1,-\sqrt3)\\
E_{13}&(1,1)&(1,\sqrt3)\\
E_{31}&(-1,-1)&(-1,-\sqrt3)\\
H_1,H_2&(0,0)&(0,0)
\end{array}
$$

The six nonzero weights have [weight multiplicity](../../../semisimple-lie-algebra.md#weight-multiplicity) one, and zero has multiplicity two. Thus $\boxed{\dim R(1,1)=6+2=8}$. Its irreducibility follows also because an adjoint-invariant subspace is an ideal and $\mathfrak{sl}_3(\mathbb C)$ is a [simple Lie algebra](../../../semisimple-lie-algebra.md#simple-lie-algebra).

For $(3,0)$, take the [symmetric cubic representation of SU(3)](../../../topological-group.md#symmetric-cubic-representation-of-su-3), $\operatorname{Sym}^3\mathbb C^3$, realized by homogeneous degree-three polynomials. Here

$$
T^i{}_j=z_i\partial_{z_j}-\frac{\delta^i{}_j}{3}N,\qquad
N=\sum_kz_k\partial_{z_k},
$$

so $z_1^3$ is a [highest-weight vector](../../../semisimple-lie-algebra.md#highest-weight-vector) with eigenvalues $(3,0)$. For $a+b+c=3$,

$$
E_{2-}^{\,c}E_{1-}^{\,b+c}z_1^3
=\frac{3!}{a!}\frac{(b+c)!}{b!}\,z_1^az_2^bz_3^c,
$$

which is nonzero and constructs every monomial. These monomials form a basis and have distinct weights $(a-b,b-c)$. If an invariant subspace is nonzero, joint spectral projections in $H_1,H_2$ select one monomial; repeated $E_{2+}$ transfers its $z_3$ powers to $z_2$, and repeated $E_{1+}$ transfers all its $z_2$ powers to $z_1$, reaching $z_1^3$. Lowering then generates the whole basis, proving irreducibility without merely assuming the dimension formula. The plotted weights are

$$
\begin{array}{c|c|c}
c&y=(a+b-2c)/\sqrt3&\text{allowed }x=a-b\\\hline
0&\sqrt3&-3,-1,1,3\\
1&0&-2,0,2\\
2&-\sqrt3&-1,1\\
3&-2\sqrt3&0
\end{array}
$$

with multiplicity one at every point. Hence $\boxed{\dim R(3,0)=\binom{5}{2}=10}$.

<a id="4/image-su-3-weights-in-the-three-requested-representations-with-the-two-independent-zero-weight-octet-states-marked"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-45-su3-weights.png)

**[Figure 1](#4/image-su-3-weights-in-the-three-requested-representations-with-the-two-independent-zero-weight-octet-states-marked). SU(3) weights in the three requested representations, with the two independent zero-weight octet states marked**.

For approximate [flavor symmetry](../../../standard-model.md#flavor-symmetry), identify $e_1,e_2,e_3$ with the [up quark](../../../standard-model.md#up-quark), [down quark](../../../standard-model.md#down-quark) and [strange quark](../../../standard-model.md#strange-quark). The defining representation is their flavour triplet. The [baryon octet](../../../standard-model.md#baryon-octet) realizes $R(1,1)$ and contains the spin-$1/2$ nucleons and the $\Lambda,\Sigma,\Xi$ multiplets; its central double weight distinguishes $\Lambda$ and $\Sigma^0$. The [baryon decuplet](../../../standard-model.md#baryon-decuplet) realizes the symmetric flavour representation $R(3,0)$, containing the spin-$3/2$ $\Delta,\Sigma^*,\Xi^*,\Omega$ multiplets. In standard [isospin](../../../standard-model.md#isospin) and [flavor hypercharge](../../../standard-model.md#flavor-hypercharge) normalization, $I_3=h_1/2$ and $Y=(h_1+2h_2)/3$, so these plots use $x=2I_3$ and $y=\sqrt3Y$. Three-quark spin and flavour combine subject to the [Pauli constraint on three-quark flavour multiplets](../../../physics.md#pauli-constraint-on-three-quark-flavour-multiplets) and the antisymmetric [three-quark colour singlet](../../../physics.md#three-quark-colour-singlet). The adjoint flavour representation also describes a meson octet. A distinct, exact colour [SU(3)](../../../topological-group.md#su-3-group) gauge symmetry places [quarks](../../../standard-model.md#quark) in its defining representation and [gluons](../../../standard-model.md#gluon) in its adjoint octet; colour and flavour here are different physical group actions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
