<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K_w$ be the water [thermal conductivity](../../../../../../thermal-conductivity.md), $L_m$ the [latent heat](../../../../../../latent-heat.md) of fusion per unit ice mass, and $\rho_i$ the ice density. Define $v_m>0$ as the normal ice-retreat speed that enlarges the cavity. With the water [thermal boundary layer](../../../../../../thermal-boundary-layer.md) at $T_s$ on its warm side and $T_m$ at the melting interface, the heat supply per unit interface area is approximately

$$
q_T\simeq K_w\frac{T_s-T_m}{\delta_T}.
$$

The ice is specified to be uniformly at $T_m$, so no leading sensible-heat flux into colder ice must be subtracted. The [Stefan condition](../../../../../../stefan-condition.md) is therefore $\rho_iL_mv_m=q_T$, giving

$$
\boxed{v_m\simeq\frac{K_w(T_s-T_m)}{\rho_iL_m\delta_T},\qquad\delta_T\sim\delta_v.}
$$

Equivalently $K_w=\rho_wc_p\kappa_T$ expresses the heat flux in terms of water [thermal diffusivity](../../../../../../thermal-diffusivity.md). The imposed temperatures and constant boundary-layer thickness make this melt rate uniform and constant over the wetted interface. Melting adds latent energy demand to the flow; for an isolated finite pulse, maintaining $T_s$ indefinitely would require heat replenishment. The constant-temperature model is consequently an imposed closure, not a prediction of a permanently hot finite water volume.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
