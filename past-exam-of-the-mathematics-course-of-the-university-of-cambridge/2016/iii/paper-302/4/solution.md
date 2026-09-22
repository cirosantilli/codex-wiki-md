<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Non-Abelian gauge theory](../../../../../yang-mills-theory.md) promotes an internal [group representation](../../../../../group-representation.md) symmetry to a spacetime-dependent transformation and introduces a [gauge field](../../../../../gauge-field.md) so that differentiation transforms covariantly. The symmetry is a [gauge redundancy](../../../../../gauge-redundancy.md): physically meaningful quantities must be invariant under local changes of field representative. We work in four-dimensional [Minkowski spacetime](../../../../../minkowski-spacetime.md) with signature $(+---)$, and use [skew-Hermitian matrix](../../../../../skew-hermitian-matrix.md) generators throughout.

For the compact [Simple Lie group](../../../../../simple-lie-group.md) $G$, its real [Lie algebra](../../../../../lie-algebra-split.md) has a negative-definite [Killing form](../../../../../killing-form.md). Hence $B=-\kappa$ is a positive [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md). Choose a $B$-orthonormal basis $T_a$, $a=1,\ldots,\dim G$, with $[T_a,T_b]=f_{ab}{}^cT_c$. Invariance makes $f_{abc}=B([T_a,T_b],T_c)$ fully antisymmetric. This construction uses the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) and works independently of any chosen scalar representation.

Let $\mathcal A_\mu=\mathcal A_\mu^aT_a$ be a Lie-algebra-valued [gauge potential](../../../../../gauge-field.md), with the coupling absorbed into this connection. If $R$ is the given finite-dimensional [irreducible representation](../../../../../irreducible-representation.md) of $G$, its [Lie algebra representation](../../../../../lie-algebra-representation.md) $\rho=dR$ defines

$$
\boxed{D_\mu\Phi=\partial_\mu\Phi+\rho(\mathcal A_\mu)\Phi.}
$$

For a finite local transformation $U(x)\in G$, require $\Phi'=R(U)\Phi$ and $D'_\mu\Phi'=R(U)D_\mu\Phi$. Differentiating the first equation forces the [gauge-field transformation law](../../../../../gauge-field-transformation-law.md)

$$
\boxed{\mathcal A'_\mu=U\mathcal A_\mu U^{-1}-(\partial_\mu U)U^{-1}.}
$$

Thus the [gauge potential](../../../../../gauge-field.md) transforms inhomogeneously; an ordinary derivative alone would leave an uncancelled derivative of $U$.

The commutator of [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md) determines the [gauge field strength](../../../../../gauge-field-strength.md):

$$
[D_\mu,D_\nu]=\rho(\mathcal F_{\mu\nu}),\qquad\mathcal F_{\mu\nu}=\partial_\mu\mathcal A_\nu-\partial_\nu\mathcal A_\mu+[\mathcal A_\mu,\mathcal A_\nu].
$$

The [Lie algebra representation](../../../../../lie-algebra-representation.md) preserves the bracket, so this formula holds for any $R$, including a trivial scalar representation. The [gauge field strength](../../../../../gauge-field-strength.md) itself is defined in the gauge algebra. The transformation of the connection implies

$$
\boxed{\mathcal F'_{\mu\nu}=U\mathcal F_{\mu\nu}U^{-1}.}
$$

It is therefore covariant, rather than invariant as a Lie-algebra-valued quantity.

For infinitesimal $U=1+\epsilon+O(\epsilon^2)$, the same equations give the [infinitesimal gauge transformation with an anti-Hermitian connection](../../../../../infinitesimal-gauge-transformation-with-an-anti-hermitian-connection.md):

$$
\boxed{\delta\Phi=\rho(\epsilon)\Phi,\qquad\delta\mathcal A_\mu=-\partial_\mu\epsilon+[\epsilon,\mathcal A_\mu],\qquad\delta\mathcal F_{\mu\nu}=[\epsilon,\mathcal F_{\mu\nu}].}
$$

Substitution into $\delta(D_\mu\Phi)$ cancels the terms containing $\partial_\mu\epsilon$ and gives $\delta(D_\mu\Phi)=\rho(\epsilon)D_\mu\Phi$, the [gauge covariance of a scalar covariant derivative](../../../../../gauge-covariance-of-a-scalar-covariant-derivative.md).

The [Yang-Mills theory](../../../../../yang-mills-theory.md) has [Lagrangian density](../../../../../lagrangian-density.md)

$$
\boxed{\mathcal L_{\mathrm{YM}}=-\frac1{4g_{\mathrm{YM}}^2}B(\mathcal F_{\mu\nu},\mathcal F^{\mu\nu})=\frac1{4g_{\mathrm{YM}}^2}\kappa(\mathcal F_{\mu\nu},\mathcal F^{\mu\nu}).}
$$

This is the [Killing-form Yang-Mills Lagrangian](../../../../../killing-form-yang-mills-lagrangian.md). Its sign uses a positive internal form $B$ and the stated spacetime signature. In a $B$-orthonormal basis it is $-\mathcal F^a_{\mu\nu}\mathcal F^{a\mu\nu}/(4g_{\mathrm{YM}}^2)$. [Gauge invariance](../../../../../gauge-invariance.md) follows because $B$ is invariant under the adjoint group action. Infinitesimally, the variation is proportional to

$$
B([\epsilon,\mathcal F_{\mu\nu}],\mathcal F^{\mu\nu})+B(\mathcal F_{\mu\nu},[\epsilon,\mathcal F^{\mu\nu}])=0.
$$

After rescaling $\mathcal A_\mu=g_{\mathrm{YM}}A_\mu$, the [gauge coupling](../../../../../gauge-coupling.md) appears in $D_\mu=\partial_\mu+g_{\mathrm{YM}}\rho(A_\mu)$ and in the non-Abelian part of the canonically normalized field strength. Squaring that field strength gives cubic and quartic gauge-field self-interactions. An ordinary local quadratic mass term in the [gauge potential](../../../../../gauge-field.md) is not invariant because its transformation contains $\partial_\mu\epsilon$.

For the [scalar field](../../../../../scalar-field.md) kinetic term, compactness supplies a positive invariant [Hermitian form](../../../../../hermitian-form.md) $h$ on its representation space. One can obtain it by averaging any positive form with normalized [Haar measure](../../../../../haar-measure.md), the [unitarization of a compact-group representation](../../../../../unitarization-of-a-compact-group-representation.md). Then $R(U)$ is unitary for $h$, and $\rho(\epsilon)$ is anti-Hermitian. The [Yang-Mills theory coupled to an arbitrary scalar representation](../../../../../yang-mills-theory-coupled-to-an-arbitrary-scalar-representation.md) has

$$
\boxed{\mathcal L=\mathcal L_{\mathrm{YM}}+h(D_\mu\Phi,D^\mu\Phi)-V(\Phi).}
$$

Here $V$ is any real [gauge-invariant scalar potential](../../../../../gauge-invariant-scalar-potential.md), so $V(R(U)\Phi)=V(\Phi)$. For example,

$$
V(\Phi)=m^2h(\Phi,\Phi)+\lambda\,h(\Phi,\Phi)^2
$$

is available for every unitary representation, with $\lambda\geq0$ giving a bounded quartic contribution. Other invariant interactions may exist for particular representations; the potential is not required to depend only on $h(\Phi,\Phi)$.

The scalar kinetic term is [gauge-invariant](../../../../../gauge-invariance.md) because both covariant derivatives transform by the same unitary $R(U)$. Infinitesimally its variation vanishes by

$$
h(\rho(\epsilon)u,v)+h(u,\rho(\epsilon)v)=0.
$$

The potential is invariant by its defining condition. For a real irreducible representation, use the averaged positive symmetric form instead and write the kinetic term as $\tfrac12 h(D_\mu\Phi,D^\mu\Phi)$; all transformation and invariance arguments remain valid. Expansion of the covariant kinetic term produces both the linear gauge-scalar interaction and the quadratic term needed by local [gauge invariance](../../../../../gauge-invariance.md).

**The invariant [inner products](../../../../../inner-product.md), [gauge covariant derivatives](../../../../../gauge-covariant-derivative.md) and [gauge field strength](../../../../../gauge-field-strength.md) together construct the full theory for every compact [Simple Lie group](../../../../../simple-lie-group.md) and every supplied finite-dimensional [irreducible representation](../../../../../irreducible-representation.md) of the scalar fields.** Both finite and infinitesimal transformation laws have been included, and every sign follows the same anti-Hermitian convention.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
