<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $H_\pm=H_0\pm d$, with the upper sign referring to $y>0$, and use an [f-plane](../../../../../f-plane.md) with [Coriolis parameter](../../../../../coriolis-parameter.md) $f_0>0$ for the stated directions. The formulas retain the signed $f_0$; a positive [Rossby deformation radius](../../../../../rossby-deformation-radius.md) means $R_\pm=\sqrt{gH_\pm}/|f_0|$. Let $\rho$ be the constant fluid density.

Far from the depth step the problem is independent of $y$. The [linearized shallow water equations](../../../../../linearized-shallow-water-equations.md) imply conservation of $v_x-f_0\eta/H_\pm$. Initially this is $-f_0\eta_0\operatorname{sgn}(x)/H_\pm$. In [geostrophic balance](../../../../../geostrophic-balance.md), $u_s=0$ and $v_s=g\eta_{s,x}/f_0$, so

$$
\eta_s-R_\pm^2\eta_{s,xx}=\eta_0\operatorname{sgn}(x).
$$

Boundedness and matching of height and its derivative at $x=0$ give [geostrophic adjustment of a surface-height jump](../../../../../geostrophic-adjustment-of-a-surface-height-jump.md):

$$
\boxed{\eta_s=\eta_0\operatorname{sgn}(x)(1-e^{-|x|/R_\pm}),\qquad v_s=\frac{g\eta_0}{f_0R_\pm}e^{-|x|/R_\pm},\qquad u_s=0.}
$$

The [potential energy](../../../../../potential-energy.md) release per unit length in $y$ is the finite difference between two individually infinite energies:

$$
\Delta P_\pm=\frac{\rho g}{2}\int_{-\infty}^{\infty}(\eta_0^2-\eta_s^2)\,dx
=\frac{\rho g\eta_0^2}{2}\int_{-\infty}^{\infty}(2e^{-|x|/R_\pm}-e^{-2|x|/R_\pm})\,dx
=\boxed{\frac32\rho g\eta_0^2R_\pm.}
$$

For comparison, the final [kinetic energy](../../../../../kinetic-energy.md) is $\rho g\eta_0^2R_\pm/2$, so the energy radiated in [inertia-gravity waves](../../../../../inertia-gravity-wave.md) is $\rho g\eta_0^2R_\pm$. Integrating the depth-weighted velocity over $x$ gives the volume transports

$$
\boxed{Q_\pm=\int_{-\infty}^{\infty}H_\pm v_s\,dx=\frac{2g\eta_0H_\pm}{f_0}.}
$$

For $f_0,\eta_0>0$, $Q_-$ is towards the step and $Q_+$ is away from it. Their difference is $4g\eta_0d/f_0$; a global steady state cannot simply join the two far-field currents without additional transport along the step.

To obtain the [rotating shallow-water height equation with variable depth](../../../../../rotating-shallow-water-height-equation-with-variable-depth.md), set $\zeta=v_x-u_y$ and $J_H=\partial_x(Hv)-\partial_y(Hu)$. Direct differentiation of the original momentum and continuity equations gives

$$
\eta_{tt}=-f_0J_H+g\nabla_h\cdot(H\nabla_h\eta),\qquad (J_H)_t=f_0\eta_t+gH_y\eta_x.
$$

Consequently

$$
\boxed{\partial_t\left[\eta_{tt}+f_0^2\eta-g\nabla_h\cdot(H\nabla_h\eta)\right]+f_0gH_y\eta_x=0.}
$$

At the step, $H_y=2d\delta(y)$ is a [Dirac delta distribution](../../../../../dirac-delta-function.md); the original matching conditions are used rather than assuming a smooth depth there. Velocity elimination raises the time order: initially $\eta_t=0$ and $\eta_{tt}=g\nabla_h\cdot(H\nabla_h\eta)$, as well as the prescribed initial height.

For a decaying harmonic disturbance, the height equation on each constant-depth side gives

$$
\widehat\eta(y)=\eta_c\begin{cases}e^{\kappa_-y},&y<0,\\e^{-\kappa_+y},&y>0,\end{cases}
\qquad \kappa_\pm=\left[k^2+\frac{f_0^2-\omega^2}{gH_\pm}\right]^{1/2}>0.
$$

Solving the two momentum equations yields

$$
\widehat v=\frac{ig}{f_0^2-\omega^2}(f_0k\widehat\eta+\omega\widehat\eta_y).
$$

Continuity of $H\widehat v$ at the step gives the implicit [step-trapped topographic Rossby wave](../../../../../step-trapped-topographic-rossby-wave.md) dispersion relation

$$
\boxed{\omega(H_+\kappa_++H_-\kappa_-)=2f_0dk.}
$$

This derivation assumes $\omega^2\ne f_0^2$ and positive decay rates; it describes the low-frequency trapped branch, rather than the radiating [inertia-gravity waves](../../../../../inertia-gravity-wave.md).

In the [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md), replace $f_0^2-\omega^2$ by $f_0^2$. The resulting explicit frequency, and then its leading small-$d/H_0$ form, are

$$
\boxed{\omega_{\rm QG}=\frac{2f_0dk}{H_+\sqrt{k^2+R_+^{-2}}+H_-\sqrt{k^2+R_-^{-2}}}
\simeq\frac{f_0d}{H_0}\frac{k}{\sqrt{k^2+R_D^{-2}}},\qquad R_D=\frac{\sqrt{gH_0}}{|f_0|}.}
$$

For $d>0$, the [phase velocity](../../../../../phase-velocity.md) has the sign of $f_0$. Thus propagation is eastward in the Northern Hemisphere, with the shallower side on the right. Differentiating the leading [dispersion relation](../../../../../dispersion-relation.md) gives

$$
c_g=\frac{f_0d}{H_0}\frac{R_D^{-2}}{(k^2+R_D^{-2})^{3/2}}.
$$

In the long-wave limit the [group velocity](../../../../../group-velocity.md) and [phase velocity](../../../../../phase-velocity.md) coincide:

$$
\boxed{c_g=c_p=c_T=\frac{f_0dR_D}{H_0}.}
$$

To find the slow amplitude, integrate the low-frequency height equation across the step. This gives $\partial_t[H\eta_y]=f_0[H]\eta_x$, where brackets mean the upper-side minus lower-side value. For the given exponentially trapped outer profile, $[H\eta_y]=2H_0A/R_D$ and $\eta_x(x,0)=2\eta_0\delta(x)-A_x$. Hence [long-wave transport along a depth step](../../../../../long-wave-transport-along-a-depth-step.md) obeys

$$
\boxed{A_t+c_TA_x=2c_T\eta_0\delta(x),\qquad A(x,0)=0.}
$$

The [method of characteristics](../../../../../method-of-characteristics.md), interpreted for the [Dirac delta distribution](../../../../../dirac-delta-function.md) source, gives

$$
\boxed{A(x,t)=\eta_0[\operatorname{sgn}(x)-\operatorname{sgn}(x-c_Tt)].}
$$

For $c_T>0$ this is $2\eta_0$ in $0<x<c_Tt$ and zero outside: a surface depression is left in the wake of the wave. The sharp $x$-jump is a long-wave outer approximation. The fast adjustment region of width $O(R_D)$ near the origin, and the detailed wavefront, are unresolved. Keeping a smoothed background $\eta_s(x)$ instead would give $A_t+c_TA_x=c_T\eta_s'(x)$ and $A=\eta_s(x)-\eta_s(x-c_Tt)$ at this order.

The along-step [geostrophic flow](../../../../../geostrophic-flow.md) is $u=-g\eta_y/f_0$. Integrating separately over the two sides gives

$$
\boxed{T_-\equiv\int_{-\infty}^0H_-u\,dy=\frac{gH_-A}{f_0},\qquad T_+\equiv\int_0^\infty H_+u\,dy=-\frac{gH_+A}{f_0}.}
$$

In the wake, $T_-=Q_-$ and $T_+=-Q_+$. The shallow-side transport is eastward and the deep-side transport westward, with magnitudes equal to the respective far-field currents. The net along-step transport is $T_-+T_+=-4g\eta_0d/f_0$, balancing their mismatch. These comparisons use the stated leading long-wave and small-depth-contrast approximations.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
