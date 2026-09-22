<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For [spatially varying tension in filament bending](../../../../../../spatially-varying-tension-in-filament-bending.md), keep the derivative of the [filament tension](../../../../../../filament-tension.md) as well as the curvature term. The first variation is

$$
\delta\mathcal E=\int_0^L\{Ah''''-(\sigma h')'\}\eta\,dx+
[Ah''\eta'+(\sigma h'-Ah''')\eta]_0^L.
$$

Therefore **the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) and fluctuation operator are**

$$
\boxed{Ah''''-(\sigma h')'=Ah''''-\sigma h''-\sigma'h'=0,\qquad
K_\sigma=A\partial_x^4-\partial_x(\sigma\partial_x).}
$$

For real, sufficiently smooth $\sigma$, the boundary form is the bending boundary form minus $[\sigma(\overline u v'-\overline{u'}v)]_0^L$. Because $\sigma$ vanishes at both ends, the four [self-adjoint endpoint conditions for filament bending](../../../../../../self-adjoint-endpoint-conditions-for-filament-bending.md) still apply. The natural endpoint [force](../../../../../../force.md) also reduces there to the bending shear term. Thus $K_\sigma$ is a [self-adjoint fourth-order scalar differential operator](../../../../../../self-adjoint-fourth-order-scalar-differential-operator.md) on the same chosen domain, with [compact resolvent](../../../../../../compact-resolvent.md).

Choose a real [orthonormal basis](../../../../../../orthonormal-basis.md) $\psi_n$ of [eigenfunctions](../../../../../../eigenfunction.md), $K_\sigma\psi_n=\lambda_n\psi_n$, and write $h=\sum_nb_n\psi_n$. Using the endpoint conditions in [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_0^L[A\psi_n''\psi_m''+\sigma\psi_n'\psi_m']\,dx=\lambda_n\delta_{nm},\qquad
\mathcal E=\frac12\sum_n\lambda_nb_n^2.
$$

The [equipartition theorem](../../../../../../equipartition-theorem.md) now gives, on the strictly positive subspace,

$$
\boxed{\langle b_nb_m\rangle=\frac{k_BT}{\lambda_n}\delta_{nm},\qquad
\operatorname{Var}(h(x))=k_BT\sum_{n:\,\lambda_n>0}\frac{\psi_n(x)^2}{\lambda_n}.}
$$

This is a formal modal construction; no explicit [eigenfunctions](../../../../../../eigenfunction.md) are needed. Nonnegative [filament tension](../../../../../../filament-tension.md) makes the energy nonnegative. Any surviving [zero-energy filament modes](../../../../../../zero-energy-filament-mode.md) must again be fixed. If signed $\sigma$ permits compression, [self-adjointness](../../../../../../self-adjoint-operator.md) still holds but does not guarantee a [canonical ensemble](../../../../../../canonical-ensemble.md): sufficiently strong compression can create negative [eigenvalues](../../../../../../eigenvalue.md) and [Euler buckling of an elastic filament](../../../../../../euler-buckling-of-an-elastic-filament.md). For instance, on $A=L=1$, take $\sigma=-C x(1-x)$ and the clamped trial function $h=x^2(1-x)^2$. Then

$$
\int_0^1(h'')^2\,dx=\frac45,\qquad
\int_0^1 x(1-x)(h')^2\,dx=\frac1{315},
$$

so the energy is negative when $C>252$, despite $\sigma(0)=\sigma(1)=0$. The [equipartition theorem](../../../../../../equipartition-theorem.md) requires a stable positive quadratic energy, not merely a real modal spectrum.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
