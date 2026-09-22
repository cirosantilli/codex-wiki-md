<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose orientation $\epsilon_{1234}=1$ and the anti-Hermitian basis in the question. The [Pauli matrix commutator identity](../../../../../pauli-matrix-commutator-identity.md) gives $[e_a,e_b]=\epsilon_{abc}e_c$. Define the [gauge curvature](../../../../../gauge-field-strength.md) and [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) by

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],
\qquad D_\mu X=\partial_\mu X+[A_\mu,X].
$$

For a compactly supported variation $a_\mu=\delta A_\mu$,

$$
\delta F_{\mu\nu}=D_\mu a_\nu-D_\nu a_\mu.
$$

Antisymmetry and the invariant Lie-algebra inner product therefore give

$$
\delta V=4\int_{\mathbb R^4}\langle F_{\mu\nu},D_\mu a_\nu\rangle
=-4\int_{\mathbb R^4}\langle D_\mu F_{\mu\nu},a_\nu\rangle.
$$

Covariant integration by parts is valid because  
$\langle X,[A,Y]\rangle=-\langle[A,X],Y\rangle$. Thus the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md) are

$$
\boxed{D_\mu F_{\mu\nu}=0,\qquad
\partial_\mu F_{\mu\nu}^a+\epsilon_{abc}A_\mu^bF_{\mu\nu}^c=0.}
$$

The Euclidean [Hodge star operator](../../../../../hodge-star-operator.md) on two-forms is

$$
(*F)_{\mu\nu}=\frac12\epsilon_{\mu\nu\kappa\lambda}F_{\kappa\lambda},
\qquad *^2=1.
$$

The [Anti-self-dual Yang-Mills equations](../../../../../anti-self-dual-yang-mills-equations.md) mean $\boxed{*F=-F}$.

The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) is

$$
\boxed{D_\mu F_{\nu\rho}+D_\nu F_{\rho\mu}+D_\rho F_{\mu\nu}=0.}
$$

To prove it, act on the defining representation with $\nabla_\mu=\partial_\mu+A_\mu$. Its commutator is multiplication by $F_{\mu\nu}$. The operator [Jacobi identity](../../../../../jacobi-identity.md) for $\nabla_\mu,\nabla_\nu,\nabla_\rho$ becomes multiplication by the displayed cyclic sum, which must vanish. Equivalently, substitution of $F=dA+A\wedge A$ into $D_AF$ cancels the ordinary derivatives, leaving the Lie-algebra [Jacobi identity](../../../../../jacobi-identity.md). Contracting the cyclic identity with the alternating tensor gives $D_\mu(*F)_{\mu\nu}=0$. If $*F=-F$, this is exactly $D_\mu F_{\mu\nu}=0$, proving the first-order-to-second-order implication without assuming the field equations.

Let

$$
J=\int_{\mathbb R^4}\epsilon_{\mu\nu\kappa\lambda}
F_{\mu\nu}^aF_{\kappa\lambda}^a\,d^4x
=2\int_{\mathbb R^4}F_{\mu\nu}^a(*F)_{\mu\nu}^a\,d^4x.
$$

All squared component sums below include both orders of each antisymmetric pair, as does the printed energy. Since the [Hodge star](../../../../../hodge-star-operator.md) preserves this norm,

$$
\boxed{V=\frac12\int_{\mathbb R^4}|F+*F|^2\,d^4x-\frac J2
=\frac12\int_{\mathbb R^4}|F-*F|^2\,d^4x+\frac J2.}
$$

Consequently $V\ge |J|/2$. An anti-self-dual field has $J=-2V\le0$ and saturates the first bound. Among all finite-energy potentials with the same value of $J$, it therefore has the absolute minimum $-J/2$. For positive $J$, the saturating sign is self-duality instead; there cannot be a nonzero anti-self-dual solution in that sector. This is the [Yang-Mills instanton Bogomolny bound](../../../../../yang-mills-instanton-bogomolny-bound.md) in the paper's normalization.

For the topological meaning, regard $F=\tfrac12F_{\mu\nu}^ae_a\,dx^\mu\wedge dx^\nu$ as a matrix-valued two-form. Since $\operatorname{tr}(e_ae_b)=-\delta_{ab}/2$,

$$
\operatorname{tr}(F\wedge F)
=-\frac18\epsilon_{\mu\nu\kappa\lambda}
F_{\mu\nu}^aF_{\kappa\lambda}^a\,d^4x.
$$

In the [Second Chern number](../../../../../second-chern-number.md) convention used here,

$$
\boxed{k=\frac1{8\pi^2}\int_{\mathbb R^4}
\operatorname{tr}(F\wedge F)=-\frac{J}{64\pi^2}.}
$$

With the standard instanton boundary condition, the connection approaches a pure gauge at infinity and extends to a bundle over the compactified four-sphere. This makes $k$ an integer, the [instanton number](../../../../../instanton-number.md); reversing the orientation or using the opposite charge convention reverses its sign. The square-completion argument itself does not require quantization or a chosen framing.

One can see the boundary interpretation directly. The [Chern-Simons 3-form](../../../../../chern-simons-3-form.md) obeys

$$
d\,\operatorname{tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right)
=\operatorname{tr}(F\wedge F).
$$

For an asymptotic potential $A=-dg\,g^{-1}$, the flatness identity $dA=-A\wedge A$ gives

$$
k=\frac1{24\pi^2}\int_{S^3_\infty}
\operatorname{tr}\left[(dg\,g^{-1})^{\wedge3}\right].
$$

This is the winding number of $g:S^3_\infty\to SU(2)\cong S^3$, with the corresponding orientation convention. Smooth variations preserving that boundary class cannot change it. Thus the integral in the question labels the topological sector of the [Yang-Mills instanton](../../../../../yang-mills-instanton.md), and in an anti-self-dual sector the energy is $\boxed{V=32\pi^2k}$ with $k\ge0$ in our convention.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
