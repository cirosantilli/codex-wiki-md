<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the real Lie-algebra convention of the question, with a [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu+A_\mu$. The [gauge field strength](../../../../../gauge-field-strength.md) is its curvature:

$$
\boxed{F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\qquad[D_\mu,D_\nu]=F_{\mu\nu}.}
$$

Write $a_\mu=\delta_XA_\mu/\epsilon=-\partial_\mu X+[X,A_\mu]$. To first order in $\epsilon$,

$$
\epsilon^{-1}\delta_XF_{\mu\nu}=\partial_\mu a_\nu-\partial_\nu a_\mu+[a_\mu,A_\nu]+[A_\mu,a_\nu].
$$

Substitute $a_\mu$. The mixed second derivatives of $X$ cancel. The terms containing first derivatives of $X$ cancel in pairs. The remaining terms are

$$
[X,\partial_\mu A_\nu-\partial_\nu A_\mu]+[[X,A_\mu],A_\nu]+[A_\mu,[X,A_\nu]].
$$

The [Jacobi identity](../../../../../jacobi-identity.md) combines the last two into $[X,[A_\mu,A_\nu]]$. Consequently

$$
\boxed{\delta_XF_{\mu\nu}=\epsilon[X,F_{\mu\nu}].}
$$

The transformation is homogeneous even though the connection transformation contains an inhomogeneous derivative term.

For a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md), define its [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) by $\operatorname{ad}_X(Y)=[X,Y]$ and its [Killing form](../../../../../killing-form.md) by

$$
\kappa(X,Y)=\operatorname{Tr}_{\mathfrak g}(\operatorname{ad}_X\operatorname{ad}_Y).
$$

It is a symmetric [bilinear form](../../../../../bilinear-form.md) by cyclicity of the [trace](../../../../../matrix-trace.md). The [Jacobi identity](../../../../../jacobi-identity.md) gives $\operatorname{ad}_{[Z,X]}=[\operatorname{ad}_Z,\operatorname{ad}_X]$. Set $A=\operatorname{ad}_Z$, $B=\operatorname{ad}_X$, $C=\operatorname{ad}_Y$. Then

$$
\kappa([Z,X],Y)+\kappa(X,[Z,Y])=\operatorname{Tr}([A,B]C+B[A,C])=\operatorname{Tr}(ABC-BCA)=0.
$$

This proves the [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md) property, without assuming simplicity or nondegeneracy.

For definiteness use the [Minkowski metric](../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(1,-1,-1,-1)$ and take a real compact [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) as the gauge algebra. Its positive internal metric is $B=-\kappa$. A [Killing-form Yang-Mills Lagrangian](../../../../../killing-form-yang-mills-lagrangian.md) with the coupling absorbed into the connection is

$$
\boxed{\mathcal L=-\frac1{4g_{\rm YM}^2}B(F_{\mu\nu},F^{\mu\nu})=\frac1{4g_{\rm YM}^2}\kappa(F_{\mu\nu},F^{\mu\nu}),\qquad g_{\rm YM}^2>0.}
$$

The spacetime metric is unchanged by internal [gauge transformations](../../../../../gauge-transformation.md). Hence

$$
\delta_X\mathcal L=\frac{\epsilon}{4g_{\rm YM}^2}\{\kappa([X,F_{\mu\nu}],F^{\mu\nu})+\kappa(F_{\mu\nu},[X,F^{\mu\nu}])\}=0.
$$

Thus [gauge invariance](../../../../../gauge-invariance.md) follows directly from invariance of the [Killing form](../../../../../killing-form.md). Other overall conventions are possible, but the energy sign must be checked rather than inferred from a prefactor in isolation.

For physical kinetic terms the internal form must be real, nondegenerate and positive definite after choosing the overall sign. If $\mathcal E_i=F_{0i}$ and $\mathcal B_i=\tfrac12\epsilon_{ijk}F_{jk}$, the above convention has Lagrangian $[B(\mathcal E_i,\mathcal E_i)-B(\mathcal B_i,\mathcal B_i)]/(2g_{\rm YM}^2)$ and physical [energy](../../../../../energy.md) density

$$
\mathcal H=\frac1{2g_{\rm YM}^2}\sum_i[B(\mathcal E_i,\mathcal E_i)+B(\mathcal B_i,\mathcal B_i)]\ge0.
$$

The canonical [Hamiltonian](../../../../../hamiltonian.md) density also contains the nondynamical multiplier and a spatial divergence. With $\Pi_i=\mathcal E_i/g_{\rm YM}^2$ and $D_i\Pi_i=\partial_i\Pi_i+[A_i,\Pi_i]$, [integration by parts](../../../../../integration-by-parts.md) using the [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md) gives

$$
\mathcal H_{\rm can}=\mathcal H-B(A_0,D_i\Pi_i)+\partial_i B(A_0,\Pi_i).
$$

The [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md) sets $D_i\Pi_i=0$. If the boundary flux vanishes, or the appropriate boundary contribution is included, the integrated physical [Hamiltonian](../../../../../hamiltonian.md) is the positive [energy](../../../../../energy.md) displayed above.

An indefinite internal form would give gauge-field polarizations with opposite kinetic signs. A degenerate form would fail to supply a kinetic term for some directions. The [compactness criterion from the Killing form](../../../../../compactness-criterion-from-the-killing-form.md) says that negative-definiteness of the [Killing form](../../../../../killing-form.md) of a real finite-dimensional algebra is equivalent to compact semisimplicity; thus the pure Killing-form construction selects compact semisimple real forms. One cannot use a complex-bilinear [Killing form](../../../../../killing-form.md) on arbitrary complex field components as if it were a positive Hermitian metric.

This does not prohibit Abelian gauge theories. A compact Abelian factor has zero [Killing form](../../../../../killing-form.md), so it needs a separately chosen positive [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md), rather than the [Killing form](../../../../../killing-form.md). More generally an algebra with a [positive invariant metric on a Lie algebra](../../../../../positive-invariant-metric-on-a-lie-algebra.md) is compact reductive, namely a direct sum of a compact semisimple algebra and an Abelian center. A noncompact group can also share the same compact [Lie algebra](../../../../../lie-algebra-split.md) through global covering choices in an Abelian factor; positivity is a statement about the algebra and internal metric, not by itself a classification of global gauge-group topology. Quantum matter anomalies and global restrictions would require additional input; no matter content is specified here.

For the finite matrix transformation, let $g(x)\in SU(N)$ and regard $g$ as a multiplication operator. The identity $\partial_\mu g^{-1}=-g^{-1}(\partial_\mu g)g^{-1}$ gives

$$
D'_\mu=gD_\mu g^{-1}=\partial_\mu+gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.
$$

Taking commutators of these differential operators cancels the adjacent multiplication operators $g^{-1}g$, yielding

$$
\boxed{F'_{\mu\nu}=gF_{\mu\nu}g^{-1}.}
$$

This argument keeps the derivatives acting on test fields and avoids treating $D_\mu$ as just a matrix.

There is a normalization issue in the printed last paragraph. The standard [Killing form](../../../../../killing-form.md) defined through the adjoint [trace](../../../../../matrix-trace.md) on $\mathfrak{su}(N)$ is

$$
\kappa_{\rm Kill}(X,Y)=2N\operatorname{tr}_{\mathbb C^N}(XY),
$$

not simply $\operatorname{tr}(XY)$. For example, with $N=2$ and $X=Y=-i\sigma_3/2$, the defining trace is $-1/2$, whereas the adjoint trace is $-2$. The printed [trace](../../../../../matrix-trace.md) formula can be used as a rescaled invariant form, with the constant absorbed into the gauge coupling; it has exactly the invariance needed here. For either normalization,

$$
\operatorname{tr}(F'_{\mu\nu}F'^{\mu\nu})=\operatorname{tr}(gF_{\mu\nu}F^{\mu\nu}g^{-1})=\operatorname{tr}(F_{\mu\nu}F^{\mu\nu}),
$$

by cyclicity. This proves finite [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) invariance, with the healthy sign chosen for anti-Hermitian gauge fields. The normalization discrepancy is not a failure of [gauge invariance](../../../../../gauge-invariance.md).

Finally let $g(x)=e^{\epsilon X(x)}=I+\epsilon X(x)+O(\epsilon^2)$. Since $X\in\mathfrak{su}(N)$ is traceless and skew-Hermitian, this exponential lies in $SU(N)$. Expanding the finite formula gives

$$
A'_\mu=A_\mu+\epsilon[X,A_\mu]-\epsilon\partial_\mu X+O(\epsilon^2),\qquad F'_{\mu\nu}=F_{\mu\nu}+\epsilon[X,F_{\mu\nu}]+O(\epsilon^2).
$$

Thus **the stated infinitesimal transformation is the derivative of the finite transformation at the identity**. It describes transformations in the identity component; arbitrary global or large [gauge transformations](../../../../../gauge-transformation.md) need not be generated by one globally defined infinitesimal parameter.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
