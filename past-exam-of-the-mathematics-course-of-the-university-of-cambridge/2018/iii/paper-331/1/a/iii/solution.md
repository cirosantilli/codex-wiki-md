<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [linearized boundary condition](../../../../../../../linearized-boundary-condition.md): evaluate at $z=0$ and discard products of perturbations. The [kinematic boundary condition](../../../../../../../kinematic-boundary-condition.md) and [Young–Laplace equation](../../../../../../../young-laplace-equation.md) become

$$
\partial_z\phi_1=\partial_z\phi_2=\eta_t,\qquad
\rho_1\phi_{1t}-\rho_2\phi_{2t}+g(\rho_1-\rho_2)\eta=-\gamma\eta_{xx}.
$$

[Incompressible flow](../../../../../../../incompressible-flow.md) and [irrotational flow](../../../../../../../irrotational-flow.md) give the [Laplace equation](../../../../../../../laplace-equation.md) for each potential. For a [normal mode](../../../../../../../normal-mode.md), the wall conditions select

$$
\phi_1=A_1\cosh[k(z-L_1)]e^{i(kx-\omega t)},\qquad
\phi_2=A_2\cosh[k(z+L_2)]e^{i(kx-\omega t)}.
$$

With $\eta=Be^{i(kx-\omega t)}$, the kinematic conditions give $A_1=i\omega B/[k\sinh(kL_1)]$ and $A_2=-i\omega B/[k\sinh(kL_2)]$. Hence $\widehat\phi_1(0)=i\omega B\coth(kL_1)/k$ and $\widehat\phi_2(0)=-i\omega B\coth(kL_2)/k$. Substitution into the dynamic condition gives the [finite-depth Rayleigh-Taylor dispersion relation](../../../../../../../finite-depth-rayleigh-taylor-dispersion-relation.md):

$$
\boxed{\omega^2[\rho_1\coth(kL_1)+\rho_2\coth(kL_2)]=-g(\rho_1-\rho_2)k+\gamma k^3.}
$$

Its denominator is positive. Assuming $g>0$ and $\gamma>0$, negative $\omega^2$ therefore produces a growing branch $\omega=i\sigma$ with $\sigma>0$, as in [Rayleigh-Taylor instability](../../../../../../../rayleigh-taylor-instability.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
