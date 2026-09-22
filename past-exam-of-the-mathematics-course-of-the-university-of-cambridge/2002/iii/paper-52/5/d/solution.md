<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the closed box have ceiling height $H$ above the source. The printed width $2R$ alone does not specify this height, so it must appear as an additional geometrical parameter. Take $t=0$ here when the plume has first reached the ceiling and its thin outflow has spread across the box. The leading [filling box model](../../../../../../filling-box-model.md) assumes a negligible source volume, insulated boundaries, fast horizontal spreading, slow evolution compared with the plume transit time, negligible diffusion, and $b\ll R$. Below the interface the ambient still has its original [temperature](../../../../../../temperature.md), so the local plume flux remains $q(z)=2\alpha w_*z$ from part (c).

The ceiling outflow creates a warm upper region. [Fluid entrainment](../../../../../../fluid-entrainment.md) draws the original lower fluid into the plume, making that upper region deepen. The [filling-box first front](../../../../../../filling-box-first-front.md) is the lower material boundary of fluid already modified by plume discharge, separating it from the initially unmodified ambient; it need not bound a uniformly mixed upper layer. With negligible occupied plume area, [volume conservation](../../../../../../volume-conservation.md) at its height $h(t)$ gives

$$
2R\dot h=-q(h)=-2\alpha w_*h.
$$

Therefore

$$
\boxed{h(t)=H e^{-t/t_f},\qquad t_f=\frac{R}{\alpha w_*}=\frac{2R}{(2\alpha)^{2/3}\mathcal B_0^{1/3}}.}
$$

If source switch-on is the time origin instead, replace $t$ by elapsed time after the initial transit and spreading stage; the quasi-steady model does not resolve that stage.

The [buoyancy](../../../../../../buoyancy.md) jump requires distinguishing ambient fluid at the front from the plume crossing it. Just after the first ceiling outflow, the ambient [buoyancy](../../../../../../buoyancy.md) immediately above the nascent front is

$$
G_H=\frac{\mathcal B_0}{q(H)}=\frac{w_*^2}{H}.
$$

Outside the narrow plume, ambient [temperature](../../../../../../temperature.md) is transported without diffusion. If $G_a$ is its [buoyancy](../../../../../../buoyancy.md) relative to the original fluid, its equation is

$$
\partial_tG_a-\frac{q(z)}{2R}\partial_zG_a=0.
$$

The first front follows precisely these material trajectories, so the [temperature](../../../../../../temperature.md) of the fluid immediately above it is conserved. The initially unmodified fluid below has $G_a=0$. Thus the ambient jump is

$$
\boxed{[G_a]_{\text{above}-\text{below}}=\frac{w_*^2}{H},\qquad [T_a]=\frac{w_*^2}{g\beta H}.}
$$

By contrast, the contemporaneous plume immediately below the front has $G_p(h,t)=w_*^2/h(t)$, which grows as the front descends. That plume value is not the ambient jump across the material first front. Equating the two would inadvertently impose a uniformly mixed upper layer and discard the [stable density stratification](../../../../../../stable-density-stratification.md) of the standard [filling box model](../../../../../../filling-box-model.md). Diffusion or extensive interfacial mixing can smooth and alter the ideal jump.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
