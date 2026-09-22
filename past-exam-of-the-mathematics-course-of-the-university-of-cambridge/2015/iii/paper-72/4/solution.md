<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $\alpha>0$; a real disturbance with negative [wavenumber](../../../../../wavenumber.md) is recovered by [complex conjugation](../../../../../complex-conjugation.md). To obtain the [pressure equation for a shear-flow normal mode](../../../../../pressure-equation-for-a-shear-flow-normal-mode.md), apply $i\alpha$ to the streamwise momentum equation and differentiate the normal momentum equation. The [mass conservation](../../../../../mass-conservation.md) equation cancels the viscous divergence and the terms proportional to $U-c$, leaving $2i\alpha U'v=\alpha^2p-p''$. Thus **the [fluid pressure](../../../../../fluid-pressure.md) equation and wall value are**

$$
\boxed{p''-\alpha^2p=-2i\alpha U'v,\qquad
p(0)=\frac{u''(0)}{i\alpha R}=\frac{v^{(3)}(0)}{\alpha^2R}.}
$$

The wall value follows from streamwise momentum with [no-slip boundary condition](../../../../../no-slip-boundary-condition.md). Normal momentum also gives $p'(0)=v''(0)/R$.

In the lower [viscous boundary layer](../../../../../viscous-boundary-layer.md), [mass conservation](../../../../../mass-conservation.md) gives $v=O(\alpha\delta)$ if $u=O(1)$. Since $U\sim y$, convection and shear have size $\alpha\delta$ when $c=O(\delta)$; matching these with transverse viscous diffusion gives $R^{-1}\delta^{-2}\sim\alpha\delta$. The [pressure gradient](../../../../../pressure-gradient.md) balance then gives $p=O(\delta)$. Thus **the lower scalings are**

$$
\boxed{\delta=(\alpha R)^{-1/3},\quad c=\delta C,\quad
v=\alpha\delta V,\quad p=\delta P.}
$$

The neglected streamwise viscous term is smaller by $(\alpha\delta)^2$. In these variables the leading equations are

$$
V_Y=-iu,\qquad i(Y-C)u+V=-iP+u_{YY},\qquad P_Y=0.
$$

Differentiating the second and using the first yields **the Airy reduction** $\boxed{u_{YYY}=i(Y-C)u_Y}$.

Put $q=e^{i\pi/6}$, so $q^3=i$. The bounded matching branch of the [Airy function](../../../../../airy-function.md) gives $u_Y=A\operatorname{Ai}(q(Y-C))$; the other independent Airy solution grows along the ray and is excluded. Integrating with the two wall conditions gives

$$
u(Y)=A\int_0^Y\operatorname{Ai}(q(s-C))\,ds,\qquad
V(Y)=-iA\int_0^Y(Y-s)\operatorname{Ai}(q(s-C))\,ds,
$$

while the wall momentum equation gives the constant [fluid pressure](../../../../../fluid-pressure.md)

$$
P_0=-iAq\operatorname{Ai}'(-qC).
$$

Define the convergent [Airy displacement integrals](../../../../../airy-displacement-integral.md)

$$
I_0(C)=\int_0^\infty\operatorname{Ai}(q(s-C))\,ds,\qquad
I_1(C)=\int_0^\infty s\operatorname{Ai}(q(s-C))\,ds.
$$

The [Airy function](../../../../../airy-function.md) equation and its decaying [derivative](../../../../../derivative.md) imply $I_1-CI_0=iq\operatorname{Ai}'(-qC)$. Consequently, as $Y\to\infty$,

$$
\boxed{u\to B=AI_0,\qquad P\to P_0=A(CI_0-I_1),\qquad
V=-iBY+iAI_1+o(1).}
$$

Both differentiated lower momentum and the constant of integration are satisfied; retaining that constant is essential for the final matching.

For the middle region introduce a perturbation [stream function](../../../../../stream-function.md) $\Phi$ with $u=\Phi'$ and $v=-i\alpha\Phi$. The leading [inviscid flow](../../../../../inviscid-flow.md) streamwise equation is

$$
(U-c)\Phi'-U'\Phi=-p,\qquad
\left(\frac{\Phi}{U-c}\right)'=-\frac{p}{(U-c)^2}.
$$

For a [shear flow](../../../../../shear-flow.md), this is the integrated form of the [Rayleigh equation for inviscid shear flow](../../../../../rayleigh-equation-for-inviscid-shear-flow.md). The leading matched solution for fixed $y=O(1)$ is $\Phi\sim BU$, so $u\sim BU'$ and $v\sim-i\alpha BU$. In the overlap with the lower [viscous boundary layer](../../../../../viscous-boundary-layer.md), the first constant correction is

$$
\Phi\sim B(y-c)+\delta P_0=By-\delta AI_1,
$$

which agrees with the integrated lower solution. For a regular smooth profile, the normal momentum equation gives $p'\sim-\alpha^2(U-c)\Phi$. Thus [fluid pressure](../../../../../fluid-pressure.md) variation across a fixed-width middle region is $O(\alpha^2B)$; in the final distinguished scaling this is smaller than its $O(\delta)$ value, so $p\sim\delta P_0$ throughout that region. Since $U\to1$, **the middle [velocity](../../../../../velocity.md) tends to** $\boxed{v\sim-i\alpha B}$, which does not decay and requires another region.

The [fluid pressure](../../../../../fluid-pressure.md) equation becomes $p''-\alpha^2p=0$ when $U\sim1$. Therefore the upper scale is $\Delta=1/\alpha$, with $z=\alpha y$. The inviscid decaying upper solution is

$$
\boxed{p=P_\infty e^{-z},\quad
v=-\frac{iP_\infty}{1-c}e^{-z},\quad
u=-\frac{P_\infty}{1-c}e^{-z}.}
$$

Matching [velocity](../../../../../velocity.md) as $z\downarrow0$ gives $P_\infty\sim\alpha B$; matching [fluid pressure](../../../../../fluid-pressure.md) to the middle region gives $\delta P_0\sim\alpha B$. This is [three-layer long-wave shear-flow matching](../../../../../three-layer-long-wave-shear-flow-matching.md), expressed as a [matched asymptotic expansion](../../../../../matched-asymptotic-expansion.md).

Under $\alpha=kR^{-1/4}$ with fixed positive $k$, $\delta=k^{-1/3}R^{-1/4}$, and $\alpha/\delta=k^{4/3}$. Eliminating the nonzero amplitude $A$ gives **the [Airy wall-layer matching determinant](../../../../../airy-wall-layer-matching-determinant.md) and [dispersion relation](../../../../../dispersion-relation.md)**

$$
\boxed{k^{4/3}I_0(C)+iq\operatorname{Ai}'(-qC)=0.}
$$

Equivalently, with $\mathcal T(C)=\int_{-qC}^{\infty e^{i\pi/6}}\operatorname{Ai}(\zeta)\,d\zeta=qI_0(C)$,

$$
\boxed{k^{4/3}\mathcal T(C)=e^{-i\pi/6}\operatorname{Ai}'(-qC).}
$$

The determinant form does not divide by a possibly vanishing $I_0$. The [wavespeed](../../../../../wave-speed.md) is $c=\delta C$; temporal growth has sign $\operatorname{Im}C$ for positive $\alpha$.

There is a genuine conflict in the printed assumptions: fixed-$k$ $\alpha=kR^{-1/4}$ cannot satisfy $R^{-1/7}\ll\alpha$ as $R\to\infty$. For order-one lower matching amplitudes, constant leading middle [fluid pressure](../../../../../fluid-pressure.md) requires $\alpha^2\ll\delta$, equivalently $\alpha\ll R^{-1/7}$; this is the reverse inequality and is satisfied by the final distinguished scaling. Thinness also requires $\alpha R\gg1$. The [dispersion relation](../../../../../dispersion-relation.md) above is therefore derived under the final distinguished limit, for which the complete consistent window is $R^{-1}\ll\alpha\ll R^{-1/7}$. Both printed limits cannot be imposed simultaneously.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
