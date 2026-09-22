<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) acts on the algebra itself: $\operatorname{ad}_X(Y)=[X,Y]$. In the basis $T_b$, its [matrices](../../../../../matrix.md) are

$$
\boxed{(T_a^{\rm ad})^c{}_b=c^c{}_{ab}.}
$$

For any algebra element $X$, the [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[T_a^{\rm ad},T_b^{\rm ad}]X=[T_a,[T_b,X]]-[T_b,[T_a,X]]=[[T_a,T_b],X].
$$

Therefore the $D\times D$ [matrices](../../../../../matrix.md) satisfy the same [Lie bracket](../../../../../lie-bracket.md) relations:

$$
\boxed{[T_a^{\rm ad},T_b^{\rm ad}]=c^c{}_{ab}T_c^{\rm ad}.}
$$

This construction does not require that the algebra be simple or that the adjoint action be faithful.

For the field calculation, write $A_\mu=A_\mu^aT_a$ and $\lambda=\lambda^aT_a$. In the derivative-plus-connection convention the [Yang-Mills field strength](../../../../../gauge-field-strength.md) is

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\qquad
\delta A_\mu=\partial_\mu\lambda+[A_\mu,\lambda].
$$

The sign of the parameter here is the negative of the matter-field parameter in the usual [gauge transformation in the derivative-plus-connection convention](../../../../../gauge-transformation-in-the-derivative-plus-connection-convention.md). Work with the stated $\lambda$ throughout. Expanding the variation gives

$$
\begin{aligned}
\delta F_{\mu\nu}={}&[\partial_\mu A_\nu-\partial_\nu A_\mu,\lambda]
+[A_\nu,\partial_\mu\lambda]-[A_\mu,\partial_\nu\lambda]\\
&+[\partial_\mu\lambda,A_\nu]+[A_\mu,\partial_\nu\lambda]
+[[A_\mu,\lambda],A_\nu]+[A_\mu,[A_\nu,\lambda]].
\end{aligned}
$$

The second derivatives cancel by commutativity of partial derivatives, and all remaining derivatives of $\lambda$ cancel by antisymmetry of the [Lie bracket](../../../../../lie-bracket.md). The [Jacobi identity](../../../../../jacobi-identity.md) makes the last two terms $[[A_\mu,A_\nu],\lambda]$. Hence

$$
\boxed{\delta F_{\mu\nu}=[F_{\mu\nu},\lambda],\qquad
\delta F^a_{\mu\nu}=c^a{}_{bc}F^b_{\mu\nu}\lambda^c.}
$$

Unlike the connection, the curvature has no inhomogeneous derivative term: it transforms in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md).

The quadratic form $\kappa_{ab}=\operatorname{tr}(T_a^{\rm ad}T_b^{\rm ad})$ is the [Killing form](../../../../../killing-form.md). Its symmetry follows from cyclicity of the [matrix trace](../../../../../matrix-trace.md). Using the just-proved adjoint commutators,

$$
\begin{aligned}
c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}
&=\operatorname{tr}\left([T_c^{\rm ad},T_a^{\rm ad}]T_b^{\rm ad}
+T_a^{\rm ad}[T_c^{\rm ad},T_b^{\rm ad}]\right)\\
&=\operatorname{tr}[T_c^{\rm ad},T_a^{\rm ad}T_b^{\rm ad}]=0.
\end{aligned}
$$

Thus

$$
\boxed{c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}=0.}
$$

Equivalently, each adjoint generator is skew with respect to this invariant bilinear form. This invariance holds even when the [Killing form](../../../../../killing-form.md) is degenerate; no inverse form is needed here.

The spacetime metric used to raise Lorentz indices is unaffected by the internal [gauge transformation](../../../../../gauge-transformation.md). Since $\delta F=-\operatorname{ad}_\lambda F$, invariance gives

$$
\begin{aligned}
\delta\bigl(\kappa_{ab}F^{a\mu\nu}F^b_{\mu\nu}\bigr)
&=\kappa(\delta F^{\mu\nu},F_{\mu\nu})+\kappa(F^{\mu\nu},\delta F_{\mu\nu})\\
&=-\lambda^c\left[c^d{}_{ca}\kappa_{db}+c^d{}_{cb}\kappa_{ad}\right]
F^{a\mu\nu}F^b_{\mu\nu}=0.
\end{aligned}
$$

Therefore **the Killing-form contraction of the field strengths is gauge invariant**, as required for the internal contraction in a [Yang-Mills action](../../../../../yang-mills-action.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
