<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take a local [gauge transformation](../../../../../gauge-transformation.md) $g(x)$ acting on the adjoint field by $\Phi'=g\Phi g^{-1}$. The connection convention $D_\mu=\partial_\mu+[A_\mu,\cdot]$ is compatible with

$$
\boxed{A_\mu'=gA_\mu g^{-1}-(\partial_\mu g)g^{-1},\qquad
D_\mu'\Phi'=g(D_\mu\Phi)g^{-1}.}
$$

Indeed, differentiating $\Phi'$ gives the extra [commutator](../../../../../commutator.md) $[(\partial_\mu g)g^{-1},\Phi']$, exactly cancelled by the inhomogeneous term in the transformed [gauge potential](../../../../../gauge-field.md).

For a direct proof of the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) of curvature, put $\Omega_\mu=(\partial_\mu g)g^{-1}$ and $B_\mu=gA_\mu g^{-1}$. Differentiation gives

$$
\partial_\mu B_\nu=g(\partial_\mu A_\nu)g^{-1}+[\Omega_\mu,B_\nu],
\qquad
\partial_\mu\Omega_\nu-\partial_\nu\Omega_\mu=[\Omega_\mu,\Omega_\nu].
$$

Substituting $A_\mu'=B_\mu-\Omega_\mu$ into the [Yang-Mills field strength](../../../../../gauge-field-strength.md) cancels all terms involving $\Omega$ and leaves

$$
\boxed{F_{\mu\nu}'=gF_{\mu\nu}g^{-1}.}
$$

This direct calculation also applies when the adjoint action has a kernel.

Expand $D_\mu F_{\nu\rho}+D_\nu F_{\rho\mu}+D_\rho F_{\mu\nu}$. The mixed second derivatives of $A$ cancel in pairs. The first-derivative terms from differentiating $[A_\nu,A_\rho]$ cancel the terms from $[A_\mu,\partial_\nu A_\rho-\partial_\rho A_\nu]$. The remaining sum is

$$
[A_\mu,[A_\nu,A_\rho]]+[A_\nu,[A_\rho,A_\mu]]
+[A_\rho,[A_\mu,A_\nu]]=0
$$

by the [Jacobi identity](../../../../../jacobi-identity.md). Thus the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) is

$$
\boxed{D_\mu F_{\nu\rho}+D_\nu F_{\rho\mu}+D_\rho F_{\mu\nu}=0.}
$$

For the variation of the [Yang-Mills action](../../../../../yang-mills-action.md), write $a_\mu=\delta A_\mu$. Differentiating the curvature gives $\delta F_{\mu\nu}=D_\mu a_\nu-D_\nu a_\mu$. Invariance of the [Killing form](../../../../../killing-form.md) implies

$$
\partial_\mu\kappa(X,Y)=\kappa(D_\mu X,Y)+\kappa(X,D_\mu Y).
$$

This is [invariant integration by parts for a gauge covariant derivative](../../../../../invariant-integration-by-parts-for-a-gauge-covariant-derivative.md). Using symmetry of the [Killing form](../../../../../killing-form.md), antisymmetry of $F$, and compactly supported variations,

$$
\begin{aligned}
\delta S_{\mathrm{YM}}
&=\frac1{2e^2}\int d^4x\,\kappa(\delta F_{\mu\nu},F^{\mu\nu})\\
&=\frac1{e^2}\int d^4x\,\kappa(D_\mu a_\nu,F^{\mu\nu})\\
&=-\frac1{e^2}\int d^4x\,\kappa(a_\nu,D_\mu F^{\mu\nu}).
\end{aligned}
$$

Since the [Killing form](../../../../../killing-form.md) of a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) is nondegenerate and the variations are arbitrary, the [Yang-Mills equations](../../../../../yang-mills-equations.md) are

$$
\boxed{D_\mu F^{\mu\nu}=0.}
$$

For the constant [Yang-Mills theta term](../../../../../yang-mills-theta-term.md), symmetry under exchanging the two antisymmetric index pairs gives

$$
\begin{aligned}
\delta S_\theta
&=2\theta\int d^4x\,\epsilon^{\mu\nu\rho\sigma}
\kappa(\delta F_{\mu\nu},F_{\rho\sigma})\\
&=4\theta\int d^4x\,\epsilon^{\mu\nu\rho\sigma}
\kappa(D_\mu a_\nu,F_{\rho\sigma})\\
&=-4\theta\int d^4x\,\epsilon^{\mu\nu\rho\sigma}
\kappa(a_\nu,D_\mu F_{\rho\sigma}),
\end{aligned}
$$

up to the [boundary variation of the Yang-Mills theta term](../../../../../boundary-variation-of-the-yang-mills-theta-term.md). Contracting the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) with $\epsilon^{\mu\nu\rho\sigma}$ makes the last integrand vanish. Therefore **a constant theta term does not alter the bulk [Yang-Mills equations](../../../../../yang-mills-equations.md): $D_\mu F^{\mu\nu}=0$.** Its variation is a boundary term, so this conclusion uses compact support or boundary conditions that remove that term.

Finally apply $D^\rho$ to the [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md), obtaining

$$
D^\rho D_\rho F_{\mu\nu}
=-D^\rho D_\mu F_{\nu\rho}-D^\rho D_\nu F_{\rho\mu}.
$$

The [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) obeys $[D_\alpha,D_\beta]X=[F_{\alpha\beta},X]$. Commute $D^\rho$ past the other derivative. The differentiated divergences vanish by the [Yang-Mills equations](../../../../../yang-mills-equations.md), leaving

$$
\begin{aligned}
D^\rho D_\rho F_{\mu\nu}
&=-[F^\rho{}_\mu,F_{\nu\rho}]
  -[F^\rho{}_\nu,F_{\rho\mu}]\\
&=[F_\mu{}^\rho,F_{\nu\rho}]
  +[F_{\mu\rho},F_\nu{}^\rho].
\end{aligned}
$$

In the last line the second [commutator](../../../../../commutator.md) needs its sign tracked carefully: directly,

$$
-[F^\rho{}_\nu,F_{\rho\mu}]
=-[F_\nu{}^\rho,F_{\mu\rho}]
=[F_{\mu\rho},F_\nu{}^\rho]
=[F_\mu{}^\rho,F_{\nu\rho}].
$$

Thus the simplified sum gives the [covariant wave equation for the Yang-Mills field strength](../../../../../covariant-wave-equation-for-the-yang-mills-field-strength.md)

$$
\boxed{D^\rho D_\rho F_{\mu\nu}
=2[F_\mu{}^\rho,F_{\nu\rho}].}
$$

All spacetime derivatives and index manipulations here use the fixed flat metric.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
