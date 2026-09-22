<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At leading order in the [lubrication approximation](../../../../../lubrication-theory.md), surface arclength is horizontal distance. An [insoluble surfactant](../../../../../insoluble-surfactant.md) is transported by the surface [velocity](../../../../../velocity.md), without bulk exchange or diffusion. [Conservation of insoluble surfactant on a moving interface](../../../../../conservation-of-insoluble-surfactant-on-a-moving-interface.md) therefore becomes

$$
\boxed{C_t+\partial_x(Cu_s)=0,\qquad u_s=u(x,h,t).}
$$

The local [hydrostatic pressure](../../../../../hydrostatic-pressure.md) and capillary normal [stress](../../../../../stress.md) give

$$
p_x=\rho g h_x-\partial_x(\gamma h_{xx}).
$$

Solve $\mu u_{zz}=p_x$ with [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) at $z=0$ and [Marangoni stress](../../../../../marangoni-effect.md) $\mu u_z(h)=\gamma_x=-AC_x$. The [velocity](../../../../../velocity.md), surface [velocity](../../../../../velocity.md) and [volume flux per unit width](../../../../../volume-flux-per-unit-width.md) are

$$
\begin{aligned}
u(z)&=\frac{p_x}{2\mu}(z^2-2hz)+\frac{\gamma_x}{\mu}z,\\
u_s&=-\frac{h^2p_x}{2\mu}-\frac{AhC_x}{\mu},\\
q&=-\frac{h^3p_x}{3\mu}-\frac{Ah^2C_x}{2\mu}.
\end{aligned}
$$

[Mass conservation](../../../../../mass-conservation.md), $h_t+q_x=0$, yields the [thin-film equations with insoluble surfactant](../../../../../thin-film-equations-with-insoluble-surfactant.md):

$$
\boxed{h_t=\frac{A}{2\mu}\partial_x(h^2C_x)+\frac{\rho g}{3\mu}\partial_x(h^3h_x)-\frac1{3\mu}\partial_x\left[h^3\partial_x(\gamma h_{xx})\right],}
$$

and the corresponding [surfactant](../../../../../surfactant.md) equation is

$$
\boxed{C_t=\frac{A}{\mu}\partial_x(hCC_x)+\frac{\rho g}{2\mu}\partial_x(Ch^2h_x)-\frac1{2\mu}\partial_x\left[Ch^2\partial_x(\gamma h_{xx})\right].}
$$

The hydrostatic and capillary terms thus affect both the film flux and the surface transport, with different coefficients.

For [finite-mass Marangoni spreading on a liquid film](../../../../../finite-mass-marangoni-spreading-on-a-liquid-film.md), first neglect both pressure-gradient terms. If the spread has size $\ell$, then $C\sim M/\ell$ and $C_x\sim M/\ell^2$, giving surface speed $u_s\sim AMh_0/(\mu\ell^2)$. Equating $\ell/t$ to this speed gives

$$
\boxed{\ell(t)\sim\left(\frac{AMh_0t}{\mu}\right)^{1/3}.}
$$

Set $\ell=(AMh_0t/\mu)^{1/3}$ exactly as a similarity scale, and write

$$
\eta=x/\ell,\qquad h=h_0H(\eta),\qquad C=(M/\ell)\Gamma(\eta).
$$

On the positive half of the pool, substitution produces two [ordinary differential equations](../../../../../ordinary-differential-equation.md):

$$
\boxed{-\frac23\eta H'=(H^2\Gamma')',\qquad-\frac13(\eta\Gamma)'=(H\Gamma\Gamma')'.}
$$

Symmetry fixes the flux integration constant in the second equation to zero, giving $H\Gamma'=-\eta/3$ wherever $\Gamma>0$. Substitution into the first equation gives $\eta H'=H$. Thus the [linear similarity profiles for surfactant spreading](../../../../../linear-similarity-profiles-for-surfactant-spreading.md) have the form

$$
H=k\eta,\qquad\Gamma=\frac{\eta_N-\eta}{3k},\qquad0\leq\eta\leq\eta_N.
$$

The concentration vanishes at the moving front. The two integral constraints are total [surfactant](../../../../../surfactant.md) mass and conservation of the fluid volume relative to the undisturbed layer:

$$
\boxed{2\int_0^{\eta_N}\Gamma\,d\eta=1,\qquad\int_0^{\eta_N}(H-1)\,d\eta=0.}
$$

The first gives $k=\eta_N^2/3$; the second gives $k\eta_N=2$. Therefore $\eta_N^3=6$. In physical variables, the solution is

$$
\boxed{x_N=\left(\frac{6AMh_0t}{\mu}\right)^{1/3},\quad h=\frac{2h_0|x|}{x_N},\quad C=\frac{M}{x_N}\left(1-\frac{|x|}{x_N}\right)\quad(|x|<x_N).}
$$

Outside the pool the leading outer solution has $h=h_0$, $C=0$. In particular, **$h(x_{N-},t)=2h_0$**: the subscript means the one-sided limit just behind the front. As a consistency check, the surface speed there is $x_N/(3t)=\dot x_N$ and the fluid jump satisfies the moving-front [mass conservation](../../../../../mass-conservation.md) condition. This ideal outer solution has a height jump from $2h_0$ to $h_0$.

That jump cannot persist in a physical interface with nonzero gravity or [surface tension](../../../../../surface-tension.md). Across a smoothing region of width $\Delta$, $h$ changes by $O(h_0)$. The Marangoni flux scales as $AMh_0^2/(\mu x_N^2)$. At $g=0$, its balance with the capillary flux $\gamma_0h_0^4/(\mu\Delta^3)$ gives [capillary smoothing of a Marangoni front](../../../../../capillary-smoothing-of-a-marangoni-front.md):

$$
\boxed{\Delta\sim\left(\frac{\gamma_0h_0^2x_N^2}{AM}\right)^{1/3}\propto t^{2/9}.}
$$

Here the [surface tension](../../../../../surface-tension.md) approaches $\gamma_0$ at the surfactant-free edge. The assumed concentration-gradient scale is $M/x_N^2$ even inside the smoothing region.

When gravity dominates capillarity, the hydrostatic flux is $\rho gh_0^4/(\mu\Delta)$. The same balance gives [gravity smoothing of a Marangoni front](../../../../../gravity-smoothing-of-a-marangoni-front.md):

$$
\boxed{\Delta\sim\frac{\rho gh_0^2x_N^2}{AM}\propto t^{2/3}.}
$$

The gravity-dominated condition is $\Delta^2\gg\gamma_0/(\rho g)$, the square of the [capillary length](../../../../../capillary-length.md). **The printed condition omits $\rho$; the expression above restores dimensional consistency.**

This width grows faster than $x_N$. It becomes comparable with the pool size when

$$
\boxed{x_N^*\sim\frac{AM}{\rho gh_0^2},\qquad t^*\sim\frac{\mu(AM)^2}{(\rho g)^3h_0^7}.}
$$

The time is a scaling estimate, so numerical factors cannot be fixed by the width balance. For $t\gg t^*$, the sharp-front similarity profile no longer describes the film: [hydrostatic pressure](../../../../../hydrostatic-pressure.md) levels the layer over the whole pool, and its thickness tends towards $h_0$ with an increasingly small depression beneath the [surfactant](../../../../../surfactant.md). The surface can still spread by [Marangoni stress](../../../../../marangoni-effect.md) while a hydrostatic-pressure-driven return flow nearly cancels the net film flux. In this [gravity-levelled surfactant film](../../../../../gravity-levelled-surfactant-film.md), $q\simeq0$ gives $h_x\simeq-3AC_x/(2\rho gh_0)$, so the fractional height variation is of order $AM/(\rho gh_0^2x_N)\ll1$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
