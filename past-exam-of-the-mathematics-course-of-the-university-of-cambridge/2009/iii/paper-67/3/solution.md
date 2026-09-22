<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let the layer depth be $d$, its imposed temperature drop $\Delta T$, and its dimensional vertical field $B_0\widehat{\mathbf z}$. Use length $d$, thermal time $d^2/\kappa$, velocity $\kappa/d$, temperature $\Delta T$ and field $B_0$ as units. Write the total dimensionless field as $\widehat{\mathbf z}+\mathbf b$, and temperature as the conductive profile plus $\theta$. The [Boussinesq equations](../../../../../boussinesq-equations.md) coupled to the [resistive induction equation](../../../../../resistive-induction-equation.md) are

$$
\begin{aligned}
\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u
&=-\nabla p+\sigma\nabla^2\mathbf u+\sigma R\theta\widehat{\mathbf z}
+\sigma Q(\nabla\times\mathbf b)\times(\widehat{\mathbf z}+\mathbf b),\\
\partial_t\theta+\mathbf u\cdot\nabla\theta&=w+\nabla^2\theta,\\
\partial_t\mathbf b&=\nabla\times[\mathbf u\times(\widehat{\mathbf z}+\mathbf b)]+\zeta\nabla^2\mathbf b,\\
\nabla\cdot\mathbf u&=\nabla\cdot\mathbf b=0.
\end{aligned}
$$

The dimensionless parameters in this normalization are

$$
\boxed{R=\frac{g\alpha_T\Delta T\,d^3}{\nu\kappa},\qquad
\sigma=\frac\nu\kappa,\qquad\zeta=\frac\eta\kappa,\qquad
Q=\frac{B_0^2d^2}{\mu_0\rho\nu\kappa}.}
$$

Here $\alpha_T$ is the thermal expansion coefficient, $\nu$ is [kinematic viscosity](../../../../../kinematic-viscosity.md), $\kappa$ is [thermal diffusivity](../../../../../thermal-diffusivity.md), and $\eta$ is [magnetic diffusivity](../../../../../magnetic-diffusivity.md). The first parameter is the [Rayleigh number](../../../../../rayleigh-number.md) and $\sigma$ is the [Prandtl number](../../../../../prandtl-number.md).

The displayed dispersion relation fixes the magnetic normalization: its $Q$ must be the [thermal-diffusion magnetic-field parameter](../../../../../thermal-diffusion-magnetic-field-parameter.md) above. The conventional [Chandrasekhar number](../../../../../chandrasekhar-number.md) is instead $Q_{\mathrm{Ch}}=B_0^2d^2/(\mu_0\rho\nu\eta)$, so $Q=\zeta Q_{\mathrm{Ch}}$. If $Q$ is reserved for that conventional definition, the magnetic term in the printed polynomial requires an extra factor $\zeta$. We keep $Q$ for the printed polynomial throughout the following calculation.

Linearize about the conductive state. Absorbing linear magnetic pressure into $p$, the magnetic force becomes $\sigma Q\partial_z\mathbf b$. The pressure-eliminated vertical momentum equation is

$$
(\partial_t-\sigma\nabla^2)\nabla^2w
=\sigma R\nabla_h^2\theta+\sigma Q\partial_z\nabla^2b_z.
$$

The normal mode implicit in the given relation has $w,\theta\propto\sin\pi z$ and $b_z\propto\cos\pi z$, as for stress-free, fixed-temperature boundaries with the corresponding vertical-field magnetic conditions. Put $x=k^2$, $p_0=\pi^2$ and $m=x+p_0=\beta^2$. Taking growth proportional to $e^{st+i\mathbf k\cdot\mathbf x_h}$ gives the amplitude equations

$$
(s+m)\Theta=W,\qquad(s+\zeta m)C=\pi W,
\qquad
m(s+\sigma m)W=\sigma R x\Theta-\sigma Qm\pi C.
$$

Their determinant is

$$
\boxed{m(s+m)(s+\sigma m)(s+\zeta m)+\sigma Qmp_0(s+m)-R\sigma x(s+\zeta m)=0.}
$$

This is the stated [vertical-field magnetoconvection dispersion relation](../../../../../vertical-field-magnetoconvection-dispersion-relation.md) after accounting for its field-strength convention. The determinant derivation remains valid even at values where an intermediate division by $s+m$ or $s+\zeta m$ would not be allowed.

For steady marginality set $s=0$. One obtains

$$
\boxed{R_s(x)=\frac{m^3+(Qp_0/\zeta)m}{x}.}
$$

For oscillatory marginality write $s=i\omega$ with $\omega\ne0$. Dividing the polynomial by $m$ gives a real cubic $s^3+A s^2+B s+C_0$, where

$$
A=m(1+\sigma+\zeta),\quad
B=m^2(\sigma+\zeta+\sigma\zeta)+\sigma Qp_0-\frac{R\sigma x}{m},
$$



$$
C_0=\sigma\zeta m^3+\sigma Qp_0m-R\sigma\zeta x.
$$

Its real and imaginary parts imply $\omega^2=B$ and $C_0=AB$. Solving for the [oscillatory convection](../../../../../oscillatory-convection.md) threshold gives

$$
\boxed{R_o(x)=\frac{(\sigma+\zeta)(1+\zeta)}{\sigma}\frac{m^3}{x}
+\frac{\sigma+\zeta}{1+\sigma}\frac{Qp_0m}{x},}
$$

and

$$
\boxed{\omega^2=\frac{\sigma(1-\zeta)}{1+\sigma}Qp_0-\zeta^2m^2.}
$$

A physical oscillatory branch therefore requires $0<\zeta<1$ and positive frequency squared. In particular an algebraic continuation of $R_o$ into $\omega^2<0$ is not an oscillatory onset.

The [steady-Hopf merger in vertical-field magnetoconvection](../../../../../steady-hopf-merger-in-vertical-field-magnetoconvection.md) occurs at zero frequency:

$$
\boxed{Qp_0=\frac{\zeta^2(1+\sigma)}{\sigma(1-\zeta)}m^2.}
$$

Substitution verifies $R_s=R_o$. Equivalently the merged horizontal wavenumber satisfies

$$
k_m^2=\left[\frac{\sigma(1-\zeta)Qp_0}{\zeta^2(1+\sigma)}\right]^{1/2}-p_0.
$$

A finite-wavenumber intersection exists only when this expression is positive. At the intersection the growth polynomial has a double zero root: the nonzero-frequency neutral branch ends there.

For the requested [merger at a magnetoconvection neutral-curve minimum](../../../../../merger-at-a-magnetoconvection-neutral-curve-minimum.md), first note that a curve of the form $R=[A_*m^3+C_*m]/x$ has derivative zero exactly when

$$
A_*m^2(2x-p_0)=C_*p_0.
$$

Its unique positive minimum has $x>p_0/2$, because the left side increases there from zero to infinity. At this minimum $R_c=2A_*m^3/p_0$.

**Merger at the steady minimum.** For $R_s$, the stationarity condition is $m_s^2(2x_s-p_0)=Qp_0^2/\zeta$. Combining it with the merger equation gives

$$
\boxed{x_s=\frac{p_0(\sigma+\zeta)}{2\sigma(1-\zeta)},\qquad
Q_s=\frac{p_0\zeta^2(1+\sigma)(3\sigma-2\sigma\zeta+\zeta)^2}{4\sigma^3(1-\zeta)^3}.}
$$

The corresponding critical Rayleigh number is $R_{s,c}=2(x_s+p_0)^3/p_0$. For fixed positive $\sigma$ and large $Q$, set $\zeta=1-\delta_s$ and retain the leading powers. Then

$$
\boxed{\delta_s\sim\frac{1+\sigma}{\sigma}\left(\frac{\pi^2}{4Q}\right)^{1/3},\qquad
k_s\sim\left(\frac{Q\pi^4}{2}\right)^{1/6},\qquad R_{s,c}\sim\pi^2Q.}
$$

More generally, before taking $\zeta\to1$, the steady minimum obeys $k_s^2\sim[Q\pi^4/(2\zeta)]^{1/3}$.

**Merger at the oscillatory minimum.** Define $A_o=(\sigma+\zeta)(1+\zeta)/\sigma$. The stationarity condition for $R_o$ is

$$
m_o^2(2x_o-p_0)=\frac{\sigma Qp_0^2}{(1+\sigma)(1+\zeta)}.
$$

Combining it with the zero-frequency relation instead gives

$$
\boxed{x_o=\frac{p_0}{2(1-\zeta^2)},\qquad
Q_o=\frac{p_0\zeta^2(1+\sigma)(3-2\zeta^2)^2}{4\sigma(1-\zeta)^3(1+\zeta)^2}.}
$$

Here $R_{o,c}=2A_o(x_o+p_0)^3/p_0$. For fixed $\sigma>0$ and $Q\gg1$, setting $\zeta=1-\delta_o$ gives

$$
\boxed{\delta_o\sim\left[\frac{(1+\sigma)\pi^2}{16\sigma Q}\right]^{1/3},\qquad
k_o\sim\left[\frac{\sigma Q\pi^4}{4(1+\sigma)}\right]^{1/6},\qquad R_{o,c}\sim\pi^2Q.}
$$

These two merger conditions are distinct parameter surfaces, not simultaneous assertions about the same minimum. Both have the [strong-field wavenumber selection in magnetoconvection](../../../../../strong-field-wavenumber-selection-in-magnetoconvection.md) scaling $k=O(Q^{1/6})$.

If the first subleading Rayleigh corrections are desired, let $X_s=[Qp_0^2/(2\zeta)]^{1/3}$ and $X_o=[\sigma Qp_0^2/(2(1+\sigma)(1+\zeta))]^{1/3}$. With parameters bounded in the above regime,

$$
R_{s,c}=\frac{Qp_0}{\zeta}+3X_s^2+O(Q^{1/3}),\qquad
R_{o,c}=\frac{\sigma+\zeta}{1+\sigma}Qp_0+3A_oX_o^2+O(Q^{1/3}).
$$

These retain the $O(Q^{2/3})$ corrections, including the effect of the $O(Q^{-1/3})$ diffusivity deficit at a merger.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
