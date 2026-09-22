<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the planar geometry indicated by the supplied $x,z$ equation and [streamfunction](../../../../../stream-function.md); the source heat input is then measured per unit out-of-plane span. Let $\Theta=T-T_0$ and define

$$
\beta=\frac{\rho_0g\alpha\Pi}{\mu}>0,\qquad w=\beta\Theta.
$$

This is the buoyancy part of [Darcy law](../../../../../darcy-law.md). Let $C_h$ denote the constant [heat capacity](../../../../../heat-capacity.md) per volume consistent with the given transport equation; for the fluid heat-flux convention $C_h=\rho_0c_p$. [Porosity](../../../../../porosity.md) or matrix heat-storage factors, if retained, must be used consistently in this coefficient and the effective transport parameters.

For plume width $b\ll z$, continuity gives $u\sim wb/z$. Both $u\Theta_x$ and $w\Theta_z$ are consequently of order $w\Theta/z$: lateral advection must not be discarded. Lateral thermal diffusion is of order $\kappa\Theta/b^2$, while vertical diffusion is smaller by $(b/z)^2$. The slender steady [porous thermal plume](../../../../../porous-thermal-plume.md) model is therefore

$$
\boxed{u\Theta_x+w\Theta_z=\kappa\Theta_{xx},\qquad u_x+w_z=0,\qquad w=\beta\Theta.}
$$

Writing it in conservative form,

$$
\partial_z(w\Theta)+\partial_x(u\Theta-\kappa\Theta_x)=0,
$$

and integrating across the plume, where $\Theta$ and lateral diffusive/advective heat transport vanish at large $|x|$, proves

$$
\boxed{F_h=C_h\int_{-\infty}^{\infty}w\Theta\,dx=\text{constant}.}
$$

In steady state with no lateral heat loss and negligible vertical conductive flux, this equals the heat supplied at the source. Define $Q=\beta F_h/C_h=\int w^2dx>0$.

For characteristic velocity $W$ and width $b$, flux conservation gives $W^2b\sim Q$ and the advection-diffusion balance gives $Wb^2\sim\kappa z$. Consequently

$$
\boxed{b\propto z^{2/3},\qquad W\propto z^{-1/3},\qquad
\Theta\propto z^{-1/3},\qquad u\propto z^{-2/3}.}
$$

The dimensional scales are $b\sim(\kappa^2z^2/Q)^{1/3}$ and $W\sim(Q^2/(\kappa z))^{1/3}$. The plume becomes relatively more slender, $b/z\propto z^{-1/3}$, away from the source.

To find the profile, put $\eta=x/b(z)$ and $\psi=-W(z)b(z)f(\eta)$, so $w=Wf'$ and

$$
u=-\frac{Wb}{3z}(f-2\eta f').
$$

Inserting into $uw_x+ww_z=\kappa w_{xx}$ gives

$$
f'''+\frac{Wb^2}{3\kappa z}(ff''+f'^2)=0.
$$

Its coefficient is constant under the derived scaling. Choose the width normalization $Wb^2=6\kappa z$. Integrating once with decaying velocity derivatives gives $f''+2ff'=0$. A second integration gives $f'+f^2=1$ after normalizing the centreline velocity to $W$; symmetry has $f(0)=0$. The decaying, positive solution is $f=\tanh\eta$. Hence the [hyperbolic-secant porous plume profile](../../../../../hyperbolic-secant-porous-plume-profile.md) is

$$
\boxed{w=W\operatorname{sech}^2(x/b),\quad
T-T_0=\frac W\beta\operatorname{sech}^2(x/b),\quad
\psi=-Wb\tanh(x/b).}
$$

Since $\int_{-\infty}^{\infty}\operatorname{sech}^4\eta\,d\eta=4/3$, the precise amplitudes are

$$
\boxed{b(z)=\left(\frac{48\kappa^2z^2}{Q}\right)^{1/3},\qquad
W(z)=\left(\frac{3Q^2}{32\kappa z}\right)^{1/3}.}
$$

They satisfy both $Wb^2=6\kappa z$ and $(4/3)W^2b=Q$. The derived $u$ supplies lateral [entrainment](../../../../../fluid-entrainment.md); setting $u=0$ would not reproduce this profile or satisfy continuity.

A [heat-weighted head speed of a porous plume](../../../../../heat-weighted-head-speed-of-a-porous-plume.md) estimate follows by filling the column below a head height $Z_h(t)$ with this steady profile. Its excess heat per unit height is

$$
\mathcal H(z)=C_h\int\Theta\,dx=\frac{2C_hWb}{\beta}.
$$

Conservation of the total injected heat gives $F_ht\simeq\int_0^{Z_h}\mathcal H(z)dz$. Differentiating,

$$
\boxed{\dot Z_h\simeq\frac{F_h}{\mathcal H(Z_h)}
=\frac{\int w^2dx}{\int wdx}=\frac23W(Z_h).}
$$

Thus a heat-weighted head advances at a speed of order the local centreline velocity and decelerates as $Z_h^{-1/3}$. With $K=(3Q^2/(32\kappa))^{1/3}$,

$$
\boxed{Z_h(t)\simeq\left(\frac89Kt\right)^{3/4}.}
$$

The factor $2/3$ is the energy-conserving estimate for a truncated steady column; the foremost centreline parcels have characteristic speed $W(Z_h)$ instead. The steady calculation does not resolve the transient nose or define an exact sharp temperature front. A truly axisymmetric point-source plume would require different geometry and cannot use this planar profile unchanged.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 65](../../paper-65-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
