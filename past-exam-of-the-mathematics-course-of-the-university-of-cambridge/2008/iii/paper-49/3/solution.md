<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose the convention $\psi'=g\psi$ for a field in the defining representation and $D_\mu=\partial_\mu+A_\mu$. Requiring $D_\mu'\psi'=gD_\mu\psi$ gives the [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md)

$$
\boxed{A_\mu'=gA_\mu g^{-1}-(\partial_\mu g)g^{-1}.}
$$

The [gauge field strength](../../../../../gauge-field-strength.md) is the curvature $[D_\mu,D_\nu]=F_{\mu\nu}$, so

$$
\boxed{F_{\mu\nu}'=gF_{\mu\nu}g^{-1}.}
$$

For an adjoint field $Y$, the [adjoint covariant derivative](../../../../../adjoint-covariant-derivative.md) is $D_\mu Y=\partial_\mu Y+[A_\mu,Y]$, and direct substitution gives $D_\mu'Y'=g(D_\mu Y)g^{-1}$. Consequently $D_\mu F_{\nu\rho}$ transforms by conjugation too.

The [Killing-form invariance under a Lie-group adjoint action](../../../../../killing-form-invariance-under-a-lie-group-adjoint-action.md) gives $\kappa(gYg^{-1},gZg^{-1})=\kappa(Y,Z)$. Its proof is that the adjoint matrices are conjugated by the same invertible map, leaving their trace product unchanged. With $s=\kappa(F_{\mu\nu},F^{\mu\nu})$, both $s^p$ and $\kappa(D_\mu F_{\nu\rho},D^\mu F^{\nu\rho})$ are therefore gauge invariant.

For their field equations, take a compactly supported variation $a_\mu=\delta A_\mu$. Curvature varies by

$$
\delta F_{\mu\nu}=D_\mu a_\nu-D_\nu a_\mu.
$$

The invariant form permits [gauge-covariant integration by parts](../../../../../gauge-covariant-integration-by-parts.md), because $\partial_\mu\kappa(Y,Z)=\kappa(D_\mu Y,Z)+\kappa(Y,D_\mu Z)$. Antisymmetry of $F$ gives

$$
\delta(s^p)=4p\,s^{p-1}\kappa(D_\mu a_\nu,F^{\mu\nu}).
$$

Integrating, the [power of the Yang-Mills invariant](../../../../../power-of-the-yang-mills-invariant.md) gives the equation

$$
\boxed{D_\mu\bigl(s^{p-1}F^{\mu\nu}\bigr)=0.}
$$

For $p=1$ this recovers the [Yang-Mills equations](../../../../../yang-mills-equations.md). For larger $p$, keep the displayed product form, including at $s=0$.

For the derivative-squared action, write $B_{\mu\nu\rho}=D_\mu F_{\nu\rho}$. Varying the derivative as well as the curvature gives

$$
\delta B_{\mu\nu\rho}=D_\mu\delta F_{\nu\rho}+[a_\mu,F_{\nu\rho}].
$$

Its first variation is

$$
\delta S_2=2\int\kappa(D^\mu F^{\nu\rho},D_\mu\delta F_{\nu\rho})\,d^4x
+2\int\kappa(D^\mu F^{\nu\rho},[a_\mu,F_{\nu\rho}])\,d^4x.
$$

Integrate the first term once, substitute $\delta F_{\nu\rho}=D_\nu a_\rho-D_\rho a_\nu$, and integrate again. It becomes $4\int\kappa(a_\nu,D_\mu D^2F^{\mu\nu})d^4x$, where $D^2=D_\lambda D^\lambda$. Invariance converts the second term into $2\int\kappa(a_\nu,[F_{\rho\sigma},D^\nu F^{\rho\sigma}])d^4x$. Nondegeneracy of the Killing form and arbitrary variations yield the [derivative-squared Yang-Mills action](../../../../../derivative-squared-yang-mills-action.md) equation

$$
\boxed{2D_\mu D_\lambda D^\lambda F^{\mu\nu}+[F_{\rho\sigma},D^\nu F^{\rho\sigma}]=0.}
$$

The derivative order matters because covariant derivatives generally do not commute. In an abelian limit the commutator term vanishes and the equation reduces to $\Box\partial_\mu F^{\mu\nu}=0$, a useful check on the fourth-order equation for the potential.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
