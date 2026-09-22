<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use signature $\eta=\operatorname{diag}(1,-1,-1,-1)$, the numerical [matrices](../../../../../matrix.md) $\sigma_\mu=(I,\sigma_i)$ and $\bar\sigma_\mu=(I,-\sigma_i)$ given in the question, and raise genuine [tensor](../../../../../tensor.md) indices with $\eta$. A real [Minkowski spacetime](../../../../../minkowski-spacetime.md) vector corresponds to the [Hermitian matrix](../../../../../hermitian-operator.md)

$$
X=x^0I+\mathbf x\cdot\boldsymbol\sigma,\qquad \det X=(x^0)^2-|\mathbf x|^2.
$$

For [SL(2,C)](../../../../../complex-special-linear-group-in-dimension-two.md) [matrices](../../../../../matrix.md), $X'=AXA^\dagger$ is Hermitian and has the same [determinant](../../../../../determinant.md). It therefore induces a real linear [Lorentz transformation](../../../../../lorentz-transformation.md); composition of the congruence actions agrees with [matrix](../../../../../matrix.md) multiplication. The kernel consists of $\pm I$: preservation of $X=I$ makes a kernel element unitary, and preservation of every Hermitian $X$ makes it scalar.

[Polar decomposition of an invertible complex matrix](../../../../../polar-decomposition-of-an-invertible-complex-matrix.md) connects every determinant-one complex [matrix](../../../../../matrix.md) to its unitary factor, so the group is connected. The action gives the [Lorentz spinor double cover](../../../../../lorentz-spinor-double-cover.md) of the [Proper orthochronous Lorentz group](../../../../../proper-orthochronous-lorentz-group.md). It covers rotations via $A_R=e^{-i\vartheta\mathbf n\cdot\boldsymbol\sigma/2}$ and boosts via the positive Hermitian [matrices](../../../../../matrix.md) below. Every proper orthochronous transformation is a boost followed by a rotation, since one can first match its image of the future unit time vector and then use its rotation stabilizer. **The congruence construction does not cover spatial parity or time reversal.** In particular parity has [determinant](../../../../../determinant.md) $-1$ as a four-vector transformation; all transformations continuously produced from [SL(2,C)](../../../../../complex-special-linear-group-in-dimension-two.md) have [determinant](../../../../../determinant.md) $+1$.

Set $c_\theta=\cosh(\theta/2)$, $s_\theta=\sinh(\theta/2)$ and $N=\mathbf n\cdot\boldsymbol\sigma$. The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $N^2=I$. The proposed boost [matrix](../../../../../matrix.md) is $A_B=c_\theta I+s_\theta N$, with [eigenvalues](../../../../../eigenvalue.md) $e^{\pm\theta/2}$, [determinant](../../../../../determinant.md) one and $A_B^\dagger=A_B$. Split $\mathbf x=x_\parallel\mathbf n+\mathbf x_\perp$. The perpendicular Pauli part anticommutes with $N$, so multiplication gives

$$
\boxed{x'^0=\cosh\theta\,x^0+\sinh\theta\,x_\parallel,\qquad
x'_\parallel=\sinh\theta\,x^0+\cosh\theta\,x_\parallel,\qquad
\mathbf x'_\perp=\mathbf x_\perp.}
$$

This is an active [Lorentz boost](../../../../../lorentz-boost.md). The image of a rest worldline has velocity **$\mathbf v=\tanh\theta\,\mathbf n$**, fixing the velocity sign convention.

For two nonzero boosts, write $A'=c'I+s'\mathbf n'\cdot\boldsymbol\sigma$ and $A=cI+s\mathbf n\cdot\boldsymbol\sigma$. Their product is

$$
A'A=(c'c+s's\mathbf n'\cdot\mathbf n)I
+(c's\mathbf n+s'c\mathbf n')\cdot\boldsymbol\sigma
+i s's(\mathbf n'\times\mathbf n)\cdot\boldsymbol\sigma.
$$

The last term is anti-Hermitian. Thus $A'A$ is not Hermitian unless the axes are collinear; a pure boost has Hermitian lifts $\pm A_B$, so it cannot give the same Lorentz transformation. The [noncollinear boost obstruction from Pauli products](../../../../../noncollinear-boost-obstruction-from-pauli-products.md) is therefore

$$
\boxed{\text{two nonzero noncollinear boosts require an accompanying rotation}.}
$$

That rotation is a [Wigner rotation](../../../../../wigner-rotation.md). A zero-rapidity factor is the trivial exception, regardless of the arbitrary axis assigned to it.

Define $J_i=\tfrac12\epsilon_{ijk}M_{jk}$ and $K_i=M_{0i}$. The printed [Lorentz algebra](../../../../../lorentz-algebra.md) brackets give

$$
[J_i,J_j]=i\epsilon_{ijk}J_k,\qquad
[J_i,K_j]=i\epsilon_{ijk}K_k,\qquad
[K_i,K_j]=-i\epsilon_{ijk}J_k.
$$

Set $L_i=(J_i+iK_i)/2$, $R_i=(J_i-iK_i)/2$. Then

$$
\boxed{[L_i,L_j]=i\epsilon_{ijk}L_k,\quad
[R_i,R_j]=i\epsilon_{ijk}R_k,\quad [L_i,R_j]=0.}
$$

This is the [chiral decomposition of the complex Lorentz algebra](../../../../../chiral-decomposition-of-the-complex-lorentz-algebra.md). The two copies are the complexifications of the [SU(2)](../../../../../su-2-group.md) algebras conventionally labelled left and right. They are not two independent compact real subalgebras of the real Lorentz algebra: $L,R$ are complex linear combinations of the real generators. The distinction is needed for noncompact boosts.

To verify the infinitesimal two-component action, put

$$
a=\frac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu,\qquad A=I+a+O(\omega^2).
$$

Its trace vanishes by antisymmetry, so $\det A=1+O(\omega^2)$. The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) implies

$$
\sigma_\mu\bar\sigma_\nu\sigma_\rho+\sigma_\rho\bar\sigma_\nu\sigma_\mu
=2(\eta_{\mu\nu}\sigma_\rho+\eta_{\nu\rho}\sigma_\mu-\eta_{\mu\rho}\sigma_\nu).
$$

Since $a^\dagger=\tfrac14\omega^{\mu\nu}\bar\sigma_\nu\sigma_\mu$, antisymmetrizing this identity yields

$$
a\sigma_\rho+\sigma_\rho a^\dagger
=\omega^\mu{}_{\rho}\sigma_\mu.
$$

Consequently $AXA^\dagger=X+\sigma_\mu\omega^\mu{}_{\nu}x^\nu+O(\omega^2)$, exactly the claimed infinitesimal coordinate transformation with $\omega^\mu{}_{\nu}=\omega^{\mu\rho}\eta_{\rho\nu}$.

The two [Weyl spinor](../../../../../weyl-spinor.md) representations transform as

$$
\boxed{\psi_L\mapsto A\psi_L,\qquad \psi_R\mapsto(A^\dagger)^{-1}\psi_R.}
$$

Both maps preserve group multiplication. For $\Lambda=e^\omega$, choose its spin lift and write the finite [matrices](../../../../../matrix.md) as

$$
A=\exp\left(\frac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu\right),\qquad
(A^\dagger)^{-1}=\exp\left(\frac14\omega^{\mu\nu}\bar\sigma_\mu\sigma_\nu\right).
$$

For rotations these coincide as the [SU(2)](../../../../../su-2-group.md) doublet; for boosts their generator signs are opposite. Any complex-linear intertwiner would commute with all rotations and hence be scalar by the [Schur lemma](../../../../../schur-s-lemma.md), but a nonzero scalar cannot intertwine the opposite boost [matrices](../../../../../matrix.md). They are therefore inequivalent. Infinitesimally their $K_i$ [matrices](../../../../../matrix.md) are $-i\sigma_i/2$ and $+i\sigma_i/2$, while their $J_i$ [matrices](../../../../../matrix.md) are both $\sigma_i/2$. Thus they have chiral labels $(1/2,0)$ and $(0,1/2)$. The finite [matrices](../../../../../matrix.md) are representations of the spin cover; choosing $A$ or $-A$ matters for spinors even though their four-vector transformations coincide.

Using the supplied block [gamma matrices](../../../../../gamma-matrices.md), the generator of the [Dirac spinor](../../../../../dirac-spinor.md) is

$$
\Omega=\frac14\omega^{\mu\nu}\gamma_{\mu\nu}
=\begin{pmatrix}\tfrac14\omega^{\mu\nu}\sigma_\mu\bar\sigma_\nu&0\\0&\tfrac14\omega^{\mu\nu}\bar\sigma_\mu\sigma_\nu\end{pmatrix}.
$$

The antisymmetry of $\omega$ removes the symmetric Clifford part. Hence

$$
\boxed{\psi\mapsto S\psi,\qquad S=e^\Omega=\operatorname{diag}(A,(A^\dagger)^{-1}).}
$$

There is a conjugation-order error in the last displayed gamma identity in the PDF. The [Clifford algebra](../../../../../clifford-algebra.md) gives, with $\gamma^\rho=\eta^{\rho\sigma}\gamma_\sigma$,

$$
[\gamma_{\mu\nu},\gamma^\rho]=2(\delta_\nu^\rho\gamma_\mu-\delta_\mu^\rho\gamma_\nu),\qquad
[\Omega,\gamma^\rho]=-\omega^\rho{}_{\mu}\gamma^\mu.
$$

Exponentiating this linear [commutator](../../../../../commutator.md) action proves the [inverse Lorentz action on gamma matrices](../../../../../inverse-lorentz-action-on-gamma-matrices.md)

$$
\boxed{S\gamma^\rho S^{-1}=(\Lambda^{-1})^\rho{}_{\mu}\gamma^\mu,\qquad
S^{-1}\gamma^\rho S=\Lambda^\rho{}_{\mu}\gamma^\mu.}
$$

The second identity is the order required for the requested bilinears when $\psi\mapsto S\psi$. An explicit countercheck to the printed order is a positive boost along the third axis: $\omega^{03}=-\theta$ gives

$$
S\gamma^0S^{-1}=\cosh\theta\,\gamma^0-\sinh\theta\,\gamma^3,
$$

whereas the printed right side has a plus sign. This cannot be repaired by dropping index raising; the same raising convention is needed in the preceding coordinate transformation.

The adjoint relation supplied in the question gives $\Omega^\dagger\gamma^0=-\gamma^0\Omega$, hence the [Dirac spinor pseudo-unitarity](../../../../../dirac-spinor-pseudo-unitarity.md) identity $S^\dagger\gamma^0S=\gamma^0$. The [Dirac adjoint](../../../../../dirac-adjoint.md) therefore transforms as $\bar\psi\mapsto\bar\psi S^{-1}$. It now follows that the [Dirac scalar bilinear](../../../../../dirac-scalar-bilinear.md) is

$$
\boxed{\bar\psi'\psi'=\bar\psi S^{-1}S\psi=\bar\psi\psi,}
$$

the vector is

$$
\boxed{\bar\psi'\gamma^\rho\psi'=\Lambda^\rho{}_{\mu}\bar\psi\gamma^\mu\psi,}
$$

and the antisymmetric second-rank [tensor](../../../../../tensor.md) is

$$
\boxed{\bar\psi' i[\gamma^\rho,\gamma^\sigma]\psi'
=\Lambda^\rho{}_{\mu}\Lambda^\sigma{}_{\nu}\bar\psi i[\gamma^\mu,\gamma^\nu]\psi.}
$$

These are respectively a [Lorentz scalar](../../../../../lorentz-scalar.md), [Lorentz four-vector](../../../../../four-vector.md) and [Lorentz tensor](../../../../../lorentz-tensor.md). The source's inconsistent gamma identity is replaced by its correct inverse/order pair; all three transformation laws then follow with the stated spinor transformation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
