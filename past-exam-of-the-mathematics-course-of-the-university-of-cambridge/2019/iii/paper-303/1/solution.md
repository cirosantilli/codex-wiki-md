<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md) step has three parts. First split the field into slow and fast [Fourier modes](../../../../../fourier-mode.md), $\phi=\phi_<+\phi_>$, and integrate over the shell $\Lambda/\zeta<|q|<\Lambda$. Second rescale $q'=\zeta q$, or equivalently $x'=x/\zeta$, to restore the [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) to $\Lambda$. Third rescale the field so that the coefficient of $(\nabla\phi)^2/2$ returns to its chosen normalization. The resulting [free energy](../../../../../thermodynamic-free-energy.md) has the same operator expansion but new couplings; iteration traces a [renormalization-group flow](../../../../../renormalization-group-flow.md) in coupling space.

For the first step only, write $F=F_0+V$ and average over the fast modes of the [Gaussian field theory](../../../../../gaussian-field-theory.md). The [cumulant expansion](../../../../../cumulant-expansion.md) gives

$$
F_{\rm eff}[\phi_<]=F_0[\phi_<]+\langle V\rangle_>
-\frac12\langle V^2\rangle_{>,c}
+\frac16\langle V^3\rangle_{>,c}+\cdots.
$$

Here

$$
V=\lambda_0\int d^dx\,
(\phi_<^3+3\phi_<^2\phi_>+3\phi_<\phi_>^2+\phi_>^3).
$$

At order $\lambda_0^2$, the connected contraction of two $3\lambda_0\phi_<\phi_>^2$ vertices gives the low-momentum two-point term. Since $\langle\phi_>^2(x)\phi_>^2(y)\rangle_c=2G_>(x-y)^2$,

$$
\delta F^{(2)}=-9\lambda_0^2
\int d^dx\,d^dy\,\phi_<(x)G_>(x-y)^2\phi_<(y).
$$

Expanding at small external momentum and matching $(\mu'^2/2)\int\phi_<^2$ yields

$$
\boxed{\mu'^2=\mu_0^2-18\lambda_0^2
\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}
\frac1{(q^2+\mu_0^2)^2}+O(\lambda_0^4).}
$$

The first cumulant also produces a term linear in $\phi_<$; it is removed by fixing the one-point function, or equivalently by a [field redefinition](../../../../../field-redefinition.md), and does not change the displayed [one-particle-irreducible correlation function](../../../../../one-particle-irreducible-correlation-function.md) correction to the mass.

The leading vertex correction is order $\lambda_0^3$. Taking $3\lambda_0\phi_<\phi_>^2$ from each of three vertices, the connected [Wick contractions](../../../../../wick-contraction.md) form a triangle. There are eight contractions, so the third cumulant contributes $27\times8/3!=36$ times the triangle integral. At zero external momentum,

$$
\boxed{\lambda'=\lambda_0+36\lambda_0^3
\int_{\Lambda/\zeta<|q|<\Lambda}\frac{d^dq}{(2\pi)^d}
\frac1{(q^2+\mu_0^2)^3}+O(\lambda_0^5).}
$$

For nonzero external momenta the three propagators carry the corresponding shifted loop momenta, with every internal line restricted to the fast shell.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 303](../../paper-303-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
