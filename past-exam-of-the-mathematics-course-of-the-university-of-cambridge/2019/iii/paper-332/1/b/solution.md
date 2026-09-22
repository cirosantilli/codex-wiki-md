<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Before drainage reaches the divide, most of the aquifer fills locally to height $H=Rt/\phi$. Only a growing [boundary layer](../../../../../../boundary-layer.md) beside the river departs substantially from this height. Write $D=u_b\beta/2$.

At early times $H\ll2/\beta$, the mobility is $u_bh$. The balance between storage and [nonlinear diffusion](../../../../../../nonlinear-diffusion-equation.md) gives

$$
\ell_e(t)=\frac{\sqrt{u_bR}}{\phi}t,\qquad h=\frac{Rt}{\phi}F_e(\eta),\qquad \eta=x/\ell_e.
$$

Substitution into the governing equation gives the [forced filling similarity for power-law diffusion](../../../../../../forced-filling-similarity-for-power-law-diffusion.md) with exponent $m=1$:

$$
(F_eF_e')'+1-F_e+\eta F_e'=0,\qquad F_e(0)=0,\qquad F_e(\infty)=1.
$$

The positive outward [volume flux per unit width](../../../../../../volume-flux-per-unit-width.md) is

$$
\boxed{Q_e=c_e\frac{\sqrt{u_b}\,R^{3/2}}{\phi}t,\qquad c_e=\lim_{\eta\downarrow0}F_eF_e'=2\int_0^\infty(1-F_e)\,d\eta.}
$$

The boundary slope is singular, but $F_e\sim(2c_e\eta)^{1/2}$ gives a finite flux.

At intermediate times $H\gg2/\beta$, the large-depth mobility is $Dh^2$. The corresponding [similarity solution](../../../../../../similarity-solution.md) is

$$
\ell_i(t)=\left(\frac{DR^2t^3}{\phi^3}\right)^{1/2},\qquad h=\frac{Rt}{\phi}F_i(\eta),\qquad \eta=x/\ell_i,
$$

with

$$
(F_i^2F_i')'+1-F_i+\frac32\eta F_i'=0,\qquad F_i(0)=0,\qquad F_i(\infty)=1.
$$

Consequently,

$$
\boxed{Q_i=c_i\frac{\sqrt D\,R^2}{\phi^{3/2}}t^{3/2},\qquad c_i=\lim_{\eta\downarrow0}F_i^2F_i'=\frac52\int_0^\infty(1-F_i)\,d\eta.}
$$

Here $F_i\sim(3c_i\eta)^{1/3}$ is the outer outlet profile. The height actually vanishes at the river, so an [outlet layer in a deep unconfined aquifer](../../../../../../outlet-layer-in-a-deep-unconfined-aquifer.md) restores the $u_bh$ mobility extremely close to the boundary while transmitting this same leading discharge.

The mobility changes when $H\sim2/\beta$, whereas the divide first affects the deep filling solution when $\ell_i\sim L$. Thus

$$
\boxed{t_\beta=\frac{2\phi}{R\beta},\qquad t_{\rm fill}=\phi\left(\frac LR\right)^{2/3}D^{-1/3}.}
$$

A distinct intermediate regime requires $t_\beta\ll t_{\rm fill}$. If the divide is reached while the aquifer is still shallow, the early filling law instead crosses directly toward the steady state, at a time of order $\phi L/\sqrt{u_bR}$. The faster intermediate discharge growth comes from increasing [permeability of a porous medium](../../../../../../permeability-of-a-porous-medium.md) as deeper parts of the aquifer become saturated; once the finite domain is felt, the discharge approaches $RL$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
