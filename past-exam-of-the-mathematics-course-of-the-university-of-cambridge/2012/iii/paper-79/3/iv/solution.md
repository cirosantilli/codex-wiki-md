<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For very stable continuously turbulent conditions, $z\gg\ell_O>0$, local eddies lose leading dependence on their distance from the wall. In [very stable surface-layer similarity](../../../../../../very-stable-surface-layer-similarity.md), the dimensionless functions must therefore scale as $\phi_m\sim c_m\zeta$ and $\phi_h\sim c_h\zeta$, with positive closure constants. Using $\ell_O=u_*^3/(\kappa|B_0|)$ gives

$$
\boxed{U_z\sim c_m\frac{|B_0|}{u_*^2},\qquad U(z)-U(z_r)\sim c_m\frac{|B_0|}{u_*^2}(z-z_r),\qquad N^2\sim c_h\frac{|B_0|^2}{u_*^4}.}
$$

Thus the mean velocity is approximately linear in height and the real [buoyancy frequency](../../../../../../buoyancy-frequency.md) is approximately constant, $N\sim\sqrt{c_h}|B_0|/u_*^2$. Under the [Reynolds analogy](../../../../../../reynolds-analogy.md), $c_h=c_m$.

The [local turbulent kinetic energy balance](../../../../../../local-turbulent-kinetic-energy-balance.md) gives

$$
\boxed{\epsilon=P-|B_0|\sim(c_m-1)|B_0|,\qquad \ell_\epsilon\sim\frac{u_*^3}{\epsilon}=\frac{u_*^3}{(c_m-1)|B_0|}.}
$$

Positive dissipation requires $c_m>1$. The turbulent energy-turnover length is of order $u_*^3/|B_0|$, hence of order the [Obukhov length](../../../../../../monin-obukhov-length.md), independent of observation height. A related buoyancy-limited length is $u_*/N$. The [Ozmidov length](../../../../../../ozmidov-length.md) follows by equating an eddy turnover time $\ell^{2/3}\epsilon^{-1/3}$ with $N^{-1}$:

$$
\ell_{\rm Oz}=(\epsilon/N^3)^{1/2}\sim\frac{\sqrt{c_m-1}}{c_h^{3/4}}\frac{u_*^3}{|B_0|}.
$$

These are turbulent turnover or buoyancy-transition scales. If “the scale at which dissipation occurs” means the actual viscous cutoff, molecular viscosity is also required: the [Kolmogorov microscales](../../../../../../kolmogorov-microscales.md) give

$$
\boxed{\eta_K=(\nu^3/\epsilon)^{1/4}\sim\left[\frac{\nu^3}{(c_m-1)|B_0|}\right]^{1/4}.}
$$

Without $\nu$, the viscous length cannot be fixed by the supplied stress and flux alone. Separating it from the turbulent turnover length avoids confusing an energy-budget estimate with the molecular cutoff.

Finally,

$$
\boxed{\mathrm{Ri}_f\longrightarrow\frac1{c_m},\qquad \mathrm{Ri}_g\longrightarrow\frac{c_h}{c_m^2}.}
$$

They become height-independent constants. The commonly used continuation $c_m=c_h=5$ gives $\mathrm{Ri}_f=\mathrm{Ri}_g\simeq0.2$ and $\epsilon\simeq4|B_0|$. This numerical value is a closure choice, not a deduction from units; setting $c_m=1$ would incorrectly leave zero dissipation. Extremely stable intermittent or collapsed turbulence need not satisfy this local-equilibrium model. The relation between the Obukhov and buoyancy-dissipation lengths in the local regime is also analyzed in [Grachev and colleagues' similarity study](https://arxiv.org/abs/1404.1397).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
