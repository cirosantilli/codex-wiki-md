<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [single-layer greenhouse model](../../../../../../single-layer-greenhouse-model.md) with a blackbody surface and one isothermal atmospheric layer. The layer is transparent to incoming stellar radiation, absorbs a fraction $\alpha$ of the surface's thermal radiation, and has the same thermal [emissivity](../../../../../../emissivity.md) $\alpha$ by [Kirchhoff's law of thermal radiation](../../../../../../kirchhoff-s-law-of-thermal-radiation.md). Here $0\leq\alpha\leq1$, and $T_e$ is the [planetary equilibrium temperature](../../../../../../planetary-equilibrium-temperature.md) defined by the absorbed global stellar flux $\sigma_{\rm SB}T_e^4$. Neglect [convection](../../../../../../convection.md), latent heat transport and intrinsic heat.

The layer absorbs $\alpha\sigma_{\rm SB}T_s^4$ and emits $\alpha\sigma_{\rm SB}T_a^4$ upward and downward. For $\alpha>0$, its energy balance gives

$$
\alpha\sigma_{\rm SB}T_s^4=2\alpha\sigma_{\rm SB}T_a^4,\qquad T_a^4=T_s^4/2.
$$

The surface receives the absorbed stellar flux plus downward atmospheric emission, so

$$
\sigma_{\rm SB}T_s^4=\sigma_{\rm SB}T_e^4+\alpha\sigma_{\rm SB}T_a^4.
$$

Eliminating $T_a$ yields

$$
\boxed{T_s=\left(\frac{2}{2-\alpha}\right)^{1/4}T_e}.
$$

The outgoing top-of-atmosphere flux is $(1-\alpha)\sigma_{\rm SB}T_s^4+\alpha\sigma_{\rm SB}T_a^4=\sigma_{\rm SB}T_e^4$, confirming overall energy conservation. At $\alpha=0$, $T_s=T_e$ and the decoupled layer's [temperature](../../../../../../temperature.md) is not determined; at $\alpha=1$, $T_s=2^{1/4}T_e$. This warming is the restriction of thermal escape by the absorbing and emitting layer.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
