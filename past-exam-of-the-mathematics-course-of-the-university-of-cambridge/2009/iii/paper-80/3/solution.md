<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use an inertial [gravity-current box model](../../../../../gravity-current-box-model.md) in a horizontal prismatic V-shaped valley. Let its section have area $A(h)=\lambda h^2$ and width $2\lambda h$, where the dimensionless constant $\lambda>0$ is half-width divided by depth. Let $X(t)$ be front position and $h(t)$ the representative uniform current depth. Assume negligible [entrainment](../../../../../fluid-entrainment.md) and volume loss, hydrostatic cross-sections, large Reynolds number, and negligible bed friction and axial bed slope. These assumptions describe the bulk spreading after the short dam-break adjustment; they do not give a universal law for a steep or friction-dominated valley.

For water of fixed volume $W$, conservation gives $W=\lambda h^2X$. Close the front speed by the [gravity-current front condition](../../../../../gravity-current-front-condition.md) $\dot X=\operatorname{Fr}\sqrt{gh}$, where $\operatorname{Fr}$ is a constant order-one [Froude number](../../../../../froude-number.md) for the chosen inertial front model. Therefore

$$
\dot X=K_wX^{-1/4},\qquad
K_w=\operatorname{Fr}\sqrt g\,(W/\lambda)^{1/4}.
$$

Integration gives $X^{5/4}=X_0^{5/4}+5K_wt/4$. Once the initial reservoir length $X_0$ is negligible, the [inertial dam-break current in a triangular valley](../../../../../inertial-dam-break-current-in-a-triangular-valley.md) satisfies

$$
\boxed{X(t)=\left[\frac54\operatorname{Fr}\sqrt g\,(W/\lambda)^{1/4}t\right]^{4/5}
\propto W^{1/5}t^{4/5}.}
$$

The time exponent differs from a flat-bottomed channel because a V-shaped section stores volume proportional to $h^2$. A viscous [V-shaped channel gravity current](../../../../../v-shaped-channel-gravity-current.md) obeys a different spreading law, so retaining the inertial assumption is essential.

For the short-lived eruption, interpret $W$ as the bulk mixture volume released during the event. Let $\phi(t)$ be the well-mixed particle volume fraction, initially $\phi_0$, let $\rho_p$ and $\rho_a$ be particle and ambient carrier densities, and assume a dilute [Boussinesq approximation](../../../../../boussinesq-approximation.md) for the mixture. The particles provide [reduced gravity](../../../../../reduced-gravity-split.md)

$$
g'(t)=G\phi(t),\qquad G=g\frac{\rho_p-\rho_a}{\rho_a},\qquad g'_0=G\phi_0.
$$

Assume thermal [buoyancy](../../../../../buoyancy.md), compressibility, erosion and continued injection are negligible, and that the carrier volume remains $W$. Turbulent mixing keeps the particles suspended uniformly while they settle vertically at a constant terminal [settling velocity](../../../../../settling-velocity.md) $w_s$. For small spherical particles of radius $a_p$ in carrier viscosity $\mu_a$, the [Stokes settling velocity](../../../../../stokes-settling-velocity.md) is $w_s=2(\rho_p-\rho_a)ga_p^2/(9\mu_a)$ when the particle Reynolds number is small. If an eruption volume is quoted as solid particle volume rather than mixture volume, replace the $W$ used here by that volume divided by $\phi_0$.

The [particle deposition flux](../../../../../particle-deposition-flux.md) per horizontal projected bed area is $w_s\phi$. The current's projected settling area is $2\lambda hX$, so

$$
\frac d{dt}(\phi W)=-2\lambda hXw_s\phi,
\qquad\boxed{\dot\phi=-\frac{2w_s}{h}\phi.}
$$

The factor two reflects the triangular section's mean depth $h/2$. Put $s=\sqrt{\phi/\phi_0}$ and $K=\operatorname{Fr}\sqrt{g'_0}(W/\lambda)^{1/4}$. The front and concentration balances become

$$
\dot X=KsX^{-1/4},\qquad
\dot s=-w_s\sqrt{\lambda/W}\,sX^{1/2},\qquad
\frac{ds}{dX}=-\frac{w_s}{K}\sqrt{\lambda/W}\,X^{3/4}.
$$

Taking the initial release length negligible compared with the final runout, integration yields the [constant-settling runout in a triangular valley](../../../../../constant-settling-runout-in-a-triangular-valley.md):

$$
\boxed{s=1-(X/R)^{7/4},\qquad
\phi(X)=\phi_0[1-(X/R)^{7/4}]^2,\qquad
R=\left[\frac{7\operatorname{Fr}\sqrt{g'_0}}{4w_s}(W/\lambda)^{3/4}\right]^{4/7}.}
$$

In particular $R\propto W^{3/7}(g'_0)^{2/7}w_s^{-4/7}$ at fixed valley shape and front coefficient. With a finite initial length, replace $R^{7/4}$ by $X_0^{7/4}+7K\sqrt{W/\lambda}/(4w_s)$ in the corresponding integrated relation.

The whole time dependence is determined analytically by the quadrature

$$
\boxed{t=\frac{R^{5/4}}K\int_0^{X/R}\frac{y^{1/4}}{1-y^{7/4}}\,dy.}
$$

Early spreading has $X\simeq(5Kt/4)^{4/5}$, the water law with $g$ replaced by $g'_0$. At late times the concentration loss slows the flow, and $R-X$ decays exponentially with rate $7K/(4R^{5/4})=w_s/h_R$, where $h_R=\sqrt{W/(\lambda R)}$. The final length $R$ is a limiting runout reached as $t\to\infty$, not a finite-time stopping event in this ideal model.

To calculate the [deposit profile of a finite triangular-valley particle current](../../../../../deposit-profile-of-a-finite-triangular-valley-particle-current.md), let $m_d(x)$ be final deposited particle mass per unit downstream length, and $M_0=\rho_p\phi_0W$ the initial particle mass. Deposition at a fixed section starts at arrival time $t_a(x)$, when the front first reaches $x$. With the instantaneous front coordinate denoted $\xi$, use $dt=\xi^{1/4}d\xi/[K(1-(\xi/R)^{7/4})]$ to obtain

$$
m_d(x)=\int_{t_a(x)}^{\infty}2\lambda h(t)w_s\rho_p\phi(t)\,dt
=\frac{2w_s\rho_p\phi_0\sqrt{\lambda W}}K
\int_x^R\xi^{-1/4}[1-(\xi/R)^{7/4}]\,d\xi.
$$

Writing $\eta=x/R$, this evaluates to

$$
\boxed{m_d(x)=\frac{M_0}{R}\left[\frac{14}3(1-\eta^{3/4})-\frac75(1-\eta^{5/2})\right],
\quad0\leq x\leq R,}
$$

and $m_d=0$ beyond $R$. The profile decreases downstream, vanishes quadratically at the runout, and obeys $\int_0^Rm_d(x)dx=M_0$. This integral check ensures that all initially suspended particle mass is accounted for.

For an areal rather than a linear deposit density, the changing valley width must also be specified. At lateral coordinate $y_\perp$, the current covers the bed only while $|y_\perp|\leq\lambda h$. Set $Z=\min(R,\lambda W/y_\perp^2)$, with $Z=R$ on the valley axis. The mass per horizontal projected bed area is zero if $Z<x$, and otherwise is

$$
\boxed{\Sigma_d(x,y_\perp)=\frac{\rho_pw_s\phi_0}K\left[
\frac45(Z^{5/4}-x^{5/4})-\frac{Z^3-x^3}{3R^{7/4}}\right].}
$$

On the axis this reduces to $\rho_p\phi_0h_R[\tfrac75(1-\eta^{5/4})-\tfrac7{12}(1-\eta^3)]$. Divide projected areal density by $\sqrt{1+\lambda^{-2}}$ to obtain mass per actual sloping bed area. A specified packed deposit density then converts this areal mass to local deposit thickness; the spreading model itself predicts deposited mass, not a packing fraction.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
