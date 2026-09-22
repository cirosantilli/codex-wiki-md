<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use anti-Hermitian representation matrices for the [unitary representation](../../../../../unitary-representation.md), so $R(X)^\dagger=-R(X)$. Absorb the [gauge coupling](../../../../../gauge-coupling.md) into the connection, consistently with the transformation law in the PDF. The appropriate [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) is

$$
\boxed{D_\mu\phi=\partial_\mu\phi+R(A_\mu)\phi.}
$$

This has a plus sign because the inhomogeneous part of the connection transformation is $-\epsilon\partial_\mu X$. Its variation is

$$
\begin{aligned}
\frac1\epsilon\delta_X(D_\mu\phi)
&=R(\partial_\mu X)\phi+R(X)\partial_\mu\phi
-R(\partial_\mu X)\phi+R([X,A_\mu])\phi+R(A_\mu)R(X)\phi\\
&=R(X)\partial_\mu\phi+[R(X),R(A_\mu)]\phi+R(A_\mu)R(X)\phi\\
&=R(X)D_\mu\phi.
\end{aligned}
$$

Thus [gauge covariance of a scalar covariant derivative](../../../../../gauge-covariance-of-a-scalar-covariant-derivative.md) gives

$$
\boxed{\delta_X(D_\mu\phi)=\epsilon R(X)D_\mu\phi.}
$$

The cancellation uses that $R$ is a [Lie algebra representation](../../../../../lie-algebra-representation.md), including its commutator identity.

The [gauge field strength](../../../../../gauge-field-strength.md) is

$$
\boxed{F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu],\qquad\delta_XF_{\mu\nu}=\epsilon[X,F_{\mu\nu}].}
$$

It is the curvature appearing in $[D_\mu,D_\nu]\phi=R(F_{\mu\nu})\phi$. The index positions in the PDF are related by the constant [Minkowski metric](../../../../../minkowski-metric.md); lowering the index in its transformation law gives the convention used here.

Take signature $(+,-,-,-)$, let $B$ be a real symmetric gauge-invariant internal form, and let $\langle\cdot,\cdot\rangle_V$ be the positive [Hermitian form](../../../../../hermitian-form.md) preserved by the unitary matter representation. One consistent [Lorentz transformation](../../../../../lorentz-transformation.md) scalar [Lagrangian density](../../../../../lagrangian-density.md) is

$$
\boxed{\mathcal L=-\frac1{4g_{\mathrm{YM}}^2}B(F_{\mu\nu},F^{\mu\nu})+\langle D_\mu\phi,D^\mu\phi\rangle_V-m^2\langle\phi,\phi\rangle_V-\lambda\langle\phi,\phi\rangle_V^2.}
$$

Here $g_{\mathrm{YM}}>0$, $m^2\geq0$, and $\lambda\geq0$ give a simple stable potential. The coupling is in the kinetic normalization because it was absorbed into $A_\mu$; it is not inserted again into $D_\mu$. Taking a zero or another gauge-invariant potential is also possible. A positive nondegenerate $B$ gives the usual physical gauge kinetic energy, as for a compact gauge algebra. More generally the invariance calculation below applies to any symmetric [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md), including the [Killing form](../../../../../killing-form.md).

Under the infinitesimal [gauge-field transformation law](../../../../../gauge-field-transformation-law.md),

$$
\delta_X B(F_{\mu\nu},F^{\mu\nu})=\epsilon\{B([X,F_{\mu\nu}],F^{\mu\nu})+B(F_{\mu\nu},[X,F^{\mu\nu}])\}=0.
$$

Invariance and symmetry of $B$ give the cancellation. For matter, both $\phi$ and $D_\mu\phi$ transform by $R(X)$, so anti-Hermiticity gives

$$
\delta_X\langle v,w\rangle_V=\epsilon\langle R(X)v,w\rangle_V+\epsilon\langle v,R(X)w\rangle_V=0
$$

for either pairing used in the Lagrangian. Its potential is a function of the invariant scalar norm. Therefore $\boxed{\delta_X\mathcal L=0}$, establishing [gauge invariance](../../../../../gauge-invariance.md) of this [Yang-Mills theory](../../../../../yang-mills-theory.md) coupled to a scalar. Contraction of spacetime indices with the Minkowski metric gives Lorentz invariance.

For the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), define the [Lie algebra structure constants](../../../../../structure-constant-of-a-lie-algebra.md) by

$$
[T^a,T^b]=f^{ab}{}_{c}T^c,\qquad\kappa^{ab}=\kappa(T^a,T^b).
$$

Internal superscripts here are basis labels, as in the paper; spacetime indices alone are raised with the Minkowski metric. The [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) and curvature have components

$$
(D_\mu\phi)^a=\partial_\mu\phi^a+f^{bc}{}_{a}A_\mu^b\phi^c,\qquad
F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+f^{bc}{}_{a}A_\mu^b A_\nu^c.
$$

These formulas involve no extra factor of $i$, because the generators use the Lie-algebra convention rather than Hermitian physics generators.

To make the Killing-form sign explicit, write $B=s\kappa$ and $\langle\phi,\psi\rangle_V=s\kappa^{ab}(\phi^a)^*\psi^b$. The literal contraction requested in the paper corresponds to $s=1$. For a [compact real form](../../../../../compact-real-form-of-a-complex-semisimple-lie-algebra.md) of a complex semisimple gauge algebra, its actual positive [inner product](../../../../../inner-product.md) has $s=-1$, since the Killing form is negative definite. With a complex adjoint scalar, the fully expanded [Killing-form Lagrangian for an adjoint scalar](../../../../../killing-form-lagrangian-for-an-adjoint-scalar.md) is

$$
\boxed{\begin{aligned}
\mathcal L_s={}&-\frac{s}{4g_{\mathrm{YM}}^2}\kappa^{ab}
(\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+f^{cd}{}_{a}A_\mu^cA_\nu^d)
(\partial^\mu A^{b\nu}-\partial^\nu A^{b\mu}+f^{ef}{}_{b}A^{e\mu}A^{f\nu})\\
&+s\kappa^{ab}(\partial_\mu\phi^a+f^{cd}{}_{a}A_\mu^c\phi^d)^*
(\partial^\mu\phi^b+f^{ef}{}_{b}A^{e\mu}\phi^f)\\
&-s m^2\kappa^{ab}(\phi^a)^*\phi^b
-\lambda\bigl(\kappa^{ab}(\phi^a)^*\phi^b\bigr)^2.
\end{aligned}}
$$

All repeated internal labels are summed; $s^2=1$ explains the absence of $s$ from the quartic term. Invariance is equivalently the component identity $f^{ca}{}_{d}\kappa^{db}+f^{cb}{}_{d}\kappa^{ad}=0$. For a real adjoint scalar, omit complex conjugation and insert $1/2$ in the scalar kinetic and quadratic mass terms; the same invariance proof applies.

The PDF's identification of the Killing form with an inner product thus requires a sign convention. It also requires nondegeneracy if it is to give ordinary kinetic terms: on an Abelian gauge factor the Killing form vanishes, so an additional invariant metric is needed there. These qualifications do not alter the covariance identities or the formal gauge invariance of the displayed Killing-form contractions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 302](../../paper-302-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
