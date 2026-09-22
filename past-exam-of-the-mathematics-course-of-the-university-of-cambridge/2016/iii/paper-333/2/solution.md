<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The vertical component $q_z=\zeta-f\eta/H$ is $H$ times the first-order anomaly in [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) about rest:

$$
\frac{f+\zeta}{H+\eta}=\frac fH+\frac1H\left(\zeta-\frac{f\eta}{H}\right)+O(\eta^2,\eta\zeta).
$$

Thus $\mathbf q=q_z\widehat{\mathbf z}$ records the combination of [relative vorticity](../../../../../relative-vorticity.md) and column stretching that is conserved by the unforced [linearized shallow water equations](../../../../../linearized-shallow-water-equations.md). Indeed their curl and [continuity equation](../../../../../continuity-equation.md) give $(q_z)_t=0$. It is the persistent forcing of the balanced component during [geostrophic adjustment](../../../../../geostrophic-adjustment.md), while [inertia-gravity waves](../../../../../inertia-gravity-wave.md) carry away the unbalanced component.

Initially $q_z=-f\eta_0\operatorname{sgn}(x)/H$. In the final [geostrophic flow](../../../../../geostrophic-flow.md), $u=0$, $v=g\eta_x/f$, and $\zeta=g\eta_{xx}/f$. Conservation of the linearized [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) therefore gives

$$
\eta_{xx}-R_D^{-2}\eta=-R_D^{-2}\eta_0\operatorname{sgn}(x),\qquad R_D=c/f.
$$

Boundedness on both sides and continuity of $\eta,\eta_x$ at the origin determine the constants:

$$
\boxed{\eta=\begin{cases}\eta_0(1-e^{-x/R_D}),&x>0,\\ \eta_0(-1+e^{x/R_D}),&x<0,\end{cases}\qquad v=\frac{g\eta_0}{fR_D}e^{-|x|/R_D}.}
$$

The solution is the locally attained balanced state after outgoing [inertia-gravity waves](../../../../../inertia-gravity-wave.md) have departed; the full inviscid system need not lose its globally conserved wave energy. The signed [volume flux](../../../../../volumetric-flow-rate.md) in the $y$ direction is

$$
\boxed{\int_{-\infty}^{\infty}Hv\,dx=\frac{gH}{f}[\eta(+\infty)-\eta(-\infty)]=\frac{2c^2\eta_0}{f}.}
$$

For [double Kelvin-wave adjustment at a depth step](../../../../../double-kelvin-wave-adjustment-at-a-depth-step.md), put $c_\pm=\sqrt{gH^\pm}$ and use $R_D^\pm=c_\pm/f$ on the corresponding side of the step. The PDF's far-field wording must mean $\eta\to\eta_0\operatorname{sgn}(x)$, rather than $\eta_0$ for every $x$. In the exponentially trapped outer response, cross-step [geostrophic balance](../../../../../geostrophic-balance.md) gives, at $y=0$,

$$
u^+=-\frac{c_+}{H^+}A,\qquad u^-=\frac{c_-}{H^-}A.
$$

To retain the propagation of this slowly varying trapped disturbance, the along-step acceleration in $u_t-fv=-g\eta_x$ must also be retained. It supplies the small cross-step [ageostrophic flow](../../../../../ageostrophic-flow.md). Thus the two cross-step [volume fluxes](../../../../../volumetric-flow-rate.md) are

$$
H^+v^+=\frac1f\left[c_+^2(2\eta_0\delta(x)-A_x)-c_+A_t\right],\qquad H^-v^-=\frac1f\left[c_-^2(2\eta_0\delta(x)-A_x)+c_-A_t\right].
$$

Here $d\operatorname{sgn}(x)/dx=2\delta(x)$ as a [distributional derivative](../../../../../distributional-derivative.md). Equating the fluxes and dividing by $c_++c_-$ gives

$$
\boxed{A_t+\Delta c\,A_x=2\Delta c\,\eta_0\delta(x),\qquad \Delta c=c_+-c_->0.}
$$

**The printed forcing is missing a factor of two.** It cannot follow from the printed sign-function surface profile with the usual [Dirac delta distribution](../../../../../dirac-delta-function.md) normalization. Pure [geostrophic balance](../../../../../geostrophic-balance.md) in both horizontal directions would also omit $A_t$ and could not determine the wave evolution.

The [method of characteristics](../../../../../method-of-characteristics.md) with zero initial amplitude gives the corrected weak solution

$$
\boxed{A=2\eta_0[\Theta(x)-\Theta(x-\Delta c\,t)]=\eta_0[\operatorname{sgn}(x)-\operatorname{sgn}(x-\Delta c\,t)].}
$$

Behind the eastward front, $0<x<\Delta c\,t$, the surface elevation at the step becomes $-\eta_0$, matching the upstream side. All the original cross-step transport is diverted into flow along the step once the wave has passed a fixed location: $v=0$ there, with opposing along-step velocities above and below the step. This is the **complete barrier in the adjusted region**, and in the long-time limit at every fixed $x$. At finite time a front still carries cross-step flux: the formulas above give $H^\pm v^\pm=(2\eta_0c_+c_-/f)\delta(x-\Delta c\,t)$. The discontinuous outer representation does not resolve the short-scale fast adjustment at either front.

For completeness, solving the equation literally as printed instead gives $A=\eta_0[\Theta(x)-\Theta(x-\Delta c\,t)]$. Its amplitude is half that required; $\eta(x,0,t)$ retains a jump $\eta_0$ at the origin after passage, so that literal equation does not imply complete blocking. The corrected equation and the literal printed equation are distinguished rather than asserting an inconsistent barrier result.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
