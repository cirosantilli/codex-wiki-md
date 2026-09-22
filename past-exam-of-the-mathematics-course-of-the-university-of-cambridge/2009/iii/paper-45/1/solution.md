<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md) is obtained by writing a traceless Hermitian matrix as $X=x_i\sigma_i$, where the $\sigma_i$ are the [Pauli matrices](../../../../../pauli-matrices.md), and defining $AXA^\dagger=(R(A)x)_i\sigma_i$. Explicitly,

$$
R_{ij}(A)=\frac12\operatorname{tr}(\sigma_iA\sigma_jA^\dagger).
$$

Conjugation preserves $\tfrac12\operatorname{tr}X^2=|x|^2$, so $R(A)$ is orthogonal; connectedness of [SU(2)](../../../../../su-2-group.md) gives $\det R(A)=1$. Composition of conjugations makes $R$ a [group homomorphism](../../../../../group-homomorphism.md). A matrix in its kernel commutes with every [Pauli matrix](../../../../../pauli-matrices.md), so is scalar, and unit determinant then gives $A=\pm I$. Every spatial rotation occurs: $A=\exp(-i\theta\widehat n\cdot\sigma/2)$ induces the rotation through angle $\theta$ about $\widehat n$. Thus

$$
\boxed{SO(3)\cong SU(2)/\{\pm I\}.}
$$

Since [SU(2)](../../../../../su-2-group.md) is the simply connected three-sphere, this is the universal double cover; the two [Lie algebras](../../../../../lie-algebra-split.md) are isomorphic, although the [groups](../../../../../group-split.md) are not.

Define the [conjugate fundamental spinor of SU(2)](../../../../../conjugate-fundamental-spinor-of-su-2.md) by $\bar\eta_\alpha=(\eta^\alpha)^*$. Regard $\bar\eta$ as a row, so unitarity gives

$$
\boxed{\bar\eta'_\alpha=\bar\eta_\beta(A^\dagger)^\beta{}_\alpha=\bar\eta_\beta(A^{-1})^\beta{}_\alpha.}
$$

Consequently $\bar\eta_\alpha\xi^\alpha$ is an invariant Hermitian pairing. The basic [invariant tensors](../../../../../invariant-tensor.md) are the [Kronecker delta](../../../../../kronecker-delta.md) $\delta^\alpha{}_\beta$ and the alternating tensors $\epsilon_{\alpha\beta}$ and $\epsilon^{\alpha\beta}$. Choose $\epsilon_{12}=1$, $\epsilon^{12}=-1$, so that $\epsilon^{\alpha\gamma}\epsilon_{\gamma\beta}=\delta^\alpha{}_\beta$. The unit-determinant identity $A^T\epsilon A=\epsilon$ makes $[\eta,\xi]=\epsilon_{\alpha\beta}\eta^\alpha\xi^\beta$ invariant; its inverse gives the corresponding upper-index invariant. These contractions generate the tensor invariants of the defining representation. In particular $\widetilde\eta^\alpha=\epsilon^{\alpha\beta}\bar\eta_\beta$ transforms by $A$, showing that the conjugate representation is equivalent to the defining one. The antilinear map $\eta\mapsto\widetilde\eta$ squares to $-I$, so this is a [pseudoreal representation](../../../../../pseudoreal-representation.md), rather than a real structure.

For [Representation theory of SU2](../../../../../representation-theory-of-su-2.md), take $V_n=\operatorname{Sym}^n\mathbb C^2$, with $A$ acting on every index of a [symmetric tensor](../../../../../symmetric-tensor.md). Its independent components are determined by the number $r$ of indices equal to $2$, so there are $n+1$ of them. Equivalently, the [homogeneous polynomial representation of SU2](../../../../../homogeneous-polynomial-representation-of-su2.md) has basis $z_1^{n-r}z_2^r$, $0\leq r\leq n$, with

$$
H=z_1\partial_{z_1}-z_2\partial_{z_2},\qquad E_+=z_1\partial_{z_2},\qquad E_-=z_2\partial_{z_1}.
$$

The basis weights are $n,n-2,\ldots,-n$, and the [raising operator](../../../../../raising-operator.md) and [lowering operator](../../../../../lowering-operator.md) connect consecutive basis vectors with nonzero coefficients until their endpoints. Any nonzero invariant subspace contains a weight vector, by applying polynomial spectral projections in $H$. Raising it reaches $z_1^n$, and lowering then obtains the entire basis. Thus $V_n$ is an [irreducible representation](../../../../../irreducible-representation.md), of [spin](../../../../../spin.md) $j=n/2$. The [classification of finite-dimensional representations of SU2](../../../../../classification-of-finite-dimensional-representations-of-su2.md) gives every finite-dimensional complex irreducible representation in this way. The central element $-I$ acts on a rank-$n$ tensor as $(-1)^n$, so [descent of an SU(2) representation to SO(3)](../../../../../descent-of-an-su-2-representation-to-so-3.md) gives

$$
\boxed{\dim V_n=n+1,\qquad V_n\text{ descends to }SO(3)\iff n\text{ is even}.}
$$

For the [tensor contractions in the SU2 Clebsch-Gordan decomposition](../../../../../tensor-contractions-in-the-su2-clebsch-gordan-decomposition.md), contract $r$ indices of $S$ with $r$ indices of $T$ using $\epsilon$, and symmetrize all the remaining free indices:

$$
U_r^{\alpha_1\ldots\alpha_{m+n-2r}}=
\operatorname{Sym}_{\alpha_1,\ldots,\alpha_{m+n-2r}}
\left(\epsilon_{\beta_1\gamma_1}\cdots\epsilon_{\beta_r\gamma_r}
S^{\alpha_1\ldots\alpha_{m-r}\beta_1\ldots\beta_r}
T^{\alpha_{m-r+1}\ldots\alpha_{m+n-2r}\gamma_1\ldots\gamma_r}\right),
\qquad 0\leq r\leq\min(m,n).
$$

Each $U_r$ is an irreducible symmetric tensor in $V_{m+n-2r}$. To prove these are precisely the constituents, use two sets of formal variables $z,w$. The [highest-weight vectors](../../../../../highest-weight-vector.md)

$$
F_r=(z_1w_2-z_2w_1)^r z_1^{m-r}w_1^{n-r}
$$

are killed by the total [raising operator](../../../../../raising-operator.md) $z_1\partial_{z_2}+w_1\partial_{w_2}$ and have weights $m+n-2r$. The determinant factor is invariant; lowering the remaining factor gives an irreducible string of dimension $m+n-2r+1$. Distinct highest weights give inequivalent summands. The [unitary representation](../../../../../unitary-representation.md) on this tensor product makes invariant complements available, and the dimension check

$$
\sum_{r=0}^{\min(m,n)}(m+n-2r+1)=(m+1)(n+1)
$$

exhausts the space. Hence the contractions above are its irreducible projections, up to normalization, and the [Clebsch-Gordan decomposition for SU2](../../../../../clebsch-gordan-decomposition-for-su2.md) is

$$
\boxed{V_m\otimes V_n\cong\bigoplus_{r=0}^{\min(m,n)}V_{m+n-2r}.}
$$

For the [decomposition of three SU(2) spinors](../../../../../decomposition-of-three-su-2-spinors.md), write $Q^{\alpha\beta\gamma}=\eta_1^\alpha\eta_2^\beta\eta_3^\gamma$ and $S^{\alpha\beta\gamma}=Q^{(\alpha\beta\gamma)}$. The contractions

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

In the [quark model](../../../../../quark-model.md), three spin-$1/2$ [quarks](../../../../../quark.md) therefore have total quark [spin](../../../../../spin.md) $S=3/2$ or $S=1/2$. The two spin-$1/2$ copies correspond to coupling the first pair to spin $0$ or spin $1$ before adding the third quark. For ground-state [baryons](../../../../../baryon.md) with orbital angular momentum $L=0$, total $J=S$: the [nucleon](../../../../../nucleon.md) has $J=1/2$ and the [Delta baryon](../../../../../delta-baryon.md) has $J=3/2$. These two coupling copies alone do not assert two unrestricted physical baryon families. The antisymmetric [three-quark colour singlet](../../../../../three-quark-colour-singlet.md), the spatial wavefunction and [flavor symmetry](../../../../../flavor-symmetry.md) must also satisfy the [Pauli constraint on three-quark flavour multiplets](../../../../../pauli-constraint-on-three-quark-flavour-multiplets.md); orbital excitations can give other total angular momenta.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
