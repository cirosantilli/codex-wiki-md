<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the unperturbed interface rise at pore velocity $U/\phi$, and write its displacement as

$$
\eta=\widehat\eta e^{i\alpha x+\sigma t}.
$$

In each fluid, [Darcy's law](../../../../../darcy-law.md) and [incompressible flow](../../../../../incompressible-flow.md) imply

$$
\mathbf u_j=-\frac{k}{\mu_j}(\nabla p_j+\rho_jg\widehat{\mathbf z}),
\qquad
\nabla^2p_j=0.
$$

The decaying pressure perturbations are proportional to $e^{-\alpha|z|}$. Continuity of normal velocity, the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) $\phi\eta_t=u_n'$, and continuity of pressure give

$$
\boxed{
\sigma=\frac{\alpha U}{\phi}
\left[M+\frac{(\rho_2-\rho_1)kg}{(\mu_1+\mu_2)U}\right]},
\qquad
M=\frac{\mu_2-\mu_1}{\mu_2+\mu_1}.
$$

Thus a less mobile displaced fluid, $\mu_2>\mu_1$, and a denser fluid above a lighter one both drive the [Saffman–Taylor instability](../../../../../saffman-taylor-instability.md).

For immiscible fluids, the [Young–Laplace equation](../../../../../young-laplace-equation.md) adds the pressure jump $-\gamma\eta_{xx}$. The [dispersion relation](../../../../../dispersion-relation.md) becomes

$$
\boxed{
\sigma(\alpha)=\frac{\alpha U}{\phi}
\left[A-C\alpha^2\right]},
$$

where

$$
A=M+\frac{(\rho_2-\rho_1)kg}{(\mu_1+\mu_2)U},
\qquad
C=\frac{\gamma k}{(\mu_1+\mu_2)U}.
$$

If $A>0$, the unstable band is $0<\alpha<\sqrt{A/C}$ and differentiation gives

$$
\boxed{\alpha_{\max}=\sqrt{\frac{A}{3C}}}.
$$

Define the signed characteristic buoyancy velocity

$$
U_b=\frac{k(\rho_2-\rho_1)g}{\mu_2}.
$$

Since $\mu_2/(\mu_1+\mu_2)=(1+M)/2$ and $Ca=\mu_2U/\gamma$,

$$
\boxed{
\alpha_{\max}
=\left[\frac{2Ca}{3k(1+M)}
\left(M+\frac{1+M}{2}\frac{U_b}{U}\right)\right]^{1/2}}.
$$

This expression applies when the quantity in the final parentheses is positive.

Every growth curve starts at the origin. For equal densities its initial slope is proportional to $M$; for $\rho_2>\rho_1$ buoyancy shifts that slope upward, while for $\rho_2<\rho_1$ it shifts it downward. When $A>0$, the curve rises to one positive maximum and then crosses zero before its stabilizing $-\alpha^3$ capillary tail. When $A\leq0$, every nonzero wavenumber decays.

For a prescribed nonzero wavenumber, neutral stability requires

$$
(\mu_2-\mu_1)U+(\rho_2-\rho_1)kg-\gamma k\alpha^2=0,
$$

or

$$
\boxed{
\rho_2=\rho_1-\frac{(\mu_2-\mu_1)U}{kg}
+\frac{\gamma\alpha^2}{g}}.
$$

In the quasistatic limit $U\to0$, viscosity contrast disappears and this reduces to the capillary [Rayleigh-Taylor instability](../../../../../rayleigh-taylor-instability.md) threshold $\rho_2-\rho_1=\gamma\alpha^2/g$. Without surface tension, neutral stability in that limit simply requires equal densities.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
