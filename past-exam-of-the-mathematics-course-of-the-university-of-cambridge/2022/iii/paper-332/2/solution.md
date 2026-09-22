<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In the frame of a planar interface moving at speed $V$, the steady liquid temperature obeys $-VT_z=\kappa T_{zz}$ and approaches $T_\infty$. Thus

$$
T=T_\infty+(T_i-T_\infty)e^{-Vz/\kappa}.
$$

The [Stefan condition](../../../../../stefan-condition.md), with negligible solid-side heat flux, gives

$$
LV=c_p(T_i-T_\infty)V,
$$

so $T_i-T_\infty=L/c_p=S\Delta T$. The [kinetic undercooling](../../../../../kinetic-undercooling.md) law then gives

$$
\boxed{V=G(T_m-T_i)=G\Delta T(1-S),}
$$

which requires $S<1$ for advancing solidification.

Scale length with $\kappa/V$, time with $\kappa/V^2$, and temperature with $\Delta T$. The base liquid temperature is $\Theta_0=Se^{-z}$. For an interface displacement $\zeta e^{i\alpha x+\sigma t}$, write the thermal perturbation as

$$
\theta=Ae^{-\lambda z+i\alpha x+\sigma t}.
$$

The [heat equation](../../../../../heat-equation.md) gives

$$
\boxed{\lambda^2-\lambda-\alpha^2-\sigma=0,
\qquad
\lambda=\frac12\left[1+\sqrt{1+4(\alpha^2+\sigma)}\right].}
$$

Linearizing the [Stefan condition](../../../../../stefan-condition.md) gives

$$
\lambda A=S(1+\sigma)\zeta,
$$

while the kinetic law with stabilizing curvature undercooling gives

$$
A=\left[S-(1-S)(\sigma+\Gamma\alpha^2)\right]\zeta,
\qquad
\Gamma=\frac{\gamma G}{\kappa}.
$$

Eliminating $A$ gives the general implicit [dispersion relation](../../../../../dispersion-relation.md)

$$
\boxed{
\frac{S(1+\sigma)}{\lambda}
=S-(1-S)(\sigma+\Gamma\alpha^2),
\qquad
\lambda^2-\lambda=\alpha^2+\sigma.}
$$

At marginal stability $\sigma=0$,

$$
\lambda=\frac12(1+\sqrt{1+4\alpha^2}),
$$

and the dispersion relation becomes

$$
\boxed{\frac S{1-S}=\Gamma\frac{\lambda}{\lambda-1}\alpha^2.}
$$

Since $\alpha^2=\lambda(\lambda-1)$ on this curve, the right-hand side is simply $\Gamma\lambda^2$. A positive cutoff wavenumber therefore exists exactly when

$$
\frac S{\Gamma(1-S)}>1,
\qquad\text{that is,}\qquad
\boxed{S>\frac{\Gamma}{1+\Gamma}.}
$$

The unstable band is $0<\alpha<\alpha_c$, where

$$
\lambda_c=\left[\frac S{\Gamma(1-S)}\right]^{1/2},
\qquad
\alpha_c^2=\lambda_c(\lambda_c-1).
$$

A sketch of $\Gamma\lambda^2$ against the constant $S/(1-S)$ shows no crossing above $\alpha=0$ below threshold and one cutoff above it. As $S\uparrow1$, $\lambda_c$ and $\alpha_c$ diverge like $(1-S)^{-1/2}$, so the range of the [morphological instability of a kinetically limited solidification front](../../../../../morphological-instability-of-a-kinetically-limited-solidification-front.md) becomes unbounded.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
