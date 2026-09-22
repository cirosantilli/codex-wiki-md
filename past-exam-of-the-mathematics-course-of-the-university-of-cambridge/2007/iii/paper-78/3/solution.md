<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [insoluble surfactant](../../../../../insoluble-surfactant.md) is advected with the surface fluid and has no exchange with the bulk. With negligible surface diffusion, its amount on a material surface strip is conserved. Under the small-slope [lubrication approximation](../../../../../lubrication-theory.md), surface arclength equals projected horizontal length to leading order, giving

$$
\boxed{C_t+\partial_x(Cu_s)=0,\qquad u_s=u(x,h(x,t),t).}
$$

This is the leading planar form of [conservation of insoluble surfactant on a moving interface](../../../../../conservation-of-insoluble-surfactant-on-a-moving-interface.md).

Let $y$ measure height above the substrate. The normal-stress and vertical momentum conditions give $p=p_{\mathrm{atm}}-\gamma h_{xx}+\rho g(h-y)$, so $p_x=\rho gh_x-(\gamma h_{xx})_x$. Horizontal [Stokes flow](../../../../../stokes-flow-split.md) obeys $\mu u_{yy}=p_x$, with no slip at $y=0$ and [Marangoni stress](../../../../../marangoni-effect.md) $\mu u_y(h)=\gamma_x$. Thus

$$
u=\frac{p_x}{2\mu}(y^2-2hy)+\frac{\gamma_x}\mu y,
$$



$$
q=\int_0^hu\,dy=-\frac{h^3}{3\mu}p_x+\frac{h^2}{2\mu}\gamma_x,\qquad
u_s=-\frac{h^2}{2\mu}p_x+\frac h\mu\gamma_x.
$$

Use $h_t+q_x=0$ and $\gamma_x=-AC_x$ to obtain the [thin-film equations with insoluble surfactant](../../../../../thin-film-equations-with-insoluble-surfactant.md):

$$
\boxed{h_t=\frac A{2\mu}(h^2C_x)_x+\frac{\rho g}{3\mu}(h^3h_x)_x-\frac1{3\mu}[h^3(\gamma h_{xx})_x]_x,}
$$



$$
\boxed{C_t=\frac A\mu(hCC_x)_x+\frac{\rho g}{2\mu}(h^2Ch_x)_x-\frac1{2\mu}[h^2C(\gamma h_{xx})_x]_x.}
$$

The differing flux coefficients are essential: the [surfactant](../../../../../surfactant.md) travels at the surface [velocity](../../../../../velocity.md), not at the depth-averaged liquid [velocity](../../../../../velocity.md).

Neglect the two [pressure](../../../../../pressure.md)-gradient terms for the spreading outer region. If its half-length is $\ell$, fixed [surfactant](../../../../../surfactant.md) mass gives $C\sim M/\ell$, $C_x\sim M/\ell^2$. The surface [velocity](../../../../../velocity.md) is then $u_s\sim AMh_0/(\mu\ell^2)$. Equating this to $\ell/t$ gives **$\ell\propto t^{1/3}$**. For the precise [finite-mass Marangoni spreading on a liquid film](../../../../../finite-mass-marangoni-spreading-on-a-liquid-film.md) solution choose

$$
L(t)=\left(\frac{AMh_0t}\mu\right)^{1/3},\qquad\eta=\frac xL,\qquad h=h_0H(\eta),\quad C=\frac ML\Gamma(\eta),
$$

with symmetry about zero and support $0\leq\eta\leq\eta_N$ on the positive half-line. The reduced differential equations are

$$
\boxed{-\frac13\eta H'=\frac12(H^2\Gamma')',\qquad -\frac13(\eta\Gamma)'=(H\Gamma\Gamma')'.}
$$

Their boundary conditions are zero flux at the centre and zero concentration at the moving front. The two integral constraints express conserved surfactant mass and zero net change of liquid volume relative to the original uniform layer:

$$
\boxed{2\int_0^{\eta_N}\Gamma\,d\eta=1,\qquad\int_0^{\eta_N}(H-1)\,d\eta=0.}
$$

The second follows by integrating $h_t+q_x=0$ across the whole layer: the localized release adds surfactant but no liquid, and the flux vanishes at infinity. Outside the spreading region the leading depth remains $h_0$.

Integrating the concentration equation from the centre gives $H\Gamma\Gamma'=-\eta\Gamma/3$. Where $\Gamma>0$, this is $H\Gamma'=-\eta/3$. Substituting into the height equation gives

$$
-\frac13\eta H'=-\frac16(H+\eta H'),\qquad\eta H'=H.
$$

Therefore $H=c\eta$, and $\Gamma'= -1/(3c)$. With $\Gamma(\eta_N)=0$, the [linear similarity profiles for surfactant spreading](../../../../../linear-similarity-profiles-for-surfactant-spreading.md) are $\Gamma=(\eta_N-\eta)/(3c)$. The liquid-volume constraint gives $c\eta_N=2$, while the surfactant constraint gives $\eta_N^2/(3c)=1$. Thus $\eta_N^3=6$, and

$$
\boxed{x_N=\eta_NL=\left(\frac{6AMh_0t}\mu\right)^{1/3}.}
$$

In physical variables, the leading profiles on the whole line are

$$
\boxed{h(x,t)=2h_0\frac{|x|}{x_N},\qquad C(x,t)=\frac M{x_N}\left(1-\frac{|x|}{x_N}\right),\quad |x|<x_N.}
$$

Outside this interval $h=h_0$ and $C=0$. The formal outer solution reaches zero depth at the central point, and height $2h_0$ immediately inside the front. It is not a microscopic description of the central dry region or of the front transition. As a conservation check, the front [velocity](../../../../../velocity.md) equals both the incoming surface [velocity](../../../../../velocity.md) and the liquid Rankine–Hugoniot speed $q/(2h_0-h_0)=2AMh_0/(\mu x_N^2)=\dot x_N$.

The jump from $2h_0$ to $h_0$ cannot persist as a smooth solution with both hydrostatic and capillary gradients absent. In an edge region of width $\Delta$, a depth change of order $h_0$ produces $h_x\sim h_0/\Delta$ and $h_{xxx}\sim h_0/\Delta^3$. Keep the stipulated concentration-gradient scale $M/x_N^2$. The three liquid-flux scales are

$$
q_M\sim\frac{AMh_0^2}{\mu x_N^2},\qquad q_g\sim\frac{\rho gh_0^4}{\mu\Delta},\qquad q_\gamma\sim\frac{\gamma_0h_0^4}{\mu\Delta^3}.
$$

For $g=0$, balancing $q_M$ and $q_\gamma$ gives the [capillary smoothing of a Marangoni front](../../../../../capillary-smoothing-of-a-marangoni-front.md) width

$$
\boxed{\Delta\sim\left(\frac{\gamma_0h_0^2x_N^2}{AM}\right)^{1/3}\propto t^{2/9}.}
$$

Gravity dominates capillarity when $q_g/q_\gamma\sim\rho g\Delta^2/\gamma_0\gg1$. In physical units the condition is $\Delta^2\gg\gamma_0/(\rho g)$: the printed $\gamma_0/g$ omits density and is dimensionally incomplete unless [surface tension](../../../../../surface-tension.md) has already been divided by density. Balancing the gravity flux with $q_M$ yields the [gravity smoothing of a Marangoni front](../../../../../gravity-smoothing-of-a-marangoni-front.md):

$$
\boxed{\Delta\sim\frac{\rho gh_0^2x_N^2}{AM}\propto t^{2/3}.}
$$

This layer grows faster than the spreading half-length. It reaches the whole pool when

$$
\boxed{x_N\sim\frac{AM}{\rho gh_0^2},\qquad t_*\sim\frac{\mu(AM)^2}{(\rho g)^3h_0^7}.}
$$

Only scaling constants can be fixed by this balance, so an exact numerical coefficient in $t_*$ is not implied. The gravity-dominant assumption must hold at this crossover as well.

For $t\gg t_*$, the sharp-front linear-depth outer profile is replaced by a [gravity-levelled surfactant film](../../../../../gravity-levelled-surfactant-film.md): the height approaches $h_0$, with a small depression under the surfactant and redistributed liquid outside. The rapid hydrostatic return flow almost cancels the net Marangoni liquid flux. Setting $q\simeq0$ and $h\simeq h_0$ gives $h_x\simeq-3AC_x/(2\rho gh_0)$ and fractional depth variation $O(AM/(\rho gh_0^2x_N))\ll1$. The surface still moves outward, with $u_s\simeq-Ah_0C_x/(4\mu)$, so leveling the bulk liquid does not stop surfactant spreading.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 78](../../paper-78-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
